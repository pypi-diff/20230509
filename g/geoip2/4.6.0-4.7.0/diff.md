# Comparing `tmp/geoip2-4.6.0.tar.gz` & `tmp/geoip2-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoip2-4.6.0.tar", last modified: Tue Jun 21 16:18:47 2022, max compression
+gzip compressed data, was "geoip2-4.7.0.tar", last modified: Tue May  9 20:26:38 2023, max compression
```

## Comparing `geoip2-4.6.0.tar` & `geoip2-4.7.0.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2022-06-21 16:18:47.750541 geoip2-4.6.0/
--rw-r--r--   0 greg      (1000) greg      (1000)    11898 2022-06-21 16:05:22.000000 geoip2-4.6.0/HISTORY.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    11358 2019-02-08 20:42:43.000000 geoip2-4.6.0/LICENSE
--rw-r--r--   0 greg      (1000) greg      (1000)      127 2021-09-20 17:34:42.000000 geoip2-4.6.0/MANIFEST.in
--rw-r--r--   0 greg      (1000) greg      (1000)    18040 2022-06-21 16:18:47.750541 geoip2-4.6.0/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)    16880 2022-06-21 15:45:27.000000 geoip2-4.6.0/README.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2022-06-21 16:18:47.742541 geoip2-4.6.0/docs/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2022-06-21 16:18:47.742541 geoip2-4.6.0/docs/html/
--rw-r--r--   0 greg      (1000) greg      (1000)      230 2022-06-21 16:18:47.000000 geoip2-4.6.0/docs/html/.buildinfo
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2022-06-21 16:18:47.742541 geoip2-4.6.0/docs/html/_sources/
--rw-r--r--   0 greg      (1000) greg      (1000)      763 2022-03-04 21:37:06.000000 geoip2-4.6.0/docs/html/_sources/index.rst.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2022-06-21 16:18:47.746541 geoip2-4.6.0/docs/html/_static/
--rw-r--r--   0 greg      (1000) greg      (1000)    14692 2022-06-21 16:18:47.000000 geoip2-4.6.0/docs/html/_static/basic.css
--rw-r--r--   0 greg      (1000) greg      (1000)      107 2020-07-21 17:29:28.000000 geoip2-4.6.0/docs/html/_static/contents.png
--rw-r--r--   0 greg      (1000) greg      (1000)    10766 2022-03-28 19:26:41.000000 geoip2-4.6.0/docs/html/_static/doctools.js
--rw-r--r--   0 greg      (1000) greg      (1000)      422 2022-06-21 16:18:47.000000 geoip2-4.6.0/docs/html/_static/documentation_options.js
--rw-r--r--   0 greg      (1000) greg      (1000)      286 2020-07-21 17:29:28.000000 geoip2-4.6.0/docs/html/_static/file.png
--rw-r--r--   0 greg      (1000) greg      (1000)   287630 2020-07-21 17:29:28.000000 geoip2-4.6.0/docs/html/_static/jquery-3.5.1.js
--rw-r--r--   0 greg      (1000) greg      (1000)    89476 2020-07-21 17:29:28.000000 geoip2-4.6.0/docs/html/_static/jquery.js
--rw-r--r--   0 greg      (1000) greg      (1000)    10854 2022-06-21 16:18:47.000000 geoip2-4.6.0/docs/html/_static/language_data.js
--rw-r--r--   0 greg      (1000) greg      (1000)       90 2020-07-21 17:29:28.000000 geoip2-4.6.0/docs/html/_static/minus.png
--rw-r--r--   0 greg      (1000) greg      (1000)      120 2020-07-21 17:29:28.000000 geoip2-4.6.0/docs/html/_static/navigation.png
--rw-r--r--   0 greg      (1000) greg      (1000)       90 2020-07-21 17:29:28.000000 geoip2-4.6.0/docs/html/_static/plus.png
--rw-r--r--   0 greg      (1000) greg      (1000)     4846 2022-06-21 16:18:47.000000 geoip2-4.6.0/docs/html/_static/pygments.css
--rw-r--r--   0 greg      (1000) greg      (1000)    16634 2022-03-28 19:26:41.000000 geoip2-4.6.0/docs/html/_static/searchtools.js
--rw-r--r--   0 greg      (1000) greg      (1000)     6236 2022-06-21 16:18:47.000000 geoip2-4.6.0/docs/html/_static/sphinxdoc.css
--rw-r--r--   0 greg      (1000) greg      (1000)    68420 2021-09-20 17:44:35.000000 geoip2-4.6.0/docs/html/_static/underscore-1.13.1.js
--rw-r--r--   0 greg      (1000) greg      (1000)    35168 2020-07-21 17:29:28.000000 geoip2-4.6.0/docs/html/_static/underscore-1.3.1.js
--rw-r--r--   0 greg      (1000) greg      (1000)    19530 2021-09-20 17:44:35.000000 geoip2-4.6.0/docs/html/_static/underscore.js
--rw-r--r--   0 greg      (1000) greg      (1000)    29048 2022-06-21 16:18:47.000000 geoip2-4.6.0/docs/html/genindex.html
--rw-r--r--   0 greg      (1000) greg      (1000)   286972 2022-06-21 16:18:47.000000 geoip2-4.6.0/docs/html/index.html
--rw-r--r--   0 greg      (1000) greg      (1000)     1400 2022-06-21 16:18:47.000000 geoip2-4.6.0/docs/html/objects.inv
--rw-r--r--   0 greg      (1000) greg      (1000)     4600 2022-06-21 16:18:47.000000 geoip2-4.6.0/docs/html/py-modindex.html
--rw-r--r--   0 greg      (1000) greg      (1000)     3358 2022-06-21 16:18:47.000000 geoip2-4.6.0/docs/html/search.html
--rw-r--r--   0 greg      (1000) greg      (1000)    12046 2022-06-21 16:18:47.000000 geoip2-4.6.0/docs/html/searchindex.js
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2022-06-21 16:18:47.746541 geoip2-4.6.0/geoip2/
--rw-r--r--   0 greg      (1000) greg      (1000)      199 2022-06-21 16:18:36.000000 geoip2-4.6.0/geoip2/__init__.py
--rw-r--r--   0 greg      (1000) greg      (1000)     9137 2022-06-21 15:52:53.000000 geoip2-4.6.0/geoip2/database.py
--rw-r--r--   0 greg      (1000) greg      (1000)     2545 2022-06-21 16:05:57.000000 geoip2-4.6.0/geoip2/errors.py
--rw-r--r--   0 greg      (1000) greg      (1000)      410 2020-07-14 21:41:43.000000 geoip2-4.6.0/geoip2/mixins.py
--rw-r--r--   0 greg      (1000) greg      (1000)    17590 2022-06-09 15:31:38.000000 geoip2-4.6.0/geoip2/models.py
--rw-r--r--   0 greg      (1000) greg      (1000)        0 2020-07-28 17:27:21.000000 geoip2-4.6.0/geoip2/py.typed
--rw-r--r--   0 greg      (1000) greg      (1000)    25548 2022-06-09 15:31:38.000000 geoip2-4.6.0/geoip2/records.py
--rw-r--r--   0 greg      (1000) greg      (1000)      160 2020-07-14 21:41:43.000000 geoip2-4.6.0/geoip2/types.py
--rw-r--r--   0 greg      (1000) greg      (1000)    17340 2022-06-21 16:04:25.000000 geoip2-4.6.0/geoip2/webservice.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2022-06-21 16:18:47.746541 geoip2-4.6.0/geoip2.egg-info/
--rw-r--r--   0 greg      (1000) greg      (1000)    18040 2022-06-21 16:18:47.000000 geoip2-4.6.0/geoip2.egg-info/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     2935 2022-06-21 16:18:47.000000 geoip2-4.6.0/geoip2.egg-info/SOURCES.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2022-06-21 16:18:47.000000 geoip2-4.6.0/geoip2.egg-info/dependency_links.txt
--rw-r--r--   0 greg      (1000) greg      (1000)       93 2022-06-21 16:18:47.000000 geoip2-4.6.0/geoip2.egg-info/requires.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        7 2022-06-21 16:18:47.000000 geoip2-4.6.0/geoip2.egg-info/top_level.txt
--rw-r--r--   0 greg      (1000) greg      (1000)       93 2021-09-24 18:42:59.000000 geoip2-4.6.0/requirements.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      410 2022-06-21 16:18:47.750541 geoip2-4.6.0/setup.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)     1707 2022-06-21 15:45:27.000000 geoip2-4.6.0/setup.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2022-06-21 16:18:47.746541 geoip2-4.6.0/tests/
--rw-r--r--   0 greg      (1000) greg      (1000)        0 2019-02-08 20:42:43.000000 geoip2-4.6.0/tests/__init__.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2022-06-21 16:18:47.742541 geoip2-4.6.0/tests/data/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2022-06-21 16:18:47.750541 geoip2-4.6.0/tests/data/test-data/
--rw-r--r--   0 greg      (1000) greg      (1000)     4382 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-Anonymous-IP-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    20887 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-City-Test-Broken-Double-Format.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    21281 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-City-Test-Invalid-Node-Count.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    21261 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-City-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     4423 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-Connection-Type-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    19583 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-Country-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3065 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-DensityIncome-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     6326 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-Domain-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     8317 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-Enterprise-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    76623 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-ISP-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    16753 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-Precision-Enterprise-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     9750 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-Static-IP-Score-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     4818 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoIP2-User-Count-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    12665 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoLite2-ASN-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    20809 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoLite2-City-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    17952 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/GeoLite2-Country-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)      618 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-no-ipv4-search-tree.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1341 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-string-value-entries.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1289 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-broken-pointers-24.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1298 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-broken-search-tree-24.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3191 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-decoder.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1298 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-ipv4-24.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1462 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-ipv4-28.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1626 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-ipv4-32.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     2806 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-ipv6-24.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3222 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-ipv6-28.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3638 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-ipv6-32.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     2258 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-metadata-pointers.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3066 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-mixed-24.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3511 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-mixed-28.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3956 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-mixed-32.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3802 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-nested.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1737 2021-11-17 17:00:38.000000 geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-pointer-decoder.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    10158 2022-06-21 15:45:27.000000 geoip2-4.6.0/tests/database_test.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    16377 2022-06-21 15:52:54.000000 geoip2-4.6.0/tests/models_test.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    12944 2020-09-25 15:00:20.000000 geoip2-4.6.0/tests/webservice_test.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:26:38.130013 geoip2-4.7.0/
+-rw-r--r--   0 greg      (1000) greg      (1000)    12054 2023-05-09 20:21:36.000000 geoip2-4.7.0/HISTORY.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)    11358 2019-02-08 20:42:43.000000 geoip2-4.7.0/LICENSE
+-rw-r--r--   0 greg      (1000) greg      (1000)      127 2021-09-20 17:34:42.000000 geoip2-4.7.0/MANIFEST.in
+-rw-r--r--   0 greg      (1000) greg      (1000)    17990 2023-05-09 20:26:38.130013 geoip2-4.7.0/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)    16880 2023-01-17 16:27:12.000000 geoip2-4.7.0/README.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:26:38.114013 geoip2-4.7.0/docs/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:26:38.118013 geoip2-4.7.0/docs/html/
+-rw-r--r--   0 greg      (1000) greg      (1000)      230 2023-05-09 20:26:38.000000 geoip2-4.7.0/docs/html/.buildinfo
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:26:38.118013 geoip2-4.7.0/docs/html/_sources/
+-rw-r--r--   0 greg      (1000) greg      (1000)      763 2022-03-04 21:37:06.000000 geoip2-4.7.0/docs/html/_sources/index.rst.txt
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:26:38.122013 geoip2-4.7.0/docs/html/_static/
+-rw-r--r--   0 greg      (1000) greg      (1000)    14692 2023-05-09 20:26:38.000000 geoip2-4.7.0/docs/html/_static/basic.css
+-rw-r--r--   0 greg      (1000) greg      (1000)      107 2020-07-21 17:29:28.000000 geoip2-4.7.0/docs/html/_static/contents.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    10766 2022-03-28 19:26:41.000000 geoip2-4.7.0/docs/html/_static/doctools.js
+-rw-r--r--   0 greg      (1000) greg      (1000)      422 2023-05-09 20:26:38.000000 geoip2-4.7.0/docs/html/_static/documentation_options.js
+-rw-r--r--   0 greg      (1000) greg      (1000)      286 2020-07-21 17:29:28.000000 geoip2-4.7.0/docs/html/_static/file.png
+-rw-r--r--   0 greg      (1000) greg      (1000)   287630 2020-07-21 17:29:28.000000 geoip2-4.7.0/docs/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 greg      (1000) greg      (1000)    89476 2020-07-21 17:29:28.000000 geoip2-4.7.0/docs/html/_static/jquery.js
+-rw-r--r--   0 greg      (1000) greg      (1000)    10854 2023-05-09 20:26:38.000000 geoip2-4.7.0/docs/html/_static/language_data.js
+-rw-r--r--   0 greg      (1000) greg      (1000)       90 2020-07-21 17:29:28.000000 geoip2-4.7.0/docs/html/_static/minus.png
+-rw-r--r--   0 greg      (1000) greg      (1000)      120 2020-07-21 17:29:28.000000 geoip2-4.7.0/docs/html/_static/navigation.png
+-rw-r--r--   0 greg      (1000) greg      (1000)       90 2020-07-21 17:29:28.000000 geoip2-4.7.0/docs/html/_static/plus.png
+-rw-r--r--   0 greg      (1000) greg      (1000)     4846 2023-05-09 20:26:38.000000 geoip2-4.7.0/docs/html/_static/pygments.css
+-rw-r--r--   0 greg      (1000) greg      (1000)    16634 2022-03-28 19:26:41.000000 geoip2-4.7.0/docs/html/_static/searchtools.js
+-rw-r--r--   0 greg      (1000) greg      (1000)     6236 2023-05-09 20:26:38.000000 geoip2-4.7.0/docs/html/_static/sphinxdoc.css
+-rw-r--r--   0 greg      (1000) greg      (1000)    68420 2021-09-20 17:44:35.000000 geoip2-4.7.0/docs/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 greg      (1000) greg      (1000)    35168 2020-07-21 17:29:28.000000 geoip2-4.7.0/docs/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 greg      (1000) greg      (1000)    19530 2021-09-20 17:44:35.000000 geoip2-4.7.0/docs/html/_static/underscore.js
+-rw-r--r--   0 greg      (1000) greg      (1000)    29048 2023-05-09 20:26:38.000000 geoip2-4.7.0/docs/html/genindex.html
+-rw-r--r--   0 greg      (1000) greg      (1000)   287087 2023-05-09 20:26:38.000000 geoip2-4.7.0/docs/html/index.html
+-rw-r--r--   0 greg      (1000) greg      (1000)     1400 2023-05-09 20:26:38.000000 geoip2-4.7.0/docs/html/objects.inv
+-rw-r--r--   0 greg      (1000) greg      (1000)     4600 2023-05-09 20:26:38.000000 geoip2-4.7.0/docs/html/py-modindex.html
+-rw-r--r--   0 greg      (1000) greg      (1000)     3358 2023-05-09 20:26:38.000000 geoip2-4.7.0/docs/html/search.html
+-rw-r--r--   0 greg      (1000) greg      (1000)    12053 2023-05-09 20:26:38.000000 geoip2-4.7.0/docs/html/searchindex.js
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:26:38.122013 geoip2-4.7.0/geoip2/
+-rw-r--r--   0 greg      (1000) greg      (1000)      199 2023-05-09 20:26:25.000000 geoip2-4.7.0/geoip2/__init__.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     9137 2023-01-17 17:40:13.000000 geoip2-4.7.0/geoip2/database.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     2545 2023-01-17 16:27:12.000000 geoip2-4.7.0/geoip2/errors.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      410 2023-01-17 17:40:13.000000 geoip2-4.7.0/geoip2/mixins.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    17590 2022-06-09 15:31:38.000000 geoip2-4.7.0/geoip2/models.py
+-rw-r--r--   0 greg      (1000) greg      (1000)        0 2020-07-28 17:27:21.000000 geoip2-4.7.0/geoip2/py.typed
+-rw-r--r--   0 greg      (1000) greg      (1000)    25548 2023-01-17 17:38:28.000000 geoip2-4.7.0/geoip2/records.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      160 2020-07-14 21:41:43.000000 geoip2-4.7.0/geoip2/types.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    17287 2023-02-28 22:24:20.000000 geoip2-4.7.0/geoip2/webservice.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:26:38.122013 geoip2-4.7.0/geoip2.egg-info/
+-rw-r--r--   0 greg      (1000) greg      (1000)    17990 2023-05-09 20:26:38.000000 geoip2-4.7.0/geoip2.egg-info/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     2950 2023-05-09 20:26:38.000000 geoip2-4.7.0/geoip2.egg-info/SOURCES.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-05-09 20:26:38.000000 geoip2-4.7.0/geoip2.egg-info/dependency_links.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)       70 2023-05-09 20:26:38.000000 geoip2-4.7.0/geoip2.egg-info/requires.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        7 2023-05-09 20:26:38.000000 geoip2-4.7.0/geoip2.egg-info/top_level.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      169 2023-02-28 22:24:20.000000 geoip2-4.7.0/pyproject.toml
+-rw-r--r--   0 greg      (1000) greg      (1000)       70 2023-05-09 20:21:15.000000 geoip2-4.7.0/requirements.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      805 2023-05-09 20:26:38.130013 geoip2-4.7.0/setup.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)     1659 2023-05-08 21:15:16.000000 geoip2-4.7.0/setup.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:26:38.122013 geoip2-4.7.0/tests/
+-rw-r--r--   0 greg      (1000) greg      (1000)        0 2019-02-08 20:42:43.000000 geoip2-4.7.0/tests/__init__.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:26:38.114013 geoip2-4.7.0/tests/data/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:26:38.130013 geoip2-4.7.0/tests/data/test-data/
+-rw-r--r--   0 greg      (1000) greg      (1000)     4382 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-Anonymous-IP-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    20887 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-City-Test-Broken-Double-Format.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    21281 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-City-Test-Invalid-Node-Count.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    21261 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-City-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     4423 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-Connection-Type-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    19583 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-Country-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3065 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-DensityIncome-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     6326 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-Domain-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     8317 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-Enterprise-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    76623 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-ISP-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    16753 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-Precision-Enterprise-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     9750 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-Static-IP-Score-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     4818 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoIP2-User-Count-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    12665 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoLite2-ASN-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    20809 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoLite2-City-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    17952 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/GeoLite2-Country-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)      618 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-no-ipv4-search-tree.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1341 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-string-value-entries.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1289 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-broken-pointers-24.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1298 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-broken-search-tree-24.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3191 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-decoder.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1298 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-ipv4-24.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1462 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-ipv4-28.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1626 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-ipv4-32.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     2806 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-ipv6-24.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3222 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-ipv6-28.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3638 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-ipv6-32.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     2258 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-metadata-pointers.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3066 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-mixed-24.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3511 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-mixed-28.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3956 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-mixed-32.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3802 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-nested.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1737 2021-11-17 17:00:38.000000 geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-pointer-decoder.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    10158 2022-06-21 15:45:27.000000 geoip2-4.7.0/tests/database_test.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    16376 2023-02-28 22:24:20.000000 geoip2-4.7.0/tests/models_test.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    13078 2023-05-08 21:15:16.000000 geoip2-4.7.0/tests/webservice_test.py
```

### Comparing `geoip2-4.6.0/HISTORY.rst` & `geoip2-4.7.0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 
 .. :changelog:
 
 History
 -------
 
