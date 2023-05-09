# Comparing `tmp/daktari-0.0.96.tar.gz` & `tmp/daktari-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daktari-0.0.96.tar", last modified: Mon May  8 07:14:05 2023, max compression
+gzip compressed data, was "daktari-0.0.97.tar", last modified: Tue May  9 09:15:10 2023, max compression
```

## Comparing `daktari-0.0.96.tar` & `daktari-0.0.97.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:14:05.140724 daktari-0.0.96/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-08 07:13:53.000000 daktari-0.0.96/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 07:13:53.000000 daktari-0.0.96/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-08 07:14:05.136724 daktari-0.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-08 07:13:54.000000 daktari-0.0.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:14:05.136724 daktari-0.0.96/daktari/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 07:13:54.000000 daktari-0.0.96/daktari/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/check_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/check_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/check_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:14:05.136724 daktari-0.0.96/daktari/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/direnv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/flutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/intellij_idea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/nodejs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/onepassword.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/test_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/test_java.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/test_yarn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/checks/yarn.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/collection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/command_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/os.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/resource_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:14:05.136724 daktari-0.0.96/daktari/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/resources/daktari-local-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/resources/mock_cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/result_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/test_check_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/test_check_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/test_check_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/test_collection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/test_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-08 07:13:53.000000 daktari-0.0.96/daktari/version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:14:05.136724 daktari-0.0.96/daktari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-08 07:14:05.000000 daktari-0.0.96/daktari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-08 07:14:05.000000 daktari-0.0.96/daktari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:14:05.000000 daktari-0.0.96/daktari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 07:14:05.000000 daktari-0.0.96/daktari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-08 07:14:05.000000 daktari-0.0.96/daktari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 07:14:05.000000 daktari-0.0.96/daktari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-08 07:13:53.000000 daktari-0.0.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-08 07:13:53.000000 daktari-0.0.96/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:14:05.140724 daktari-0.0.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 07:13:54.000000 daktari-0.0.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:15:10.584625 daktari-0.0.97/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-09 09:14:59.000000 daktari-0.0.97/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 09:14:59.000000 daktari-0.0.97/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-09 09:15:10.584625 daktari-0.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-09 09:15:01.000000 daktari-0.0.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:15:10.580625 daktari-0.0.97/daktari/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 09:15:01.000000 daktari-0.0.97/daktari/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1427 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/check_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/check_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/check_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:15:10.584625 daktari-0.0.97/daktari/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/direnv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/flutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/intellij_idea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/nodejs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/onepassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/test_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/test_java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/test_yarn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/yarn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/command_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/resource_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:15:10.584625 daktari-0.0.97/daktari/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/resources/daktari-local-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/resources/mock_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/result_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_check_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_check_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_check_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_result_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:15:10.580625 daktari-0.0.97/daktari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-09 09:15:10.000000 daktari-0.0.97/daktari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-09 09:15:10.000000 daktari-0.0.97/daktari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:15:10.000000 daktari-0.0.97/daktari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 09:15:10.000000 daktari-0.0.97/daktari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-09 09:15:10.000000 daktari-0.0.97/daktari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 09:15:10.000000 daktari-0.0.97/daktari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-09 09:14:59.000000 daktari-0.0.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-09 09:14:59.000000 daktari-0.0.97/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:15:10.584625 daktari-0.0.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-09 09:15:01.000000 daktari-0.0.97/setup.py
```

### Comparing `daktari-0.0.96/LICENSE.txt` & `daktari-0.0.97/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/PKG-INFO` & `daktari-0.0.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daktari
-Version: 0.0.96
+Version: 0.0.97
 Summary: Assist in setting up and maintaining developer environments
 Home-page: https://github.com/sonocent/daktari
 Author: Matt Russell
 Author-email: matthew.russell@sonocent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 ## Configuration
 
 In the root of the project repository, create a `.daktari.py` configuration file listing the checks you want run. For example,
 
 ```python
 from daktari.checks.git import *
 
-version = "0.0.96"
+version = "0.0.97"
 title = "My Project"
 
 checks = [
     GitInstalled(),
     GitLfsInstalled(),
     GitLfsSetUpForUser(),
     GitLfsFilesDownloaded(),
```

