# Comparing `tmp/geomulticorr-0.1.1.tar.gz` & `tmp/geomulticorr-0.1.2.tar.gz`

## Comparing `geomulticorr-0.1.1.tar` & `geomulticorr-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/src/geomulticorr/__init__.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/src/geomulticorr/geomorph.py
--rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/src/geomulticorr/pair.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/src/geomulticorr/pzone.py
--rw-r--r--   0        0        0    20444 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/src/geomulticorr/session.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/src/geomulticorr/spine.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/src/geomulticorr/thumb.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/src/geomulticorr/xzone.py
--rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
--rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/src/geomulticorr/resources/project_template/map_template-project.qgz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/tests/test_geomorph.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/tests/test_pair.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/tests/test_pzone.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/tests/test_session.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/tests/test_thumb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/tests/test_xzone.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/LICENSE.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/__init__.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/geomorph.py
+-rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/pair.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/pzone.py
+-rw-r--r--   0        0        0    20444 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/session.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/spine.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/thumb.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/xzone.py
+-rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
+-rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/resources/project_template/map_template-project.qgz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/test_geomorph.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/test_pair.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/test_pzone.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/test_session.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/test_thumb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/test_xzone.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/PKG-INFO
```

### Comparing `geomulticorr-0.1.1/src/geomulticorr/geomorph.py` & `geomulticorr-0.1.2/src/geomulticorr/geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/src/geomulticorr/pair.py` & `geomulticorr-0.1.2/src/geomulticorr/pair.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/src/geomulticorr/pzone.py` & `geomulticorr-0.1.2/src/geomulticorr/pzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/src/geomulticorr/session.py` & `geomulticorr-0.1.2/src/geomulticorr/session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/src/geomulticorr/spine.py` & `geomulticorr-0.1.2/src/geomulticorr/spine.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/src/geomulticorr/thumb.py` & `geomulticorr-0.1.2/src/geomulticorr/thumb.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/src/geomulticorr/xzone.py` & `geomulticorr-0.1.2/src/geomulticorr/xzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/src/geomulticorr/resources/map_styles/vector-field_style_1.qml` & `geomulticorr-0.1.2/src/geomulticorr/resources/map_styles/vector-field_style_1.qml`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg` & `geomulticorr-0.1.2/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/src/geomulticorr/resources/project_template/map_template-project.qgz` & `geomulticorr-0.1.2/src/geomulticorr/resources/project_template/map_template-project.qgz`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/tests/test_geomorph.py` & `geomulticorr-0.1.2/tests/test_geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/tests/test_pair.py` & `geomulticorr-0.1.2/tests/test_pair.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/tests/test_pzone.py` & `geomulticorr-0.1.2/tests/test_pzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/tests/test_session.py` & `geomulticorr-0.1.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/tests/test_thumb.py` & `geomulticorr-0.1.2/tests/test_thumb.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/LICENSE.md` & `geomulticorr-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.1/pyproject.toml` & `geomulticorr-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geomulticorr"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Thibaut Duvanel", email="thibaut.duvanel@univ-smb.fr" },
 ]
 description = "A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `geomulticorr-0.1.1/PKG-INFO` & `geomulticorr-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomulticorr
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline
 Author-email: Thibaut Duvanel <thibaut.duvanel@univ-smb.fr>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