+4.7.0 (2023-05-09)
+++++++++++++++++++
+
+* IMPORTANT: Python 3.7 or greater is required. If you are using an older
+  version, please use an earlier release.
+
 4.6.0 (2022-06-21)
 ++++++++++++++++++
 
 * The ``AddressNotFoundError`` class now has an ``ip_address`` attribute
   with the lookup address and ``network`` property for the empty network
   in the database containing the IP address. These are only available
   when using a database, not the web service. Pull request by illes.
```

### Comparing `geoip2-4.6.0/LICENSE` & `geoip2-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/PKG-INFO` & `geoip2-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoip2
-Version: 4.6.0
+Version: 4.7.0
 Summary: MaxMind GeoIP2 API
 Home-page: http://www.maxmind.com/
 Author: Gregory Oschwald
 Author-email: goschwald@maxmind.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://geoip2.readthedocs.org/
 Project-URL: Source Code, https://github.com/maxmind/GeoIP2-python
@@ -12,23 +12,22 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Internet
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 =========================
 MaxMind GeoIP2 Python API
 =========================
 
 Description
@@ -514,15 +513,15 @@
 If you are a paying MaxMind customer and you're not sure where to submit a
 correction, please `contact MaxMind support
 <http://www.maxmind.com/en/support>`_ for help.
 
 Requirements
 ------------
 
-Python 3.6 or greater is required. Older versions are not supported.
+Python 3.7 or greater is required. Older versions are not supported.
 
 The Requests HTTP library is also required. See
 <http://python-requests.org> for details.
 
 Versioning
 ----------
```

### Comparing `geoip2-4.6.0/README.rst` & `geoip2-4.7.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -485,15 +485,15 @@
 If you are a paying MaxMind customer and you're not sure where to submit a
 correction, please `contact MaxMind support
 <http://www.maxmind.com/en/support>`_ for help.
 
 Requirements
 ------------
 
-Python 3.6 or greater is required. Older versions are not supported.
+Python 3.7 or greater is required. Older versions are not supported.
 
 The Requests HTTP library is also required. See
 <http://python-requests.org> for details.
 
 Versioning
 ----------
```

### Comparing `geoip2-4.6.0/docs/html/_sources/index.rst.txt` & `geoip2-4.7.0/docs/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/docs/html/_static/basic.css` & `geoip2-4.7.0/docs/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/docs/html/_static/doctools.js` & `geoip2-4.7.0/docs/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/docs/html/_static/jquery-3.5.1.js` & `geoip2-4.7.0/docs/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/docs/html/_static/jquery.js` & `geoip2-4.7.0/docs/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/docs/html/_static/language_data.js` & `geoip2-4.7.0/docs/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/docs/html/_static/pygments.css` & `geoip2-4.7.0/docs/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/docs/html/_static/searchtools.js` & `geoip2-4.7.0/docs/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/docs/html/_static/sphinxdoc.css` & `geoip2-4.7.0/docs/html/_static/sphinxdoc.css`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/docs/html/_static/underscore-1.13.1.js` & `geoip2-4.7.0/docs/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/docs/html/_static/underscore-1.3.1.js` & `geoip2-4.7.0/docs/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/docs/html/_static/underscore.js` & `geoip2-4.7.0/docs/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/docs/html/genindex.html` & `geoip2-4.7.0/docs/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; geoip2 4.6.0 documentation</title>
+    <title>Index &#8212; geoip2 4.7.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinxdoc.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="#" />
@@ -20,15 +20,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">geoip2 4.6.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">geoip2 4.7.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -689,15 +689,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">geoip2 4.6.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">geoip2 4.7.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2013-2022, MaxMind, Inc..
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.5.0.
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * geoip2_4.6.0_documentation »
+    * geoip2_4.7.0_documentation »
     * Index
 ****** Index ******
 A | C | D | E | G | H | I | L | M | N | O | P | Q | R | S | T | U
 ***** A *****
     * accuracy_radius_                    * AuthenticationError
       (geoip2.records.Location            * autonomous_system_number_
       attribute)                            (geoip2.models.ASN_attribute)
@@ -210,10 +210,10 @@
     * user_count_(geoip2.records.Traits     * user_type_(geoip2.records.Traits
       attribute)                              attribute)
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * geoip2_4.6.0_documentation »
+    * geoip2_4.7.0_documentation »
     * Index
 © Copyright 2013-2022, MaxMind, Inc.. Created using Sphinx 4.5.0.
```

### Comparing `geoip2-4.6.0/docs/html/index.html` & `geoip2-4.7.0/docs/html/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>MaxMind GeoIP2 Python API &#8212; geoip2 4.6.0 documentation</title>
+    <title>MaxMind GeoIP2 Python API &#8212; geoip2 4.7.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinxdoc.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -21,15 +21,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">geoip2 4.6.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">geoip2 4.7.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">MaxMind GeoIP2 Python API</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -42,20 +42,20 @@
 <section id="description">
 <h2>Description<a class="headerlink" href="#description" title="Permalink to this headline">¶</a></h2>
 <p>This package provides an API for the GeoIP2 and GeoLite2 <a class="reference external" href="https://dev.maxmind.com/geoip/docs/web-services?lang=en">web services</a> and <a class="reference external" href="https://dev.maxmind.com/geoip/docs/databases?lang=en">databases</a>.</p>
 </section>
 <section id="installation">
 <h2>Installation<a class="headerlink" href="#installation" title="Permalink to this headline">¶</a></h2>
 <p>To install the <code class="docutils literal notranslate"><span class="pre">geoip2</span></code> module, type:</p>
-<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$ pip install geoip2
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span>pip<span class="w"> </span>install<span class="w"> </span>geoip2
 </pre></div>
 </div>
 <p>If you are not able to use pip, you may also use easy_install from the
 source directory:</p>
-<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$ easy_install .
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span>easy_install<span class="w"> </span>.
 </pre></div>
 </div>
 <section id="database-reader-extension">
 <h3>Database Reader Extension<a class="headerlink" href="#database-reader-extension" title="Permalink to this headline">¶</a></h3>
 <p>If you wish to use the C extension for the database reader, you must first
 install the <a class="reference external" href="https://github.com/maxmind/libmaxminddb">libmaxminddb C API</a>.
 Please <a class="reference external" href="https://github.com/maxmind/libmaxminddb/blob/main/README.md">see the instructions distributed with it</a>.</p>
