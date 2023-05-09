# Comparing `tmp/flask-useful-0.2.0.tar.gz` & `tmp/flask-useful-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-useful-0.2.0.tar", last modified: Tue May  2 16:20:15 2023, max compression
+gzip compressed data, was "flask-useful-0.2.1.tar", last modified: Tue May  9 11:08:34 2023, max compression
```

## Comparing `flask-useful-0.2.0.tar` & `flask-useful-0.2.1.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.000060 flask-useful-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.000060 flask-useful-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-02 16:20:03.000000 flask-useful-0.2.0/.github/workflows/publish-stable.yml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-02 16:20:03.000000 flask-useful-0.2.0/.github/workflows/publish-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 16:20:03.000000 flask-useful-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-02 16:20:03.000000 flask-useful-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-02 16:20:15.004060 flask-useful-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 16:20:03.000000 flask-useful-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/examples/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/examples/blueprints/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/examples/blueprints/routes/api/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/examples/blueprints/routes/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/api/v1/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/examples/blueprints/routes/api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/api/v2/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/flask_useful/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/flask_access.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/sqla.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/flask_useful/wtforms/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/wtforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/wtforms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/wtforms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/wtforms/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/wtforms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/flask_useful.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-02 16:20:14.000000 flask-useful-0.2.0/flask_useful.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-02 16:20:15.000000 flask-useful-0.2.0/flask_useful.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:20:14.000000 flask-useful-0.2.0/flask_useful.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 16:20:14.000000 flask-useful-0.2.0/flask_useful.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 16:20:14.000000 flask-useful-0.2.0/flask_useful.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-02 16:20:03.000000 flask-useful-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:20:15.004060 flask-useful-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.550535 flask-useful-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.538535 flask-useful-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.542535 flask-useful-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-09 11:08:18.000000 flask-useful-0.2.1/.github/workflows/publish-stable.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-09 11:08:18.000000 flask-useful-0.2.1/.github/workflows/publish-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 11:08:18.000000 flask-useful-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-09 11:08:18.000000 flask-useful-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-09 11:08:34.546535 flask-useful-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 11:08:18.000000 flask-useful-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.542535 flask-useful-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-09 11:08:18.000000 flask-useful-0.2.1/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.542535 flask-useful-0.2.1/examples/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-09 11:08:18.000000 flask-useful-0.2.1/examples/blueprints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.542535 flask-useful-0.2.1/examples/blueprints/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:08:18.000000 flask-useful-0.2.1/examples/blueprints/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.542535 flask-useful-0.2.1/examples/blueprints/routes/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-09 11:08:18.000000 flask-useful-0.2.1/examples/blueprints/routes/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.542535 flask-useful-0.2.1/examples/blueprints/routes/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-09 11:08:18.000000 flask-useful-0.2.1/examples/blueprints/routes/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-09 11:08:18.000000 flask-useful-0.2.1/examples/blueprints/routes/api/v1/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.542535 flask-useful-0.2.1/examples/blueprints/routes/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-09 11:08:18.000000 flask-useful-0.2.1/examples/blueprints/routes/api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-09 11:08:18.000000 flask-useful-0.2.1/examples/blueprints/routes/api/v2/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-09 11:08:18.000000 flask-useful-0.2.1/examples/blueprints/routes/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-09 11:08:18.000000 flask-useful-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:08:34.550535 flask-useful-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.542535 flask-useful-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.546535 flask-useful-0.2.1/src/flask_useful/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/flask_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/sqla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.546535 flask-useful-0.2.1/src/flask_useful/wtforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/wtforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/wtforms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/wtforms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/wtforms/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-09 11:08:18.000000 flask-useful-0.2.1/src/flask_useful/wtforms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:08:34.546535 flask-useful-0.2.1/src/flask_useful.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-09 11:08:34.000000 flask-useful-0.2.1/src/flask_useful.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-09 11:08:34.000000 flask-useful-0.2.1/src/flask_useful.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:08:34.000000 flask-useful-0.2.1/src/flask_useful.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-09 11:08:34.000000 flask-useful-0.2.1/src/flask_useful.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 11:08:34.000000 flask-useful-0.2.1/src/flask_useful.egg-info/top_level.txt
```

### Comparing `flask-useful-0.2.0/.github/workflows/publish-stable.yml` & `flask-useful-0.2.1/.github/workflows/publish-stable.yml`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.0/.github/workflows/publish-test.yml` & `flask-useful-0.2.1/.github/workflows/publish-test.yml`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.0/LICENSE` & `flask-useful-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.0/PKG-INFO` & `flask-useful-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-useful
-Version: 0.2.0
+Version: 0.2.1
 Summary: A set of useful tools for the Flask microframework.
 Author-email: Kirill Vercetti <office@kyzima-spb.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/kyzima-spb/flask-useful
 Project-URL: Repository, https://github.com/kyzima-spb/flask-useful.git
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `flask-useful-0.2.0/flask_useful/app.py` & `flask-useful-0.2.1/src/flask_useful/app.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.0/flask_useful/flask_access.py` & `flask-useful-0.2.1/src/flask_useful/flask_access.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.0/flask_useful/sqla.py` & `flask-useful-0.2.1/src/flask_useful/sqla.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.0/flask_useful/utils.py` & `flask-useful-0.2.1/src/flask_useful/utils.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.0/flask_useful/views.py` & `flask-useful-0.2.1/src/flask_useful/views.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.0/flask_useful/wtforms/fields.py` & `flask-useful-0.2.1/src/flask_useful/wtforms/fields.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.0/flask_useful/wtforms/validators.py` & `flask-useful-0.2.1/src/flask_useful/wtforms/validators.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.0/flask_useful/wtforms/widgets.py` & `flask-useful-0.2.1/src/flask_useful/wtforms/widgets.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.2.0/flask_useful.egg-info/PKG-INFO` & `flask-useful-0.2.1/src/flask_useful.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-useful
-Version: 0.2.0
+Version: 0.2.1
 Summary: A set of useful tools for the Flask microframework.
 Author-email: Kirill Vercetti <office@kyzima-spb.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/kyzima-spb/flask-useful
 Project-URL: Repository, https://github.com/kyzima-spb/flask-useful.git
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `flask-useful-0.2.0/flask_useful.egg-info/SOURCES.txt` & `flask-useful-0.2.1/src/flask_useful.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 examples/blueprints/routes/__init__.py
 examples/blueprints/routes/docs.py
 examples/blueprints/routes/api/__init__.py
 examples/blueprints/routes/api/v1/__init__.py
 examples/blueprints/routes/api/v1/users.py
 examples/blueprints/routes/api/v2/__init__.py
 examples/blueprints/routes/api/v2/users.py
