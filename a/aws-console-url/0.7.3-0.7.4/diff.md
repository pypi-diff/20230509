# Comparing `tmp/aws_console_url-0.7.3.tar.gz` & `tmp/aws_console_url-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_console_url-0.7.3.tar", last modified: Mon Mar 13 13:16:40 2023, max compression
+gzip compressed data, was "aws_console_url-0.7.4.tar", last modified: Tue May  9 19:41:36 2023, max compression
```

## Comparing `aws_console_url-0.7.3.tar` & `aws_console_url-0.7.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-13 13:16:40.106062 aws_console_url-0.7.3/
--rw-r--r--   0 sanhehu    (505) staff       (20)      509 2022-12-20 15:00:45.000000 aws_console_url-0.7.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     1125 2022-12-20 15:00:45.000000 aws_console_url-0.7.3/LICENSE.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      323 2022-12-20 15:00:44.000000 aws_console_url-0.7.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)     3983 2023-03-13 13:16:40.105858 aws_console_url-0.7.3/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)    15928 2023-03-13 13:07:44.000000 aws_console_url-0.7.3/Public-API.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     2905 2023-02-03 16:36:24.000000 aws_console_url-0.7.3/README.rst
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-13 13:16:40.079663 aws_console_url-0.7.3/aws_console_url/
--rw-r--r--   0 sanhehu    (505) staff       (20)      427 2023-02-03 17:52:26.000000 aws_console_url-0.7.3/aws_console_url/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-03-13 13:13:56.000000 aws_console_url-0.7.3/aws_console_url/_version.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      336 2023-01-14 04:05:55.000000 aws_console_url-0.7.3/aws_console_url/compat.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     3555 2023-03-13 13:07:44.000000 aws_console_url-0.7.3/aws_console_url/console.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-13 13:16:40.086700 aws_console_url-0.7.3/aws_console_url/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2022-12-20 15:00:45.000000 aws_console_url-0.7.3/aws_console_url/docs/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     6437 2023-02-05 14:00:22.000000 aws_console_url-0.7.3/aws_console_url/model.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1213 2023-03-13 13:07:44.000000 aws_console_url-0.7.3/aws_console_url/resource.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-13 13:16:40.101355 aws_console_url-0.7.3/aws_console_url/srv/
--rw-r--r--   0 sanhehu    (505) staff       (20)       45 2022-12-20 15:03:32.000000 aws_console_url-0.7.3/aws_console_url/srv/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2769 2023-02-03 15:09:41.000000 aws_console_url-0.7.3/aws_console_url/srv/a2i.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5747 2023-02-03 03:49:41.000000 aws_console_url-0.7.3/aws_console_url/srv/awslambda.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    14455 2023-03-13 13:11:35.000000 aws_console_url-0.7.3/aws_console_url/srv/cloudformation.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     4619 2023-02-21 19:29:04.000000 aws_console_url-0.7.3/aws_console_url/srv/cloudwatch.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5455 2023-02-03 04:28:28.000000 aws_console_url-0.7.3/aws_console_url/srv/codebuild.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     4116 2023-02-03 12:49:50.000000 aws_console_url-0.7.3/aws_console_url/srv/codecommit.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1617 2023-02-03 15:07:45.000000 aws_console_url-0.7.3/aws_console_url/srv/dynamodb.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1831 2023-02-03 16:53:57.000000 aws_console_url-0.7.3/aws_console_url/srv/ec2.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1553 2023-02-03 17:22:40.000000 aws_console_url-0.7.3/aws_console_url/srv/ecr.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     4386 2023-02-03 15:06:06.000000 aws_console_url-0.7.3/aws_console_url/srv/glue.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1596 2023-02-03 15:12:36.000000 aws_console_url-0.7.3/aws_console_url/srv/ground_truth.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     4917 2023-02-03 03:28:33.000000 aws_console_url-0.7.3/aws_console_url/srv/iam.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2502 2023-02-05 14:45:44.000000 aws_console_url-0.7.3/aws_console_url/srv/s3.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1207 2023-02-03 17:57:59.000000 aws_console_url-0.7.3/aws_console_url/srv/sagemaker.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      857 2023-02-03 17:11:02.000000 aws_console_url-0.7.3/aws_console_url/srv/secretmanager.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1834 2023-02-03 03:41:51.000000 aws_console_url-0.7.3/aws_console_url/srv/sqs.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1546 2023-02-03 17:05:35.000000 aws_console_url-0.7.3/aws_console_url/srv/ssm.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5562 2023-02-03 16:10:31.000000 aws_console_url-0.7.3/aws_console_url/srv/step_function.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2810 2023-02-05 15:22:37.000000 aws_console_url-0.7.3/aws_console_url/srv/vpc.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-13 13:16:40.103390 aws_console_url-0.7.3/aws_console_url/tests/
--rw-r--r--   0 sanhehu    (505) staff       (20)      352 2023-03-07 17:38:29.000000 aws_console_url-0.7.3/aws_console_url/tests/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1215 2023-02-03 15:55:58.000000 aws_console_url-0.7.3/aws_console_url/tests/helper.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      370 2022-12-07 01:32:30.000000 aws_console_url-0.7.3/aws_console_url/tests/paths.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-13 13:16:40.086127 aws_console_url-0.7.3/aws_console_url.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)     3983 2023-03-13 13:16:39.000000 aws_console_url-0.7.3/aws_console_url.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     1322 2023-03-13 13:16:39.000000 aws_console_url-0.7.3/aws_console_url.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-03-13 13:16:39.000000 aws_console_url-0.7.3/aws_console_url.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      300 2023-03-13 13:16:39.000000 aws_console_url-0.7.3/aws_console_url.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       16 2023-03-13 13:16:39.000000 aws_console_url-0.7.3/aws_console_url.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)     2224 2023-03-13 13:14:49.000000 aws_console_url-0.7.3/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      297 2023-01-14 04:43:04.000000 aws_console_url-0.7.3/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      621 2022-12-20 15:00:45.000000 aws_console_url-0.7.3/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      189 2023-01-14 04:43:20.000000 aws_console_url-0.7.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      117 2023-01-14 04:42:47.000000 aws_console_url-0.7.3/requirements.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-03-13 13:16:40.106120 aws_console_url-0.7.3/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     7661 2023-01-14 06:27:10.000000 aws_console_url-0.7.3/setup.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-03-13 13:16:40.105467 aws_console_url-0.7.3/tests/
--rw-r--r--   0 sanhehu    (505) staff       (20)      290 2023-01-15 18:07:31.000000 aws_console_url-0.7.3/tests/test_builder.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1658 2023-03-13 13:07:44.000000 aws_console_url-0.7.3/tests/test_import.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.026028 aws_console_url-0.7.4/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      323 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3983 2023-05-09 19:41:36.025890 aws_console_url-0.7.4/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)    15928 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/Public-API.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2905 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.022227 aws_console_url-0.7.4/aws_console_url/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-09 19:39:37.000000 aws_console_url-0.7.4/aws_console_url/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      336 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/compat.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3555 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/console.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.022886 aws_console_url-0.7.4/aws_console_url/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6437 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/model.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1213 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/resource.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.025198 aws_console_url-0.7.4/aws_console_url/srv/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       45 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2769 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/a2i.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5747 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/awslambda.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    14455 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/cloudformation.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4619 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/cloudwatch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5455 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/codebuild.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4116 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/codecommit.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1617 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1831 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1553 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/ecr.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4386 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/glue.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1596 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/ground_truth.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4917 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/iam.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2502 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/s3.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1207 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/sagemaker.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      857 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/secretmanager.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1834 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/sqs.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1607 2023-05-09 19:38:31.000000 aws_console_url-0.7.4/aws_console_url/srv/ssm.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5552 2023-05-09 19:36:47.000000 aws_console_url-0.7.4/aws_console_url/srv/step_function.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2810 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/srv/vpc.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.025515 aws_console_url-0.7.4/aws_console_url/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      352 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1215 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/aws_console_url/tests/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.022776 aws_console_url-0.7.4/aws_console_url.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3983 2023-05-09 19:41:35.000000 aws_console_url-0.7.4/aws_console_url.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1322 2023-05-09 19:41:36.000000 aws_console_url-0.7.4/aws_console_url.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-09 19:41:35.000000 aws_console_url-0.7.4/aws_console_url.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      300 2023-05-09 19:41:36.000000 aws_console_url-0.7.4/aws_console_url.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       16 2023-05-09 19:41:36.000000 aws_console_url-0.7.4/aws_console_url.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2424 2023-05-09 19:41:20.000000 aws_console_url-0.7.4/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      297 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      189 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      117 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-09 19:41:36.026066 aws_console_url-0.7.4/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7661 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-09 19:41:36.025724 aws_console_url-0.7.4/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      290 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/tests/test_builder.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1658 2023-05-09 19:32:30.000000 aws_console_url-0.7.4/tests/test_import.py
```

### Comparing `aws_console_url-0.7.3/LICENSE.txt` & `aws_console_url-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/PKG-INFO` & `aws_console_url-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_console_url
-Version: 0.7.3
+Version: 0.7.4
 Summary: Build AWS Console Url for debugging.
 Home-page: https://github.com/MacHu-GWU/aws_console_url-project
