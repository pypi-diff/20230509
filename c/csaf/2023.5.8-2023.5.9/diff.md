# Comparing `tmp/csaf-2023.5.8.tar.gz` & `tmp/csaf-2023.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csaf-2023.5.8.tar", last modified: Mon May  8 19:17:40 2023, max compression
+gzip compressed data, was "csaf-2023.5.9.tar", last modified: Tue May  9 17:00:04 2023, max compression
```

## Comparing `csaf-2023.5.8.tar` & `csaf-2023.5.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-08 19:17:40.427214 csaf-2023.5.8/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 csaf-2023.5.8/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 csaf-2023.5.8/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     3732 2023-05-08 19:17:40.426897 csaf-2023.5.8/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     2576 2023-05-06 13:23:15.000000 csaf-2023.5.8/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-08 19:17:40.306978 csaf-2023.5.8/csaf/
--rw-r--r--   0 ruth       (501) staff       (20)     1984 2023-05-08 19:14:20.000000 csaf-2023.5.8/csaf/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      246 2022-03-13 14:31:06.000000 csaf-2023.5.8/csaf/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:57.000000 csaf-2023.5.8/csaf/category.py
--rw-r--r--   0 ruth       (501) staff       (20)     4112 2023-01-02 18:40:21.000000 csaf-2023.5.8/csaf/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)      647 2022-12-21 15:07:30.000000 csaf-2023.5.8/csaf/config.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:02.000000 csaf-2023.5.8/csaf/cpe.py
--rw-r--r--   0 ruth       (501) staff       (20)    16866 2022-12-21 15:35:09.000000 csaf-2023.5.8/csaf/csaf.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:06.000000 csaf-2023.5.8/csaf/cve.py
--rw-r--r--   0 ruth       (501) staff       (20)    11239 2023-05-06 14:07:29.000000 csaf-2023.5.8/csaf/cvss.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:10.000000 csaf-2023.5.8/csaf/cwe.py
--rw-r--r--   0 ruth       (501) staff       (20)    12425 2023-05-06 13:11:03.000000 csaf-2023.5.8/csaf/definitions.py
--rw-r--r--   0 ruth       (501) staff       (20)    14924 2022-07-31 13:30:33.000000 csaf-2023.5.8/csaf/document.py
--rw-r--r--   0 ruth       (501) staff       (20)     1284 2022-03-13 20:11:44.000000 csaf-2023.5.8/csaf/env.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:45.000000 csaf-2023.5.8/csaf/hash.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-08 19:17:40.417227 csaf-2023.5.8/csaf/mandatory/
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-14 21:10:09.000000 csaf-2023.5.8/csaf/mandatory/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)     1325 2021-12-16 11:48:56.000000 csaf-2023.5.8/csaf/mandatory/acyclic_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2023 2021-12-16 11:48:42.000000 csaf-2023.5.8/csaf/mandatory/consistent_product_status.py
--rw-r--r--   0 ruth       (501) staff       (20)     1435 2022-02-13 17:11:58.000000 csaf-2023.5.8/csaf/mandatory/defined_group_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2548 2022-02-13 17:04:26.000000 csaf-2023.5.8/csaf/mandatory/defined_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     5288 2022-06-19 10:04:43.000000 csaf-2023.5.8/csaf/mandatory/rules.py
--rw-r--r--   0 ruth       (501) staff       (20)      981 2022-02-13 16:48:33.000000 csaf-2023.5.8/csaf/mandatory/translator_and_source_lang.py
--rw-r--r--   0 ruth       (501) staff       (20)     1267 2022-02-13 20:44:51.000000 csaf-2023.5.8/csaf/mandatory/unique_group_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     1192 2022-02-13 20:40:08.000000 csaf-2023.5.8/csaf/mandatory/unique_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2390 2022-02-13 16:48:33.000000 csaf-2023.5.8/csaf/mandatory/valid_category_name.py
--rw-r--r--   0 ruth       (501) staff       (20)    16500 2022-07-31 13:32:20.000000 csaf-2023.5.8/csaf/product.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:21.000000 csaf-2023.5.8/csaf/purl.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:33.000000 csaf-2023.5.8/csaf/terminal.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:41.000000 csaf-2023.5.8/csaf/tlp.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:29.000000 csaf-2023.5.8/csaf/version.py
--rw-r--r--   0 ruth       (501) staff       (20)     3354 2022-03-13 16:02:22.000000 csaf-2023.5.8/csaf/vuln_types.py
--rw-r--r--   0 ruth       (501) staff       (20)    13724 2023-05-08 18:30:19.000000 csaf-2023.5.8/csaf/vulnerability.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-08 19:17:40.309314 csaf-2023.5.8/csaf.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     3732 2023-05-08 19:17:40.000000 csaf-2023.5.8/csaf.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1204 2023-05-08 19:17:40.000000 csaf-2023.5.8/csaf.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-05-08 19:17:40.000000 csaf-2023.5.8/csaf.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-08 19:17:40.000000 csaf-2023.5.8/csaf.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      222 2023-05-08 19:17:40.000000 csaf-2023.5.8/csaf.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)        5 2023-05-08 19:17:40.000000 csaf-2023.5.8/csaf.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     3004 2023-05-08 18:38:37.000000 csaf-2023.5.8/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-08 19:17:40.427296 csaf-2023.5.8/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-08 19:17:40.426241 csaf-2023.5.8/test/
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:24.000000 csaf-2023.5.8/test/test_category.py
--rw-r--r--   0 ruth       (501) staff       (20)      544 2023-05-06 14:12:39.000000 csaf-2023.5.8/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:47.000000 csaf-2023.5.8/test/test_config.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:50.000000 csaf-2023.5.8/test/test_cpe.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:53.000000 csaf-2023.5.8/test/test_csaf.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:20.000000 csaf-2023.5.8/test/test_cve.py
--rw-r--r--   0 ruth       (501) staff       (20)     8920 2023-05-08 15:23:14.000000 csaf-2023.5.8/test/test_cvss.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:26.000000 csaf-2023.5.8/test/test_cwe.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:29.000000 csaf-2023.5.8/test/test_document.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:33:14.000000 csaf-2023.5.8/test/test_env.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:43.000000 csaf-2023.5.8/test/test_product.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:46.000000 csaf-2023.5.8/test/test_purl.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:49.000000 csaf-2023.5.8/test/test_terminal.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:52.000000 csaf-2023.5.8/test/test_tlp.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:55.000000 csaf-2023.5.8/test/test_version.py
--rw-r--r--   0 ruth       (501) staff       (20)     2259 2023-05-08 18:29:00.000000 csaf-2023.5.8/test/test_vulnerability.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 17:00:04.037012 csaf-2023.5.9/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 csaf-2023.5.9/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 csaf-2023.5.9/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3732 2023-05-09 17:00:04.036798 csaf-2023.5.9/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2576 2023-05-06 13:23:15.000000 csaf-2023.5.9/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 17:00:03.945976 csaf-2023.5.9/csaf/
+-rw-r--r--   0 ruth       (501) staff       (20)     1984 2023-05-09 16:52:48.000000 csaf-2023.5.9/csaf/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      246 2022-03-13 14:31:06.000000 csaf-2023.5.9/csaf/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:57.000000 csaf-2023.5.9/csaf/category.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4112 2023-01-02 18:40:21.000000 csaf-2023.5.9/csaf/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)      647 2022-12-21 15:07:30.000000 csaf-2023.5.9/csaf/config.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:02.000000 csaf-2023.5.9/csaf/cpe.py
+-rw-r--r--   0 ruth       (501) staff       (20)    17012 2023-05-09 16:26:07.000000 csaf-2023.5.9/csaf/csaf.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:06.000000 csaf-2023.5.9/csaf/cve.py
+-rw-r--r--   0 ruth       (501) staff       (20)    11239 2023-05-06 14:07:29.000000 csaf-2023.5.9/csaf/cvss.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:10.000000 csaf-2023.5.9/csaf/cwe.py
+-rw-r--r--   0 ruth       (501) staff       (20)    12425 2023-05-06 13:11:03.000000 csaf-2023.5.9/csaf/definitions.py
+-rw-r--r--   0 ruth       (501) staff       (20)    14924 2022-07-31 13:30:33.000000 csaf-2023.5.9/csaf/document.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1284 2022-03-13 20:11:44.000000 csaf-2023.5.9/csaf/env.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:45.000000 csaf-2023.5.9/csaf/hash.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 17:00:04.027477 csaf-2023.5.9/csaf/mandatory/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-14 21:10:09.000000 csaf-2023.5.9/csaf/mandatory/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1325 2021-12-16 11:48:56.000000 csaf-2023.5.9/csaf/mandatory/acyclic_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2023 2021-12-16 11:48:42.000000 csaf-2023.5.9/csaf/mandatory/consistent_product_status.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1435 2022-02-13 17:11:58.000000 csaf-2023.5.9/csaf/mandatory/defined_group_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2548 2022-02-13 17:04:26.000000 csaf-2023.5.9/csaf/mandatory/defined_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     5288 2022-06-19 10:04:43.000000 csaf-2023.5.9/csaf/mandatory/rules.py
+-rw-r--r--   0 ruth       (501) staff       (20)      981 2022-02-13 16:48:33.000000 csaf-2023.5.9/csaf/mandatory/translator_and_source_lang.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1267 2022-02-13 20:44:51.000000 csaf-2023.5.9/csaf/mandatory/unique_group_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1192 2022-02-13 20:40:08.000000 csaf-2023.5.9/csaf/mandatory/unique_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2390 2022-02-13 16:48:33.000000 csaf-2023.5.9/csaf/mandatory/valid_category_name.py
+-rw-r--r--   0 ruth       (501) staff       (20)    16500 2022-07-31 13:32:20.000000 csaf-2023.5.9/csaf/product.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:21.000000 csaf-2023.5.9/csaf/purl.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:33.000000 csaf-2023.5.9/csaf/terminal.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:41.000000 csaf-2023.5.9/csaf/tlp.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:29.000000 csaf-2023.5.9/csaf/version.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3354 2022-03-13 16:02:22.000000 csaf-2023.5.9/csaf/vuln_types.py
+-rw-r--r--   0 ruth       (501) staff       (20)    13724 2023-05-08 18:30:19.000000 csaf-2023.5.9/csaf/vulnerability.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 17:00:04.021664 csaf-2023.5.9/csaf.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3732 2023-05-09 17:00:03.000000 csaf-2023.5.9/csaf.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     1204 2023-05-09 17:00:03.000000 csaf-2023.5.9/csaf.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-05-09 17:00:03.000000 csaf-2023.5.9/csaf.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-09 17:00:03.000000 csaf-2023.5.9/csaf.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      222 2023-05-09 17:00:03.000000 csaf-2023.5.9/csaf.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        5 2023-05-09 17:00:03.000000 csaf-2023.5.9/csaf.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     3004 2023-05-09 16:28:24.000000 csaf-2023.5.9/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-09 17:00:04.037076 csaf-2023.5.9/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 17:00:04.036148 csaf-2023.5.9/test/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:24.000000 csaf-2023.5.9/test/test_category.py
+-rw-r--r--   0 ruth       (501) staff       (20)      544 2023-05-06 14:12:39.000000 csaf-2023.5.9/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:47.000000 csaf-2023.5.9/test/test_config.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:50.000000 csaf-2023.5.9/test/test_cpe.py
+-rw-r--r--   0 ruth       (501) staff       (20)     9011 2023-05-09 16:51:44.000000 csaf-2023.5.9/test/test_csaf.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:20.000000 csaf-2023.5.9/test/test_cve.py
+-rw-r--r--   0 ruth       (501) staff       (20)     8678 2023-05-09 16:51:33.000000 csaf-2023.5.9/test/test_cvss.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:26.000000 csaf-2023.5.9/test/test_cwe.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:29.000000 csaf-2023.5.9/test/test_document.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:33:14.000000 csaf-2023.5.9/test/test_env.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:43.000000 csaf-2023.5.9/test/test_product.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:46.000000 csaf-2023.5.9/test/test_purl.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:49.000000 csaf-2023.5.9/test/test_terminal.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:52.000000 csaf-2023.5.9/test/test_tlp.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:55.000000 csaf-2023.5.9/test/test_version.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2259 2023-05-08 18:29:00.000000 csaf-2023.5.9/test/test_vulnerability.py
```

### Comparing `csaf-2023.5.8/LICENSE` & `csaf-2023.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/PKG-INFO` & `csaf-2023.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csaf
-Version: 2023.5.8
+Version: 2023.5.9
 Summary: Common Security Advisory Framework (CSAF) Verification, Validation, and Application Programming Interface (API).
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/csaf
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/csaf
 Project-URL: Documentation, https://codes.dilettant.life/docs/csaf
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/csaf
```

### Comparing `csaf-2023.5.8/README.md` & `csaf-2023.5.9/README.md`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/__init__.py` & `csaf-2023.5.9/csaf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 
 
 init_logger(name=APP_ENV, level=logging.DEBUG if DEBUG else None)
 
 from csaf.csaf import is_valid  # noqa
 
 # [[[fill git_describe()]]]
-__version__ = '2023.5.8+parent.aa36605a'
-# [[[end]]] (checksum: 99e36df585743bf57b7cbd29fd80ca8c)
+__version__ = '2023.5.9+parent.0a298a86'
+# [[[end]]] (checksum: 72eec31730ba0300fcb5d605f8aec1d6)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 __all__ = ['is_valid', 'log']
```

