# Comparing `tmp/scrippy-snmp-1.0.1.tar.gz` & `tmp/scrippy-snmp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrippy-snmp-1.0.1.tar", last modified: Mon May  8 11:53:55 2023, max compression
+gzip compressed data, was "scrippy-snmp-1.0.2.tar", last modified: Tue May  9 11:20:35 2023, max compression
```

## Comparing `scrippy-snmp-1.0.1.tar` & `scrippy-snmp-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:53:55.123368 scrippy-snmp-1.0.1/
--rwxr-xr-x   0 root         (0) root         (0)     1179 2023-05-08 11:52:48.000000 scrippy-snmp-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5852 2023-05-08 11:53:55.124368 scrippy-snmp-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5060 2023-05-08 11:52:48.000000 scrippy-snmp-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      210 2023-05-08 11:52:48.000000 scrippy-snmp-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1340 2023-05-08 11:53:55.145368 scrippy-snmp-1.0.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)       38 2023-05-08 11:52:48.000000 scrippy-snmp-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:53:55.061370 scrippy-snmp-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:53:55.077370 scrippy-snmp-1.0.1/src/scrippy_snmp/
--rw-r--r--   0 root         (0) root         (0)      768 2023-05-08 11:52:48.000000 scrippy-snmp-1.0.1/src/scrippy_snmp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:53:55.100369 scrippy-snmp-1.0.1/src/scrippy_snmp/snmp/
--rwxr-xr-x   0 root         (0) root         (0)     3525 2023-05-08 11:52:48.000000 scrippy-snmp-1.0.1/src/scrippy_snmp/snmp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:53:55.099369 scrippy-snmp-1.0.1/src/scrippy_snmp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5852 2023-05-08 11:53:54.000000 scrippy-snmp-1.0.1/src/scrippy_snmp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2023-05-08 11:53:55.000000 scrippy-snmp-1.0.1/src/scrippy_snmp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 11:53:54.000000 scrippy-snmp-1.0.1/src/scrippy_snmp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-08 11:53:54.000000 scrippy-snmp-1.0.1/src/scrippy_snmp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 11:53:54.000000 scrippy-snmp-1.0.1/src/scrippy_snmp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:53:55.109369 scrippy-snmp-1.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)     3484 2023-05-08 11:52:48.000000 scrippy-snmp-1.0.1/tests/test_snmp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:20:35.312242 scrippy-snmp-1.0.2/
+-rwxr-xr-x   0 root         (0) root         (0)     1179 2023-05-09 11:19:28.000000 scrippy-snmp-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-05-09 11:20:35.312242 scrippy-snmp-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5060 2023-05-09 11:19:28.000000 scrippy-snmp-1.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      210 2023-05-09 11:19:28.000000 scrippy-snmp-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-05-09 11:20:35.313242 scrippy-snmp-1.0.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)       38 2023-05-09 11:19:28.000000 scrippy-snmp-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:20:35.261243 scrippy-snmp-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:20:35.264243 scrippy-snmp-1.0.2/src/scrippy_snmp/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-05-09 11:19:28.000000 scrippy-snmp-1.0.2/src/scrippy_snmp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:20:35.282242 scrippy-snmp-1.0.2/src/scrippy_snmp/snmp/
+-rwxr-xr-x   0 root         (0) root         (0)     3539 2023-05-09 11:19:28.000000 scrippy-snmp-1.0.2/src/scrippy_snmp/snmp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:20:35.282242 scrippy-snmp-1.0.2/src/scrippy_snmp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-05-09 11:20:35.000000 scrippy-snmp-1.0.2/src/scrippy_snmp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-05-09 11:20:35.000000 scrippy-snmp-1.0.2/src/scrippy_snmp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 11:20:35.000000 scrippy-snmp-1.0.2/src/scrippy_snmp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-09 11:20:35.000000 scrippy-snmp-1.0.2/src/scrippy_snmp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 11:20:35.000000 scrippy-snmp-1.0.2/src/scrippy_snmp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 11:20:35.300242 scrippy-snmp-1.0.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     3484 2023-05-09 11:19:28.000000 scrippy-snmp-1.0.2/tests/test_snmp.py
```

### Comparing `scrippy-snmp-1.0.1/LICENSE` & `scrippy-snmp-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrippy-snmp-1.0.1/PKG-INFO` & `scrippy-snmp-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrippy-snmp
-Version: 1.0.1
+Version: 1.0.2
 Summary: "SNMP capabilities for Scrippy framework"
 Home-page: https://codeberg.org/scrippy/scrippy-snmp
 Author: Michael Costa, Florent Chevalier
 Author-email: michael.costa@mcos.nc, florent.chevalier.nc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scrippy-snmp-1.0.1/README.md` & `scrippy-snmp-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scrippy-snmp-1.0.1/setup.cfg` & `scrippy-snmp-1.0.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.0.1
+version = 1.0.2
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
```

### Comparing `scrippy-snmp-1.0.1/src/scrippy_snmp/__init__.py` & `scrippy-snmp-1.0.2/src/scrippy_snmp/__init__.py`

 * *Files identical despite different names*

### Comparing `scrippy-snmp-1.0.1/src/scrippy_snmp/snmp/__init__.py` & `scrippy-snmp-1.0.2/src/scrippy_snmp/snmp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     elif error_status > 0:
       err_index = "?"
       if error_index > 0:
         err_index = var_binds[int(error_index) - 1]
       err_msg = f"{error_status.prettyPrint()} at {err_index}"
     raise ScrippySnmpError(err_msg)
 
-  def walk(self, oid):
-    logging.info(f"[+] Retrieving OID {oid}")
+  def walk(self, oid=".1.3.6"):
+    logging.info(f"[+] Retrieving from OID {oid}")
     error_indication, error_status, error_index, var_binds = self.generator.nextCmd(self.community, self.transport, oid)
     if error_indication is None and error_status == 0:
       try:
         return [tuple(var[0].prettyPrint().split(" = ")) for var in var_binds]
       except IndexError as err:
         err_msg = f"Unexpected answer from remote host: {str(var_binds)}"
         raise ScrippySnmpError(err_msg) from err
```

### Comparing `scrippy-snmp-1.0.1/src/scrippy_snmp.egg-info/PKG-INFO` & `scrippy-snmp-1.0.2/src/scrippy_snmp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrippy-snmp
-Version: 1.0.1
+Version: 1.0.2
 Summary: "SNMP capabilities for Scrippy framework"
 Home-page: https://codeberg.org/scrippy/scrippy-snmp
 Author: Michael Costa, Florent Chevalier
 Author-email: michael.costa@mcos.nc, florent.chevalier.nc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scrippy-snmp-1.0.1/tests/test_snmp.py` & `scrippy-snmp-1.0.2/tests/test_snmp.py`

 * *Files identical despite different names*

