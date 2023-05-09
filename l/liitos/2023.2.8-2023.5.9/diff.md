# Comparing `tmp/liitos-2023.2.8.tar.gz` & `tmp/liitos-2023.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liitos-2023.2.8.tar", last modified: Tue Feb  7 23:01:04 2023, max compression
+gzip compressed data, was "liitos-2023.5.9.tar", last modified: Tue May  9 21:01:33 2023, max compression
```

## Comparing `liitos-2023.2.8.tar` & `liitos-2023.5.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-07 23:01:04.955176 liitos-2023.2.8/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 liitos-2023.2.8/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       95 2023-01-11 18:32:01.000000 liitos-2023.2.8/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     2540 2023-02-07 23:01:04.955014 liitos-2023.2.8/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1623 2023-01-22 12:34:33.000000 liitos-2023.2.8/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-07 23:01:04.930702 liitos-2023.2.8/liitos/
--rw-r--r--   0 ruth       (501) staff       (20)     5044 2023-02-07 22:59:13.000000 liitos-2023.2.8/liitos/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      125 2022-11-23 21:28:47.000000 liitos-2023.2.8/liitos/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     3875 2023-02-04 14:18:21.000000 liitos-2023.2.8/liitos/approvals.py
--rw-r--r--   0 ruth       (501) staff       (20)     1787 2023-02-07 22:52:39.000000 liitos-2023.2.8/liitos/captions.py
--rw-r--r--   0 ruth       (501) staff       (20)     4295 2023-02-04 14:18:21.000000 liitos-2023.2.8/liitos/changes.py
--rw-r--r--   0 ruth       (501) staff       (20)    10260 2023-02-07 22:48:13.000000 liitos-2023.2.8/liitos/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)    31810 2023-02-04 14:18:21.000000 liitos-2023.2.8/liitos/concat.py
--rw-r--r--   0 ruth       (501) staff       (20)     1642 2023-01-02 19:46:21.000000 liitos-2023.2.8/liitos/configure.py
--rw-r--r--   0 ruth       (501) staff       (20)     1780 2023-01-29 18:11:25.000000 liitos-2023.2.8/liitos/description_lists.py
--rw-r--r--   0 ruth       (501) staff       (20)     1958 2023-01-02 19:41:38.000000 liitos-2023.2.8/liitos/eject.py
--rw-r--r--   0 ruth       (501) staff       (20)     1650 2022-12-06 19:43:32.000000 liitos-2023.2.8/liitos/figures.py
--rw-r--r--   0 ruth       (501) staff       (20)    11799 2023-01-21 21:35:47.000000 liitos-2023.2.8/liitos/gather.py
--rw-r--r--   0 ruth       (501) staff       (20)     3896 2022-12-09 18:24:04.000000 liitos-2023.2.8/liitos/labels.py
--rw-r--r--   0 ruth       (501) staff       (20)       55 2022-09-17 11:23:46.000000 liitos-2023.2.8/liitos/liitos.py
--rw-r--r--   0 ruth       (501) staff       (20)    41648 2023-02-04 14:18:21.000000 liitos-2023.2.8/liitos/meta.py
--rw-r--r--   0 ruth       (501) staff       (20)      624 2023-01-31 19:15:44.000000 liitos-2023.2.8/liitos/patch.py
--rw-r--r--   0 ruth       (501) staff       (20)    15890 2023-02-06 19:25:05.000000 liitos-2023.2.8/liitos/render.py
--rw-r--r--   0 ruth       (501) staff       (20)    12596 2023-02-01 20:20:42.000000 liitos-2023.2.8/liitos/tables.py
--rw-r--r--   0 ruth       (501) staff       (20)     1489 2023-01-02 19:38:06.000000 liitos-2023.2.8/liitos/template_loader.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-07 23:01:04.938453 liitos-2023.2.8/liitos/templates/
--rw-r--r--   0 ruth       (501) staff       (20)      116 2022-12-01 18:05:38.000000 liitos-2023.2.8/liitos/templates/approvals.yml
--rw-r--r--   0 ruth       (501) staff       (20)     1198 2023-01-17 20:23:10.000000 liitos-2023.2.8/liitos/templates/bookmatter.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)      109 2023-01-17 18:43:02.000000 liitos-2023.2.8/liitos/templates/changes.yml
--rw-r--r--   0 ruth       (501) staff       (20)      853 2022-11-29 20:13:39.000000 liitos-2023.2.8/liitos/templates/driver.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)       97 2022-12-05 14:36:30.000000 liitos-2023.2.8/liitos/templates/meta-patch.yml
--rw-r--r--   0 ruth       (501) staff       (20)     1448 2023-01-17 20:30:00.000000 liitos-2023.2.8/liitos/templates/meta.yml
--rw-r--r--   0 ruth       (501) staff       (20)     2505 2023-01-17 20:37:22.000000 liitos-2023.2.8/liitos/templates/metadata.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     1538 2022-12-14 16:45:30.000000 liitos-2023.2.8/liitos/templates/mkdocs.yml.in
--rw-r--r--   0 ruth       (501) staff       (20)     1106 2022-12-04 13:44:55.000000 liitos-2023.2.8/liitos/templates/publisher.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     9614 2023-02-01 20:13:41.000000 liitos-2023.2.8/liitos/templates/setup.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     7450 2023-01-17 20:39:19.000000 liitos-2023.2.8/liitos/templates/vocabulary.yml
--rw-r--r--   0 ruth       (501) staff       (20)     7417 2023-02-06 18:39:24.000000 liitos-2023.2.8/liitos/tools.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-07 23:01:04.933173 liitos-2023.2.8/liitos.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     2540 2023-02-07 23:01:04.000000 liitos-2023.2.8/liitos.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1264 2023-02-07 23:01:04.000000 liitos-2023.2.8/liitos.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-02-07 23:01:04.000000 liitos-2023.2.8/liitos.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       42 2023-02-07 23:01:04.000000 liitos-2023.2.8/liitos.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      179 2023-02-07 23:01:04.000000 liitos-2023.2.8/liitos.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       15 2023-02-07 23:01:04.000000 liitos-2023.2.8/liitos.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2645 2023-02-07 22:44:17.000000 liitos-2023.2.8/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-02-07 23:01:04.955215 liitos-2023.2.8/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-07 23:01:04.954700 liitos-2023.2.8/test/
--rw-r--r--   0 ruth       (501) staff       (20)      499 2022-12-06 21:07:15.000000 liitos-2023.2.8/test/test_approvals.py
--rw-r--r--   0 ruth       (501) staff       (20)     1708 2023-02-07 22:58:06.000000 liitos-2023.2.8/test/test_captions.py
--rw-r--r--   0 ruth       (501) staff       (20)      433 2022-12-06 21:11:22.000000 liitos-2023.2.8/test/test_changes.py
--rw-r--r--   0 ruth       (501) staff       (20)     3720 2023-02-04 14:19:55.000000 liitos-2023.2.8/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     6984 2022-12-09 17:00:57.000000 liitos-2023.2.8/test/test_concat.py
--rw-r--r--   0 ruth       (501) staff       (20)     1073 2022-12-05 16:28:35.000000 liitos-2023.2.8/test/test_eject.py
--rw-r--r--   0 ruth       (501) staff       (20)     2689 2022-12-07 18:21:39.000000 liitos-2023.2.8/test/test_figures.py
--rw-r--r--   0 ruth       (501) staff       (20)    10449 2022-11-02 19:26:27.000000 liitos-2023.2.8/test/test_gather.py
--rw-r--r--   0 ruth       (501) staff       (20)     1410 2022-12-05 16:41:47.000000 liitos-2023.2.8/test/test_labels.py
--rw-r--r--   0 ruth       (501) staff       (20)       89 2022-08-01 14:41:37.000000 liitos-2023.2.8/test/test_liitos.py
--rw-r--r--   0 ruth       (501) staff       (20)    15742 2023-02-04 14:19:02.000000 liitos-2023.2.8/test/test_meta.py
--rw-r--r--   0 ruth       (501) staff       (20)      669 2022-12-05 18:19:44.000000 liitos-2023.2.8/test/test_patch.py
--rw-r--r--   0 ruth       (501) staff       (20)      486 2023-01-31 21:27:46.000000 liitos-2023.2.8/test/test_render.py
--rw-r--r--   0 ruth       (501) staff       (20)      883 2022-12-09 17:00:56.000000 liitos-2023.2.8/test/test_tables.py
--rw-r--r--   0 ruth       (501) staff       (20)      431 2022-12-06 20:22:36.000000 liitos-2023.2.8/test/test_template_loader.py
--rw-r--r--   0 ruth       (501) staff       (20)     1436 2023-01-31 21:28:22.000000 liitos-2023.2.8/test/test_tools.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 21:01:33.403590 liitos-2023.5.9/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 liitos-2023.5.9/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       95 2023-01-11 18:32:01.000000 liitos-2023.5.9/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3036 2023-05-09 21:01:33.403441 liitos-2023.5.9/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2068 2023-03-14 22:27:04.000000 liitos-2023.5.9/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 21:01:33.388730 liitos-2023.5.9/liitos/
+-rw-r--r--   0 ruth       (501) staff       (20)     5000 2023-05-09 20:59:17.000000 liitos-2023.5.9/liitos/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      125 2022-11-23 21:28:47.000000 liitos-2023.5.9/liitos/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3875 2023-02-04 14:18:21.000000 liitos-2023.5.9/liitos/approvals.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1825 2023-04-25 19:10:10.000000 liitos-2023.5.9/liitos/captions.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4295 2023-02-04 14:18:21.000000 liitos-2023.5.9/liitos/changes.py
+-rw-r--r--   0 ruth       (501) staff       (20)    10260 2023-02-07 22:48:13.000000 liitos-2023.5.9/liitos/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)    31810 2023-02-04 14:18:21.000000 liitos-2023.5.9/liitos/concat.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1642 2023-01-02 19:46:21.000000 liitos-2023.5.9/liitos/configure.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1818 2023-04-25 19:46:43.000000 liitos-2023.5.9/liitos/description_lists.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1958 2023-01-02 19:41:38.000000 liitos-2023.5.9/liitos/eject.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1688 2023-04-25 19:10:05.000000 liitos-2023.5.9/liitos/figures.py
+-rw-r--r--   0 ruth       (501) staff       (20)    11799 2023-01-21 21:35:47.000000 liitos-2023.5.9/liitos/gather.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4375 2023-04-25 19:50:27.000000 liitos-2023.5.9/liitos/labels.py
+-rw-r--r--   0 ruth       (501) staff       (20)       55 2022-09-17 11:23:46.000000 liitos-2023.5.9/liitos/liitos.py
+-rw-r--r--   0 ruth       (501) staff       (20)    41648 2023-02-04 14:18:21.000000 liitos-2023.5.9/liitos/meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)      624 2023-01-31 19:15:44.000000 liitos-2023.5.9/liitos/patch.py
+-rw-r--r--   0 ruth       (501) staff       (20)    18808 2023-05-09 18:42:29.000000 liitos-2023.5.9/liitos/render.py
+-rw-r--r--   0 ruth       (501) staff       (20)    25061 2023-05-09 20:43:04.000000 liitos-2023.5.9/liitos/tables.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1489 2023-01-02 19:38:06.000000 liitos-2023.5.9/liitos/template_loader.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 21:01:33.396442 liitos-2023.5.9/liitos/templates/
+-rw-r--r--   0 ruth       (501) staff       (20)      116 2022-12-01 18:05:38.000000 liitos-2023.5.9/liitos/templates/approvals.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     1198 2023-01-17 20:23:10.000000 liitos-2023.5.9/liitos/templates/bookmatter.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)      109 2023-01-17 18:43:02.000000 liitos-2023.5.9/liitos/templates/changes.yml
+-rw-r--r--   0 ruth       (501) staff       (20)      853 2022-11-29 20:13:39.000000 liitos-2023.5.9/liitos/templates/driver.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)       97 2022-12-05 14:36:30.000000 liitos-2023.5.9/liitos/templates/meta-patch.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     1448 2023-01-17 20:30:00.000000 liitos-2023.5.9/liitos/templates/meta.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     2505 2023-01-17 20:37:22.000000 liitos-2023.5.9/liitos/templates/metadata.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     1538 2022-12-14 16:45:30.000000 liitos-2023.5.9/liitos/templates/mkdocs.yml.in
+-rw-r--r--   0 ruth       (501) staff       (20)     1106 2023-05-09 18:17:09.000000 liitos-2023.5.9/liitos/templates/publisher.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     9709 2023-02-14 22:04:11.000000 liitos-2023.5.9/liitos/templates/setup.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     7450 2023-01-17 20:39:19.000000 liitos-2023.5.9/liitos/templates/vocabulary.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     7497 2023-04-25 19:15:13.000000 liitos-2023.5.9/liitos/tools.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 21:01:33.391412 liitos-2023.5.9/liitos.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3036 2023-05-09 21:01:33.000000 liitos-2023.5.9/liitos.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     1264 2023-05-09 21:01:33.000000 liitos-2023.5.9/liitos.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-05-09 21:01:33.000000 liitos-2023.5.9/liitos.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       42 2023-05-09 21:01:33.000000 liitos-2023.5.9/liitos.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      179 2023-05-09 21:01:33.000000 liitos-2023.5.9/liitos.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       15 2023-05-09 21:01:33.000000 liitos-2023.5.9/liitos.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2691 2023-05-09 18:21:47.000000 liitos-2023.5.9/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-09 21:01:33.403627 liitos-2023.5.9/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-09 21:01:33.403142 liitos-2023.5.9/test/
+-rw-r--r--   0 ruth       (501) staff       (20)      499 2022-12-06 21:07:15.000000 liitos-2023.5.9/test/test_approvals.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1708 2023-02-07 22:58:06.000000 liitos-2023.5.9/test/test_captions.py
+-rw-r--r--   0 ruth       (501) staff       (20)      433 2022-12-06 21:11:22.000000 liitos-2023.5.9/test/test_changes.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3720 2023-02-04 14:19:55.000000 liitos-2023.5.9/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     6984 2022-12-09 17:00:57.000000 liitos-2023.5.9/test/test_concat.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1073 2022-12-05 16:28:35.000000 liitos-2023.5.9/test/test_eject.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2689 2022-12-07 18:21:39.000000 liitos-2023.5.9/test/test_figures.py
+-rw-r--r--   0 ruth       (501) staff       (20)    10449 2022-11-02 19:26:27.000000 liitos-2023.5.9/test/test_gather.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1410 2022-12-05 16:41:47.000000 liitos-2023.5.9/test/test_labels.py
+-rw-r--r--   0 ruth       (501) staff       (20)       89 2022-08-01 14:41:37.000000 liitos-2023.5.9/test/test_liitos.py
+-rw-r--r--   0 ruth       (501) staff       (20)    15742 2023-02-04 14:19:02.000000 liitos-2023.5.9/test/test_meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)      669 2022-12-05 18:19:44.000000 liitos-2023.5.9/test/test_patch.py
+-rw-r--r--   0 ruth       (501) staff       (20)      486 2023-01-31 21:27:46.000000 liitos-2023.5.9/test/test_render.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3608 2023-05-09 18:14:35.000000 liitos-2023.5.9/test/test_tables.py
+-rw-r--r--   0 ruth       (501) staff       (20)      431 2022-12-06 20:22:36.000000 liitos-2023.5.9/test/test_template_loader.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1436 2023-01-31 21:28:22.000000 liitos-2023.5.9/test/test_tools.py
```

### Comparing `liitos-2023.2.8/LICENSE` & `liitos-2023.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/PKG-INFO` & `liitos-2023.5.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: liitos
-Version: 2023.2.8
+Version: 2023.5.9
 Summary: Splice (Finnish liitos) contributions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/liitos
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/liitos
 Project-URL: Documentation, https://codes.dilettant.life/docs/liitos
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/liitos
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/liitos
 Keywords: developer-tools,validation,verification
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Liitos
 
