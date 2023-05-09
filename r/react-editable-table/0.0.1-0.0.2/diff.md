# Comparing `tmp/react_editable_table-0.0.1.tar.gz` & `tmp/react_editable_table-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "react_editable_table-0.0.1.tar", last modified: Fri May  5 06:03:07 2023, max compression
+gzip compressed data, was "react_editable_table-0.0.2.tar", last modified: Tue May  9 02:52:16 2023, max compression
```

## Comparing `react_editable_table-0.0.1.tar` & `react_editable_table-0.0.2.tar`

### file list

```diff
@@ -1,48 +1,54 @@
-drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-05 06:03:07.377022 react_editable_table-0.0.1/
--rw-r--r--   0 jway       (501) staff       (20)      683 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/MANIFEST.in
--rw-r--r--   0 jway       (501) staff       (20)     3233 2023-05-05 06:03:07.377112 react_editable_table-0.0.1/PKG-INFO
--rw-r--r--   0 jway       (501) staff       (20)     2315 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/README.md
-drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-05 06:03:07.364562 react_editable_table-0.0.1/examples/
--rw-r--r--   0 jway       (501) staff       (20)     2853 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/examples/introduction.ipynb
--rw-r--r--   0 jway       (501) staff       (20)      201 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/install.json
--rw-r--r--   0 jway       (501) staff       (20)     2896 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/package.json
--rw-r--r--   0 jway       (501) staff       (20)      145 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/pyproject.toml
-drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-05 06:03:07.365848 react_editable_table-0.0.1/react_editable_table/
--rw-r--r--   0 jway       (501) staff       (20)     1905 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/react_editable_table/__init__.py
--rw-r--r--   0 jway       (501) staff       (20)      253 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/react_editable_table/_frontend.py
--rw-r--r--   0 jway       (501) staff       (20)      198 2023-05-05 06:01:24.000000 react_editable_table-0.0.1/react_editable_table/_version.py
-drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-05 06:03:07.368030 react_editable_table-0.0.1/react_editable_table/labextension/
--rw-r--r--   0 jway       (501) staff       (20)     3012 2023-05-05 05:54:51.000000 react_editable_table-0.0.1/react_editable_table/labextension/package.json
-drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-05 06:03:07.370681 react_editable_table-0.0.1/react_editable_table/labextension/static/
--rw-r--r--   0 jway       (501) staff       (20)    17371 2023-05-05 05:54:51.000000 react_editable_table-0.0.1/react_editable_table/labextension/static/367.3d04076279ae73bb45ed.js
--rw-r--r--   0 jway       (501) staff       (20)     1061 2023-05-05 05:54:51.000000 react_editable_table-0.0.1/react_editable_table/labextension/static/480.fda11aa309243be0db4c.js
--rw-r--r--   0 jway       (501) staff       (20)      641 2023-05-05 05:54:51.000000 react_editable_table-0.0.1/react_editable_table/labextension/static/568.e0e647aedd1424b2d8cf.js
--rw-r--r--   0 jway       (501) staff       (20)     6340 2023-05-05 05:54:51.000000 react_editable_table-0.0.1/react_editable_table/labextension/static/remoteEntry.b35d3910be71a545f174.js
--rw-r--r--   0 jway       (501) staff       (20)      118 2023-05-05 05:54:51.000000 react_editable_table-0.0.1/react_editable_table/labextension/static/style.js
--rw-r--r--   0 jway       (501) staff       (20)     1240 2023-05-05 05:54:51.000000 react_editable_table-0.0.1/react_editable_table/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-05 06:03:07.372628 react_editable_table-0.0.1/react_editable_table/nbextension/
--rw-r--r--   0 jway       (501) staff       (20)      432 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/react_editable_table/nbextension/extension.js
--rw-r--r--   0 jway       (501) staff       (20)   150480 2023-05-05 05:52:40.000000 react_editable_table-0.0.1/react_editable_table/nbextension/index.js
--rw-r--r--   0 jway       (501) staff       (20)      788 2023-05-05 05:52:40.000000 react_editable_table-0.0.1/react_editable_table/nbextension/index.js.LICENSE.txt
--rw-r--r--   0 jway       (501) staff       (20)   418406 2023-05-05 05:52:40.000000 react_editable_table-0.0.1/react_editable_table/nbextension/index.js.map
--rw-r--r--   0 jway       (501) staff       (20)     2120 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/react_editable_table/widget.py
-drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-05 06:03:07.367684 react_editable_table-0.0.1/react_editable_table.egg-info/
--rw-r--r--   0 jway       (501) staff       (20)     3233 2023-05-05 06:03:07.000000 react_editable_table-0.0.1/react_editable_table.egg-info/PKG-INFO
--rw-r--r--   0 jway       (501) staff       (20)     1278 2023-05-05 06:03:07.000000 react_editable_table-0.0.1/react_editable_table.egg-info/SOURCES.txt
--rw-r--r--   0 jway       (501) staff       (20)        1 2023-05-05 06:03:07.000000 react_editable_table-0.0.1/react_editable_table.egg-info/dependency_links.txt
--rw-r--r--   0 jway       (501) staff       (20)      183 2023-05-05 06:03:07.000000 react_editable_table-0.0.1/react_editable_table.egg-info/requires.txt
--rw-r--r--   0 jway       (501) staff       (20)       21 2023-05-05 06:03:07.000000 react_editable_table-0.0.1/react_editable_table.egg-info/top_level.txt
--rw-r--r--   0 jway       (501) staff       (20)       74 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/react_editable_table.json
--rw-r--r--   0 jway       (501) staff       (20)      187 2023-05-05 06:03:07.383463 react_editable_table-0.0.1/setup.cfg
--rw-r--r--   0 jway       (501) staff       (20)     3295 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/setup.py
-drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-05 06:03:07.376191 react_editable_table-0.0.1/src/
--rw-r--r--   0 jway       (501) staff       (20)      628 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/src/extension.ts
--rw-r--r--   0 jway       (501) staff       (20)      140 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/src/index.ts
--rw-r--r--   0 jway       (501) staff       (20)     1121 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/src/plugin.ts
-drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-05 06:03:07.376795 react_editable_table-0.0.1/src/react/
--rw-r--r--   0 jway       (501) staff       (20)     1721 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/src/react/ReactEditableTable.tsx
--rw-r--r--   0 jway       (501) staff       (20)     2603 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/src/react/model.ts
--rw-r--r--   0 jway       (501) staff       (20)      569 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/src/version.ts
--rw-r--r--   0 jway       (501) staff       (20)     1988 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/src/widget.ts
--rw-r--r--   0 jway       (501) staff       (20)      555 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/tsconfig.json
--rw-r--r--   0 jway       (501) staff       (20)     2394 2023-05-05 05:44:06.000000 react_editable_table-0.0.1/webpack.config.js
+drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-09 02:52:16.982412 react_editable_table-0.0.2/
+-rw-r--r--   0 jway       (501) staff       (20)      683 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/MANIFEST.in
+-rw-r--r--   0 jway       (501) staff       (20)     3233 2023-05-09 02:52:16.982499 react_editable_table-0.0.2/PKG-INFO
+-rw-r--r--   0 jway       (501) staff       (20)     2315 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/README.md
+drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-09 02:52:16.950203 react_editable_table-0.0.2/examples/
+-rw-r--r--   0 jway       (501) staff       (20)     2853 2023-05-09 02:08:01.000000 react_editable_table-0.0.2/examples/introduction.ipynb
+-rw-r--r--   0 jway       (501) staff       (20)      201 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/install.json
+-rw-r--r--   0 jway       (501) staff       (20)     3019 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/package.json
+-rw-r--r--   0 jway       (501) staff       (20)      145 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/pyproject.toml
+drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-09 02:52:16.951617 react_editable_table-0.0.2/react_editable_table/
+-rw-r--r--   0 jway       (501) staff       (20)     1905 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/react_editable_table/__init__.py
+-rw-r--r--   0 jway       (501) staff       (20)      253 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/react_editable_table/_frontend.py
+-rw-r--r--   0 jway       (501) staff       (20)      198 2023-05-09 02:25:53.000000 react_editable_table-0.0.2/react_editable_table/_version.py
+drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-09 02:52:16.954090 react_editable_table-0.0.2/react_editable_table/labextension/
+-rw-r--r--   0 jway       (501) staff       (20)    21952 2023-05-09 02:42:29.000000 react_editable_table-0.0.2/react_editable_table/labextension/build_log.json
+-rw-r--r--   0 jway       (501) staff       (20)     3135 2023-05-09 02:42:31.000000 react_editable_table-0.0.2/react_editable_table/labextension/package.json
+drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-09 02:52:16.961981 react_editable_table-0.0.2/react_editable_table/labextension/static/
+-rw-r--r--   0 jway       (501) staff       (20)     1384 2023-05-09 02:42:31.000000 react_editable_table-0.0.2/react_editable_table/labextension/static/lib_index_js.e6966c837e725382f93e.js
+-rw-r--r--   0 jway       (501) staff       (20)      401 2023-05-09 02:42:31.000000 react_editable_table-0.0.2/react_editable_table/labextension/static/lib_index_js.e6966c837e725382f93e.js.map
+-rw-r--r--   0 jway       (501) staff       (20)     2541 2023-05-09 02:42:31.000000 react_editable_table-0.0.2/react_editable_table/labextension/static/lib_plugin_js.1e650cc31d573daec095.js
+-rw-r--r--   0 jway       (501) staff       (20)     1839 2023-05-09 02:42:31.000000 react_editable_table-0.0.2/react_editable_table/labextension/static/lib_plugin_js.1e650cc31d573daec095.js.map
+-rw-r--r--   0 jway       (501) staff       (20)    14364 2023-05-09 02:42:31.000000 react_editable_table-0.0.2/react_editable_table/labextension/static/lib_widget_js.e581d1c3446a69e4da81.js
+-rw-r--r--   0 jway       (501) staff       (20)    15405 2023-05-09 02:42:31.000000 react_editable_table-0.0.2/react_editable_table/labextension/static/lib_widget_js.e581d1c3446a69e4da81.js.map
+-rw-r--r--   0 jway       (501) staff       (20)    28750 2023-05-09 02:42:31.000000 react_editable_table-0.0.2/react_editable_table/labextension/static/remoteEntry.33176020e90c68450293.js
+-rw-r--r--   0 jway       (501) staff       (20)    27490 2023-05-09 02:42:31.000000 react_editable_table-0.0.2/react_editable_table/labextension/static/remoteEntry.33176020e90c68450293.js.map
+-rw-r--r--   0 jway       (501) staff       (20)      118 2023-05-09 02:42:29.000000 react_editable_table-0.0.2/react_editable_table/labextension/static/style.js
+-rw-r--r--   0 jway       (501) staff       (20)  2800741 2023-05-09 02:42:31.000000 react_editable_table-0.0.2/react_editable_table/labextension/static/vendors-node_modules_mantine_core_esm_index_js-node_modules_ahooks_es_index_js-node_modules_i-d1af73.0f5a02a624163810708e.js
+-rw-r--r--   0 jway       (501) staff       (20)  3089532 2023-05-09 02:42:31.000000 react_editable_table-0.0.2/react_editable_table/labextension/static/vendors-node_modules_mantine_core_esm_index_js-node_modules_ahooks_es_index_js-node_modules_i-d1af73.0f5a02a624163810708e.js.map
+drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-09 02:52:16.978134 react_editable_table-0.0.2/react_editable_table/nbextension/
+-rw-r--r--   0 jway       (501) staff       (20)      432 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/react_editable_table/nbextension/extension.js
+-rw-r--r--   0 jway       (501) staff       (20)   261230 2023-05-09 01:56:18.000000 react_editable_table-0.0.2/react_editable_table/nbextension/index.js
+-rw-r--r--   0 jway       (501) staff       (20)     1035 2023-05-09 01:56:18.000000 react_editable_table-0.0.2/react_editable_table/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0 jway       (501) staff       (20)   916623 2023-05-09 01:56:18.000000 react_editable_table-0.0.2/react_editable_table/nbextension/index.js.map
+-rw-r--r--   0 jway       (501) staff       (20)     3041 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/react_editable_table/widget.py
+drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-09 02:52:16.953197 react_editable_table-0.0.2/react_editable_table.egg-info/
+-rw-r--r--   0 jway       (501) staff       (20)     3233 2023-05-09 02:52:16.000000 react_editable_table-0.0.2/react_editable_table.egg-info/PKG-INFO
+-rw-r--r--   0 jway       (501) staff       (20)     1954 2023-05-09 02:52:16.000000 react_editable_table-0.0.2/react_editable_table.egg-info/SOURCES.txt
+-rw-r--r--   0 jway       (501) staff       (20)        1 2023-05-09 02:52:16.000000 react_editable_table-0.0.2/react_editable_table.egg-info/dependency_links.txt
+-rw-r--r--   0 jway       (501) staff       (20)      183 2023-05-09 02:52:16.000000 react_editable_table-0.0.2/react_editable_table.egg-info/requires.txt
+-rw-r--r--   0 jway       (501) staff       (20)       21 2023-05-09 02:52:16.000000 react_editable_table-0.0.2/react_editable_table.egg-info/top_level.txt
+-rw-r--r--   0 jway       (501) staff       (20)       74 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/react_editable_table.json
+-rw-r--r--   0 jway       (501) staff       (20)      187 2023-05-09 02:52:16.982893 react_editable_table-0.0.2/setup.cfg
+-rw-r--r--   0 jway       (501) staff       (20)     3295 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/setup.py
+drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-09 02:52:16.981526 react_editable_table-0.0.2/src/
+-rw-r--r--   0 jway       (501) staff       (20)      628 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/src/extension.ts
+-rw-r--r--   0 jway       (501) staff       (20)      140 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/src/index.ts
+-rw-r--r--   0 jway       (501) staff       (20)     1121 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/src/plugin.ts
+drwxr-xr-x   0 jway       (501) staff       (20)        0 2023-05-09 02:52:16.982230 react_editable_table-0.0.2/src/react/
+-rw-r--r--   0 jway       (501) staff       (20)     3552 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/src/react/ReactEditableTable.tsx
+-rw-r--r--   0 jway       (501) staff       (20)     2619 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/src/react/model.ts
+-rw-r--r--   0 jway       (501) staff       (20)      569 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/src/version.ts
+-rw-r--r--   0 jway       (501) staff       (20)     1978 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/src/widget.ts
+-rw-r--r--   0 jway       (501) staff       (20)      555 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/tsconfig.json
+-rw-r--r--   0 jway       (501) staff       (20)     2394 2023-05-09 01:53:36.000000 react_editable_table-0.0.2/webpack.config.js
```

### Comparing `react_editable_table-0.0.1/MANIFEST.in` & `react_editable_table-0.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `react_editable_table-0.0.1/PKG-INFO` & `react_editable_table-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: react_editable_table
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Custom Jupyter Widget Library
 Home-page: https://github.com/tidbcloud/react-editable-table
 Author: zoubingwu
 Author-email: zoubingwu@gmail.com
 License: BSD
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
```