### Comparing `daktari-0.0.96/README.md` & `daktari-0.0.97/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## Configuration
 
 In the root of the project repository, create a `.daktari.py` configuration file listing the checks you want run. For example,
 
 ```python
 from daktari.checks.git import *
 
-version = "0.0.96"
+version = "0.0.97"
 title = "My Project"
 
 checks = [
     GitInstalled(),
     GitLfsInstalled(),
     GitLfsSetUpForUser(),
     GitLfsFilesDownloaded(),
```

### Comparing `daktari-0.0.96/daktari/__main__.py` & `daktari-0.0.97/daktari/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     config = read_config(args.config_path)
     if config is None:
         return 1
 
     os.chdir(args.config_path.parent.absolute())
     print_config_messages(config, args)
 
-    all_passed = run_checks(config.checks)
+    all_passed = run_checks(config.checks, args.quiet_mode or config.quiet_mode)
     print("")
     return 0 if all_passed else 1
 
 
 def print_config_messages(config: Config, args):
     if config.title:
         print_logo(config.title)
```

### Comparing `daktari-0.0.96/daktari/check.py` & `daktari-0.0.97/daktari/check.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/check_runner.py` & `daktari-0.0.97/daktari/check_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,47 +5,47 @@
 
 from daktari.check import Check, CheckStatus, CheckResult
 from daktari.check_sorter import sort_checks
 from daktari.os import detect_os
 from daktari.result_printer import print_check_result
 
 
-def run_checks(checks: List[Check]) -> bool:
-    return CheckRunner(checks).run()
+def run_checks(checks: List[Check], hide_passing_checks: bool) -> bool:
+    return CheckRunner(checks, hide_passing_checks).run()
 
 
 class CheckRunner:
-    def __init__(self, checks: List[Check]):
-        self.checks = checks
+    def __init__(self, checks: List[Check], quiet_mode: bool):
+        self.checks = [check for check in checks if check.run_on is None or check.run_on == detect_os()]
         self.all_passed = True
         self.checks_passed: Set[str] = set()
+        self.quiet_mode = quiet_mode
 
     def run(self) -> bool:
-        for check in sort_checks(self.checks):
-            self.try_run_check(check)
+        for idx, check in enumerate(sort_checks(self.checks)):
+            self.try_run_check(idx, check)
         return self.all_passed
 
-    def try_run_check(self, check: Check):
-        if check.run_on and check.run_on != detect_os():
-            return
+    def try_run_check(self, idx: int, check: Check):
         dependencies_met = all([dependency.name in self.checks_passed for dependency in check.depends_on])
         if dependencies_met:
-            self.run_check(check)
+            self.run_check(idx, check)
         else:
             self.diagnose_missing_dependency(check)
 
-    def run_check(self, check: Check):
+    def run_check(self, idx: int, check: Check):
         logging.info(f"Running check {check.name}")
         result = self.run_check_in_try(check)
-        print_check_result(result)
         if result.status in (CheckStatus.PASS, CheckStatus.PASS_WITH_WARNING):
             self.checks_passed.add(check.name)
         else:
             self.all_passed = False
 
+        print_check_result(result, self.quiet_mode, idx, len(self.checks))
+
     def run_check_in_try(self, check: Check) -> CheckResult:
         try:
             return check.check()
         except Exception as err:
             logging.debug(f"Exception running check {check.name}", exc_info=True)
             return CheckResult(check.name, CheckStatus.ERROR, f"Check failed with unhandled {type(err).__name__}", {})