@@ -80,101 +80,101 @@
 endpoint you called. This model in turn contains multiple record classes,
 each of which represents part of the data returned by the web service.</p>
 <p>If the request fails, the client class throws an exception.</p>
 </section>
 <section id="sync-web-service-example">
 <h2>Sync Web Service Example<a class="headerlink" href="#sync-web-service-example" title="Permalink to this headline">¶</a></h2>
 <div class="highlight-pycon notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">geoip2.webservice</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># This creates a Client object that can be reused across requests.</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># Replace &quot;42&quot; with your account ID and &quot;license_key&quot; with your license</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># key. Set the &quot;host&quot; keyword argument to &quot;geolite.info&quot; to use the</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># GeoLite2 web service instead of the GeoIP2 web service.</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="k">with</span> <span class="n">geoip2</span><span class="o">.</span><span class="n">webservice</span><span class="o">.</span><span class="n">Client</span><span class="p">(</span><span class="mi">42</span><span class="p">,</span> <span class="s1">&#39;license_key&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">client</span><span class="p">:</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># Replace &quot;city&quot; with the method corresponding to the web service</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># that you are using, i.e., &quot;country&quot;, &quot;city&quot;, or &quot;insights&quot;. Please</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># note that Insights is not supported by the GeoLite2 web service.</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span> <span class="o">=</span> <span class="n">client</span><span class="o">.</span><span class="n">city</span><span class="p">(</span><span class="s1">&#39;203.0.113.0&#39;</span><span class="p">)</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">iso_code</span>
 <span class="go">&#39;US&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">name</span>
 <span class="go">&#39;United States&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">names</span><span class="p">[</span><span class="s1">&#39;zh-CN&#39;</span><span class="p">]</span>
 <span class="go">u&#39;美国&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">subdivisions</span><span class="o">.</span><span class="n">most_specific</span><span class="o">.</span><span class="n">name</span>
 <span class="go">&#39;Minnesota&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">subdivisions</span><span class="o">.</span><span class="n">most_specific</span><span class="o">.</span><span class="n">iso_code</span>
 <span class="go">&#39;MN&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">city</span><span class="o">.</span><span class="n">name</span>
 <span class="go">&#39;Minneapolis&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">postal</span><span class="o">.</span><span class="n">code</span>
 <span class="go">&#39;55455&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">location</span><span class="o">.</span><span class="n">latitude</span>
 <span class="go">44.9733</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">location</span><span class="o">.</span><span class="n">longitude</span>
 <span class="go">-93.2323</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">traits</span><span class="o">.</span><span class="n">network</span>
 <span class="go">IPv4Network(&#39;203.0.113.0/32&#39;)</span>
 </pre></div>
 </div>
 </section>
 <section id="async-web-service-example">
 <h2>Async Web Service Example<a class="headerlink" href="#async-web-service-example" title="Permalink to this headline">¶</a></h2>
 <div class="highlight-pycon notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">asyncio</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">geoip2.webservice</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="k">async</span> <span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># This creates an AsyncClient object that can be reused across</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># requests on the running event loop. If you are using multiple event</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># loops, you must ensure the object is not used on another loop.</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1">#</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># Replace &quot;42&quot; with your account ID and &quot;license_key&quot; with your license</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># key. Set the &quot;host&quot; keyword argument to &quot;geolite.info&quot; to use the</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># GeoLite2 web service instead of the GeoIP2 web service.</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="k">async</span> <span class="k">with</span> <span class="n">geoip2</span><span class="o">.</span><span class="n">webservice</span><span class="o">.</span><span class="n">AsyncClient</span><span class="p">(</span><span class="mi">42</span><span class="p">,</span> <span class="s1">&#39;license_key&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">client</span><span class="p">:</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="c1"># Replace &quot;city&quot; with the method corresponding to the web service</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="c1"># that you are using, i.e., &quot;country&quot;, &quot;city&quot;, or &quot;insights&quot;. Please</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="c1"># note that Insights is not supported by the GeoLite2 web service.</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="n">response</span> <span class="o">=</span> <span class="k">await</span> <span class="n">client</span><span class="o">.</span><span class="n">city</span><span class="p">(</span><span class="s1">&#39;203.0.113.0&#39;</span><span class="p">)</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">iso_code</span>
 <span class="go">&#39;US&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">name</span>
 <span class="go">&#39;United States&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">names</span><span class="p">[</span><span class="s1">&#39;zh-CN&#39;</span><span class="p">]</span>
 <span class="go">u&#39;美国&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="n">response</span><span class="o">.</span><span class="n">subdivisions</span><span class="o">.</span><span class="n">most_specific</span><span class="o">.</span><span class="n">name</span>
 <span class="go">&#39;Minnesota&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="n">response</span><span class="o">.</span><span class="n">subdivisions</span><span class="o">.</span><span class="n">most_specific</span><span class="o">.</span><span class="n">iso_code</span>
 <span class="go">&#39;MN&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="n">response</span><span class="o">.</span><span class="n">city</span><span class="o">.</span><span class="n">name</span>
 <span class="go">&#39;Minneapolis&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="n">response</span><span class="o">.</span><span class="n">postal</span><span class="o">.</span><span class="n">code</span>
 <span class="go">&#39;55455&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="n">response</span><span class="o">.</span><span class="n">location</span><span class="o">.</span><span class="n">latitude</span>
 <span class="go">44.9733</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="n">response</span><span class="o">.</span><span class="n">location</span><span class="o">.</span><span class="n">longitude</span>
 <span class="go">-93.2323</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>        <span class="n">response</span><span class="o">.</span><span class="n">traits</span><span class="o">.</span><span class="n">network</span>
 <span class="go">IPv4Network(&#39;203.0.113.0/32&#39;)</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">asyncio</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">main</span><span class="p">())</span>
 </pre></div>
 </div>
 </section>
 <section id="web-service-client-exceptions">
 <h2>Web Service Client Exceptions<a class="headerlink" href="#web-service-client-exceptions" title="Permalink to this headline">¶</a></h2>
 <p>For details on the possible errors returned by the web service itself, see
@@ -203,61 +203,61 @@
 <p>If the request fails, the reader class throws an exception.</p>
 </section>
 <section id="database-example">
 <h2>Database Example<a class="headerlink" href="#database-example" title="Permalink to this headline">¶</a></h2>
 <section id="city-database">
 <h3>City Database<a class="headerlink" href="#city-database" title="Permalink to this headline">¶</a></h3>
 <div class="highlight-pycon notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">geoip2.database</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># This creates a Reader object. You should use the same object</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># across multiple requests as creation of it is expensive.</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="k">with</span> <span class="n">geoip2</span><span class="o">.</span><span class="n">database</span><span class="o">.</span><span class="n">Reader</span><span class="p">(</span><span class="s1">&#39;/path/to/GeoLite2-City.mmdb&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">reader</span><span class="p">:</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># Replace &quot;city&quot; with the method corresponding to the database</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># that you are using, e.g., &quot;country&quot;.</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span> <span class="o">=</span> <span class="n">reader</span><span class="o">.</span><span class="n">city</span><span class="p">(</span><span class="s1">&#39;203.0.113.0&#39;</span><span class="p">)</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">iso_code</span>
 <span class="go">&#39;US&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">name</span>
 <span class="go">&#39;United States&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">names</span><span class="p">[</span><span class="s1">&#39;zh-CN&#39;</span><span class="p">]</span>
 <span class="go">u&#39;美国&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">subdivisions</span><span class="o">.</span><span class="n">most_specific</span><span class="o">.</span><span class="n">name</span>
 <span class="go">&#39;Minnesota&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">subdivisions</span><span class="o">.</span><span class="n">most_specific</span><span class="o">.</span><span class="n">iso_code</span>
 <span class="go">&#39;MN&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">city</span><span class="o">.</span><span class="n">name</span>
 <span class="go">&#39;Minneapolis&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">postal</span><span class="o">.</span><span class="n">code</span>
 <span class="go">&#39;55455&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">location</span><span class="o">.</span><span class="n">latitude</span>
 <span class="go">44.9733</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">location</span><span class="o">.</span><span class="n">longitude</span>
 <span class="go">-93.2323</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">traits</span><span class="o">.</span><span class="n">network</span>
 <span class="go">IPv4Network(&#39;203.0.113.0/24&#39;)</span>
 </pre></div>
 </div>
 </section>
 <section id="anonymous-ip-database">
 <h3>Anonymous IP Database<a class="headerlink" href="#anonymous-ip-database" title="Permalink to this headline">¶</a></h3>
 <div class="highlight-pycon notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">geoip2.database</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># This creates a Reader object. You should use the same object</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># across multiple requests as creation of it is expensive.</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="k">with</span> <span class="n">geoip2</span><span class="o">.</span><span class="n">database</span><span class="o">.</span><span class="n">Reader</span><span class="p">(</span><span class="s1">&#39;/path/to/GeoIP2-Anonymous-IP.mmdb&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">reader</span><span class="p">:</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span> <span class="o">=</span> <span class="n">reader</span><span class="o">.</span><span class="n">anonymous_ip</span><span class="p">(</span><span class="s1">&#39;203.0.113.0&#39;</span><span class="p">)</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">is_anonymous</span>
 <span class="go">True</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">is_anonymous_vpn</span>
 <span class="go">False</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">is_hosting_provider</span>
 <span class="go">False</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">is_public_proxy</span>
@@ -272,15 +272,15 @@
 <span class="go">IPv4Network(&#39;203.0.113.0/24&#39;)</span>
 </pre></div>
 </div>
 </section>
 <section id="asn-database">
 <h3>ASN Database<a class="headerlink" href="#asn-database" title="Permalink to this headline">¶</a></h3>
 <div class="highlight-pycon notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">geoip2.database</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># This creates a Reader object. You should use the same object</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># across multiple requests as creation of it is expensive.</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="k">with</span> <span class="n">geoip2</span><span class="o">.</span><span class="n">database</span><span class="o">.</span><span class="n">Reader</span><span class="p">(</span><span class="s1">&#39;/path/to/GeoLite2-ASN.mmdb&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">reader</span><span class="p">:</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span> <span class="o">=</span> <span class="n">reader</span><span class="o">.</span><span class="n">asn</span><span class="p">(</span><span class="s1">&#39;203.0.113.0&#39;</span><span class="p">)</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">autonomous_system_number</span>
 <span class="go">1221</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">autonomous_system_organization</span>
@@ -291,15 +291,15 @@
 <span class="go">IPv4Network(&#39;203.0.113.0/24&#39;)</span>
 </pre></div>
 </div>
 </section>
 <section id="connection-type-database">
 <h3>Connection-Type Database<a class="headerlink" href="#connection-type-database" title="Permalink to this headline">¶</a></h3>
 <div class="highlight-pycon notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">geoip2.database</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># This creates a Reader object. You should use the same object</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># across multiple requests as creation of it is expensive.</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="k">with</span> <span class="n">geoip2</span><span class="o">.</span><span class="n">database</span><span class="o">.</span><span class="n">Reader</span><span class="p">(</span><span class="s1">&#39;/path/to/GeoIP2-Connection-Type.mmdb&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">reader</span><span class="p">:</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span> <span class="o">=</span> <span class="n">reader</span><span class="o">.</span><span class="n">connection_type</span><span class="p">(</span><span class="s1">&#39;203.0.113.0&#39;</span><span class="p">)</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">connection_type</span>
 <span class="go">&#39;Corporate&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">ip_address</span>
@@ -308,77 +308,77 @@
 <span class="go">IPv4Network(&#39;203.0.113.0/24&#39;)</span>
 </pre></div>
 </div>
 </section>
 <section id="domain-database">
 <h3>Domain Database<a class="headerlink" href="#domain-database" title="Permalink to this headline">¶</a></h3>
 <div class="highlight-pycon notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">geoip2.database</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># This creates a Reader object. You should use the same object</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># across multiple requests as creation of it is expensive.</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="k">with</span> <span class="n">geoip2</span><span class="o">.</span><span class="n">database</span><span class="o">.</span><span class="n">Reader</span><span class="p">(</span><span class="s1">&#39;/path/to/GeoIP2-Domain.mmdb&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">reader</span><span class="p">:</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span> <span class="o">=</span> <span class="n">reader</span><span class="o">.</span><span class="n">domain</span><span class="p">(</span><span class="s1">&#39;203.0.113.0&#39;</span><span class="p">)</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">domain</span>
 <span class="go">&#39;umn.edu&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">ip_address</span>
 <span class="go">&#39;203.0.113.0&#39;</span>
 </pre></div>
 </div>
 </section>
 <section id="enterprise-database">
 <h3>Enterprise Database<a class="headerlink" href="#enterprise-database" title="Permalink to this headline">¶</a></h3>
 <div class="highlight-pycon notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">geoip2.database</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># This creates a Reader object. You should use the same object</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># across multiple requests as creation of it is expensive.</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="k">with</span> <span class="n">geoip2</span><span class="o">.</span><span class="n">database</span><span class="o">.</span><span class="n">Reader</span><span class="p">(</span><span class="s1">&#39;/path/to/GeoIP2-Enterprise.mmdb&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">reader</span><span class="p">:</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="c1"># Use the .enterprise method to do a lookup in the Enterprise database</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span> <span class="o">=</span> <span class="n">reader</span><span class="o">.</span><span class="n">enterprise</span><span class="p">(</span><span class="s1">&#39;203.0.113.0&#39;</span><span class="p">)</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">confidence</span>
 <span class="go">99</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">iso_code</span>
 <span class="go">&#39;US&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">name</span>
 <span class="go">&#39;United States&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">names</span><span class="p">[</span><span class="s1">&#39;zh-CN&#39;</span><span class="p">]</span>
 <span class="go">u&#39;美国&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">subdivisions</span><span class="o">.</span><span class="n">most_specific</span><span class="o">.</span><span class="n">name</span>
 <span class="go">&#39;Minnesota&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">subdivisions</span><span class="o">.</span><span class="n">most_specific</span><span class="o">.</span><span class="n">iso_code</span>
 <span class="go">&#39;MN&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">subdivisions</span><span class="o">.</span><span class="n">most_specific</span><span class="o">.</span><span class="n">confidence</span>
 <span class="go">77</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">city</span><span class="o">.</span><span class="n">name</span>
 <span class="go">&#39;Minneapolis&#39;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">country</span><span class="o">.</span><span class="n">confidence</span>
 <span class="go">11</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">postal</span><span class="o">.</span><span class="n">code</span>
 <span class="go">&#39;55455&#39;</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">location</span><span class="o">.</span><span class="n">accuracy_radius</span>
 <span class="go">50</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">location</span><span class="o">.</span><span class="n">latitude</span>
 <span class="go">44.9733</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">location</span><span class="o">.</span><span class="n">longitude</span>
 <span class="go">-93.2323</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">traits</span><span class="o">.</span><span class="n">network</span>
 <span class="go">IPv4Network(&#39;203.0.113.0/24&#39;)</span>
 </pre></div>
 </div>
 </section>
 <section id="isp-database">
 <h3>ISP Database<a class="headerlink" href="#isp-database" title="Permalink to this headline">¶</a></h3>
 <div class="highlight-pycon notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">geoip2.database</span>
-<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># This creates a Reader object. You should use the same object</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># across multiple requests as creation of it is expensive.</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="k">with</span> <span class="n">geoip2</span><span class="o">.</span><span class="n">database</span><span class="o">.</span><span class="n">Reader</span><span class="p">(</span><span class="s1">&#39;/path/to/GeoIP2-ISP.mmdb&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">reader</span><span class="p">:</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span> <span class="o">=</span> <span class="n">reader</span><span class="o">.</span><span class="n">isp</span><span class="p">(</span><span class="s1">&#39;203.0.113.0&#39;</span><span class="p">)</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">autonomous_system_number</span>
 <span class="go">1221</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">response</span><span class="o">.</span><span class="n">autonomous_system_organization</span>
@@ -475,15 +475,15 @@
 names”, etc.). Once the correction is part of the GeoNames data set, it
 will be automatically incorporated into future MaxMind releases.</p>
 <p>If you are a paying MaxMind customer and you’re not sure where to submit a
 correction, please <a class="reference external" href="http://www.maxmind.com/en/support">contact MaxMind support</a> for help.</p>
 </section>
 <section id="requirements">
 <h2>Requirements<a class="headerlink" href="#requirements" title="Permalink to this headline">¶</a></h2>
-<p>Python 3.6 or greater is required. Older versions are not supported.</p>
+<p>Python 3.7 or greater is required. Older versions are not supported.</p>
 <p>The Requests HTTP library is also required. See
 &lt;<a class="reference external" href="http://python-requests.org">http://python-requests.org</a>&gt; for details.</p>
 </section>
 <section id="versioning">
 <h2>Versioning<a class="headerlink" href="#versioning" title="Permalink to this headline">¶</a></h2>
 <p>The GeoIP2 Python API uses <a class="reference external" href="http://semver.org/">Semantic Versioning</a>.</p>
 </section>
@@ -496,15 +496,15 @@
 </section>
 <section id="module-geoip2">
 <span id="modules"></span><h1>Modules<a class="headerlink" href="#module-geoip2" title="Permalink to this headline">¶</a></h1>
 <span class="target" id="module-geoip2.database"></span><section id="geoip2-database-reader">
 <h2>GeoIP2 Database Reader<a class="headerlink" href="#geoip2-database-reader" title="Permalink to this headline">¶</a></h2>
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.database.Reader">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.database.</span></span><span class="sig-name descname"><span class="pre">Reader</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fileish</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.AnyStr" title="(in Python v3.10)"><span class="pre">AnyStr</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/os.html#os.PathLike" title="(in Python v3.10)"><span class="pre">os.PathLike</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.IO" title="(in Python v3.10)"><span class="pre">IO</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.database.Reader" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.database.</span></span><span class="sig-name descname"><span class="pre">Reader</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fileish</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.AnyStr" title="(in Python v3.11)"><span class="pre">AnyStr</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/os.html#os.PathLike" title="(in Python v3.11)"><span class="pre">os.PathLike</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.IO" title="(in Python v3.11)"><span class="pre">IO</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.database.Reader" title="Permalink to this definition">¶</a></dt>
 <dd><p>GeoIP2 database Reader object.</p>
 <p>Instances of this class provide a reader for the GeoIP2 database format.
 IP addresses can be looked up using the <code class="docutils literal notranslate"><span class="pre">country</span></code> and <code class="docutils literal notranslate"><span class="pre">city</span></code> methods.</p>
 <p>The basic API for this class is the same for every database. First, you
 create a reader object, specifying a file name or file descriptor.
 You then call the method corresponding to the specific database, passing
 it the IP address you want to look up.</p>
@@ -515,119 +515,119 @@
 record class will have a <code class="docutils literal notranslate"><span class="pre">None</span></code> value.</p>
 <p>If the address is not in the database, an
 <code class="docutils literal notranslate"><span class="pre">geoip2.errors.AddressNotFoundError</span></code> exception will be thrown. If the
 database is corrupt or invalid, a <code class="docutils literal notranslate"><span class="pre">maxminddb.InvalidDatabaseError</span></code> will
 be thrown.</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.database.Reader.anonymous_ip">
-<span class="sig-name descname"><span class="pre">anonymous_ip</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.AnonymousIP" title="geoip2.models.AnonymousIP"><span class="pre">geoip2.models.AnonymousIP</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.anonymous_ip" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">anonymous_ip</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.AnonymousIP" title="geoip2.models.AnonymousIP"><span class="pre">geoip2.models.AnonymousIP</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.anonymous_ip" title="Permalink to this definition">¶</a></dt>
 <dd><p>Get the AnonymousIP object for the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string.</p>
 </dd>
 <dt class="field-even">Returns</dt>
 <dd class="field-even"><p><a class="reference internal" href="#geoip2.models.AnonymousIP" title="geoip2.models.AnonymousIP"><code class="xref py py-class docutils literal notranslate"><span class="pre">geoip2.models.AnonymousIP</span></code></a> object</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.database.Reader.asn">
-<span class="sig-name descname"><span class="pre">asn</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.ASN" title="geoip2.models.ASN"><span class="pre">geoip2.models.ASN</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.asn" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">asn</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.ASN" title="geoip2.models.ASN"><span class="pre">geoip2.models.ASN</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.asn" title="Permalink to this definition">¶</a></dt>
 <dd><p>Get the ASN object for the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string.</p>
 </dd>
 <dt class="field-even">Returns</dt>
 <dd class="field-even"><p><a class="reference internal" href="#geoip2.models.ASN" title="geoip2.models.ASN"><code class="xref py py-class docutils literal notranslate"><span class="pre">geoip2.models.ASN</span></code></a> object</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.database.Reader.city">
-<span class="sig-name descname"><span class="pre">city</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.City" title="geoip2.models.City"><span class="pre">geoip2.models.City</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.city" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">city</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.City" title="geoip2.models.City"><span class="pre">geoip2.models.City</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.city" title="Permalink to this definition">¶</a></dt>
 <dd><p>Get the City object for the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string.</p>
 </dd>
 <dt class="field-even">Returns</dt>
 <dd class="field-even"><p><a class="reference internal" href="#geoip2.models.City" title="geoip2.models.City"><code class="xref py py-class docutils literal notranslate"><span class="pre">geoip2.models.City</span></code></a> object</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.database.Reader.close">
-<span class="sig-name descname"><span class="pre">close</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.close" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">close</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.close" title="Permalink to this definition">¶</a></dt>
 <dd><p>Closes the GeoIP2 database.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.database.Reader.connection_type">
-<span class="sig-name descname"><span class="pre">connection_type</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.ConnectionType" title="geoip2.models.ConnectionType"><span class="pre">geoip2.models.ConnectionType</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.connection_type" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">connection_type</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.ConnectionType" title="geoip2.models.ConnectionType"><span class="pre">geoip2.models.ConnectionType</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.connection_type" title="Permalink to this definition">¶</a></dt>
 <dd><p>Get the ConnectionType object for the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string.</p>
 </dd>
 <dt class="field-even">Returns</dt>
 <dd class="field-even"><p><a class="reference internal" href="#geoip2.models.ConnectionType" title="geoip2.models.ConnectionType"><code class="xref py py-class docutils literal notranslate"><span class="pre">geoip2.models.ConnectionType</span></code></a> object</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.database.Reader.country">
-<span class="sig-name descname"><span class="pre">country</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Country" title="geoip2.models.Country"><span class="pre">geoip2.models.Country</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.country" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">country</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Country" title="geoip2.models.Country"><span class="pre">geoip2.models.Country</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.country" title="Permalink to this definition">¶</a></dt>
 <dd><p>Get the Country object for the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string.</p>
 </dd>
 <dt class="field-even">Returns</dt>
 <dd class="field-even"><p><a class="reference internal" href="#geoip2.models.Country" title="geoip2.models.Country"><code class="xref py py-class docutils literal notranslate"><span class="pre">geoip2.models.Country</span></code></a> object</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.database.Reader.domain">
-<span class="sig-name descname"><span class="pre">domain</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Domain" title="geoip2.models.Domain"><span class="pre">geoip2.models.Domain</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.domain" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">domain</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Domain" title="geoip2.models.Domain"><span class="pre">geoip2.models.Domain</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.domain" title="Permalink to this definition">¶</a></dt>
 <dd><p>Get the Domain object for the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string.</p>
 </dd>
 <dt class="field-even">Returns</dt>
 <dd class="field-even"><p><a class="reference internal" href="#geoip2.models.Domain" title="geoip2.models.Domain"><code class="xref py py-class docutils literal notranslate"><span class="pre">geoip2.models.Domain</span></code></a> object</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.database.Reader.enterprise">
-<span class="sig-name descname"><span class="pre">enterprise</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Enterprise" title="geoip2.models.Enterprise"><span class="pre">geoip2.models.Enterprise</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.enterprise" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">enterprise</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Enterprise" title="geoip2.models.Enterprise"><span class="pre">geoip2.models.Enterprise</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.enterprise" title="Permalink to this definition">¶</a></dt>
 <dd><p>Get the Enterprise object for the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string.</p>
 </dd>
 <dt class="field-even">Returns</dt>
 <dd class="field-even"><p><a class="reference internal" href="#geoip2.models.Enterprise" title="geoip2.models.Enterprise"><code class="xref py py-class docutils literal notranslate"><span class="pre">geoip2.models.Enterprise</span></code></a> object</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.database.Reader.isp">
-<span class="sig-name descname"><span class="pre">isp</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.ISP" title="geoip2.models.ISP"><span class="pre">geoip2.models.ISP</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.isp" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">isp</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.ISP" title="geoip2.models.ISP"><span class="pre">geoip2.models.ISP</span></a></span></span><a class="headerlink" href="#geoip2.database.Reader.isp" title="Permalink to this definition">¶</a></dt>
 <dd><p>Get the ISP object for the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string.</p>
 </dd>
 <dt class="field-even">Returns</dt>
 <dd class="field-even"><p><a class="reference internal" href="#geoip2.models.ISP" title="geoip2.models.ISP"><code class="xref py py-class docutils literal notranslate"><span class="pre">geoip2.models.ISP</span></code></a> object</p>
@@ -663,15 +663,15 @@
 <p>The service may not return any information for an entire record, in which
 case all of the attributes for that record class will be empty.</p>
 <section id="ssl">
 <h3>SSL<a class="headerlink" href="#ssl" title="Permalink to this headline">¶</a></h3>
 <p>Requests to the web service are always made with SSL.</p>
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.webservice.AsyncClient">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.webservice.</span></span><span class="sig-name descname"><span class="pre">AsyncClient</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">account_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">license_key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">host</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'geoip.maxmind.com'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">timeout</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.10)"><span class="pre">float</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">60</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.webservice.AsyncClient" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.webservice.</span></span><span class="sig-name descname"><span class="pre">AsyncClient</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">account_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">license_key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">host</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'geoip.maxmind.com'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">timeout</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">60</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.webservice.AsyncClient" title="Permalink to this definition">¶</a></dt>
 <dd><p>An async GeoIP2 client.</p>
 <p>It accepts the following required arguments:</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>account_id</strong> – Your MaxMind account ID.</p></li>
 <li><p><strong>license_key</strong> – Your MaxMind license key.</p></li>
@@ -717,15 +717,15 @@
 a basic auth username and password, e.g.,
 <code class="docutils literal notranslate"><span class="pre">http://username:password&#64;host:port</span></code>.</p></li>
 </ul>
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.webservice.AsyncClient.city">
-<em class="property"><span class="pre">async</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">city</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'me'</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.City" title="geoip2.models.City"><span class="pre">geoip2.models.City</span></a></span></span><a class="headerlink" href="#geoip2.webservice.AsyncClient.city" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">async</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">city</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'me'</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.City" title="geoip2.models.City"><span class="pre">geoip2.models.City</span></a></span></span><a class="headerlink" href="#geoip2.webservice.AsyncClient.city" title="Permalink to this definition">¶</a></dt>
 <dd><p>Call City Plus endpoint with the specified IP.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string. If no
 address is provided, the address that the web service is
 called from will be used.</p>
 </dd>
@@ -740,15 +740,15 @@
 <em class="property"><span class="pre">async</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">close</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.webservice.AsyncClient.close" title="Permalink to this definition">¶</a></dt>
 <dd><p>Close underlying session</p>
 <p>This will close the session and any associated connections.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.webservice.AsyncClient.country">
-<em class="property"><span class="pre">async</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">country</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'me'</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Country" title="geoip2.models.Country"><span class="pre">geoip2.models.Country</span></a></span></span><a class="headerlink" href="#geoip2.webservice.AsyncClient.country" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">async</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">country</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'me'</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Country" title="geoip2.models.Country"><span class="pre">geoip2.models.Country</span></a></span></span><a class="headerlink" href="#geoip2.webservice.AsyncClient.country" title="Permalink to this definition">¶</a></dt>
 <dd><p>Call the GeoIP2 Country endpoint with the specified IP.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string. If no address
 is provided, the address that the web service is called from will
 be used.</p>
 </dd>
@@ -756,15 +756,15 @@
 <dd class="field-even"><p><a class="reference internal" href="#geoip2.models.Country" title="geoip2.models.Country"><code class="xref py py-class docutils literal notranslate"><span class="pre">geoip2.models.Country</span></code></a> object</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.webservice.AsyncClient.insights">
-<em class="property"><span class="pre">async</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">insights</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'me'</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Insights" title="geoip2.models.Insights"><span class="pre">geoip2.models.Insights</span></a></span></span><a class="headerlink" href="#geoip2.webservice.AsyncClient.insights" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">async</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">insights</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'me'</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Insights" title="geoip2.models.Insights"><span class="pre">geoip2.models.Insights</span></a></span></span><a class="headerlink" href="#geoip2.webservice.AsyncClient.insights" title="Permalink to this definition">¶</a></dt>
 <dd><p>Call the Insights endpoint with the specified IP.</p>
 <p>Insights is only supported by the GeoIP2 web service. The GeoLite2 web
 service does not support it.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string. If no address
 is provided, the address that the web service is called from will
@@ -776,15 +776,15 @@
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.webservice.Client">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.webservice.</span></span><span class="sig-name descname"><span class="pre">Client</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">account_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">license_key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">host</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'geoip.maxmind.com'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">timeout</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.10)"><span class="pre">float</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">60</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.webservice.Client" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.webservice.</span></span><span class="sig-name descname"><span class="pre">Client</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">account_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">license_key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">host</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'geoip.maxmind.com'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">timeout</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">60</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.webservice.Client" title="Permalink to this definition">¶</a></dt>
 <dd><p>A synchronous GeoIP2 client.</p>
 <p>It accepts the following required arguments:</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>account_id</strong> – Your MaxMind account ID.</p></li>
 <li><p><strong>license_key</strong> – Your MaxMind license key.</p></li>
@@ -830,15 +830,15 @@
 a basic auth username and password, e.g.,
 <code class="docutils literal notranslate"><span class="pre">http://username:password&#64;host:port</span></code>.</p></li>
 </ul>
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.webservice.Client.city">
-<span class="sig-name descname"><span class="pre">city</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'me'</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.City" title="geoip2.models.City"><span class="pre">geoip2.models.City</span></a></span></span><a class="headerlink" href="#geoip2.webservice.Client.city" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">city</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'me'</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.City" title="geoip2.models.City"><span class="pre">geoip2.models.City</span></a></span></span><a class="headerlink" href="#geoip2.webservice.Client.city" title="Permalink to this definition">¶</a></dt>
 <dd><p>Call City Plus endpoint with the specified IP.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string. If no
 address is provided, the address that the web service is
 called from will be used.</p>
 </dd>
@@ -853,15 +853,15 @@
 <span class="sig-name descname"><span class="pre">close</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.webservice.Client.close" title="Permalink to this definition">¶</a></dt>
 <dd><p>Close underlying session</p>
 <p>This will close the session and any associated connections.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.webservice.Client.country">
-<span class="sig-name descname"><span class="pre">country</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'me'</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Country" title="geoip2.models.Country"><span class="pre">geoip2.models.Country</span></a></span></span><a class="headerlink" href="#geoip2.webservice.Client.country" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">country</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'me'</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Country" title="geoip2.models.Country"><span class="pre">geoip2.models.Country</span></a></span></span><a class="headerlink" href="#geoip2.webservice.Client.country" title="Permalink to this definition">¶</a></dt>
 <dd><p>Call the GeoIP2 Country endpoint with the specified IP.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string. If no address
 is provided, the address that the web service is called from will
 be used.</p>
 </dd>
@@ -869,15 +869,15 @@
 <dd class="field-even"><p><a class="reference internal" href="#geoip2.models.Country" title="geoip2.models.Country"><code class="xref py py-class docutils literal notranslate"><span class="pre">geoip2.models.Country</span></code></a> object</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="geoip2.webservice.Client.insights">
-<span class="sig-name descname"><span class="pre">insights</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'me'</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Insights" title="geoip2.models.Insights"><span class="pre">geoip2.models.Insights</span></a></span></span><a class="headerlink" href="#geoip2.webservice.Client.insights" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">insights</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">'me'</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#geoip2.models.Insights" title="geoip2.models.Insights"><span class="pre">geoip2.models.Insights</span></a></span></span><a class="headerlink" href="#geoip2.webservice.Client.insights" title="Permalink to this definition">¶</a></dt>
 <dd><p>Call the Insights endpoint with the specified IP.</p>
 <p>Insights is only supported by the GeoIP2 web service. The GeoLite2 web
 service does not support it.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><p><strong>ip_address</strong> – IPv4 or IPv6 address as a string. If no address
 is provided, the address that the web service is called from will
@@ -898,172 +898,172 @@
 <p>These classes provide models for the data returned by the GeoIP2
 web service and databases.</p>
 <p>The only difference between the City and Insights model classes is which
 fields in each record may be populated. See
 <a class="reference external" href="https://dev.maxmind.com/geoip/docs/web-services?lang=en">https://dev.maxmind.com/geoip/docs/web-services?lang=en</a> for more details.</p>
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.models.ASN">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">ASN</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.ASN" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">ASN</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.ASN" title="Permalink to this definition">¶</a></dt>
 <dd><p>Model class for the GeoLite2 ASN.</p>
 <p>This class provides the following attribute:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ASN.autonomous_system_number">
 <span class="sig-name descname"><span class="pre">autonomous_system_number</span></span><a class="headerlink" href="#geoip2.models.ASN.autonomous_system_number" title="Permalink to this definition">¶</a></dt>
 <dd><p>The autonomous system number associated with the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ASN.autonomous_system_organization">
 <span class="sig-name descname"><span class="pre">autonomous_system_organization</span></span><a class="headerlink" href="#geoip2.models.ASN.autonomous_system_organization" title="Permalink to this definition">¶</a></dt>
 <dd><p>The organization associated with the registered autonomous system number
 for the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ASN.ip_address">
 <span class="sig-name descname"><span class="pre">ip_address</span></span><a class="headerlink" href="#geoip2.models.ASN.ip_address" title="Permalink to this definition">¶</a></dt>
 <dd><p>The IP address used in the lookup.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ASN.network">
 <span class="sig-name descname"><span class="pre">network</span></span><a class="headerlink" href="#geoip2.models.ASN.network" title="Permalink to this definition">¶</a></dt>
 <dd><p>The network associated with the record. In particular, this is the
 largest network where all of the fields besides ip_address have the same
 value.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.10)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.10)">ipaddress.IPv6Network</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.11)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.11)">ipaddress.IPv6Network</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.models.AnonymousIP">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">AnonymousIP</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.AnonymousIP" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">AnonymousIP</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.AnonymousIP" title="Permalink to this definition">¶</a></dt>
 <dd><p>Model class for the GeoIP2 Anonymous IP.</p>
 <p>This class provides the following attribute:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.AnonymousIP.is_anonymous">
 <span class="sig-name descname"><span class="pre">is_anonymous</span></span><a class="headerlink" href="#geoip2.models.AnonymousIP.is_anonymous" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP address belongs to any sort of anonymous network.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.AnonymousIP.is_anonymous_vpn">
 <span class="sig-name descname"><span class="pre">is_anonymous_vpn</span></span><a class="headerlink" href="#geoip2.models.AnonymousIP.is_anonymous_vpn" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP address is registered to an anonymous VPN
 provider.</p>
 <p>If a VPN provider does not register subnets under names associated with
 them, we will likely only flag their IP ranges using the
 <code class="docutils literal notranslate"><span class="pre">is_hosting_provider</span></code> attribute.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.AnonymousIP.is_hosting_provider">
 <span class="sig-name descname"><span class="pre">is_hosting_provider</span></span><a class="headerlink" href="#geoip2.models.AnonymousIP.is_hosting_provider" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP address belongs to a hosting or VPN provider
 (see description of <code class="docutils literal notranslate"><span class="pre">is_anonymous_vpn</span></code> attribute).</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.AnonymousIP.is_public_proxy">
 <span class="sig-name descname"><span class="pre">is_public_proxy</span></span><a class="headerlink" href="#geoip2.models.AnonymousIP.is_public_proxy" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP address belongs to a public proxy.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.AnonymousIP.is_residential_proxy">
 <span class="sig-name descname"><span class="pre">is_residential_proxy</span></span><a class="headerlink" href="#geoip2.models.AnonymousIP.is_residential_proxy" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP address is on a suspected anonymizing network
 and belongs to a residential ISP.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.AnonymousIP.is_tor_exit_node">
 <span class="sig-name descname"><span class="pre">is_tor_exit_node</span></span><a class="headerlink" href="#geoip2.models.AnonymousIP.is_tor_exit_node" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP address is a Tor exit node.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.AnonymousIP.ip_address">
 <span class="sig-name descname"><span class="pre">ip_address</span></span><a class="headerlink" href="#geoip2.models.AnonymousIP.ip_address" title="Permalink to this definition">¶</a></dt>
 <dd><p>The IP address used in the lookup.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.AnonymousIP.network">
 <span class="sig-name descname"><span class="pre">network</span></span><a class="headerlink" href="#geoip2.models.AnonymousIP.network" title="Permalink to this definition">¶</a></dt>
 <dd><p>The network associated with the record. In particular, this is the
 largest network where all of the fields besides ip_address have the same
 value.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.10)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.10)">ipaddress.IPv6Network</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.11)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.11)">ipaddress.IPv6Network</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.models.City">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">City</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw_response</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Any" title="(in Python v3.10)"><span class="pre">Any</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.City" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">City</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw_response</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Any" title="(in Python v3.11)"><span class="pre">Any</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.City" title="Permalink to this definition">¶</a></dt>
 <dd><p>Model for the City Plus web service and the City database.</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.City.city">
 <span class="sig-name descname"><span class="pre">city</span></span><a class="headerlink" href="#geoip2.models.City.city" title="Permalink to this definition">¶</a></dt>
 <dd><p>City object for the requested IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
@@ -1177,15 +1177,15 @@
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.models.ConnectionType">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">ConnectionType</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.ConnectionType" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">ConnectionType</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.ConnectionType" title="Permalink to this definition">¶</a></dt>
 <dd><p>Model class for the GeoIP2 Connection-Type.</p>
 <p>This class provides the following attribute:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ConnectionType.connection_type">
 <span class="sig-name descname"><span class="pre">connection_type</span></span><a class="headerlink" href="#geoip2.models.ConnectionType.connection_type" title="Permalink to this definition">¶</a></dt>
 <dd><p>The connection type may take the following values:</p>
 <ul class="simple">
@@ -1193,48 +1193,48 @@
 <li><p>Cable/DSL</p></li>
 <li><p>Corporate</p></li>
 <li><p>Cellular</p></li>
 </ul>
 <p>Additional values may be added in the future.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ConnectionType.ip_address">
 <span class="sig-name descname"><span class="pre">ip_address</span></span><a class="headerlink" href="#geoip2.models.ConnectionType.ip_address" title="Permalink to this definition">¶</a></dt>
 <dd><p>The IP address used in the lookup.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ConnectionType.network">
 <span class="sig-name descname"><span class="pre">network</span></span><a class="headerlink" href="#geoip2.models.ConnectionType.network" title="Permalink to this definition">¶</a></dt>
 <dd><p>The network associated with the record. In particular, this is the
 largest network where all of the fields besides ip_address have the same
 value.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.10)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.10)">ipaddress.IPv6Network</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.11)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.11)">ipaddress.IPv6Network</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.models.Country">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">Country</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw_response</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Any" title="(in Python v3.10)"><span class="pre">Any</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.Country" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">Country</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw_response</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Any" title="(in Python v3.11)"><span class="pre">Any</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.Country" title="Permalink to this definition">¶</a></dt>
 <dd><p>Model for the Country web service and Country database.</p>
 <p>This class provides the following attributes:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.Country.continent">
 <span class="sig-name descname"><span class="pre">continent</span></span><a class="headerlink" href="#geoip2.models.Country.continent" title="Permalink to this definition">¶</a></dt>
 <dd><p>Continent object for the requested IP address.</p>
 <dl class="field-list simple">