### Comparing `react_editable_table-0.0.1/README.md` & `react_editable_table-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `react_editable_table-0.0.1/examples/introduction.ipynb` & `react_editable_table-0.0.2/examples/introduction.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.9.6'}}"}*

```diff
@@ -101,13 +101,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.6.3"
+            "version": "3.9.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `react_editable_table-0.0.1/package.json` & `react_editable_table-0.0.2/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.995943204868154%*

 * *Differences: {"'devDependencies'": "{'@emotion/react': '^11.11.0', '@mantine/core': '^6.0.10', "*

 * *                      "'@mantine/hooks': '^6.0.10', 'ahooks': '^3.7.7'}"}*

```diff
@@ -20,21 +20,25 @@
     },
     "description": "A Custom Jupyter Widget Library",
     "devDependencies": {
         "@babel/core": "^7.21.4",
         "@babel/preset-env": "^7.21.4",
         "@babel/preset-react": "^7.18.6",
         "@babel/preset-typescript": "^7.21.4",
+        "@emotion/react": "^11.11.0",
         "@jupyterlab/builder": "^3.6.3",
         "@lumino/application": "^2.1.0",
         "@lumino/widgets": "^2.1.0",
+        "@mantine/core": "^6.0.10",
+        "@mantine/hooks": "^6.0.10",
         "@types/react": "^17.0.2",
         "@types/react-dom": "^17.0.2",
         "@types/webpack": "^5.28.1",
         "@types/webpack-env": "^1.18.0",
+        "ahooks": "^3.7.7",
         "babel-loader": "^9.1.2",
         "css-loader": "^6.7.3",
         "fs-extra": "^11.1.1",
         "immer": "^10.0.1",
         "mkdirp": "^3.0.1",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.8",
```

