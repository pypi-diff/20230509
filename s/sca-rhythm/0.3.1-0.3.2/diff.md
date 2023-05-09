# Comparing `tmp/sca_rhythm-0.3.1.tar.gz` & `tmp/sca_rhythm-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sca_rhythm-0.3.1.tar", max compression
+gzip compressed data, was "sca_rhythm-0.3.2.tar", max compression
```

## Comparing `sca_rhythm-0.3.1.tar` & `sca_rhythm-0.3.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.3.1/LICENSE.md
--rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.3.1/README.md
--rw-r--r--   0        0        0      358 2023-05-06 00:00:30.340969 sca_rhythm-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    15364 2023-05-06 00:00:07.562543 sca_rhythm-0.3.1/sca_rhythm/__init__.py
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 sca_rhythm-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.3.2/README.md
+-rw-r--r--   0        0        0      357 2023-05-09 02:24:40.562616 sca_rhythm-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    15364 2023-05-06 00:00:07.562543 sca_rhythm-0.3.2/sca_rhythm/__init__.py
+-rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 sca_rhythm-0.3.2/PKG-INFO
```

### Comparing `sca_rhythm-0.3.1/LICENSE.md` & `sca_rhythm-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.3.1/README.md` & `sca_rhythm-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.3.1/sca_rhythm/__init__.py` & `sca_rhythm-0.3.2/sca_rhythm/__init__.py`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.3.1/PKG-INFO` & `sca_rhythm-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: sca-rhythm
-Version: 0.3.1
+Version: 0.3.2
 Summary: Create and manage workflows using Celery tasks
 Author: Deepak Duggirala
 Author-email: deepakduggi@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: celery (>=5.2.7,<6.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Rhythm
 Rhythm allows you to design and control workflows made of Celery tasks. A workflow is a sequence of steps to run one after the other. Rhythm simplifies the process of executing workflows consisting of long-running tasks with reliability.
```