-Download-URL: https://pypi.python.org/pypi/aws_console_url/0.7.3#downloads
+Download-URL: https://pypi.python.org/pypi/aws_console_url/0.7.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_console_url-0.7.3/Public-API.rst` & `aws_console_url-0.7.4/Public-API.rst`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/README.rst` & `aws_console_url-0.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/console.py` & `aws_console_url-0.7.4/aws_console_url/console.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/model.py` & `aws_console_url-0.7.4/aws_console_url/model.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/resource.py` & `aws_console_url-0.7.4/aws_console_url/resource.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/a2i.py` & `aws_console_url-0.7.4/aws_console_url/srv/a2i.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/awslambda.py` & `aws_console_url-0.7.4/aws_console_url/srv/awslambda.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/cloudformation.py` & `aws_console_url-0.7.4/aws_console_url/srv/cloudformation.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/cloudwatch.py` & `aws_console_url-0.7.4/aws_console_url/srv/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/codebuild.py` & `aws_console_url-0.7.4/aws_console_url/srv/codebuild.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/codecommit.py` & `aws_console_url-0.7.4/aws_console_url/srv/codecommit.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/dynamodb.py` & `aws_console_url-0.7.4/aws_console_url/srv/dynamodb.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/ec2.py` & `aws_console_url-0.7.4/aws_console_url/srv/ec2.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/ecr.py` & `aws_console_url-0.7.4/aws_console_url/srv/ecr.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/glue.py` & `aws_console_url-0.7.4/aws_console_url/srv/glue.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/ground_truth.py` & `aws_console_url-0.7.4/aws_console_url/srv/ground_truth.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/iam.py` & `aws_console_url-0.7.4/aws_console_url/srv/iam.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/s3.py` & `aws_console_url-0.7.4/aws_console_url/srv/s3.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/sagemaker.py` & `aws_console_url-0.7.4/aws_console_url/srv/sagemaker.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/secretmanager.py` & `aws_console_url-0.7.4/aws_console_url/srv/secretmanager.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/sqs.py` & `aws_console_url-0.7.4/aws_console_url/srv/sqs.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/ssm.py` & `aws_console_url-0.7.4/aws_console_url/srv/ssm.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,11 +44,13 @@
         return (
             f"{self._service_root}/parameters"
             f"/?region={self._region}&tab=Table#list_parameter_filters={search}"
         )
 
     def get_parameter(self, name_or_arn: str) -> str:
         name = self._ensure_name(name_or_arn, self._parameter_arn_to_name)