### Comparing `react_editable_table-0.0.1/react_editable_table/__init__.py` & `react_editable_table-0.0.2/react_editable_table/__init__.py`

 * *Files identical despite different names*

### Comparing `react_editable_table-0.0.1/react_editable_table/labextension/package.json` & `react_editable_table-0.0.2/react_editable_table/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950240872210953%*

 * *Differences: {"'devDependencies'": "{'@emotion/react': '^11.11.0', '@mantine/core': '^6.0.10', "*

 * *                      "'@mantine/hooks': '^6.0.10', 'ahooks': '^3.7.7'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.33176020e90c68450293.js'}}"}*

```diff
@@ -20,21 +20,25 @@
     },
     "description": "A Custom Jupyter Widget Library",
     "devDependencies": {
         "@babel/core": "^7.21.4",
         "@babel/preset-env": "^7.21.4",
         "@babel/preset-react": "^7.18.6",
         "@babel/preset-typescript": "^7.21.4",
+        "@emotion/react": "^11.11.0",
         "@jupyterlab/builder": "^3.6.3",
         "@lumino/application": "^2.1.0",
         "@lumino/widgets": "^2.1.0",
+        "@mantine/core": "^6.0.10",
+        "@mantine/hooks": "^6.0.10",
         "@types/react": "^17.0.2",
         "@types/react-dom": "^17.0.2",
         "@types/webpack": "^5.28.1",
         "@types/webpack-env": "^1.18.0",
+        "ahooks": "^3.7.7",
         "babel-loader": "^9.1.2",
         "css-loader": "^6.7.3",
         "fs-extra": "^11.1.1",
         "immer": "^10.0.1",
         "mkdirp": "^3.0.1",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.8.8",
@@ -51,15 +55,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/tidbcloud/react-editable-table",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b35d3910be71a545f174.js"
+            "load": "static/remoteEntry.33176020e90c68450293.js"
         },
         "extension": "lib/plugin",
         "outputDir": "react_editable_table/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
```