-flask_useful/__init__.py
-flask_useful/app.py
-flask_useful/decorators.py
-flask_useful/flask_access.py
-flask_useful/sqla.py
-flask_useful/utils.py
-flask_useful/views.py
-flask_useful.egg-info/PKG-INFO
-flask_useful.egg-info/SOURCES.txt
-flask_useful.egg-info/dependency_links.txt
-flask_useful.egg-info/requires.txt
-flask_useful.egg-info/top_level.txt
-flask_useful/wtforms/__init__.py
-flask_useful/wtforms/fields.py
-flask_useful/wtforms/filters.py
-flask_useful/wtforms/validators.py
-flask_useful/wtforms/widgets.py
+src/flask_useful/__init__.py
+src/flask_useful/app.py
+src/flask_useful/decorators.py
+src/flask_useful/flask_access.py
+src/flask_useful/mail.py
+src/flask_useful/py.typed
+src/flask_useful/sqla.py
+src/flask_useful/utils.py
+src/flask_useful/views.py
+src/flask_useful.egg-info/PKG-INFO
+src/flask_useful.egg-info/SOURCES.txt
+src/flask_useful.egg-info/dependency_links.txt
+src/flask_useful.egg-info/requires.txt
+src/flask_useful.egg-info/top_level.txt
+src/flask_useful/wtforms/__init__.py
+src/flask_useful/wtforms/fields.py
+src/flask_useful/wtforms/filters.py
+src/flask_useful/wtforms/validators.py
+src/flask_useful/wtforms/widgets.py
```

### Comparing `flask-useful-0.2.0/pyproject.toml` & `flask-useful-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -37,10 +37,10 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
 fallback_version = "0.0.0"
 
 [tool.mypy]
-files = ["flask_useful"]
+files = ["src/flask_useful"]
 python_version = "3.7"
 strict = true
```

