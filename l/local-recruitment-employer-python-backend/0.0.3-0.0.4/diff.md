# Comparing `tmp/local-recruitment-employer-python-backend-0.0.3.tar.gz` & `tmp/local-recruitment-employer-python-backend-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-recruitment-employer-python-backend-0.0.3.tar", last modified: Sat Apr 29 10:16:19 2023, max compression
+gzip compressed data, was "local-recruitment-employer-python-backend-0.0.4.tar", last modified: Tue May  9 07:59:12 2023, max compression
```

## Comparing `local-recruitment-employer-python-backend-0.0.3.tar` & `local-recruitment-employer-python-backend-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:16:19.608783 local-recruitment-employer-python-backend-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-29 10:16:19.608783 local-recruitment-employer-python-backend-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 10:16:01.000000 local-recruitment-employer-python-backend-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:16:19.608783 local-recruitment-employer-python-backend-0.0.3/local_recruitment_employer_python_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-29 10:16:19.000000 local-recruitment-employer-python-backend-0.0.3/local_recruitment_employer_python_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-29 10:16:19.000000 local-recruitment-employer-python-backend-0.0.3/local_recruitment_employer_python_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:16:19.000000 local-recruitment-employer-python-backend-0.0.3/local_recruitment_employer_python_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:16:19.000000 local-recruitment-employer-python-backend-0.0.3/local_recruitment_employer_python_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-29 10:16:01.000000 local-recruitment-employer-python-backend-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 10:16:19.608783 local-recruitment-employer-python-backend-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:59:12.843747 local-recruitment-employer-python-backend-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-09 07:59:12.843747 local-recruitment-employer-python-backend-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 07:58:58.000000 local-recruitment-employer-python-backend-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:59:12.843747 local-recruitment-employer-python-backend-0.0.4/local_recruitment_employer_python_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-09 07:59:12.000000 local-recruitment-employer-python-backend-0.0.4/local_recruitment_employer_python_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-09 07:59:12.000000 local-recruitment-employer-python-backend-0.0.4/local_recruitment_employer_python_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:59:12.000000 local-recruitment-employer-python-backend-0.0.4/local_recruitment_employer_python_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:59:12.000000 local-recruitment-employer-python-backend-0.0.4/local_recruitment_employer_python_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-09 07:58:58.000000 local-recruitment-employer-python-backend-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:59:12.843747 local-recruitment-employer-python-backend-0.0.4/setup.cfg
```

### Comparing `local-recruitment-employer-python-backend-0.0.3/pyproject.toml` & `local-recruitment-employer-python-backend-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "local-recruitment-employer-python-backend"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="circles-zone" , email="info@circles.zone"},
 ]
 description = "local-recruitment-employer-python-backend"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