### Comparing `csaf-2023.5.8/csaf/cli.py` & `csaf-2023.5.9/csaf/cli.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/config.py` & `csaf-2023.5.9/csaf/config.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/csaf.py` & `csaf-2023.5.9/csaf/csaf.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,19 @@
             description='Represents a list of all relevant vulnerability information items.',
             min_items=1,
             title='Vulnerabilities',
         ),
     ]
 
     @no_type_check
+    def json(self, *args, **kwargs):
+        kwargs.setdefault('by_alias', True)
+        return super().json(*args, **kwargs)
+
+    @no_type_check
     @validator('vulnerabilities')
     @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('vulnerabilities present but empty')
         return v
```

### Comparing `csaf-2023.5.8/csaf/cvss.py` & `csaf-2023.5.9/csaf/cvss.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/definitions.py` & `csaf-2023.5.9/csaf/definitions.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/document.py` & `csaf-2023.5.9/csaf/document.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/env.py` & `csaf-2023.5.9/csaf/env.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/mandatory/acyclic_product_ids.py` & `csaf-2023.5.9/csaf/mandatory/acyclic_product_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/mandatory/consistent_product_status.py` & `csaf-2023.5.9/csaf/mandatory/consistent_product_status.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/mandatory/defined_group_ids.py` & `csaf-2023.5.9/csaf/mandatory/defined_group_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/mandatory/defined_product_ids.py` & `csaf-2023.5.9/csaf/mandatory/defined_product_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/mandatory/rules.py` & `csaf-2023.5.9/csaf/mandatory/rules.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/mandatory/translator_and_source_lang.py` & `csaf-2023.5.9/csaf/mandatory/translator_and_source_lang.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/mandatory/unique_group_ids.py` & `csaf-2023.5.9/csaf/mandatory/unique_group_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/mandatory/unique_product_ids.py` & `csaf-2023.5.9/csaf/mandatory/unique_product_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/mandatory/valid_category_name.py` & `csaf-2023.5.9/csaf/mandatory/valid_category_name.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/product.py` & `csaf-2023.5.9/csaf/product.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/vuln_types.py` & `csaf-2023.5.9/csaf/vuln_types.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf/vulnerability.py` & `csaf-2023.5.9/csaf/vulnerability.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/csaf.egg-info/PKG-INFO` & `csaf-2023.5.9/csaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csaf
-Version: 2023.5.8
+Version: 2023.5.9
 Summary: Common Security Advisory Framework (CSAF) Verification, Validation, and Application Programming Interface (API).
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/csaf
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/csaf
 Project-URL: Documentation, https://codes.dilettant.life/docs/csaf
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/csaf
```

### Comparing `csaf-2023.5.8/csaf.egg-info/SOURCES.txt` & `csaf-2023.5.9/csaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/pyproject.toml` & `csaf-2023.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "csaf"
-version = "2023.5.8"
+version = "2023.5.9"
 description = "Common Security Advisory Framework (CSAF) Verification, Validation, and Application Programming Interface (API)."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `csaf-2023.5.8/test/test_cli.py` & `csaf-2023.5.9/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.8/test/test_cvss.py` & `csaf-2023.5.9/test/test_cvss.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,30 +35,24 @@
     assert vector_string in json_rep_of_vs[0]
     assert '"vectorString":' in json_rep_of_vs[0]
 
     expected_schema = {
         'title': 'CVSS31',
         'type': 'object',
         'properties': {
-            'version': {
-                'description': 'CVSS Version',
-                'default': '3.1',
-                'allOf': [
-                    {'$ref': '#/definitions/Version'}
-                ]
-            },
+            'version': {'description': 'CVSS Version', 'default': '3.1', 'allOf': [{'$ref': '#/definitions/Version'}]},
             'vectorString': {
                 'title': 'Vectorstring',
                 'pattern': (
                     '^CVSS:3[.]1/((AV:[NALP]|AC:[LH]|PR:[NLH]|UI:[NR]|S:[UC]|[CIA]:[NLH]|E:[XUPFH]|RL:[XOTWU]|RC:'
                     '[XURC]|[CIA]R:[XLMH]|MAV:[XNALP]|MAC:[XLH]|MPR:[XNLH]|MUI:[XNR]|MS:[XUC]|M[CIA]:[XNLH])/)*'
                     '(AV:[NALP]|AC:[LH]|PR:[NLH]|UI:[NR]|S:[UC]|[CIA]:[NLH]|E:[XUPFH]|RL:[XOTWU]|RC:[XURC]|[CIA]R:'
                     '[XLMH]|MAV:[XNALP]|MAC:[XLH]|MPR:[XNLH]|MUI:[XNR]|MS:[XUC]|M[CIA]:[XNLH])$'
                 ),
-                'type': 'string'
+                'type': 'string',
             },
             'attackVector': {'$ref': '#/definitions/AttackVectorType'},
             'attackComplexity': {'$ref': '#/definitions/AttackComplexityType'},
             'privilegesRequired': {'$ref': '#/definitions/PrivilegesRequiredType'},
             'userInteraction': {'$ref': '#/definitions/UserInteractionType'},
             'scope': {'$ref': '#/definitions/ScopeType'},
             'confidentialityImpact': {'$ref': '#/definitions/CiaType'},
@@ -79,103 +73,93 @@
             'modifiedPrivilegesRequired': {'$ref': '#/definitions/ModifiedPrivilegesRequiredType'},
             'modifiedUserInteraction': {'$ref': '#/definitions/ModifiedUserInteractionType'},
             'modifiedScope': {'$ref': '#/definitions/ModifiedScopeType'},
             'modifiedConfidentialityImpact': {'$ref': '#/definitions/ModifiedCiaType'},
             'modifiedIntegrityImpact': {'$ref': '#/definitions/ModifiedCiaType'},
             'modifiedAvailabilityImpact': {'$ref': '#/definitions/ModifiedCiaType'},
             'environmentalScore': {'$ref': '#/definitions/ScoreType'},
-            'environmentalSeverity': {'$ref': '#/definitions/SeverityType'}
+            'environmentalSeverity': {'$ref': '#/definitions/SeverityType'},
         },
         'required': ['vectorString', 'baseScore', 'baseSeverity'],
         'definitions': {
-            'Version': {
-                'title': 'Version',
-                'description': 'CVSS Version',
-                'enum': ['2.0', '3.0', '3.1']
-            },
+            'Version': {'title': 'Version', 'description': 'CVSS Version', 'enum': ['2.0', '3.0', '3.1']},
             'AttackVectorType': {
                 'title': 'AttackVectorType',
                 'description': 'An enumeration.',
-                'enum': ['NETWORK', 'ADJACENT_NETWORK', 'LOCAL', 'PHYSICAL']
+                'enum': ['NETWORK', 'ADJACENT_NETWORK', 'LOCAL', 'PHYSICAL'],
             },
             'AttackComplexityType': {
                 'title': 'AttackComplexityType',
                 'description': 'An enumeration.',
-                'enum': ['HIGH', 'LOW']
+                'enum': ['HIGH', 'LOW'],
             },
             'PrivilegesRequiredType': {
                 'title': 'PrivilegesRequiredType',
                 'description': 'An enumeration.',
-                'enum': ['HIGH', 'LOW', 'NONE']
+                'enum': ['HIGH', 'LOW', 'NONE'],
             },
             'UserInteractionType': {
                 'title': 'UserInteractionType',
                 'description': 'An enumeration.',
-                'enum': ['NONE', 'REQUIRED']
-            },
-            'ScopeType': {
-                'title': 'ScopeType',
-                'description': 'An enumeration.',
-                'enum': ['UNCHANGED', 'CHANGED']
-            },
-            'CiaType': {
-                'title': 'CiaType',
-                'description': 'An enumeration.',
-                'enum': ['NONE', 'PARTIAL', 'COMPLETE']
-            },
-            'ScoreType': {
-                'title': 'ScoreType',
-                'minimum': 0.0,
-                'maximum': 10.0,
-                'type': 'number'
+                'enum': ['NONE', 'REQUIRED'],
             },
+            'ScopeType': {'title': 'ScopeType', 'description': 'An enumeration.', 'enum': ['UNCHANGED', 'CHANGED']},
+            'CiaType': {'title': 'CiaType', 'description': 'An enumeration.', 'enum': ['NONE', 'PARTIAL', 'COMPLETE']},
+            'ScoreType': {'title': 'ScoreType', 'minimum': 0.0, 'maximum': 10.0, 'type': 'number'},
             'SeverityType': {
                 'title': 'SeverityType',
                 'description': 'An enumeration.',
-                'enum': ['NONE', 'LOW', 'MEDIUM', 'HIGH', 'CRITICAL']
+                'enum': ['NONE', 'LOW', 'MEDIUM', 'HIGH', 'CRITICAL'],
             },
             'ExploitCodeMaturityType': {
                 'title': 'ExploitCodeMaturityType',
                 'description': 'An enumeration.',
-                'enum': ['UNPROVEN', 'PROOF_OF_CONCEPT', 'FUNCTIONAL', 'HIGH', 'NOT_DEFINED']
+                'enum': ['UNPROVEN', 'PROOF_OF_CONCEPT', 'FUNCTIONAL', 'HIGH', 'NOT_DEFINED'],
             },
             'RemediationLevelType': {
-                'title': 'RemediationLevelType', 'description': 'An enumeration.',
-                'enum': ['OFFICIAL_FIX', 'TEMPORARY_FIX', 'WORKAROUND', 'UNAVAILABLE',
-                         'NOT_DEFINED']
+                'title': 'RemediationLevelType',
+                'description': 'An enumeration.',
+                'enum': ['OFFICIAL_FIX', 'TEMPORARY_FIX', 'WORKAROUND', 'UNAVAILABLE', 'NOT_DEFINED'],
             },
             'ConfidenceType': {
-                'title': 'ConfidenceType', 'description': 'An enumeration.',
-                'enum': ['UNKNOWN', 'REASONABLE', 'CONFIRMED', 'NOT_DEFINED']
+                'title': 'ConfidenceType',
+                'description': 'An enumeration.',
+                'enum': ['UNKNOWN', 'REASONABLE', 'CONFIRMED', 'NOT_DEFINED'],
             },
             'CiaRequirementType': {
-                'title': 'CiaRequirementType', 'description': 'An enumeration.',
-                'enum': ['LOW', 'MEDIUM', 'HIGH', 'NOT_DEFINED']
+                'title': 'CiaRequirementType',
+                'description': 'An enumeration.',
+                'enum': ['LOW', 'MEDIUM', 'HIGH', 'NOT_DEFINED'],
             },
             'ModifiedAttackVectorType': {
-                'title': 'ModifiedAttackVectorType', 'description': 'An enumeration.',
-                'enum': ['NETWORK', 'ADJACENT_NETWORK', 'LOCAL', 'PHYSICAL', 'NOT_DEFINED']
+                'title': 'ModifiedAttackVectorType',
+                'description': 'An enumeration.',
+                'enum': ['NETWORK', 'ADJACENT_NETWORK', 'LOCAL', 'PHYSICAL', 'NOT_DEFINED'],
             },
             'ModifiedAttackComplexityType': {
-                'title': 'ModifiedAttackComplexityType', 'description': 'An enumeration.',
-                'enum': ['HIGH', 'LOW', 'NOT_DEFINED']
+                'title': 'ModifiedAttackComplexityType',
+                'description': 'An enumeration.',
+                'enum': ['HIGH', 'LOW', 'NOT_DEFINED'],
             },
             'ModifiedPrivilegesRequiredType': {
                 'title': 'ModifiedPrivilegesRequiredType',
                 'description': 'An enumeration.',
-                'enum': ['HIGH', 'LOW', 'NONE', 'NOT_DEFINED']
+                'enum': ['HIGH', 'LOW', 'NONE', 'NOT_DEFINED'],
             },
             'ModifiedUserInteractionType': {
-                'title': 'ModifiedUserInteractionType', 'description': 'An enumeration.',
-                'enum': ['NONE', 'REQUIRED', 'NOT_DEFINED']
+                'title': 'ModifiedUserInteractionType',
+                'description': 'An enumeration.',
+                'enum': ['NONE', 'REQUIRED', 'NOT_DEFINED'],
             },
             'ModifiedScopeType': {
-                'title': 'ModifiedScopeType', 'description': 'An enumeration.',
-                'enum': ['UNCHANGED', 'CHANGED', 'NOT_DEFINED']
+                'title': 'ModifiedScopeType',
+                'description': 'An enumeration.',
+                'enum': ['UNCHANGED', 'CHANGED', 'NOT_DEFINED'],
             },
             'ModifiedCiaType': {
-                'title': 'ModifiedCiaType', 'description': 'An enumeration.',
-                'enum': ['NONE', 'LOW', 'HIGH', 'NOT_DEFINED']
-            }
-        }
+                'title': 'ModifiedCiaType',
+                'description': 'An enumeration.',
+                'enum': ['NONE', 'LOW', 'HIGH', 'NOT_DEFINED'],
+            },
+        },
     }
     assert c31.schema(by_alias=True) == expected_schema
```

### Comparing `csaf-2023.5.8/test/test_vulnerability.py` & `csaf-2023.5.9/test/test_vulnerability.py`

 * *Files identical despite different names*