```

### Comparing `daktari-0.0.96/daktari/check_sorter.py` & `daktari-0.0.97/daktari/check_sorter.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/check_utils.py` & `daktari-0.0.97/daktari/check_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/certs.py` & `daktari-0.0.97/daktari/checks/certs.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/direnv.py` & `daktari-0.0.97/daktari/checks/direnv.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/docker.py` & `daktari-0.0.97/daktari/checks/docker.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/files.py` & `daktari-0.0.97/daktari/checks/files.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/flutter.py` & `daktari-0.0.97/daktari/checks/flutter.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/git.py` & `daktari-0.0.97/daktari/checks/git.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/google.py` & `daktari-0.0.97/daktari/checks/google.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/intellij_idea.py` & `daktari-0.0.97/daktari/checks/intellij_idea.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/java.py` & `daktari-0.0.97/daktari/checks/java.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/kubernetes.py` & `daktari-0.0.97/daktari/checks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/misc.py` & `daktari-0.0.97/daktari/checks/misc.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/nodejs.py` & `daktari-0.0.97/daktari/checks/nodejs.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/onepassword.py` & `daktari-0.0.97/daktari/checks/onepassword.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/python.py` & `daktari-0.0.97/daktari/checks/python.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/ssh.py` & `daktari-0.0.97/daktari/checks/ssh.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/terraform.py` & `daktari-0.0.97/daktari/checks/terraform.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/test_certs.py` & `daktari-0.0.97/daktari/checks/test_certs.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/test_java.py` & `daktari-0.0.97/daktari/checks/test_java.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/test_ssh.py` & `daktari-0.0.97/daktari/checks/test_ssh.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/test_yarn.py` & `daktari-0.0.97/daktari/checks/test_yarn.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/xml.py` & `daktari-0.0.97/daktari/checks/xml.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/checks/yarn.py` & `daktari-0.0.97/daktari/checks/yarn.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/command_utils.py` & `daktari-0.0.97/daktari/command_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/config.py` & `daktari-0.0.97/daktari/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 @dataclass
 class Config:
     min_version: Optional[str]
     title: Optional[str]
     checks: List[Check]
     ignored_checks: List[Check] = field(default_factory=list)
+    quiet_mode: bool = False
 
 
 version_regex = re.compile('daktari_version.*"([0-9.]+)"')
 LOCAL_CONFIG_PATH = ".daktari-local.yaml"
 LOCAL_CONFIG_TEMPLATE = "daktari-local-template.yaml"
 
 
@@ -51,15 +52,20 @@
         return None
 
     # E.g. the file has been entirely commented out
     if local_config is None:
         return config
 
     ignored_checks: List[str] = local_config.get("ignoredChecks", [])
-    return remove_ignored_checks(config, ignored_checks)
+    updated_config = remove_ignored_checks(config, ignored_checks)
+
+    if local_config.get("alwaysQuiet", False):
+        updated_config = replace(updated_config, quiet_mode=True)
+
+    return updated_config
 
 
 def write_local_config_template():
     contents = get_resource(LOCAL_CONFIG_TEMPLATE)
     with open(LOCAL_CONFIG_PATH, "w") as config_file:
         config_file.write(contents)