@@ -1304,57 +1304,57 @@
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.models.Domain">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">Domain</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.Domain" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">Domain</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.Domain" title="Permalink to this definition">¶</a></dt>
 <dd><p>Model class for the GeoIP2 Domain.</p>
 <p>This class provides the following attribute:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.Domain.domain">
 <span class="sig-name descname"><span class="pre">domain</span></span><a class="headerlink" href="#geoip2.models.Domain.domain" title="Permalink to this definition">¶</a></dt>
 <dd><p>The domain associated with the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.Domain.ip_address">
 <span class="sig-name descname"><span class="pre">ip_address</span></span><a class="headerlink" href="#geoip2.models.Domain.ip_address" title="Permalink to this definition">¶</a></dt>
 <dd><p>The IP address used in the lookup.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.Domain.network">
 <span class="sig-name descname"><span class="pre">network</span></span><a class="headerlink" href="#geoip2.models.Domain.network" title="Permalink to this definition">¶</a></dt>
 <dd><p>The network associated with the record. In particular, this is the
 largest network where all of the fields besides ip_address have the same
 value.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.10)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.10)">ipaddress.IPv6Network</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.11)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.11)">ipaddress.IPv6Network</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.models.Enterprise">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">Enterprise</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw_response</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Any" title="(in Python v3.10)"><span class="pre">Any</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.Enterprise" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">Enterprise</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw_response</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Any" title="(in Python v3.11)"><span class="pre">Any</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.Enterprise" title="Permalink to this definition">¶</a></dt>
 <dd><p>Model for the GeoIP2 Enterprise database.</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.Enterprise.city">
 <span class="sig-name descname"><span class="pre">city</span></span><a class="headerlink" href="#geoip2.models.Enterprise.city" title="Permalink to this definition">¶</a></dt>
 <dd><p>City object for the requested IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