+        if name.startswith("/"):
+            name = name[1:]
         return (
             f"{self._service_root}/parameters"
             f"/{name}/description?region={self._region}&tab=Table"
         )
```

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/step_function.py` & `aws_console_url-0.7.4/aws_console_url/srv/step_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     @lru_cache(maxsize=32)
     def _get_state_machine_details(self, name_or_arn: str) -> dict:
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_state_machine
         """
         arn = self._ensure_arn(name_or_arn, self.get_state_machine_arn)
-        return self._bsm.stepfunctions_client.describe_state_machine(
+        return self._bsm.sfn_client.describe_state_machine(
             stateMachineArn=arn,
         )
 
     def _is_state_machine_type_standard(self, name_or_arn: str) -> bool:
         return self._get_state_machine_details(name_or_arn)["type"] == "STANDARD"
 
     # --- arn
```

### Comparing `aws_console_url-0.7.3/aws_console_url/srv/vpc.py` & `aws_console_url-0.7.4/aws_console_url/srv/vpc.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url/tests/helper.py` & `aws_console_url-0.7.4/aws_console_url/tests/helper.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/aws_console_url.egg-info/PKG-INFO` & `aws_console_url-0.7.4/aws_console_url.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws-console-url
-Version: 0.7.3
+Version: 0.7.4
 Summary: Build AWS Console Url for debugging.
 Home-page: https://github.com/MacHu-GWU/aws_console_url-project
-Download-URL: https://pypi.python.org/pypi/aws_console_url/0.7.3#downloads
+Download-URL: https://pypi.python.org/pypi/aws_console_url/0.7.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_console_url-0.7.3/aws_console_url.egg-info/SOURCES.txt` & `aws_console_url-0.7.4/aws_console_url.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/release-history.rst` & `aws_console_url-0.7.4/release-history.rst`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.7.4 (2023-05-09)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a bug that when SSM parameter has a prefix "/", the console url is not correct.
+
+
 0.7.3 (2023-03-13)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - cloudformation ``get_stack_set_xxx`` method now take name, stack_set_id or arn.
```

### Comparing `aws_console_url-0.7.3/requirements-doc.txt` & `aws_console_url-0.7.4/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/setup.py` & `aws_console_url-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.3/tests/test_import.py` & `aws_console_url-0.7.4/tests/test_import.py`

 * *Files identical despite different names*