@@ -36,25 +37,32 @@
 
 ## Documentation
 
 User and developer [documentation of liitos](https://codes.dilettant.life/docs/liitos).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of liitos](https://todo.sr.ht/~sthagen/liitos).
+Any feature requests or bug reports shall go to the [todos of liitos](https://todo.sr.ht/~sthagen/liitos).
 
 ## Primary Source repository
 
 The main source of `liitos` is on a mountain in central Switzerland.
 We use distributed version control (git).
 There is no central hub.
 Every clone can become a new source for the benefit of all.
 The preferred public clones of `liitos` are:
 
 * [on codeberg](https://codeberg.org/sthagen/liitos) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/liitos) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 # Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `liitos-2023.2.8/liitos/__init__.py` & `liitos-2023.5.9/liitos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 import os
 import pathlib
 import shellingham  # type: ignore
 from typing import List, no_type_check
 
 # [[[fill git_describe()]]]
-__version__ = '2023.2.8+parent.b08058c7'
-# [[[end]]] (checksum: 66a50e360bdddcd6850848c3808a189f)
+__version__ = '2023.5.9+parent.8965a930'
+# [[[end]]] (checksum: 69adc87cceb6f4a1695afccfe3f3f0ff)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_NAME = 'Splice (Finnish liitos) contributions.'
 APP_ALIAS = 'liitos'
 APP_ENV = 'LIITOS'
@@ -23,15 +23,15 @@
 QUIET = False
 STRICT = bool(os.getenv(f'{APP_ENV}_STRICT', ''))
 ENCODING = 'utf-8'
 ENCODING_ERRORS_POLICY = 'ignore'
 DEFAULT_CONFIG_NAME = '.liitos.json'
 DEFAULT_LF_ONLY = 'YES'
 FILTER_CS_LIST = 'mermaid-filter'
-FROM_FORMAT_SPEC = 'markdown+header_attributes+link_attributes+strikeout'
+FROM_FORMAT_SPEC = 'markdown'
 LATEX_PAYLOAD_NAME = 'document.tex'
 log = logging.getLogger()  # Module level logger is sufficient
 LOG_FOLDER = pathlib.Path('logs')
 LOG_FILE = f'{APP_ALIAS}.log'
 LOG_PATH = pathlib.Path(LOG_FOLDER, LOG_FILE) if LOG_FOLDER.is_dir() else pathlib.Path(LOG_FILE)
 LOG_LEVEL = logging.INFO
 LOG_SEPARATOR = '- ' * 80
```

### Comparing `liitos-2023.2.8/liitos/approvals.py` & `liitos-2023.5.9/liitos/approvals.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/captions.py` & `liitos-2023.5.9/liitos/captions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Iterable
 
 from liitos import log
 
 
-def weave(incoming: Iterable[str]) -> list[str]:
+def weave(incoming: Iterable[str], lookup: dict[str, str] | None = None) -> list[str]:
     """Later alligator."""
     outgoing = []
     modus = 'copy'
     table: list[str] = []
     caption: list[str] = []
     for slot, line in enumerate(incoming):
         if modus == 'copy':
```

### Comparing `liitos-2023.2.8/liitos/changes.py` & `liitos-2023.5.9/liitos/changes.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/cli.py` & `liitos-2023.5.9/liitos/cli.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/concat.py` & `liitos-2023.5.9/liitos/concat.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/configure.py` & `liitos-2023.5.9/liitos/configure.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/description_lists.py` & `liitos-2023.5.9/liitos/description_lists.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         except Exception as err:
             log.error(f'failed to parse option value from {text_line.strip()} with err: {err}')
             return False, text_line, ''
     else:
         return False, text_line, ''
 
 
-def options(incoming: Iterable[str]) -> list[str]:
+def options(incoming: Iterable[str], lookup: dict[str, str] | None = None) -> list[str]:
     """Later alligator. \\option[style=multiline,leftmargin=6em]"""
     outgoing = []
     modus = 'copy'
     opt = NO_OPTION
     for slot, line in enumerate(incoming):
         if modus == 'copy':
             has_opt, text_line, opt = parse_options_command(slot, line)
```

### Comparing `liitos-2023.2.8/liitos/eject.py` & `liitos-2023.5.9/liitos/eject.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/figures.py` & `liitos-2023.5.9/liitos/figures.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Iterable
 
 from liitos import log
 
 NO_RESCALE: float | int = 0
 
 
-def scale(incoming: Iterable[str]) -> list[str]:
+def scale(incoming: Iterable[str], lookup: dict[str, str] | None = None) -> list[str]:
     """Later alligator."""
     outgoing = []
     modus = 'copy'
     rescale = NO_RESCALE
     for slot, line in enumerate(incoming):
         if modus == 'copy':
             if line.startswith(r'\scale='):
```

### Comparing `liitos-2023.2.8/liitos/gather.py` & `liitos-2023.5.9/liitos/gather.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/labels.py` & `liitos-2023.5.9/liitos/labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Iterable
 
 from liitos import log
 
 NO_LABEL = 'no-label-found-ERROR'
 
 
-def inject(incoming: Iterable[str]) -> list[str]:
+def inject(incoming: Iterable[str], lookup: dict[str, str] | None = None) -> list[str]:
     """Later alligator."""
     outgoing = []
     modus = 'copy'
     label = NO_LABEL
     figure: list[str] = []
     caption: list[str] = []
     precondition = r'\begin{figure}'
@@ -30,19 +30,28 @@
                     lab = line.split('{', 1)[1]
                     lab = lab.rsplit('.', 1)[0]
                     lab = lab.rsplit('/', 1)[1]
                     adhoc_label = r'\label{fig:' + lab + '}'
                     log.info(adhoc_label)
                 except Exception as err:
                     log.error(f'failed to extract generic label from {line.strip()} with err: {err}')
+                captain = 'MISSING-CAPTION-IN-MARKDOWN'
+                try:
+                    token = line.split('{', 1)[1].rstrip('}')
+                    if lookup is not None:
+                        captain = lookup.get(token, captain)
+                except Exception as err:
+                    log.error(
+                        f'failed to extract file path token for caption lookup from {line.strip()} with err: {err}'
+                    )
                 outgoing.append('')  # TODO(sthagen) - why do we sometimes received joined strings?
                 outgoing.append(r'\begin{figure}')
                 outgoing.append(r'\centering')
                 outgoing.append(line)
-                outgoing.append(r'\caption{MISSING-CAPTION-IN-MARKDOWN ' + adhoc_label + '}')
+                outgoing.append(r'\caption{' + captain + ' ' + adhoc_label + '}')
                 outgoing.append(r'\end{figure}')
             elif line.startswith(r'\includegraphics{') and precondition_met:
                 log.info(f'within a figure environment at line #{slot + 1}')
                 log.info(line)
                 modus = 'figure'
                 figure = [line]
                 try:
```

### Comparing `liitos-2023.2.8/liitos/meta.py` & `liitos-2023.5.9/liitos/meta.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/patch.py` & `liitos-2023.5.9/liitos/patch.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/render.py` & `liitos-2023.5.9/liitos/render.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Render the concat document to pdf."""
+import json
 import os
 import pathlib
+import re
 import shutil
 import time
 from typing import no_type_check
 
 import yaml
 
 import liitos.captions as cap
@@ -30,14 +32,15 @@
 DOC_BASE = pathlib.Path('..', '..')
 STRUCTURE_PATH = DOC_BASE / 'structure.yml'
 IMAGES_FOLDER = 'images/'
 DIAGRAMS_FOLDER = 'diagrams/'
 PATCH_SPEC_NAME = 'patch.yml'
 INTER_PROCESS_SYNC_SECS = 0.1
 INTER_PROCESS_SYNC_ATTEMPTS = 10
+VENDORED_SVG_PAT = re.compile(r'^.+\]\([^.]+\.[^.]+\.svg\ .+$')
 
 
 @no_type_check
 def der(
     doc_root: str | pathlib.Path, structure_name: str, target_key: str, facet_key: str, options: dict[str, bool | str]
 ) -> int:
     """Later alligator."""
@@ -173,42 +176,44 @@
 
         special_patching = []
         log.info(LOG_SEPARATOR)
         log.info('rewriting src attribute values of SVG to PNG sources ...')
         with open('document.md', 'rt', encoding=ENCODING) as handle:
             lines = [line.rstrip() for line in handle.readlines()]
         for slot, line in enumerate(lines):
-            if '.svg' in line and line.count('.') >= 2:
-                caption, src, alt, rest = con.parse_markdown_image(line)
-                stem, app_indicator, format_suffix = src.rsplit('.', 2)
-                log.info(f'- removing application indicator ({app_indicator}) from src ...')
-                if format_suffix != 'svg':
-                    log.warning(f'  + format_suffix (.{format_suffix}) unexpected in <<{line.rstrip()}>> ...')
-                fine = f'![{caption}]({stem}.png "{alt}"){rest}'
-                log.info(f'  transform[#{slot + 1}]: {line}')
-                log.info(f'       into[#{slot + 1}]: {fine}')
-                lines[slot] = fine
-                dia_path_old = src.replace('.svg', '.png')
-                dia_path_new = f'{stem}.png'
-                dia_fine_rstrip = dia_path_new.rstrip()
-                if dia_path_old and dia_path_new:
-                    special_patching.append((dia_path_old, dia_path_new))
-                    log.info(
-                        f'post-action[#{slot + 1}]: adding to queue for sync move: ({dia_path_old}) -> ({dia_path_new})'
-                    )
-                else:
-                    log.warning(f'- old: {src.rstrip()}')
-                    log.warning(f'- new: {dia_fine_rstrip}')
-                continue
-            if '.svg' in line:
-                fine = line.replace('.svg', '.png')
-                log.info(f'  transform[#{slot + 1}]: {line}')
-                log.info(f'       into[#{slot + 1}]: {fine}')
-                lines[slot] = fine
-                continue
+            if line.startswith('![') and '](' in line:
+                if VENDORED_SVG_PAT.match(line):
+                    if '.svg' in line and line.count('.') >= 2:
+                        caption, src, alt, rest = con.parse_markdown_image(line)
+                        stem, app_indicator, format_suffix = src.rsplit('.', 2)
+                        log.info(f'- removing application indicator ({app_indicator}) from src ...')
+                        if format_suffix != 'svg':
+                            log.warning(f'  + format_suffix (.{format_suffix}) unexpected in <<{line.rstrip()}>> ...')
+                        fine = f'![{caption}]({stem}.png "{alt}"){rest}'
+                        log.info(f'  transform[#{slot + 1}]: {line}')
+                        log.info(f'       into[#{slot + 1}]: {fine}')
+                        lines[slot] = fine
+                        dia_path_old = src.replace('.svg', '.png')
+                        dia_path_new = f'{stem}.png'
+                        dia_fine_rstrip = dia_path_new.rstrip()
+                        if dia_path_old and dia_path_new:
+                            special_patching.append((dia_path_old, dia_path_new))
+                            log.info(
+                                f'post-action[#{slot + 1}]: adding to queue for sync move: ({dia_path_old}) -> ({dia_path_new})'
+                            )
+                        else:
+                            log.warning(f'- old: {src.rstrip()}')
+                            log.warning(f'- new: {dia_fine_rstrip}')
+                        continue
+                if '.svg' in line:
+                    fine = line.replace('.svg', '.png')
+                    log.info(f'  transform[#{slot + 1}]: {line}')
+                    log.info(f'       into[#{slot + 1}]: {fine}')
+                    lines[slot] = fine
+                    continue
         with open('document.md', 'wt', encoding=ENCODING) as handle:
             handle.write('\n'.join(lines))
 
         log.info(LOG_SEPARATOR)
         log.info('ensure diagram files can be found when patched ...')
         if special_patching:
             for old, mew in special_patching:
@@ -236,14 +241,78 @@
                         f' and ({round(remaining_attempts * INTER_PROCESS_SYNC_SECS, 0) :.0f} seconds waiting)'
                     )
                 shutil.move(source_asset, target_asset)
         else:
             log.info('post-action queue (from reference renaming) is empty - nothing to move')
         log.info(LOG_SEPARATOR)
 
+        # prototyping >>>
+        fmt_spec = from_format_spec
+        in_doc = 'document.md'
+        out_doc = 'ast-no-filter.json'
+        markdown_to_ast_command = [
+            'pandoc',
+            '--verbose',
+            '-f',
+            fmt_spec,
+            '-t',
+            'json',
+            in_doc,
+            '-o',
+            out_doc,
+        ]
+        log.info(LOG_SEPARATOR)
+        log.info(f'executing ({" ".join(markdown_to_ast_command)}) ...')
+        if code := too.delegate(markdown_to_ast_command, 'markdown-to-ast'):
+            return code
+
+        log.info(LOG_SEPARATOR)
+
+        doc = json.load(open(out_doc, 'rt', encoding=ENCODING))
+        blocks = doc['blocks']
+        mermaid_caption_map = {}
+        for b in blocks:
+            if b['t'] == 'CodeBlock' and b['c'][0]:
+                is_mermaid = False
+                try:
+                    is_mermaid = b['c'][0][1][0] == 'mermaid'
+                    atts = b['c'][0][2]
+                except IndexError:
+                    continue
+
+                if not is_mermaid:
+                    continue
+                m_caption, m_filename, m_format, m_loc = '', '', '', ''
+                for k, v in atts:
+                    if k == 'caption':
+                        m_caption = v
+                    elif k == 'filename':
+                        m_filename = v
+                    elif k == 'format':
+                        m_format = v
+                    elif k == 'loc':
+                        m_loc = v
+                    else:
+                        pass
+                token = f'{m_loc}/{m_filename}.{m_format}'
+                if token in mermaid_caption_map:
+                    log.warning('Duplicate token, same caption?')
+                    log.warning(f'-   prior: {token} -> {m_caption}')
+                    log.warning(f'- current: {token} -> {mermaid_caption_map[token]}')
+                mermaid_caption_map[token] = m_caption
+
+        log.info(LOG_SEPARATOR)
+        # no KISS too.ensure_separate_log_lines(json.dumps, [mermaid_caption_map, 2])
+        for line in json.dumps(mermaid_caption_map, indent=2).split('\n'):
+            for fine in line.split('\n'):
+                log.info(fine)
+        log.info(LOG_SEPARATOR)
+
+        # <<< prototyping
+
         fmt_spec = from_format_spec
         in_doc = 'document.md'
         out_doc = LATEX_PAYLOAD_NAME
         filters = [added_prefix for expr in filter_cs_list for added_prefix in ('--filter', expr)]
         markdown_to_latex_command = [
             'pandoc',
             '--verbose',
@@ -267,52 +336,58 @@
 
         lines = too.execute_filter(
             cap.weave,
             head='move any captions below tables ...',
             backup='document-before-caps-patch.tex.txt',
             label='captions-below-tables',
             text_lines=lines,
+            lookup=None,
         )
 
         lines = too.execute_filter(
             lab.inject,
             head='inject stem (derived from file name) labels ...',
             backup='document-before-inject-stem-label-patch.tex.txt',
             label='inject-stem-derived-labels',
             text_lines=lines,
+            lookup=mermaid_caption_map,
         )
 
         lines = too.execute_filter(
             fig.scale,
             head='scale figures ...',
             backup='document-before-scale-figures-patch.tex.txt',
             label='inject-scale-figures',
             text_lines=lines,
+            lookup=None,
         )
 
         lines = too.execute_filter(
             dsc.options,
             head='add options to descriptions (definition lists) ...',
             backup='document-before-description-options-patch.tex.txt',
             label='inject-description-options',
             text_lines=lines,
+            lookup=None,
         )
 
         if options.get('patch_tables', False):
             lines = too.execute_filter(
-                dsc.options,
+                tab.patch,
                 head='patching tables EXPERIMENTAL (table-shape) ...',
                 backup='document-before-table-shape-patch.tex.txt',
                 label='changed-table-shape',
                 text_lines=lines,
+                lookup=None,
             )
         else:
             log.info(LOG_SEPARATOR)
             log.info('not patching tables but commenting out (ignoring) any columns command (table-shape) ...')
             patched_lines = [f'%IGNORED_{v}' if v.startswith(r'\columns=') else v for v in lines]
+            patched_lines = [f'%IGNORED_{v}' if v.startswith(r'\tablefontsize=') else v for v in patched_lines]
             log.info('diff of the (ignore-table-shape-if-not-patched) filter result:')
             too.log_unified_diff(lines, patched_lines)
             lines = patched_lines
             log.info(LOG_SEPARATOR)
 
         if need_patching:
             log.info(LOG_SEPARATOR)
```

### Comparing `liitos-2023.2.8/liitos/template_loader.py` & `liitos-2023.5.9/liitos/template_loader.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/templates/bookmatter.tex.in` & `liitos-2023.5.9/liitos/templates/bookmatter.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/templates/driver.tex.in` & `liitos-2023.5.9/liitos/templates/driver.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/templates/meta.yml` & `liitos-2023.5.9/liitos/templates/meta.yml`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/templates/metadata.tex.in` & `liitos-2023.5.9/liitos/templates/metadata.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/templates/mkdocs.yml.in` & `liitos-2023.5.9/liitos/templates/mkdocs.yml.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/templates/publisher.tex.in` & `liitos-2023.5.9/liitos/templates/publisher.tex.in`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 \hypertarget{status-and-change-log}{%
 \section*{Status and Change Log}\label{status-and-change-log}}
 
 \begin{longtable}[]{|
   >{\raggedright\arraybackslash}p{(\columnwidth - 6\tabcolsep) * \real{0.0600}}|
   >{\raggedright\arraybackslash}p{(\columnwidth - 6\tabcolsep) * \real{0.0600}}|
-  >{\raggedright\arraybackslash}p{(\columnwidth - 6\tabcolsep) * \real{0.1600}}|
-  >{\raggedright\arraybackslash}p{(\columnwidth - 6\tabcolsep) * \real{0.6900}}|}
+  >{\raggedright\arraybackslash}p{(\columnwidth - 6\tabcolsep) * \real{0.2000}}|
+  >{\raggedright\arraybackslash}p{(\columnwidth - 6\tabcolsep) * \real{0.6500}}|}
 \hline
 \begin{minipage}[b]{\linewidth}\raggedright
 \textbf{\theChangeLogIssLabel}
 \end{minipage} & \begin{minipage}[b]{\linewidth}\raggedright
 \textbf{\theChangeLogRevLabel}
 \end{minipage} & \begin{minipage}[b]{\linewidth}\raggedright
 \textbf{\theChangeLogAuthorLabel}
```

### Comparing `liitos-2023.2.8/liitos/templates/setup.tex.in` & `liitos-2023.5.9/liitos/templates/setup.tex.in`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 \setkeys{Gin}{width=\maxwidth,height=\maxheight,keepaspectratio}
 % set default figure placement
 \makeatletter
 \def\fps@figure{h!tbp}
 \makeatother
 % enable strikeout
 \usepackage{soul}
-\usepackage{ulem}
+\usepackage[normalem]{ulem}%% package with default options change emph to become underline instead of italics =(
 \setlength{\emergencystretch}{3em} % prevent overfull lines
 \providecommand{\tightlist}{%
   \setlength{\itemsep}{0pt}\setlength{\parskip}{0pt}}
 \setcounter{secnumdepth}{5}
 %dehyphenate
 \usepackage[american=nohyphenation]{hyphsubst}
 % ... woodpecker
```

### Comparing `liitos-2023.2.8/liitos/templates/vocabulary.yml` & `liitos-2023.5.9/liitos/templates/vocabulary.yml`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/liitos/tools.py` & `liitos-2023.5.9/liitos/tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -171,21 +171,28 @@
     code = delegate(tool_version_call, f'tool-version-of-{on}')
     log.info(LOG_SEPARATOR)
 
     return code
 
 
 @no_type_check
-def execute_filter(the_filter: Callable, head: str, backup: str, label: str, text_lines: list[str]) -> list[str]:
+def execute_filter(
+    the_filter: Callable,
+    head: str,
+    backup: str,
+    label: str,
+    text_lines: list[str],
+    lookup: dict[str, str] | None = None,
+) -> list[str]:
     """Chain filter calls by storing in and out lies in files and return the resulting lines."""
     log.info(LOG_SEPARATOR)
     log.info(head)
     doc_before_caps_patch = backup
     with open(doc_before_caps_patch, 'wt', encoding=ENCODING) as handle:
         handle.write('\n'.join(text_lines))
-    patched_lines = the_filter(text_lines)
+    patched_lines = the_filter(text_lines, lookup=lookup)
     with open(LATEX_PAYLOAD_NAME, 'wt', encoding=ENCODING) as handle:
         handle.write('\n'.join(patched_lines))
     log.info(f'diff of the ({label}) filter result:')
     log_unified_diff(text_lines, patched_lines)
 
     return patched_lines
```

### Comparing `liitos-2023.2.8/liitos.egg-info/PKG-INFO` & `liitos-2023.5.9/liitos.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: liitos
-Version: 2023.2.8
+Version: 2023.5.9
 Summary: Splice (Finnish liitos) contributions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/liitos
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/liitos
 Project-URL: Documentation, https://codes.dilettant.life/docs/liitos
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/liitos
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/liitos
 Keywords: developer-tools,validation,verification
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Liitos
 
@@ -36,25 +37,32 @@
 
 ## Documentation
 
 User and developer [documentation of liitos](https://codes.dilettant.life/docs/liitos).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of liitos](https://todo.sr.ht/~sthagen/liitos).
+Any feature requests or bug reports shall go to the [todos of liitos](https://todo.sr.ht/~sthagen/liitos).
 
 ## Primary Source repository
 
 The main source of `liitos` is on a mountain in central Switzerland.
 We use distributed version control (git).
 There is no central hub.
 Every clone can become a new source for the benefit of all.
 The preferred public clones of `liitos` are:
 
 * [on codeberg](https://codeberg.org/sthagen/liitos) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/liitos) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 # Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `liitos-2023.2.8/liitos.egg-info/SOURCES.txt` & `liitos-2023.5.9/liitos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/pyproject.toml` & `liitos-2023.5.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "liitos"
-version = "2023.2.8"
+version = "2023.5.9"
 description = "Splice (Finnish liitos) contributions."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 keywords = ["developer-tools", "validation", "verification"]
 dependencies = [
     "PyYAML >= 6.0",
     "foran >= 2022.12.7",
     "shellingham >= 1.5.0.post1",
     "taksonomia >= 2023.1.24",
-    "treelib >= 1.6.1",
+    "treelib >= 1.6.4",
     "typer >= 0.7.0",
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["black", "coverage", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "ruff"]
```

### Comparing `liitos-2023.2.8/test/test_captions.py` & `liitos-2023.5.9/test/test_captions.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/test/test_cli.py` & `liitos-2023.5.9/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/test/test_concat.py` & `liitos-2023.5.9/test/test_concat.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/test/test_eject.py` & `liitos-2023.5.9/test/test_eject.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/test/test_figures.py` & `liitos-2023.5.9/test/test_figures.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/test/test_gather.py` & `liitos-2023.5.9/test/test_gather.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/test/test_labels.py` & `liitos-2023.5.9/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/test/test_meta.py` & `liitos-2023.5.9/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/test/test_patch.py` & `liitos-2023.5.9/test/test_patch.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.2.8/test/test_tools.py` & `liitos-2023.5.9/test/test_tools.py`

 * *Files identical despite different names*