### Comparing `react_editable_table-0.0.1/react_editable_table/nbextension/index.js.LICENSE.txt` & `react_editable_table-0.0.2/react_editable_table/nbextension/index.js.LICENSE.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,23 @@
  *
  * Copyright (c) Facebook, Inc. and its affiliates.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE file in the root directory of this source tree.
  */
 
+/** @license React v16.13.1
+ * react-is.production.min.js
+ *
+ * Copyright (c) Facebook, Inc. and its affiliates.
+ *
+ * This source code is licensed under the MIT license found in the
+ * LICENSE file in the root directory of this source tree.
+ */
+
 /** @license React v17.0.2
  * react-dom.production.min.js
  *
  * Copyright (c) Facebook, Inc. and its affiliates.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE file in the root directory of this source tree.
```

### Comparing `react_editable_table-0.0.1/react_editable_table/widget.py` & `react_editable_table-0.0.2/react_editable_table/widget.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,34 +11,46 @@
 from ipywidgets import DOMWidget, CallbackDispatcher
 from traitlets import Unicode, List, Dict, validate
 
 from ._frontend import module_name, module_version
 
 
 class TableWidget(DOMWidget):
-    """TODO: Add docstring here"""
+    """A Grid Widget with filter, sort and selection capabilities.
 
-    _model_name = Unicode("ExampleModel").tag(sync=True)
+    Attributes
+    ----------
+    columns : List of dict
+        A list of dict with "accessor", "header", "editable" key, to control each row,
+    data : List of dict
+        Data to display
+    meta : dict
+        A dict containing any meta info, will be passed to on_cell_change callback when cell changed
+    """
+
+    _model_name = Unicode("TableModel").tag(sync=True)
     _model_module = Unicode(module_name).tag(sync=True)
     _model_module_version = Unicode(module_version).tag(sync=True)
-    _view_name = Unicode("ExampleView").tag(sync=True)
+    _view_name = Unicode("TableView").tag(sync=True)
     _view_module = Unicode(module_name).tag(sync=True)
     _view_module_version = Unicode(module_version).tag(sync=True)
 
     # Your widget state goes here. Make sure to update the corresponding
     # JavaScript widget state (defaultModelProperties) in widget.ts
-    value = Unicode("Jupyter").tag(sync=True)
     columns = List(Dict()).tag(sync=True)
     data = List(Dict()).tag(sync=True)
+    meta = Dict().tag(sync=True)
 
-    def __init__(self, columns, data, **kwargs):
+    def __init__(self, columns, data, meta, **kwargs):
         self.columns = columns
         self.data = data
+        self.meta = meta
         super().__init__(**kwargs)
         self._cell_change_handlers = CallbackDispatcher()
+        self._cell_change_handlers.callbacks
         self.on_msg(self.__handle_custom_msg)
 
     @validate("columns")
     def _validate_columns(self, proposal):
         value = proposal["value"]
         if not all(
             isinstance(item, dict)
@@ -49,16 +61,32 @@
         return value
 
     @validate("data")
     def _validate_columns(self, proposal):
         value = proposal["value"]
         return value
 
+    @validate("meta")
+    def _validate_meta(self, proposal):
+        value = proposal["value"]
+        return value
+
     def __handle_custom_msg(self, widget, content, buffers):
         if content["type"] == "cell-changed":
             self._cell_change_handlers(content["payload"])
 
     def on_cell_change(self, callback, remove=False):
+        """Register a callback to execute when a cell value changed.
+
+        The callback will be called with one argument, the dictionary
+        containing cell information with keys
+        "row", "column", "column_index", "value".
+
+        Parameters
+        ----------
+        remove: bool (optional)
+            Set to true to remove the callback from the list of callbacks.
+        """
         self._cell_change_handlers.register_callback(callback, remove=remove)
 
     def set_row_value(self, row):
         self._cell_change_handlers(row)
```

### Comparing `react_editable_table-0.0.1/react_editable_table.egg-info/PKG-INFO` & `react_editable_table-0.0.2/react_editable_table.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: react-editable-table
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Custom Jupyter Widget Library
 Home-page: https://github.com/tidbcloud/react-editable-table
 Author: zoubingwu
 Author-email: zoubingwu@gmail.com
 License: BSD
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
```

### Comparing `react_editable_table-0.0.1/setup.py` & `react_editable_table-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `react_editable_table-0.0.1/src/extension.ts` & `react_editable_table-0.0.2/src/extension.ts`

 * *Files identical despite different names*

### Comparing `react_editable_table-0.0.1/src/plugin.ts` & `react_editable_table-0.0.2/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `react_editable_table-0.0.1/src/react/model.ts` & `react_editable_table-0.0.2/src/react/model.ts`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 }
 
 interface MessageCellChanged {
   type: 'cell-changed';
   payload: {
     row: any;
     index: number;
+    meta?: any;
   };
 }
 
 type Message = MessageCellChanged;
 
 export function useModelMessenger() {
   const model = useModel();
```

### Comparing `react_editable_table-0.0.1/src/version.ts` & `react_editable_table-0.0.2/src/version.ts`

 * *Files identical despite different names*

### Comparing `react_editable_table-0.0.1/src/widget.ts` & `react_editable_table-0.0.2/src/widget.ts`

 * *Files 12% similar despite different names*

```diff
@@ -14,63 +14,63 @@
 interface Column {
   header: string;
   accessor: string;
   editable?: boolean;
 }
 
 export interface WidgetModelState {
-  value: string;
   columns: Column[];
   data: any[];
+  loading?: boolean;
+  meta?: Record<string, any>;
 }
 
 // Your widget state goes here. Make sure to update the corresponding
 // Python state in example.py
 const defaultModelProperties: WidgetModelState = {
-  value: 'Hello World',
   columns: [],
   data: [],
 };
 
-export class ExampleModel extends DOMWidgetModel {
+export class TableModel extends DOMWidgetModel {
   defaults() {
     return {
       ...super.defaults(),
-      _model_name: ExampleModel.model_name,
-      _model_module: ExampleModel.model_module,
-      _model_module_version: ExampleModel.model_module_version,
-      _view_name: ExampleModel.view_name,
-      _view_module: ExampleModel.view_module,
-      _view_module_version: ExampleModel.view_module_version,
+      _model_name: TableModel.model_name,
+      _model_module: TableModel.model_module,
+      _model_module_version: TableModel.model_module_version,
+      _view_name: TableModel.view_name,
+      _view_module: TableModel.view_module,
+      _view_module_version: TableModel.view_module_version,
       ...defaultModelProperties,
     };
   }
 
   static serializers: ISerializers = {
     ...DOMWidgetModel.serializers,
     // Add any extra serializers here
   };
 
-  static model_name = 'ExampleModel';
+  static model_name = 'TableModel';
   static model_module = MODULE_NAME;
   static model_module_version = MODULE_VERSION;
-  static view_name = 'ExampleView'; // Set to null if no view
+  static view_name = 'TableView'; // Set to null if no view
   static view_module = MODULE_NAME; // Set to null if no view
   static view_module_version = MODULE_VERSION;
 
   initialize(attributes: any, options: any) {
     super.initialize(attributes, options);
 
     this.on('msg:custom', (message) => {
       this.send(message);
     });
   }
 }
 
-export class ExampleView extends DOMWidgetView {
+export class TableView extends DOMWidgetView {
   render() {
     const component = React.createElement(ReactEditableTable, {
       model: this.model,
     });
     ReactDOM.render(component, this.el);
   }
 }
```

### Comparing `react_editable_table-0.0.1/tsconfig.json` & `react_editable_table-0.0.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `react_editable_table-0.0.1/webpack.config.js` & `react_editable_table-0.0.2/webpack.config.js`

 * *Files identical despite different names*