@@ -1452,91 +1452,91 @@
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.models.ISP">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">ISP</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.ISP" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">ISP</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.ISP" title="Permalink to this definition">¶</a></dt>
 <dd><p>Model class for the GeoIP2 ISP.</p>
 <p>This class provides the following attribute:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ISP.autonomous_system_number">
 <span class="sig-name descname"><span class="pre">autonomous_system_number</span></span><a class="headerlink" href="#geoip2.models.ISP.autonomous_system_number" title="Permalink to this definition">¶</a></dt>
 <dd><p>The autonomous system number associated with the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ISP.autonomous_system_organization">
 <span class="sig-name descname"><span class="pre">autonomous_system_organization</span></span><a class="headerlink" href="#geoip2.models.ISP.autonomous_system_organization" title="Permalink to this definition">¶</a></dt>
 <dd><p>The organization associated with the registered autonomous system number
 for the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ISP.isp">
 <span class="sig-name descname"><span class="pre">isp</span></span><a class="headerlink" href="#geoip2.models.ISP.isp" title="Permalink to this definition">¶</a></dt>
 <dd><p>The name of the ISP associated with the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ISP.organization">
 <span class="sig-name descname"><span class="pre">organization</span></span><a class="headerlink" href="#geoip2.models.ISP.organization" title="Permalink to this definition">¶</a></dt>
 <dd><p>The name of the organization associated with the IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ISP.ip_address">
 <span class="sig-name descname"><span class="pre">ip_address</span></span><a class="headerlink" href="#geoip2.models.ISP.ip_address" title="Permalink to this definition">¶</a></dt>
 <dd><p>The IP address used in the lookup.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.ISP.network">
 <span class="sig-name descname"><span class="pre">network</span></span><a class="headerlink" href="#geoip2.models.ISP.network" title="Permalink to this definition">¶</a></dt>
 <dd><p>The network associated with the record. In particular, this is the
 largest network where all of the fields besides ip_address have the same
 value.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.10)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.10)">ipaddress.IPv6Network</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.11)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.11)">ipaddress.IPv6Network</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.models.Insights">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">Insights</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw_response</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Any" title="(in Python v3.10)"><span class="pre">Any</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.Insights" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">Insights</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw_response</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Any" title="(in Python v3.11)"><span class="pre">Any</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.Insights" title="Permalink to this definition">¶</a></dt>
 <dd><p>Model for the GeoIP2 Insights web service.</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.models.Insights.city">
 <span class="sig-name descname"><span class="pre">city</span></span><a class="headerlink" href="#geoip2.models.Insights.city" title="Permalink to this definition">¶</a></dt>
 <dd><p>City object for the requested IP address.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
@@ -1634,555 +1634,555 @@
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.models.SimpleModel">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">SimpleModel</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.10)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.SimpleModel" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.models.</span></span><span class="sig-name descname"><span class="pre">SimpleModel</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.models.SimpleModel" title="Permalink to this definition">¶</a></dt>
 <dd><p>Provides basic methods for non-location models</p>
 <dl class="py property">
 <dt class="sig sig-object py" id="geoip2.models.SimpleModel.network">
