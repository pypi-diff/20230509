# Comparing `tmp/cloud-data-connector-0.0.0.dev1.tar.gz` & `tmp/cloud_data_connector-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-data-connector-0.0.0.dev1.tar", last modified: Fri May  5 17:29:03 2023, max compression
+gzip compressed data, was "cloud_data_connector-1.0.0.tar", last modified: Tue May  9 06:17:17 2023, max compression
```

## Comparing `cloud-data-connector-0.0.0.dev1.tar` & `cloud_data_connector-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,43 @@
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:29:03.349878 cloud-data-connector-0.0.0.dev1/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2234 2023-05-05 17:29:03.349878 cloud-data-connector-0.0.0.dev1/PKG-INFO
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     1714 2023-04-21 06:51:43.000000 cloud-data-connector-0.0.0.dev1/README.md
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      756 2023-05-05 17:27:27.000000 cloud-data-connector-0.0.0.dev1/pyproject.toml
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       38 2023-05-05 17:29:03.349878 cloud-data-connector-0.0.0.dev1/setup.cfg
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:29:03.345878 cloud-data-connector-0.0.0.dev1/src/
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:29:03.349878 cloud-data-connector-0.0.0.dev1/src/cloud_data_connector.egg-info/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2234 2023-05-05 17:29:03.000000 cloud-data-connector-0.0.0.dev1/src/cloud_data_connector.egg-info/PKG-INFO
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      353 2023-05-05 17:29:03.000000 cloud-data-connector-0.0.0.dev1/src/cloud_data_connector.egg-info/SOURCES.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        1 2023-05-05 17:29:03.000000 cloud-data-connector-0.0.0.dev1/src/cloud_data_connector.egg-info/dependency_links.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       19 2023-05-05 17:29:03.000000 cloud-data-connector-0.0.0.dev1/src/cloud_data_connector.egg-info/requires.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        8 2023-05-05 17:29:03.000000 cloud-data-connector-0.0.0.dev1/src/cloud_data_connector.egg-info/top_level.txt
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:29:03.349878 cloud-data-connector-0.0.0.dev1/src/package/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        0 2023-04-20 13:31:53.000000 cloud-data-connector-0.0.0.dev1/src/package/__init__.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-05 17:29:03.349878 cloud-data-connector-0.0.0.dev1/src/package/subpackage/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        0 2023-04-20 13:39:55.000000 cloud-data-connector-0.0.0.dev1/src/package/subpackage/__init__.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       34 2023-04-20 13:46:32.000000 cloud-data-connector-0.0.0.dev1/src/package/subpackage/test.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.567636 cloud_data_connector-1.0.0/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)    17815 2023-05-09 06:17:17.567636 cloud_data_connector-1.0.0/PKG-INFO
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)    17291 2023-05-08 16:20:39.000000 cloud_data_connector-1.0.0/README.md
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     1049 2023-05-08 16:00:45.000000 cloud_data_connector-1.0.0/pyproject.toml
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      405 2023-05-03 05:11:51.000000 cloud_data_connector-1.0.0/security.md
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       38 2023-05-09 06:17:17.567636 cloud_data_connector-1.0.0/setup.cfg
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.563636 cloud_data_connector-1.0.0/src/
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.563636 cloud_data_connector-1.0.0/src/cloud_data_connector.egg-info/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)    17815 2023-05-09 06:17:16.000000 cloud_data_connector-1.0.0/src/cloud_data_connector.egg-info/PKG-INFO
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     1160 2023-05-09 06:17:17.000000 cloud_data_connector-1.0.0/src/cloud_data_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        1 2023-05-09 06:17:16.000000 cloud_data_connector-1.0.0/src/cloud_data_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      312 2023-05-09 06:17:16.000000 cloud_data_connector-1.0.0/src/cloud_data_connector.egg-info/requires.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       15 2023-05-09 06:17:16.000000 cloud_data_connector-1.0.0/src/cloud_data_connector.egg-info/top_level.txt
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.563636 cloud_data_connector-1.0.0/src/data_connector/
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)        0 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/__init__.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.563636 cloud_data_connector-1.0.0/src/data_connector/aws/
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     5811 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/aws/README.md
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      777 2023-05-03 05:11:51.000000 cloud_data_connector-1.0.0/src/data_connector/aws/__init__.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     1604 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/aws/connector.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     2966 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/aws/downloader.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     2196 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/aws/uploader.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.567636 cloud_data_connector-1.0.0/src/data_connector/azure/
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      670 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/azure/AzureML.md
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     2439 2023-05-03 05:11:51.000000 cloud_data_connector-1.0.0/src/data_connector/azure/README.md
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      942 2023-05-03 05:11:51.000000 cloud_data_connector-1.0.0/src/data_connector/azure/__init__.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     3640 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/azure/connector.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     1756 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/azure/connector_object.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     3325 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/azure/downloader.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     2173 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/azure/ml_uploader.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     4520 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/azure/uploader.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.567636 cloud_data_connector-1.0.0/src/data_connector/gcp/
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     6426 2023-05-03 05:11:51.000000 cloud_data_connector-1.0.0/src/data_connector/gcp/README.md
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      813 2023-05-03 05:11:51.000000 cloud_data_connector-1.0.0/src/data_connector/gcp/__init__.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     7435 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/gcp/connector.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     2905 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/gcp/downloader.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     7468 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/gcp/query.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     1716 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/gcp/uploader.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.567636 cloud_data_connector-1.0.0/src/data_connector/int/
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)        0 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/int/__init__.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      971 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/int/int_connector.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      912 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/int/int_downloader.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      990 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/int/int_uploader.py
+-rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      580 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/tox.ini
```