```

### Comparing `daktari-0.0.96/daktari/file_utils.py` & `daktari-0.0.97/daktari/file_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/options.py` & `daktari-0.0.97/daktari/options.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 argument_parser.add_argument(
     "-g", "--generate-local-config", action="store_true", help="generate a template file for local configuration"
 )
 argument_parser.add_argument(
     "-i", "--show-ignored", action="store_true", help="show checks affected by ignoredChecks local setting"
 )
 argument_parser.add_argument(
+    "-q", "--quiet", action="store_true", dest="quiet_mode", help="only show failed checks and overall progress"
+)
+argument_parser.add_argument(
     "-c",
     "--config",
     default=".daktari.py",
     dest="config_path",
     required=False,
     help="Python configuration file",
     metavar="FILE",
```

### Comparing `daktari-0.0.96/daktari/os.py` & `daktari-0.0.97/daktari/os.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/result_printer.py` & `daktari-0.0.97/daktari/result_printer.py`

 * *Files 25% similar despite different names*

```diff
@@ -50,16 +50,36 @@
         if len(raw_lines) > 1:
             print(f"  {line}")
         else:
             print(f"│ {line}{padding} │")
     print("└" + "─" * (max_width + 2) + "┘")
 
 
-def print_check_result(result: CheckResult):
+def print_check_result(result: CheckResult, quiet_mode: bool, idx: int, total_checks: int):
     this_os = detect_os()
     status_symbol = check_status_symbol(result.status)
     colour = check_status_colour(result.status)
-    print(f"{status_symbol} [{colour(result.name)}] {result.summary}")
-    if result.status in (CheckStatus.FAIL, CheckStatus.PASS_WITH_WARNING):
-        suggestion = get_most_specific_suggestion(this_os, result.suggestions)
-        if suggestion:
-            print_suggestion_text(suggestion)
+    if result.status != CheckStatus.PASS or not quiet_mode:
+        print(f"{status_symbol} [{colour(result.name)}] {result.summary}")
+        if result.status in (CheckStatus.FAIL, CheckStatus.PASS_WITH_WARNING):
+            suggestion = get_most_specific_suggestion(this_os, result.suggestions)
+            if suggestion:
+                print_suggestion_text(suggestion)
+        if quiet_mode:
+            print("")
+
+    if quiet_mode:
+        print_progress_bar(idx + 1, total_checks)
+
+
+def print_progress_bar(current: int, total: int):
+    end_char = "\r" if current < total else "\n"
+    print(progress_bar(current, total), end=end_char)
+
+
+def progress_bar(current: int, total: int) -> str:
+    fraction = current / total
+
+    arrow = int(fraction * 25 - 1) * "-" + ">"
+    padding = int(25 - len(arrow)) * " "
+
+    return f"Progress: [{arrow}{padding}] {int(fraction*100)}%  ({current}/{total})"
```

### Comparing `daktari-0.0.96/daktari/test_check.py` & `daktari-0.0.97/daktari/test_check.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/test_check_factory.py` & `daktari-0.0.97/daktari/test_check_factory.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/test_check_sorter.py` & `daktari-0.0.97/daktari/test_check_sorter.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/test_check_utils.py` & `daktari-0.0.97/daktari/test_check_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/test_config.py` & `daktari-0.0.97/daktari/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import unittest
+from dataclasses import replace
 from io import StringIO
 from pathlib import Path
 from unittest.mock import patch
 
 from colors import red, yellow
 from packaging import version
 from packaging.version import Version
@@ -107,14 +108,22 @@
     def test_local_config_empty_ignored_checks(self):
         self.write_to_local_config("ignoredChecks: []")
 
         config = Config(None, None, TEST_CHECKS)
         updated_config = apply_local_config(config)
         self.assertEqual(config, updated_config)
 
+    def test_local_config_always_quiet(self):
+        self.write_to_local_config("alwaysQuiet: true")
+
+        config = Config(None, None, TEST_CHECKS)
+        expected_config = replace(config, quiet_mode=True)
+        updated_config = apply_local_config(config)
+        self.assertEqual(expected_config, updated_config)
+
     def test_generate_local_config(self):
         write_local_config_template()
 
         expected_contents = get_resource(LOCAL_CONFIG_TEMPLATE)
         with open(LOCAL_CONFIG_PATH, "r", encoding="utf-8") as local_config_file:
             actual_contents = local_config_file.read()
             self.assertEqual(expected_contents, actual_contents)
```

### Comparing `daktari-0.0.96/daktari/test_version_utils.py` & `daktari-0.0.97/daktari/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari/version_utils.py` & `daktari-0.0.97/daktari/version_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/daktari.egg-info/PKG-INFO` & `daktari-0.0.97/daktari.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daktari
-Version: 0.0.96
+Version: 0.0.97
 Summary: Assist in setting up and maintaining developer environments
 Home-page: https://github.com/sonocent/daktari
 Author: Matt Russell
 Author-email: matthew.russell@sonocent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 ## Configuration
 
 In the root of the project repository, create a `.daktari.py` configuration file listing the checks you want run. For example,
 
 ```python
 from daktari.checks.git import *
 
-version = "0.0.96"
+version = "0.0.97"
 title = "My Project"
 
 checks = [
     GitInstalled(),
     GitLfsInstalled(),
     GitLfsSetUpForUser(),
     GitLfsFilesDownloaded(),
```

### Comparing `daktari-0.0.96/daktari.egg-info/SOURCES.txt` & `daktari-0.0.97/daktari.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 daktari/result_printer.py
 daktari/test_check.py
 daktari/test_check_factory.py
 daktari/test_check_sorter.py
 daktari/test_check_utils.py
 daktari/test_collection_utils.py
 daktari/test_config.py
+daktari/test_result_printer.py
 daktari/test_version_utils.py
 daktari/version_utils.py
 daktari.egg-info/PKG-INFO
 daktari.egg-info/SOURCES.txt
 daktari.egg-info/dependency_links.txt
 daktari.egg-info/entry_points.txt
 daktari.egg-info/requires.txt
```

### Comparing `daktari-0.0.96/requirements.txt` & `daktari-0.0.97/requirements.txt`

 * *Files identical despite different names*

### Comparing `daktari-0.0.96/setup.py` & `daktari-0.0.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="daktari",
-    version="0.0.96",
+    version="0.0.97",
     description="Assist in setting up and maintaining developer environments",
     long_description=README,
     long_description_content_type="text/markdown",
     license="MIT",
     author="Matt Russell",
     author_email="matthew.russell@sonocent.com",
     url="https://github.com/sonocent/daktari",
```