-<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">network</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Network</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Network</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#geoip2.models.SimpleModel.network" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">network</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Network</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Network</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#geoip2.models.SimpleModel.network" title="Permalink to this definition">¶</a></dt>
 <dd><p>The network for the record</p>
 </dd></dl>
 
 </dd></dl>
 
 </section>
 <span class="target" id="module-geoip2.records"></span><section id="records">
 <h2>Records<a class="headerlink" href="#records" title="Permalink to this headline">¶</a></h2>
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.records.City">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">City</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">confidence</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">geoname_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.City" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">City</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">confidence</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">geoname_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.City" title="Permalink to this definition">¶</a></dt>
 <dd><p>Contains data for the city record associated with an IP address.</p>
 <p>This class contains the city-level data associated with an IP address.</p>
 <p>This record is returned by <code class="docutils literal notranslate"><span class="pre">city</span></code>, <code class="docutils literal notranslate"><span class="pre">enterprise</span></code>, and <code class="docutils literal notranslate"><span class="pre">insights</span></code>.</p>
 <p>Attributes:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.City.confidence">
 <span class="sig-name descname"><span class="pre">confidence</span></span><a class="headerlink" href="#geoip2.records.City.confidence" title="Permalink to this definition">¶</a></dt>
 <dd><p>A value from 0-100 indicating MaxMind’s
 confidence that the city is correct. This attribute is only available
 from the Insights end point and the Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.City.geoname_id">
 <span class="sig-name descname"><span class="pre">geoname_id</span></span><a class="headerlink" href="#geoip2.records.City.geoname_id" title="Permalink to this definition">¶</a></dt>
 <dd><p>The GeoName ID for the city.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.City.name">
 <span class="sig-name descname"><span class="pre">name</span></span><a class="headerlink" href="#geoip2.records.City.name" title="Permalink to this definition">¶</a></dt>
 <dd><p>The name of the city based on the locales list passed to the
 constructor.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.City.names">
 <span class="sig-name descname"><span class="pre">names</span></span><a class="headerlink" href="#geoip2.records.City.names" title="Permalink to this definition">¶</a></dt>
 <dd><p>A dictionary where the keys are locale codes
 and the values are names.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.10)">dict</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.11)">dict</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.records.Continent">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Continent</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">geoname_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Continent" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Continent</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">geoname_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Continent" title="Permalink to this definition">¶</a></dt>
 <dd><p>Contains data for the continent record associated with an IP address.</p>
 <p>This class contains the continent-level data associated with an IP
 address.</p>
 <p>Attributes:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Continent.code">
 <span class="sig-name descname"><span class="pre">code</span></span><a class="headerlink" href="#geoip2.records.Continent.code" title="Permalink to this definition">¶</a></dt>
 <dd><p>A two character continent code like “NA” (North America)
 or “OC” (Oceania).</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Continent.geoname_id">
 <span class="sig-name descname"><span class="pre">geoname_id</span></span><a class="headerlink" href="#geoip2.records.Continent.geoname_id" title="Permalink to this definition">¶</a></dt>
 <dd><p>The GeoName ID for the continent.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Continent.name">
 <span class="sig-name descname"><span class="pre">name</span></span><a class="headerlink" href="#geoip2.records.Continent.name" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns the name of the continent based on the locales list passed to
 the constructor.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Continent.names">
 <span class="sig-name descname"><span class="pre">names</span></span><a class="headerlink" href="#geoip2.records.Continent.names" title="Permalink to this definition">¶</a></dt>
 <dd><p>A dictionary where the keys are locale codes
 and the values are names.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.10)">dict</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.11)">dict</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.records.Country">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Country</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">confidence</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">geoname_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_in_european_union</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">iso_code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Country" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Country</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">confidence</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">geoname_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_in_european_union</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">iso_code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Country" title="Permalink to this definition">¶</a></dt>
 <dd><p>Contains data for the country record associated with an IP address.</p>
 <p>This class contains the country-level data associated with an IP address.</p>
 <p>Attributes:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Country.confidence">
 <span class="sig-name descname"><span class="pre">confidence</span></span><a class="headerlink" href="#geoip2.records.Country.confidence" title="Permalink to this definition">¶</a></dt>
 <dd><p>A value from 0-100 indicating MaxMind’s confidence that
 the country is correct. This attribute is only available from the
 Insights end point and the Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Country.geoname_id">
 <span class="sig-name descname"><span class="pre">geoname_id</span></span><a class="headerlink" href="#geoip2.records.Country.geoname_id" title="Permalink to this definition">¶</a></dt>
 <dd><p>The GeoName ID for the country.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Country.is_in_european_union">
 <span class="sig-name descname"><span class="pre">is_in_european_union</span></span><a class="headerlink" href="#geoip2.records.Country.is_in_european_union" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the country is a member state of the European Union.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Country.iso_code">
 <span class="sig-name descname"><span class="pre">iso_code</span></span><a class="headerlink" href="#geoip2.records.Country.iso_code" title="Permalink to this definition">¶</a></dt>
 <dd><p>The two-character <a class="reference external" href="http://en.wikipedia.org/wiki/ISO_3166-1">ISO 3166-1</a> alpha code for the
 country.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Country.name">
 <span class="sig-name descname"><span class="pre">name</span></span><a class="headerlink" href="#geoip2.records.Country.name" title="Permalink to this definition">¶</a></dt>
 <dd><p>The name of the country based on the locales list passed to the
 constructor.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Country.names">
 <span class="sig-name descname"><span class="pre">names</span></span><a class="headerlink" href="#geoip2.records.Country.names" title="Permalink to this definition">¶</a></dt>
 <dd><p>A dictionary where the keys are locale codes and the values
 are names.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.10)">dict</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.11)">dict</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.records.Location">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Location</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">average_income</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">accuracy_radius</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">latitude</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.10)"><span class="pre">float</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">longitude</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.10)"><span class="pre">float</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metro_code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">population_density</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time_zone</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Location" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Location</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">average_income</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">accuracy_radius</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">latitude</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">longitude</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metro_code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">population_density</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time_zone</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Location" title="Permalink to this definition">¶</a></dt>
 <dd><p>Contains data for the location record associated with an IP address.</p>
 <p>This class contains the location data associated with an IP address.</p>
 <p>This record is returned by <code class="docutils literal notranslate"><span class="pre">city</span></code>, <code class="docutils literal notranslate"><span class="pre">enterprise</span></code>, and <code class="docutils literal notranslate"><span class="pre">insights</span></code>.</p>
 <p>Attributes:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Location.average_income">
 <span class="sig-name descname"><span class="pre">average_income</span></span><a class="headerlink" href="#geoip2.records.Location.average_income" title="Permalink to this definition">¶</a></dt>
 <dd><p>The average income in US dollars associated with the requested IP
 address. This attribute is only available from the Insights end point.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Location.accuracy_radius">
 <span class="sig-name descname"><span class="pre">accuracy_radius</span></span><a class="headerlink" href="#geoip2.records.Location.accuracy_radius" title="Permalink to this definition">¶</a></dt>
 <dd><p>The approximate accuracy radius in kilometers around the latitude and
 longitude for the IP address. This is the radius where we have a 67%
 confidence that the device using the IP address resides within the
 circle centered at the latitude and longitude with the provided radius.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Location.latitude">
 <span class="sig-name descname"><span class="pre">latitude</span></span><a class="headerlink" href="#geoip2.records.Location.latitude" title="Permalink to this definition">¶</a></dt>
 <dd><p>The approximate latitude of the location associated with the IP
 address. This value is not precise and should not be used to identify a
 particular address or household.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.10)">float</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)">float</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Location.longitude">
 <span class="sig-name descname"><span class="pre">longitude</span></span><a class="headerlink" href="#geoip2.records.Location.longitude" title="Permalink to this definition">¶</a></dt>
 <dd><p>The approximate longitude of the location associated with the IP
 address. This value is not precise and should not be used to identify a
 particular address or household.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.10)">float</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)">float</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Location.metro_code">
 <span class="sig-name descname"><span class="pre">metro_code</span></span><a class="headerlink" href="#geoip2.records.Location.metro_code" title="Permalink to this definition">¶</a></dt>
 <dd><p>The metro code of the location if the
 location is in the US. MaxMind returns the same metro codes as the
 <a class="reference external" href="https://developers.google.com/adwords/api/docs/appendix/cities-DMAregions">Google AdWords API</a>.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Location.population_density">
 <span class="sig-name descname"><span class="pre">population_density</span></span><a class="headerlink" href="#geoip2.records.Location.population_density" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <p>The estimated population per square kilometer associated with the IP
 address. This attribute is only available from the Insights end point.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Location.time_zone">
 <span class="sig-name descname"><span class="pre">time_zone</span></span><a class="headerlink" href="#geoip2.records.Location.time_zone" title="Permalink to this definition">¶</a></dt>
 <dd><p>The time zone associated with location, as specified by the <a class="reference external" href="http://www.iana.org/time-zones">IANA Time
 Zone Database</a>, e.g.,
 “America/New_York”.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.records.MaxMind">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">MaxMind</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">queries_remaining</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.MaxMind" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">MaxMind</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">queries_remaining</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.MaxMind" title="Permalink to this definition">¶</a></dt>
 <dd><p>Contains data related to your MaxMind account.</p>
 <p>Attributes:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.MaxMind.queries_remaining">
 <span class="sig-name descname"><span class="pre">queries_remaining</span></span><a class="headerlink" href="#geoip2.records.MaxMind.queries_remaining" title="Permalink to this definition">¶</a></dt>
 <dd><p>The number of remaining queries you have
 for the end point you are calling.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.records.PlaceRecord">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">PlaceRecord</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.PlaceRecord" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">PlaceRecord</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.PlaceRecord" title="Permalink to this definition">¶</a></dt>
 <dd><p>All records with <code class="xref py py-attr docutils literal notranslate"><span class="pre">names</span></code> subclass <a class="reference internal" href="#geoip2.records.PlaceRecord" title="geoip2.records.PlaceRecord"><code class="xref py py-class docutils literal notranslate"><span class="pre">PlaceRecord</span></code></a>.</p>
 <dl class="py property">
 <dt class="sig sig-object py" id="geoip2.records.PlaceRecord.name">
-<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">name</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#geoip2.records.PlaceRecord.name" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">name</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#geoip2.records.PlaceRecord.name" title="Permalink to this definition">¶</a></dt>
 <dd><p>Dict with locale codes as keys and localized name as value.</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.records.Postal">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Postal</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">confidence</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Postal" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Postal</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">confidence</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Postal" title="Permalink to this definition">¶</a></dt>
 <dd><p>Contains data for the postal record associated with an IP address.</p>
 <p>This class contains the postal data associated with an IP address.</p>
 <p>This attribute is returned by <code class="docutils literal notranslate"><span class="pre">city</span></code>, <code class="docutils literal notranslate"><span class="pre">enterprise</span></code>, and <code class="docutils literal notranslate"><span class="pre">insights</span></code>.</p>
 <p>Attributes:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Postal.code">
 <span class="sig-name descname"><span class="pre">code</span></span><a class="headerlink" href="#geoip2.records.Postal.code" title="Permalink to this definition">¶</a></dt>
 <dd><p>The postal code of the location. Postal
 codes are not available for all countries. In some countries, this will
 only contain part of the postal code.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Postal.confidence">
 <span class="sig-name descname"><span class="pre">confidence</span></span><a class="headerlink" href="#geoip2.records.Postal.confidence" title="Permalink to this definition">¶</a></dt>
 <dd><p>A value from 0-100 indicating
 MaxMind’s confidence that the postal code is correct. This attribute is
 only available from the Insights end point and the Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.records.Record">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Record</span></span><a class="headerlink" href="#geoip2.records.Record" title="Permalink to this definition">¶</a></dt>
 <dd><p>All records are subclasses of the abstract class <code class="docutils literal notranslate"><span class="pre">Record</span></code>.</p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.records.RepresentedCountry">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">RepresentedCountry</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">confidence</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">geoname_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_in_european_union</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">iso_code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">type</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.RepresentedCountry" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">RepresentedCountry</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">confidence</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">geoname_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_in_european_union</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">iso_code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">type</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.RepresentedCountry" title="Permalink to this definition">¶</a></dt>
 <dd><p>Contains data for the represented country associated with an IP address.</p>
 <p>This class contains the country-level data associated with an IP address
 for the IP’s represented country. The represented country is the country
 represented by something like a military base.</p>
 <p>Attributes:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.RepresentedCountry.confidence">
 <span class="sig-name descname"><span class="pre">confidence</span></span><a class="headerlink" href="#geoip2.records.RepresentedCountry.confidence" title="Permalink to this definition">¶</a></dt>
 <dd><p>A value from 0-100 indicating MaxMind’s confidence that
 the country is correct. This attribute is only available from the
 Insights end point and the Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.RepresentedCountry.geoname_id">
 <span class="sig-name descname"><span class="pre">geoname_id</span></span><a class="headerlink" href="#geoip2.records.RepresentedCountry.geoname_id" title="Permalink to this definition">¶</a></dt>
 <dd><p>The GeoName ID for the country.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.RepresentedCountry.is_in_european_union">
 <span class="sig-name descname"><span class="pre">is_in_european_union</span></span><a class="headerlink" href="#geoip2.records.RepresentedCountry.is_in_european_union" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the country is a member state of the European Union.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.RepresentedCountry.iso_code">
 <span class="sig-name descname"><span class="pre">iso_code</span></span><a class="headerlink" href="#geoip2.records.RepresentedCountry.iso_code" title="Permalink to this definition">¶</a></dt>
 <dd><p>The two-character <a class="reference external" href="http://en.wikipedia.org/wiki/ISO_3166-1">ISO 3166-1</a> alpha code for the country.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.RepresentedCountry.name">
 <span class="sig-name descname"><span class="pre">name</span></span><a class="headerlink" href="#geoip2.records.RepresentedCountry.name" title="Permalink to this definition">¶</a></dt>
 <dd><p>The name of the country based on the locales list passed to the
 constructor.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.RepresentedCountry.names">
 <span class="sig-name descname"><span class="pre">names</span></span><a class="headerlink" href="#geoip2.records.RepresentedCountry.names" title="Permalink to this definition">¶</a></dt>
 <dd><p>A dictionary where the keys are locale codes and the values
 are names.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.10)">dict</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.11)">dict</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.RepresentedCountry.type">
 <span class="sig-name descname"><span class="pre">type</span></span><a class="headerlink" href="#geoip2.records.RepresentedCountry.type" title="Permalink to this definition">¶</a></dt>
 <dd><p>A string indicating the type of entity that is representing the
 country. Currently we only return <code class="docutils literal notranslate"><span class="pre">military</span></code> but this could expand to
 include other types in the future.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.records.Subdivision">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Subdivision</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">confidence</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">geoname_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">iso_code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.10)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Subdivision" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Subdivision</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">confidence</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">geoname_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">iso_code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Subdivision" title="Permalink to this definition">¶</a></dt>
 <dd><p>Contains data for the subdivisions associated with an IP address.</p>
 <p>This class contains the subdivision data associated with an IP address.</p>
 <p>This attribute is returned by <code class="docutils literal notranslate"><span class="pre">city</span></code>, <code class="docutils literal notranslate"><span class="pre">enterprise</span></code>, and <code class="docutils literal notranslate"><span class="pre">insights</span></code>.</p>
 <p>Attributes:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Subdivision.confidence">
 <span class="sig-name descname"><span class="pre">confidence</span></span><a class="headerlink" href="#geoip2.records.Subdivision.confidence" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is a value from 0-100 indicating MaxMind’s
 confidence that the subdivision is correct. This attribute is only
 available from the Insights end point and the Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Subdivision.geoname_id">
 <span class="sig-name descname"><span class="pre">geoname_id</span></span><a class="headerlink" href="#geoip2.records.Subdivision.geoname_id" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is a GeoName ID for the subdivision.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Subdivision.iso_code">
 <span class="sig-name descname"><span class="pre">iso_code</span></span><a class="headerlink" href="#geoip2.records.Subdivision.iso_code" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is a string up to three characters long
 contain the subdivision portion of the <a class="reference external" href="http://en.wikipedia.org/wiki/ISO_3166-2">ISO 3166-2 code</a>.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Subdivision.name">
 <span class="sig-name descname"><span class="pre">name</span></span><a class="headerlink" href="#geoip2.records.Subdivision.name" title="Permalink to this definition">¶</a></dt>
 <dd><p>The name of the subdivision based on the locales list passed to the
 constructor.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Subdivision.names">
 <span class="sig-name descname"><span class="pre">names</span></span><a class="headerlink" href="#geoip2.records.Subdivision.names" title="Permalink to this definition">¶</a></dt>
 <dd><p>A dictionary where the keys are locale codes and the
 values are names</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.10)">dict</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.11)">dict</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.records.Subdivisions">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Subdivisions</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.10)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">subdivisions</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Subdivisions" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Subdivisions</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">locales</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.List" title="(in Python v3.11)"><span class="pre">List</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">subdivisions</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Subdivisions" title="Permalink to this definition">¶</a></dt>
 <dd><p>A tuple-like collection of subdivisions associated with an IP address.</p>
 <p>This class contains the subdivisions of the country associated with the
 IP address from largest to smallest.</p>
 <p>For instance, the response for Oxford in the United Kingdom would have
 England as the first element and Oxfordshire as the second element.</p>
 <p>This attribute is returned by <code class="docutils literal notranslate"><span class="pre">city</span></code>, <code class="docutils literal notranslate"><span class="pre">enterprise</span></code>, and <code class="docutils literal notranslate"><span class="pre">insights</span></code>.</p>
 <dl class="py property">
