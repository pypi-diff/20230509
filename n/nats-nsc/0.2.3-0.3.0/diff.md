# Comparing `tmp/nats_nsc-0.2.3.tar.gz` & `tmp/nats_nsc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats_nsc-0.2.3.tar", last modified: Sun May  7 19:32:17 2023, max compression
+gzip compressed data, was "nats_nsc-0.3.0.tar", last modified: Tue May  9 18:35:05 2023, max compression
```

## Comparing `nats_nsc-0.2.3.tar` & `nats_nsc-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/LICENSE
--rw-r--r--   0        0        0      191 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/README.md
--rw-r--r--   0        0        0      730 2023-05-07 19:32:17.558712 nats_nsc-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4489 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/src/nats_nsc/__init__.py
--rw-r--r--   0        0        0     1826 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/src/nats_nsc/common.py
--rw-r--r--   0        0        0     2085 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/src/nats_nsc/nk.py
--rw-r--r--   0        0        0     5995 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/src/nats_nsc/nsc_utils.py
--rw-r--r--   0        0        0       68 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/.gitignore
--rw-r--r--   0        0        0       71 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/keys/DO_NOT_USE
--rw-r--r--   0        0        0       75 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/.nsc
--rw-r--r--   0        0        0     1582 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt
--rw-r--r--   0        0        0      646 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt
--rw-r--r--   0        0        0      745 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      562 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      668 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      175 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nsc.json
--rw-r--r--   0        0        0      891 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/test_nk.py
--rw-r--r--   0        0        0     1412 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/test_setup.py
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 nats_nsc-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-09 18:34:39.741829 nats_nsc-0.3.0/LICENSE
+-rw-r--r--   0        0        0      191 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/README.md
+-rw-r--r--   0        0        0      777 2023-05-09 18:35:05.242029 nats_nsc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/src/nats_nsc/__init__.py
+-rw-r--r--   0        0        0     6302 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/src/nats_nsc/common.py
+-rw-r--r--   0        0        0     3945 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/src/nats_nsc/create_user.py
+-rw-r--r--   0        0        0     3327 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nats.cfg
+-rw-r--r--   0        0        0       68 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/.gitignore
+-rw-r--r--   0        0        0       71 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/keys/DO_NOT_USE
+-rw-r--r--   0        0        0       75 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/.nsc
+-rw-r--r--   0        0        0     1582 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt
+-rw-r--r--   0        0        0      646 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt
+-rw-r--r--   0        0        0      745 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      562 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      668 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      175 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/nsc_workdir/nsc.json
+-rw-r--r--   0        0        0      980 2023-05-09 18:34:39.745829 nats_nsc-0.3.0/tests/test_basic.py
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 nats_nsc-0.3.0/PKG-INFO
```

### Comparing `nats_nsc-0.2.3/LICENSE` & `nats_nsc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.3/pyproject.toml` & `nats_nsc-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 [tool.pytest.ini_options]
 pythonpath = [
     "src/",
 ]
 
 [project]
 name = "nats-nsc"
-version = "0.2.3"
-description = "Python wrapper for nsc, nats credential manager"
+version = "0.3.0"
+description = "Limited python nsc utility equivalent, for user creation and signing JWTs."
 authors = [
     { name = "Mikołaj Nowak", email = "12396461+m3nowak@users.noreply.github.com" },
 ]
 dependencies = [
     "pyJWT~=2.6.0",
     "aiofiles~=23.1.0",
+    "nkeys~=0.1.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt` & `nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt` & `nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt` & `nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt` & `nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt` & `nats_nsc-0.3.0/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt`

 * *Files identical despite different names*