@@ -2198,42 +2198,42 @@
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="geoip2.records.Traits">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Traits</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">autonomous_system_number</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">autonomous_system_organization</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">connection_type</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">domain</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_anonymous</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_anonymous_proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_anonymous_vpn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_hosting_provider</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_legitimate_proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_public_proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_residential_proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_satellite_provider</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_tor_exit_node</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">isp</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">network</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">organization</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">prefix_len</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">static_ip_score</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.10)"><span class="pre">float</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">user_count</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">user_type</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mobile_country_code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mobile_network_code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Traits" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.records.</span></span><span class="sig-name descname"><span class="pre">Traits</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">autonomous_system_number</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">autonomous_system_organization</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">connection_type</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">domain</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_anonymous</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_anonymous_proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_anonymous_vpn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_hosting_provider</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_legitimate_proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_public_proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_residential_proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_satellite_provider</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_tor_exit_node</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">isp</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">network</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">organization</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">prefix_len</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">static_ip_score</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">user_count</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">user_type</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mobile_country_code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mobile_network_code</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">_</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.records.Traits" title="Permalink to this definition">¶</a></dt>
 <dd><p>Contains data for the traits record associated with an IP address.</p>
 <p>This class contains the traits data associated with an IP address.</p>
 <p>This class has the following attributes:</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.autonomous_system_number">
 <span class="sig-name descname"><span class="pre">autonomous_system_number</span></span><a class="headerlink" href="#geoip2.records.Traits.autonomous_system_number" title="Permalink to this definition">¶</a></dt>
 <dd><p>The <a class="reference external" href="http://en.wikipedia.org/wiki/Autonomous_system_(Internet)">autonomous system
 number</a>
 associated with the IP address. This attribute is only available from
 the City Plus and Insights web services and the Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.autonomous_system_organization">
 <span class="sig-name descname"><span class="pre">autonomous_system_organization</span></span><a class="headerlink" href="#geoip2.records.Traits.autonomous_system_organization" title="Permalink to this definition">¶</a></dt>
 <dd><p>The organization associated with the registered <a class="reference external" href="http://en.wikipedia.org/wiki/Autonomous_system_(Internet)">autonomous system
 number</a> for
 the IP address. This attribute is only available from the City Plus and
 Insights web service end points and the Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.connection_type">
 <span class="sig-name descname"><span class="pre">connection_type</span></span><a class="headerlink" href="#geoip2.records.Traits.connection_type" title="Permalink to this definition">¶</a></dt>
@@ -2244,68 +2244,68 @@
 <li><p>Corporate</p></li>
 <li><p>Cellular</p></li>
 </ul>
 <p>Additional values may be added in the future.</p>
 <p>This attribute is only available in the Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.domain">
 <span class="sig-name descname"><span class="pre">domain</span></span><a class="headerlink" href="#geoip2.records.Traits.domain" title="Permalink to this definition">¶</a></dt>
 <dd><p>The second level domain associated with the
 IP address. This will be something like “example.com” or
 “example.co.uk”, not “foo.example.com”. This attribute is only available
 from the City Plus and Insights web service end points and the
 Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.ip_address">
 <span class="sig-name descname"><span class="pre">ip_address</span></span><a class="headerlink" href="#geoip2.records.Traits.ip_address" title="Permalink to this definition">¶</a></dt>
 <dd><p>The IP address that the data in the model
 is for. If you performed a “me” lookup against the web service, this
 will be the externally routable IP address for the system the code is
 running on. If the system is behind a NAT, this may differ from the IP
 address locally assigned to it.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.is_anonymous">
 <span class="sig-name descname"><span class="pre">is_anonymous</span></span><a class="headerlink" href="#geoip2.records.Traits.is_anonymous" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP address belongs to any sort of anonymous network.
 This attribute is only available from Insights.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.is_anonymous_proxy">
 <span class="sig-name descname"><span class="pre">is_anonymous_proxy</span></span><a class="headerlink" href="#geoip2.records.Traits.is_anonymous_proxy" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP is an anonymous proxy.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 <div class="deprecated">
 <p><span class="versionmodified deprecated">Deprecated since version 2.2.0: </span>Use our our <a class="reference external" href="https://www.maxmind.com/en/geoip2-anonymous-ip-databaseGeoIP2">GeoIP2 Anonymous IP database</a>
 instead.</p>
 </div>
 </dd></dl>
@@ -2317,78 +2317,78 @@
 provider.</p>
 <p>If a VPN provider does not register subnets under names associated with
 them, we will likely only flag their IP ranges using the
 <code class="docutils literal notranslate"><span class="pre">is_hosting_provider</span></code> attribute.</p>
 <p>This attribute is only available from Insights.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.is_hosting_provider">
 <span class="sig-name descname"><span class="pre">is_hosting_provider</span></span><a class="headerlink" href="#geoip2.records.Traits.is_hosting_provider" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP address belongs to a hosting or VPN provider
 (see description of <code class="docutils literal notranslate"><span class="pre">is_anonymous_vpn</span></code> attribute).
 This attribute is only available from Insights.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.is_legitimate_proxy">
 <span class="sig-name descname"><span class="pre">is_legitimate_proxy</span></span><a class="headerlink" href="#geoip2.records.Traits.is_legitimate_proxy" title="Permalink to this definition">¶</a></dt>
 <dd><p>This attribute is true if MaxMind believes this IP address to be a
 legitimate proxy, such as an internal VPN used by a corporation. This
 attribute is only available in the Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.is_public_proxy">
 <span class="sig-name descname"><span class="pre">is_public_proxy</span></span><a class="headerlink" href="#geoip2.records.Traits.is_public_proxy" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP address belongs to a public proxy. This attribute
 is only available from Insights.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.is_residential_proxy">
 <span class="sig-name descname"><span class="pre">is_residential_proxy</span></span><a class="headerlink" href="#geoip2.records.Traits.is_residential_proxy" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP address is on a suspected anonymizing network
 and belongs to a residential ISP. This attribute is only available from
 Insights.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.is_satellite_provider">
 <span class="sig-name descname"><span class="pre">is_satellite_provider</span></span><a class="headerlink" href="#geoip2.records.Traits.is_satellite_provider" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP address is from a satellite provider that
 provides service to multiple countries.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 <div class="deprecated">
 <p><span class="versionmodified deprecated">Deprecated since version 2.2.0: </span>Due to the increased coverage by mobile carriers, very few
 satellite providers now serve multiple countries. As a result, the
 output does not provide sufficiently relevant data for us to maintain
 it.</p>
@@ -2398,54 +2398,54 @@
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.is_tor_exit_node">
 <span class="sig-name descname"><span class="pre">is_tor_exit_node</span></span><a class="headerlink" href="#geoip2.records.Traits.is_tor_exit_node" title="Permalink to this definition">¶</a></dt>
 <dd><p>This is true if the IP address is a Tor exit node. This attribute is
 only available from Insights.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)">bool</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.isp">
 <span class="sig-name descname"><span class="pre">isp</span></span><a class="headerlink" href="#geoip2.records.Traits.isp" title="Permalink to this definition">¶</a></dt>
 <dd><p>The name of the ISP associated with the IP address. This attribute is
 only available from the City Plus and Insights web services and the
 Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.network">
 <span class="sig-name descname"><span class="pre">network</span></span><a class="headerlink" href="#geoip2.records.Traits.network" title="Permalink to this definition">¶</a></dt>
 <dd><p>The network associated with the record. In particular, this is the
 largest network where all of the fields besides ip_address have the same
 value.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.10)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.10)">ipaddress.IPv6Network</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.11)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.11)">ipaddress.IPv6Network</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.organization">
 <span class="sig-name descname"><span class="pre">organization</span></span><a class="headerlink" href="#geoip2.records.Traits.organization" title="Permalink to this definition">¶</a></dt>
 <dd><p>The name of the organization associated with the IP address. This
 attribute is only available from the City Plus and Insights web services
 and the Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.static_ip_score">
 <span class="sig-name descname"><span class="pre">static_ip_score</span></span><a class="headerlink" href="#geoip2.records.Traits.static_ip_score" title="Permalink to this definition">¶</a></dt>
@@ -2455,29 +2455,29 @@
 lifetime under one. Static Cable/DSL IPs typically have a lifetime above
 thirty.</p>
 <p>This indicator can be useful for deciding whether an IP address represents
 the same user over time. This attribute is only available from
 Insights.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.10)">float</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)">float</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.user_count">
 <span class="sig-name descname"><span class="pre">user_count</span></span><a class="headerlink" href="#geoip2.records.Traits.user_count" title="Permalink to this definition">¶</a></dt>
 <dd><p>The estimated number of users sharing the IP/network during the past 24
 hours. For IPv4, the count is for the individual IP. For IPv6, the count
 is for the /64 network. This attribute is only available from
 Insights.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.records.Traits.user_type">
 <span class="sig-name descname"><span class="pre">user_type</span></span><a class="headerlink" href="#geoip2.records.Traits.user_type" title="Permalink to this definition">¶</a></dt>
@@ -2501,62 +2501,62 @@
 <li><p>search_engine_spider</p></li>
 <li><p>traveler</p></li>
 </ul>
 <p>This attribute is only available from the Insights end point and the
 Enterprise database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="id0">
-<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">network</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Network</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Network</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#id0" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">network</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Network</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Network</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#id0" title="Permalink to this definition">¶</a></dt>
 <dd><p>The network for the record</p>
 </dd></dl>
 
 </dd></dl>
 
 </section>
 <span class="target" id="module-geoip2.errors"></span><section id="errors">
 <h2>Errors<a class="headerlink" href="#errors" title="Permalink to this headline">¶</a></h2>
 <dl class="py exception">
 <dt class="sig sig-object py" id="geoip2.errors.AddressNotFoundError">
-<em class="property"><span class="pre">exception</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.errors.</span></span><span class="sig-name descname"><span class="pre">AddressNotFoundError</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">message</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">prefix_len</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.errors.AddressNotFoundError" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">exception</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.errors.</span></span><span class="sig-name descname"><span class="pre">AddressNotFoundError</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">message</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">prefix_len</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.errors.AddressNotFoundError" title="Permalink to this definition">¶</a></dt>
 <dd><p>The address you were looking up was not found.</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.errors.AddressNotFoundError.ip_address">
 <span class="sig-name descname"><span class="pre">ip_address</span></span><a class="headerlink" href="#geoip2.errors.AddressNotFoundError.ip_address" title="Permalink to this definition">¶</a></dt>
 <dd><p>The IP address used in the lookup. This is only available for database
 lookups.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="geoip2.errors.AddressNotFoundError.network">
 <span class="sig-name descname"><span class="pre">network</span></span><a class="headerlink" href="#geoip2.errors.AddressNotFoundError.network" title="Permalink to this definition">¶</a></dt>
 <dd><p>The network associated with the error. In particular, this is the
 largest network where no address would be found. This is only
 available for database lookups.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.10)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.10)">ipaddress.IPv6Network</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.11)">ipaddress.IPv4Network</a> or <a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.11)">ipaddress.IPv6Network</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="id3">
-<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">network</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.10)"><span class="pre">ipaddress.IPv4Network</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.10)"><span class="pre">ipaddress.IPv6Network</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#id3" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">network</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Network" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Network</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Network" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Network</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#id3" title="Permalink to this definition">¶</a></dt>
 <dd><p>The network for the error</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py exception">
 <dt class="sig sig-object py" id="geoip2.errors.AuthenticationError">
@@ -2564,21 +2564,21 @@
 <dd><p>There was a problem authenticating the request.</p>
 </dd></dl>
 
 <dl class="py exception">
 <dt class="sig sig-object py" id="geoip2.errors.GeoIP2Error">
 <em class="property"><span class="pre">exception</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.errors.</span></span><span class="sig-name descname"><span class="pre">GeoIP2Error</span></span><a class="headerlink" href="#geoip2.errors.GeoIP2Error" title="Permalink to this definition">¶</a></dt>
 <dd><p>There was a generic error in GeoIP2.</p>
-<p>This class represents a generic error. It extends <a class="reference external" href="https://docs.python.org/3/library/exceptions.html#RuntimeError" title="(in Python v3.10)"><code class="xref py py-exc docutils literal notranslate"><span class="pre">RuntimeError</span></code></a>
+<p>This class represents a generic error. It extends <a class="reference external" href="https://docs.python.org/3/library/exceptions.html#RuntimeError" title="(in Python v3.11)"><code class="xref py py-exc docutils literal notranslate"><span class="pre">RuntimeError</span></code></a>
 and does not add any additional attributes.</p>
 </dd></dl>
 
 <dl class="py exception">
 <dt class="sig sig-object py" id="geoip2.errors.HTTPError">
-<em class="property"><span class="pre">exception</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.errors.</span></span><span class="sig-name descname"><span class="pre">HTTPError</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">message</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">http_status</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uri</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">decoded_content</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.errors.HTTPError" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">exception</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">geoip2.errors.</span></span><span class="sig-name descname"><span class="pre">HTTPError</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">message</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">http_status</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uri</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">decoded_content</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#geoip2.errors.HTTPError" title="Permalink to this definition">¶</a></dt>
 <dd><p>There was an error when making your HTTP request.</p>
 <p>This class represents an HTTP transport error. It extends
 <a class="reference internal" href="#geoip2.errors.GeoIP2Error" title="geoip2.errors.GeoIP2Error"><code class="xref py py-exc docutils literal notranslate"><span class="pre">GeoIP2Error</span></code></a> and adds attributes of its own.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Variables</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>http_status</strong> – The HTTP status code returned</p></li>
@@ -2711,15 +2711,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">geoip2 4.6.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">geoip2 4.7.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">MaxMind GeoIP2 Python API</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2013-2022, MaxMind, Inc..
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.5.0.
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * geoip2_4.6.0_documentation »
+    * geoip2_4.7.0_documentation »
     * MaxMind GeoIP2 Python API
 ****** MaxMind GeoIP2 Python APIÂ¶ ******
 ***** DescriptionÂ¶ *****
 This package provides an API for the GeoIP2 and GeoLite2 web_services and
 databases.
 
 ***** InstallationÂ¶ *****
@@ -397,15 +397,15 @@
 data (âmoveâ, âeditâ, âalternate namesâ, etc.). Once the correction
 is part of the GeoNames data set, it will be automatically incorporated into
 future MaxMind releases.
 If you are a paying MaxMind customer and youâre not sure where to submit a
 correction, please contact_MaxMind_support for help.
 
 ***** RequirementsÂ¶ *****
-Python 3.6 or greater is required. Older versions are not supported.
+Python 3.7 or greater is required. Older versions are not supported.
 The Requests HTTP library is also required. See <http://python-requests.org>
 for details.
 
 ***** VersioningÂ¶ *****
 The GeoIP2 Python API uses Semantic_Versioning.
 
 ***** SupportÂ¶ *****
@@ -1436,10 +1436,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * geoip2_4.6.0_documentation »
+    * geoip2_4.7.0_documentation »
     * MaxMind GeoIP2 Python API
 © Copyright 2013-2022, MaxMind, Inc.. Created using Sphinx 4.5.0.
```

### Comparing `geoip2-4.6.0/docs/html/objects.inv` & `geoip2-4.7.0/docs/html/objects.inv`

 * *Files 1% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: geoip2
-# Version: 4.6.0
+# Version: 4.7.0
 # The remainder of this file is compressed using zlib.
 
 geoip2 py:module 0 index.html#module-$ -
 geoip2.database py:module 0 index.html#module-$ -
 geoip2.database.Reader py:class 1 index.html#$ -
 geoip2.database.Reader.anonymous_ip py:method 1 index.html#$ -
 geoip2.database.Reader.asn py:method 1 index.html#$ -
```

### Comparing `geoip2-4.6.0/docs/html/py-modindex.html` & `geoip2-4.7.0/docs/html/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; geoip2 4.6.0 documentation</title>
+    <title>Python Module Index &#8212; geoip2 4.7.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinxdoc.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">geoip2 4.6.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">geoip2 4.7.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -107,15 +107,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">geoip2 4.6.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">geoip2 4.7.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2013-2022, MaxMind, Inc..
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.5.0.
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * geoip2_4.6.0_documentation »
+    * geoip2_4.7.0_documentation »
     * Python Module Index
 ****** Python Module Index ******
 g
      
     g
 [-] geoip2
         geoip2.database
@@ -19,10 +19,10 @@
         geoip2.records
         geoip2.webservice
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * geoip2_4.6.0_documentation »
+    * geoip2_4.7.0_documentation »
     * Python Module Index
 © Copyright 2013-2022, MaxMind, Inc.. Created using Sphinx 4.5.0.
```

### Comparing `geoip2-4.6.0/docs/html/search.html` & `geoip2-4.7.0/docs/html/search.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; geoip2 4.6.0 documentation</title>
+    <title>Search &#8212; geoip2 4.7.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinxdoc.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
@@ -26,15 +26,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">geoip2 4.6.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">geoip2 4.7.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -86,15 +86,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">geoip2 4.6.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">geoip2 4.7.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2013-2022, MaxMind, Inc..
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.5.0.
     </div>
```

#### html2text {}

```diff
@@ -2,19 +2,19 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * geoip2_4.6.0_documentation »
+    * geoip2_4.7.0_documentation »
     * Search
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
 **** Navigation ****
     * index
     * modules |
-    * geoip2_4.6.0_documentation »
+    * geoip2_4.7.0_documentation »
     * Search
 © Copyright 2013-2022, MaxMind, Inc.. Created using Sphinx 4.5.0.
```

### Comparing `geoip2-4.6.0/docs/html/searchindex.js` & `geoip2-4.7.0/docs/html/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -295,18 +295,19 @@
         "42": 0,
         "44": 0,
         "4xx": 0,
         "50": 0,
         "500": 0,
         "55455": 0,
         "5xx": 0,
-        "6": 0,
+        "6": [],
         "60": 0,
         "64": 0,
         "67": 0,
+        "7": 0,
         "77": 0,
         "93": 0,
         "9733": 0,
         "99": 0,
         "\u7f8e\u56fd": 0,
         "abstract": 0,
         "case": 0,
```

### Comparing `geoip2-4.6.0/geoip2/database.py` & `geoip2-4.7.0/geoip2/database.py`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/geoip2/errors.py` & `geoip2-4.7.0/geoip2/errors.py`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/geoip2/models.py` & `geoip2-4.7.0/geoip2/models.py`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/geoip2/records.py` & `geoip2-4.7.0/geoip2/records.py`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/geoip2/webservice.py` & `geoip2-4.7.0/geoip2/webservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,25 +138,25 @@
                 f"Received a {status} error for {uri} but it did not include "
                 + "the expected JSON body: "
                 + ", ".join(ex.args),
                 status,
                 uri,
                 body,
             )
-        else:
-            if "code" in decoded_body and "error" in decoded_body:
-                return self._exception_for_web_service_error(
-                    decoded_body.get("error"), decoded_body.get("code"), status, uri
-                )
-            return HTTPError(
-                "Response contains JSON but it does not specify code or error keys",
-                status,
-                uri,
-                body,
+
+        if "code" in decoded_body and "error" in decoded_body:
+            return self._exception_for_web_service_error(
+                decoded_body.get("error"), decoded_body.get("code"), status, uri
             )
+        return HTTPError(
+            "Response contains JSON but it does not specify code or error keys",
+            status,
+            uri,
+            body,
+        )
 
     @staticmethod
     def _exception_for_web_service_error(
         message: str, code: str, status: int, uri: str
     ) -> Union[
         AuthenticationError,
         AddressNotFoundError,
```

### Comparing `geoip2-4.6.0/geoip2.egg-info/PKG-INFO` & `geoip2-4.7.0/geoip2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoip2
-Version: 4.6.0
+Version: 4.7.0
 Summary: MaxMind GeoIP2 API
 Home-page: http://www.maxmind.com/
 Author: Gregory Oschwald
 Author-email: goschwald@maxmind.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://geoip2.readthedocs.org/
 Project-URL: Source Code, https://github.com/maxmind/GeoIP2-python
@@ -12,23 +12,22 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Internet
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 =========================
 MaxMind GeoIP2 Python API
 =========================
 
 Description
@@ -514,15 +513,15 @@
 If you are a paying MaxMind customer and you're not sure where to submit a
 correction, please `contact MaxMind support
 <http://www.maxmind.com/en/support>`_ for help.
 
 Requirements
 ------------
 
-Python 3.6 or greater is required. Older versions are not supported.
+Python 3.7 or greater is required. Older versions are not supported.
 
 The Requests HTTP library is also required. See
 <http://python-requests.org> for details.
 
 Versioning
 ----------
```

### Comparing `geoip2-4.6.0/geoip2.egg-info/SOURCES.txt` & `geoip2-4.7.0/geoip2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 docs/html/.buildinfo
 docs/html/genindex.html
 docs/html/index.html
 docs/html/objects.inv
```

### Comparing `geoip2-4.6.0/setup.py` & `geoip2-4.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,27 +20,26 @@
     author="Gregory Oschwald",
     author_email="goschwald@maxmind.com",
     url="http://www.maxmind.com/",
     packages=["geoip2"],
     package_data={"": ["LICENSE"], "geoip2": ["py.typed"]},
     package_dir={"geoip2": "geoip2"},
     include_package_data=True,
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=requirements,
-    tests_require=["mocket>=3.8.9"],
+    tests_require=["mocket>=3.11.0"],
     test_suite="tests",
     license=geoip2.__license__,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python",
         "Topic :: Internet :: Proxy Servers",
         "Topic :: Internet",
```

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-Anonymous-IP-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-Anonymous-IP-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-City-Test-Broken-Double-Format.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-City-Test-Broken-Double-Format.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-City-Test-Invalid-Node-Count.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-City-Test-Invalid-Node-Count.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-City-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-City-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-Connection-Type-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-Connection-Type-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-Country-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-Country-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-DensityIncome-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-DensityIncome-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-Domain-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-Domain-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-Enterprise-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-Enterprise-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-ISP-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-ISP-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-Precision-Enterprise-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-Precision-Enterprise-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-Static-IP-Score-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-Static-IP-Score-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoIP2-User-Count-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoIP2-User-Count-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoLite2-ASN-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoLite2-ASN-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoLite2-City-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoLite2-City-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/GeoLite2-Country-Test.mmdb` & `geoip2-4.7.0/tests/data/test-data/GeoLite2-Country-Test.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-no-ipv4-search-tree.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-no-ipv4-search-tree.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-string-value-entries.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-string-value-entries.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-broken-pointers-24.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-broken-pointers-24.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-broken-search-tree-24.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-broken-search-tree-24.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-decoder.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-decoder.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-ipv4-24.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-ipv4-24.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-ipv4-28.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-ipv4-28.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-ipv4-32.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-ipv4-32.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-ipv6-24.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-ipv6-24.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-ipv6-28.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-ipv6-28.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-ipv6-32.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-ipv6-32.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-metadata-pointers.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-metadata-pointers.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-mixed-24.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-mixed-24.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-mixed-28.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-mixed-28.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-mixed-32.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-mixed-32.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-nested.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-nested.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/data/test-data/MaxMind-DB-test-pointer-decoder.mmdb` & `geoip2-4.7.0/tests/data/test-data/MaxMind-DB-test-pointer-decoder.mmdb`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/database_test.py` & `geoip2-4.7.0/tests/database_test.py`

 * *Files identical despite different names*

### Comparing `geoip2-4.6.0/tests/models_test.py` & `geoip2-4.7.0/tests/models_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,15 +381,14 @@
             model.unk_base  # type: ignore
         with self.assertRaises(AttributeError):
             model.traits.invalid  # type: ignore
         self.assertEqual(model.traits.ip_address, "1.2.3.4", "correct ip")
 
 
 class TestNames(unittest.TestCase):
-
     raw: Dict = {
         "continent": {
             "code": "NA",
             "geoname_id": 42,
             "names": {
                 "de": "Nordamerika",
                 "en": "North America",
```

### Comparing `geoip2-4.6.0/tests/webservice_test.py` & `geoip2-4.7.0/tests/webservice_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,14 @@
             self.base_uri + "country/" + "1.2.3.11",
             status=300,
             content_type=self._content_type("country"),
         )
         with self.assertRaisesRegex(
             HTTPError, r"Received a very surprising HTTP status \(300\) for"
         ):
-
             self.run_client(self.client.country("1.2.3.11"))
 
     @httprettified
     def test_ip_address_required(self):
         self._test_error(400, "IP_ADDRESS_REQUIRED", InvalidRequestError)
 
     @httprettified
@@ -295,24 +294,26 @@
         )
         self.run_client(self.client.country("1.2.3.4"))
         request = httpretty.last_request
 
         self.assertEqual(
             request.path, "/geoip/v2.1/country/1.2.3.4", "correct URI is used"
         )
-        self.assertEqual(
-            request.headers["Accept"], "application/json", "correct Accept header"
-        )
+
+        # This is to prevent breakage if header normalization in Mocket
+        # changes again in the future.
+        headers = {k.lower(): v for k, v in request.headers.items()}
+        self.assertEqual(headers["accept"], "application/json", "correct Accept header")
         self.assertRegex(
-            request.headers["User-Agent"],
+            headers["user-agent"],
             "^GeoIP2-Python-Client/",
             "Correct User-Agent",
         )
         self.assertEqual(
-            request.headers["Authorization"],
+            headers["authorization"],
             "Basic NDI6YWJjZGVmMTIzNDU2",
             "correct auth",
         )
 
     @httprettified
     def test_city_ok(self):
         httpretty.register_uri(
```

