# Comparing `tmp/maxminddb-2.2.0.tar.gz` & `tmp/maxminddb-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/maxminddb-2.2.0.tar", last modified: Fri Sep 24 17:22:58 2021, max compression
+gzip compressed data, was "maxminddb-2.3.0.tar", last modified: Tue May  9 20:11:13 2023, max compression
```

## Comparing `maxminddb-2.2.0.tar` & `maxminddb-2.3.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.450599 maxminddb-2.2.0/
--rw-r--r--   0 greg      (1000) greg      (1000)     8438 2021-09-24 17:22:13.000000 maxminddb-2.2.0/HISTORY.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    11358 2019-01-09 22:21:10.000000 maxminddb-2.2.0/LICENSE
--rw-r--r--   0 greg      (1000) greg      (1000)      141 2021-09-21 15:14:38.000000 maxminddb-2.2.0/MANIFEST.in
--rw-r--r--   0 greg      (1000) greg      (1000)     5668 2021-09-24 17:22:58.450599 maxminddb-2.2.0/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     3852 2021-09-14 14:43:24.000000 maxminddb-2.2.0/README.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.434599 maxminddb-2.2.0/docs/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.438599 maxminddb-2.2.0/docs/html/
--rw-r--r--   0 greg      (1000) greg      (1000)      230 2021-09-24 17:22:58.000000 maxminddb-2.2.0/docs/html/.buildinfo
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.438599 maxminddb-2.2.0/docs/html/_sources/
--rw-r--r--   0 greg      (1000) greg      (1000)      762 2021-09-21 15:14:38.000000 maxminddb-2.2.0/docs/html/_sources/index.rst.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.442599 maxminddb-2.2.0/docs/html/_static/
--rw-r--r--   0 greg      (1000) greg      (1000)    14638 2021-09-24 17:22:58.000000 maxminddb-2.2.0/docs/html/_static/basic.css
--rw-r--r--   0 greg      (1000) greg      (1000)      107 2021-02-02 17:50:53.000000 maxminddb-2.2.0/docs/html/_static/contents.png
--rw-r--r--   0 greg      (1000) greg      (1000)     9630 2021-09-20 17:44:35.000000 maxminddb-2.2.0/docs/html/_static/doctools.js
--rw-r--r--   0 greg      (1000) greg      (1000)      355 2021-09-24 17:22:58.000000 maxminddb-2.2.0/docs/html/_static/documentation_options.js
--rw-r--r--   0 greg      (1000) greg      (1000)      286 2021-02-02 17:50:53.000000 maxminddb-2.2.0/docs/html/_static/file.png
--rw-r--r--   0 greg      (1000) greg      (1000)   287630 2021-02-02 17:50:53.000000 maxminddb-2.2.0/docs/html/_static/jquery-3.5.1.js
--rw-r--r--   0 greg      (1000) greg      (1000)    89476 2021-02-02 17:50:53.000000 maxminddb-2.2.0/docs/html/_static/jquery.js
--rw-r--r--   0 greg      (1000) greg      (1000)    10854 2021-09-24 17:22:58.000000 maxminddb-2.2.0/docs/html/_static/language_data.js
--rw-r--r--   0 greg      (1000) greg      (1000)       90 2021-02-02 17:50:53.000000 maxminddb-2.2.0/docs/html/_static/minus.png
--rw-r--r--   0 greg      (1000) greg      (1000)      120 2021-02-02 17:50:53.000000 maxminddb-2.2.0/docs/html/_static/navigation.png
--rw-r--r--   0 greg      (1000) greg      (1000)       90 2021-02-02 17:50:53.000000 maxminddb-2.2.0/docs/html/_static/plus.png
--rw-r--r--   0 greg      (1000) greg      (1000)     4780 2021-09-24 17:22:58.000000 maxminddb-2.2.0/docs/html/_static/pygments.css
--rw-r--r--   0 greg      (1000) greg      (1000)    16733 2021-09-20 17:44:35.000000 maxminddb-2.2.0/docs/html/_static/searchtools.js
--rw-r--r--   0 greg      (1000) greg      (1000)     6236 2021-09-24 17:22:58.000000 maxminddb-2.2.0/docs/html/_static/sphinxdoc.css
--rw-r--r--   0 greg      (1000) greg      (1000)    68420 2021-09-20 17:44:35.000000 maxminddb-2.2.0/docs/html/_static/underscore-1.13.1.js
--rw-r--r--   0 greg      (1000) greg      (1000)    35168 2021-02-02 17:50:53.000000 maxminddb-2.2.0/docs/html/_static/underscore-1.3.1.js
--rw-r--r--   0 greg      (1000) greg      (1000)    19530 2021-09-20 17:44:35.000000 maxminddb-2.2.0/docs/html/_static/underscore.js
--rw-r--r--   0 greg      (1000) greg      (1000)     9401 2021-09-24 17:22:58.000000 maxminddb-2.2.0/docs/html/genindex.html
--rw-r--r--   0 greg      (1000) greg      (1000)    44848 2021-09-24 17:22:58.000000 maxminddb-2.2.0/docs/html/index.html
--rw-r--r--   0 greg      (1000) greg      (1000)      522 2021-09-24 17:22:58.000000 maxminddb-2.2.0/docs/html/objects.inv
--rw-r--r--   0 greg      (1000) greg      (1000)     4016 2021-09-24 17:22:58.000000 maxminddb-2.2.0/docs/html/py-modindex.html
--rw-r--r--   0 greg      (1000) greg      (1000)     3367 2021-09-24 17:22:58.000000 maxminddb-2.2.0/docs/html/search.html
--rw-r--r--   0 greg      (1000) greg      (1000)     3860 2021-09-24 17:22:58.000000 maxminddb-2.2.0/docs/html/searchindex.js
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.442599 maxminddb-2.2.0/extension/
--rw-r--r--   0 greg      (1000) greg      (1000)    23381 2021-09-18 16:38:33.000000 maxminddb-2.2.0/extension/maxminddb.c
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.442599 maxminddb-2.2.0/maxminddb/
--rw-r--r--   0 greg      (1000) greg      (1000)     2557 2021-09-24 17:22:29.000000 maxminddb-2.2.0/maxminddb/__init__.py
--rw-r--r--   0 greg      (1000) greg      (1000)      122 2019-01-09 22:21:10.000000 maxminddb-2.2.0/maxminddb/const.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     7050 2020-10-16 21:27:19.000000 maxminddb-2.2.0/maxminddb/decoder.py
--rw-r--r--   0 greg      (1000) greg      (1000)      226 2019-01-09 22:21:10.000000 maxminddb-2.2.0/maxminddb/errors.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1447 2021-09-24 17:10:54.000000 maxminddb-2.2.0/maxminddb/extension.pyi
--rw-r--r--   0 greg      (1000) greg      (1000)     2153 2021-06-01 17:36:58.000000 maxminddb-2.2.0/maxminddb/file.py
--rw-r--r--   0 greg      (1000) greg      (1000)        0 2020-07-28 17:36:22.000000 maxminddb-2.2.0/maxminddb/py.typed
--rw-r--r--   0 greg      (1000) greg      (1000)    10985 2021-09-21 15:14:38.000000 maxminddb-2.2.0/maxminddb/reader.py
--rw-r--r--   0 greg      (1000) greg      (1000)      558 2020-07-10 20:06:17.000000 maxminddb-2.2.0/maxminddb/types.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.442599 maxminddb-2.2.0/maxminddb.egg-info/
--rw-r--r--   0 greg      (1000) greg      (1000)     5668 2021-09-24 17:22:58.000000 maxminddb-2.2.0/maxminddb.egg-info/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     3534 2021-09-24 17:22:58.000000 maxminddb-2.2.0/maxminddb.egg-info/SOURCES.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2021-09-24 17:22:58.000000 maxminddb-2.2.0/maxminddb.egg-info/dependency_links.txt
--rw-r--r--   0 greg      (1000) greg      (1000)       10 2021-09-24 17:22:58.000000 maxminddb-2.2.0/maxminddb.egg-info/top_level.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)      349 2021-09-24 17:22:58.450599 maxminddb-2.2.0/setup.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)     4783 2021-09-18 16:53:14.000000 maxminddb-2.2.0/setup.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.442599 maxminddb-2.2.0/tests/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.434599 maxminddb-2.2.0/tests/data/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.434599 maxminddb-2.2.0/tests/data/bad-data/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.442599 maxminddb-2.2.0/tests/data/bad-data/libmaxminddb/
--rw-r--r--   0 greg      (1000) greg      (1000)      412 2019-09-20 16:04:16.000000 maxminddb-2.2.0/tests/data/bad-data/libmaxminddb/libmaxminddb-offset-integer-overflow.mmdb
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.446599 maxminddb-2.2.0/tests/data/bad-data/maxminddb-golang/
--rw-r--r--   0 greg      (1000) greg      (1000)     2731 2019-09-20 16:04:16.000000 maxminddb-2.2.0/tests/data/bad-data/maxminddb-golang/cyclic-data-structure.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)       32 2019-09-20 16:04:16.000000 maxminddb-2.2.0/tests/data/bad-data/maxminddb-golang/invalid-bytes-length.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)      327 2019-09-20 16:04:16.000000 maxminddb-2.2.0/tests/data/bad-data/maxminddb-golang/invalid-data-record-offset.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     2731 2019-09-20 16:04:16.000000 maxminddb-2.2.0/tests/data/bad-data/maxminddb-golang/invalid-map-key-length.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)      187 2019-09-20 16:04:16.000000 maxminddb-2.2.0/tests/data/bad-data/maxminddb-golang/invalid-string-length.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)       16 2019-09-20 16:04:16.000000 maxminddb-2.2.0/tests/data/bad-data/maxminddb-golang/metadata-is-an-uint128.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     2333 2019-09-20 16:04:16.000000 maxminddb-2.2.0/tests/data/bad-data/maxminddb-golang/unexpected-bytes.mmdb
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.446599 maxminddb-2.2.0/tests/data/bad-data/maxminddb-python/
--rw-r--r--   0 greg      (1000) greg      (1000)     3535 2020-05-04 15:42:59.000000 maxminddb-2.2.0/tests/data/bad-data/maxminddb-python/bad-unicode-in-map-key.mmdb
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2021-09-24 17:22:58.446599 maxminddb-2.2.0/tests/data/test-data/
--rw-r--r--   0 greg      (1000) greg      (1000)     4382 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-Anonymous-IP-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    20620 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-City-Test-Broken-Double-Format.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    21016 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-City-Test-Invalid-Node-Count.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    20996 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-City-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3779 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-Connection-Type-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    19394 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-Country-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3065 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-DensityIncome-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     6326 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-Domain-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     7983 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-Enterprise-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    76417 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-ISP-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    16438 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-Precision-Enterprise-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     9750 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-Static-IP-Score-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     4818 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoIP2-User-Count-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    12358 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoLite2-ASN-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    20809 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoLite2-City-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)    17952 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/GeoLite2-Country-Test.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)      618 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-no-ipv4-search-tree.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1341 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-string-value-entries.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1289 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-broken-pointers-24.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1298 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-broken-search-tree-24.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3191 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-decoder.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1298 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-ipv4-24.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1462 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-ipv4-28.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1626 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-ipv4-32.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     2806 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-ipv6-24.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3222 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-ipv6-28.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3638 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-ipv6-32.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     2258 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-metadata-pointers.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3066 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-mixed-24.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3511 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-mixed-28.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3956 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-mixed-32.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     3802 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-nested.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)     1737 2021-06-01 17:37:15.000000 maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-pointer-decoder.mmdb
--rw-r--r--   0 greg      (1000) greg      (1000)       59 2019-01-09 22:21:44.000000 maxminddb-2.2.0/tests/data/test-data/maps-with-pointers.raw
--rw-r--r--   0 greg      (1000) greg      (1000)     7820 2020-09-09 22:32:06.000000 maxminddb-2.2.0/tests/decoder_test.py
--rw-r--r--   0 greg      (1000) greg      (1000)    21598 2021-09-24 17:10:57.000000 maxminddb-2.2.0/tests/reader_test.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.279801 maxminddb-2.3.0/
+-rw-r--r--   0 greg      (1000) greg      (1000)     8792 2023-05-09 20:03:29.000000 maxminddb-2.3.0/HISTORY.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)    11358 2019-01-09 22:21:10.000000 maxminddb-2.3.0/LICENSE
+-rw-r--r--   0 greg      (1000) greg      (1000)      141 2021-09-21 15:14:38.000000 maxminddb-2.3.0/MANIFEST.in
+-rw-r--r--   0 greg      (1000) greg      (1000)     5055 2023-05-09 20:11:13.279801 maxminddb-2.3.0/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     3852 2023-01-17 17:58:57.000000 maxminddb-2.3.0/README.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.263800 maxminddb-2.3.0/docs/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.267800 maxminddb-2.3.0/docs/html/
+-rw-r--r--   0 greg      (1000) greg      (1000)      230 2023-05-09 20:10:58.000000 maxminddb-2.3.0/docs/html/.buildinfo
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.267800 maxminddb-2.3.0/docs/html/_sources/
+-rw-r--r--   0 greg      (1000) greg      (1000)      762 2021-09-21 15:14:38.000000 maxminddb-2.3.0/docs/html/_sources/index.rst.txt
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.271801 maxminddb-2.3.0/docs/html/_static/
+-rw-r--r--   0 greg      (1000) greg      (1000)    14692 2023-05-09 20:10:58.000000 maxminddb-2.3.0/docs/html/_static/basic.css
+-rw-r--r--   0 greg      (1000) greg      (1000)      107 2022-03-28 19:26:41.000000 maxminddb-2.3.0/docs/html/_static/contents.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    10766 2022-03-28 19:26:41.000000 maxminddb-2.3.0/docs/html/_static/doctools.js
+-rw-r--r--   0 greg      (1000) greg      (1000)      422 2023-05-09 20:10:58.000000 maxminddb-2.3.0/docs/html/_static/documentation_options.js
+-rw-r--r--   0 greg      (1000) greg      (1000)      286 2022-03-28 19:26:41.000000 maxminddb-2.3.0/docs/html/_static/file.png
+-rw-r--r--   0 greg      (1000) greg      (1000)   287630 2022-03-28 19:26:41.000000 maxminddb-2.3.0/docs/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 greg      (1000) greg      (1000)    89476 2022-03-28 19:26:41.000000 maxminddb-2.3.0/docs/html/_static/jquery.js
+-rw-r--r--   0 greg      (1000) greg      (1000)    10854 2023-05-09 20:10:58.000000 maxminddb-2.3.0/docs/html/_static/language_data.js
+-rw-r--r--   0 greg      (1000) greg      (1000)       90 2022-03-28 19:26:41.000000 maxminddb-2.3.0/docs/html/_static/minus.png
+-rw-r--r--   0 greg      (1000) greg      (1000)      120 2022-03-28 19:26:41.000000 maxminddb-2.3.0/docs/html/_static/navigation.png
+-rw-r--r--   0 greg      (1000) greg      (1000)       90 2022-03-28 19:26:41.000000 maxminddb-2.3.0/docs/html/_static/plus.png
+-rw-r--r--   0 greg      (1000) greg      (1000)     4846 2023-05-09 20:10:58.000000 maxminddb-2.3.0/docs/html/_static/pygments.css
+-rw-r--r--   0 greg      (1000) greg      (1000)    16634 2022-03-28 19:26:41.000000 maxminddb-2.3.0/docs/html/_static/searchtools.js
+-rw-r--r--   0 greg      (1000) greg      (1000)     6236 2023-05-09 20:10:58.000000 maxminddb-2.3.0/docs/html/_static/sphinxdoc.css
+-rw-r--r--   0 greg      (1000) greg      (1000)    68420 2022-03-28 19:26:41.000000 maxminddb-2.3.0/docs/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 greg      (1000) greg      (1000)    19530 2022-03-28 19:26:41.000000 maxminddb-2.3.0/docs/html/_static/underscore.js
+-rw-r--r--   0 greg      (1000) greg      (1000)     9401 2023-05-09 20:10:58.000000 maxminddb-2.3.0/docs/html/genindex.html
+-rw-r--r--   0 greg      (1000) greg      (1000)    49839 2023-05-09 20:10:58.000000 maxminddb-2.3.0/docs/html/index.html
+-rw-r--r--   0 greg      (1000) greg      (1000)      522 2023-05-09 20:10:58.000000 maxminddb-2.3.0/docs/html/objects.inv
+-rw-r--r--   0 greg      (1000) greg      (1000)     4016 2023-05-09 20:10:58.000000 maxminddb-2.3.0/docs/html/py-modindex.html
+-rw-r--r--   0 greg      (1000) greg      (1000)     3367 2023-05-09 20:10:58.000000 maxminddb-2.3.0/docs/html/search.html
+-rw-r--r--   0 greg      (1000) greg      (1000)     3916 2023-05-09 20:10:58.000000 maxminddb-2.3.0/docs/html/searchindex.js
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.271801 maxminddb-2.3.0/extension/
+-rw-r--r--   0 greg      (1000) greg      (1000)    23421 2023-01-17 17:58:57.000000 maxminddb-2.3.0/extension/maxminddb.c
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.271801 maxminddb-2.3.0/maxminddb/
+-rw-r--r--   0 greg      (1000) greg      (1000)     2557 2023-05-09 20:09:31.000000 maxminddb-2.3.0/maxminddb/__init__.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      122 2019-01-09 22:21:10.000000 maxminddb-2.3.0/maxminddb/const.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     7005 2022-07-09 23:43:59.000000 maxminddb-2.3.0/maxminddb/decoder.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      226 2019-01-09 22:21:10.000000 maxminddb-2.3.0/maxminddb/errors.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     1447 2021-09-24 17:10:54.000000 maxminddb-2.3.0/maxminddb/extension.pyi
+-rw-r--r--   0 greg      (1000) greg      (1000)     2153 2021-06-01 17:36:58.000000 maxminddb-2.3.0/maxminddb/file.py
+-rw-r--r--   0 greg      (1000) greg      (1000)        0 2020-07-28 17:36:22.000000 maxminddb-2.3.0/maxminddb/py.typed
+-rw-r--r--   0 greg      (1000) greg      (1000)    11002 2022-06-09 15:23:43.000000 maxminddb-2.3.0/maxminddb/reader.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      558 2020-07-10 20:06:17.000000 maxminddb-2.3.0/maxminddb/types.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.271801 maxminddb-2.3.0/maxminddb.egg-info/
+-rw-r--r--   0 greg      (1000) greg      (1000)     5055 2023-05-09 20:11:13.000000 maxminddb-2.3.0/maxminddb.egg-info/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     3511 2023-05-09 20:11:13.000000 maxminddb-2.3.0/maxminddb.egg-info/SOURCES.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-05-09 20:11:13.000000 maxminddb-2.3.0/maxminddb.egg-info/dependency_links.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)       10 2023-05-09 20:11:13.000000 maxminddb-2.3.0/maxminddb.egg-info/top_level.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      169 2023-05-09 19:53:37.000000 maxminddb-2.3.0/pyproject.toml
+-rw-r--r--   0 greg      (1000) greg      (1000)      703 2023-05-09 20:11:13.279801 maxminddb-2.3.0/setup.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)     5192 2023-01-17 17:58:57.000000 maxminddb-2.3.0/setup.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.271801 maxminddb-2.3.0/tests/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.263800 maxminddb-2.3.0/tests/data/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.263800 maxminddb-2.3.0/tests/data/bad-data/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.271801 maxminddb-2.3.0/tests/data/bad-data/libmaxminddb/
+-rw-r--r--   0 greg      (1000) greg      (1000)      412 2019-09-20 16:04:16.000000 maxminddb-2.3.0/tests/data/bad-data/libmaxminddb/libmaxminddb-offset-integer-overflow.mmdb
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.275801 maxminddb-2.3.0/tests/data/bad-data/maxminddb-golang/
+-rw-r--r--   0 greg      (1000) greg      (1000)     2731 2019-09-20 16:04:16.000000 maxminddb-2.3.0/tests/data/bad-data/maxminddb-golang/cyclic-data-structure.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)       32 2019-09-20 16:04:16.000000 maxminddb-2.3.0/tests/data/bad-data/maxminddb-golang/invalid-bytes-length.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)      327 2019-09-20 16:04:16.000000 maxminddb-2.3.0/tests/data/bad-data/maxminddb-golang/invalid-data-record-offset.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     2731 2019-09-20 16:04:16.000000 maxminddb-2.3.0/tests/data/bad-data/maxminddb-golang/invalid-map-key-length.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)      187 2019-09-20 16:04:16.000000 maxminddb-2.3.0/tests/data/bad-data/maxminddb-golang/invalid-string-length.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)       16 2019-09-20 16:04:16.000000 maxminddb-2.3.0/tests/data/bad-data/maxminddb-golang/metadata-is-an-uint128.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     2333 2019-09-20 16:04:16.000000 maxminddb-2.3.0/tests/data/bad-data/maxminddb-golang/unexpected-bytes.mmdb
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.275801 maxminddb-2.3.0/tests/data/bad-data/maxminddb-python/
+-rw-r--r--   0 greg      (1000) greg      (1000)     3535 2020-05-04 15:42:59.000000 maxminddb-2.3.0/tests/data/bad-data/maxminddb-python/bad-unicode-in-map-key.mmdb
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-09 20:11:13.279801 maxminddb-2.3.0/tests/data/test-data/
+-rw-r--r--   0 greg      (1000) greg      (1000)     4382 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-Anonymous-IP-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    20620 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-City-Test-Broken-Double-Format.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    21016 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-City-Test-Invalid-Node-Count.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    20996 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-City-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3779 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-Connection-Type-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    19394 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-Country-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3065 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-DensityIncome-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     6326 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-Domain-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     7983 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-Enterprise-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    76417 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-ISP-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    16438 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-Precision-Enterprise-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     9750 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-Static-IP-Score-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     4818 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoIP2-User-Count-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    12358 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoLite2-ASN-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    20809 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoLite2-City-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)    17952 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/GeoLite2-Country-Test.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)      618 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-no-ipv4-search-tree.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1341 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-string-value-entries.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1289 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-broken-pointers-24.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1298 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-broken-search-tree-24.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3191 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-decoder.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1298 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-ipv4-24.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1462 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-ipv4-28.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1626 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-ipv4-32.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     2806 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-ipv6-24.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3222 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-ipv6-28.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3638 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-ipv6-32.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     2258 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-metadata-pointers.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3066 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-mixed-24.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3511 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-mixed-28.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3956 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-mixed-32.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     3802 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-nested.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)     1737 2021-06-01 17:37:15.000000 maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-pointer-decoder.mmdb
+-rw-r--r--   0 greg      (1000) greg      (1000)       59 2019-01-09 22:21:44.000000 maxminddb-2.3.0/tests/data/test-data/maps-with-pointers.raw
+-rw-r--r--   0 greg      (1000) greg      (1000)     7819 2023-05-09 19:53:37.000000 maxminddb-2.3.0/tests/decoder_test.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    21598 2021-09-24 17:10:57.000000 maxminddb-2.3.0/tests/reader_test.py
```

### Comparing `maxminddb-2.2.0/HISTORY.rst` & `maxminddb-2.3.0/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 .. :changelog:
 
 History
 -------
 
+2.3.0 (2023-05-09)
+++++++++++++++++++
+
+* IMPORTANT: Python 3.7 or greater is required. If you are using an older
+  version, please use an earlier release.
+* ``distutils`` is no longer used for building the C extension.
+* Missing ``Py_INCREF`` was added to module initialization for the C
+  extension. Pull request by R. Christian McDonald. GitHub #106.
+
 2.2.0 (2021-09-24)
 ++++++++++++++++++
 
 * The return type for ``maxminddb.open_database()`` has been simplified
   to be just the ``Reader`` class as opposed to a union of that with
   the extension class. This is done by casting the extension to
   ``Reader``. The extension class has the same public API as the
```

### Comparing `maxminddb-2.2.0/LICENSE` & `maxminddb-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/PKG-INFO` & `maxminddb-2.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,137 +1,144 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: maxminddb
-Version: 2.2.0
+Version: 2.3.0
 Summary: Reader for the MaxMind DB format
 Home-page: http://www.maxmind.com/
 Author: Gregory Oschwald
 Author-email: goschwald@maxmind.com
 License: Apache License, Version 2.0
-Description: ========================
-        MaxMind DB Python Module
-        ========================
-        
-        Description
-        -----------
-        
-        This is a Python module for reading MaxMind DB files. The module includes both
-        a pure Python reader and an optional C extension.
-        
-        MaxMind DB is a binary file format that stores data indexed by IP address
-        subnets (IPv4 or IPv6).
-        
-        Installation
-        ------------
-        
-        If you want to use the C extension, you must first install `libmaxminddb
-        <https://github.com/maxmind/libmaxminddb>`_ C library installed before
-        installing this extension. If the library is not available, the module will
-        fall-back to a pure Python implementation. Note that when installing the C
-        library from a package, you may be required to install additonal packages
-        containing build requirements such as `libmaxminddb-dev` on Debian.
-        
-        To install maxminddb, type:
-        
-        .. code-block:: bash
-        
-            $ pip install maxminddb
-        
-        If you are not able to use pip, you may also use easy_install from the
-        source directory:
-        
-        .. code-block:: bash
-        
-            $ easy_install .
-        
-        Usage
-        -----
-        
-        To use this module, you must first download or create a MaxMind DB file. We
-        provide `free GeoLite2 databases
-        <https://dev.maxmind.com/geoip/geolocate-an-ip/databases?lang=en>`_. These
-        files must be decompressed with ``gunzip``.
-        
-        After you have obtained a database and imported the module, call
-        ``open_database`` with a path, or file descriptor (in the case of ``MODE_FD``),
-        to the database as the first argument. Optionally, you may pass a mode as the
-        second argument. The modes are exported from ``maxminddb``. Valid modes are:
-        
-        * ``MODE_MMAP_EXT`` - use the C extension with memory map.
-        * ``MODE_MMAP`` - read from memory map. Pure Python.
-        * ``MODE_FILE`` - read database as standard file. Pure Python.
-        * ``MODE_MEMORY`` - load database into memory. Pure Python.
-        * ``MODE_FD`` - load database into memory from a file descriptor. Pure Python.
-        * ``MODE_AUTO`` - try ``MODE_MMAP_EXT``, ``MODE_MMAP``, ``MODE_FILE`` in that
-          order. Default.
-        
-        **NOTE**: When using ``MODE_FD``, it is the *caller's* responsibility to be
-        sure that the file descriptor gets closed properly. The caller may close the
-        file descriptor immediately after the ``Reader`` object is created.
-        
-        The ``open_database`` function returns a ``Reader`` object. To look up an IP
-        address, use the ``get`` method on this object. The method will return the
-        corresponding values for the IP address from the database (e.g., a dictionary
-        for GeoIP2/GeoLite2 databases). If the database does not contain a record for
-        that IP address, the method will return ``None``.
-        
-        If you wish to also retrieve the prefix length for the record, use the
-        ``get_with_prefix_len`` method. This returns a tuple containing the record
-        followed by the network prefix length associated with the record.
-        
-        Example
-        -------
-        
-        .. code-block:: pycon
-        
-            >>> import maxminddb
-            >>>
-            >>> with maxminddb.open_database('GeoLite2-City.mmdb') as reader:
-            >>>
-            >>>     reader.get('152.216.7.110')
-            {'country': ... }
-            >>>
-            >>>     reader.get_with_prefix_len('152.216.7.110')
-            ({'country': ... }, 24)
-        
-        Exceptions
-        ----------
-        
-        The module will return an ``InvalidDatabaseError`` if the database is corrupt
-        or otherwise invalid. A ``ValueError`` will be thrown if you look up an
-        invalid IP address or an IPv6 address in an IPv4 database.
-        
-        Requirements
-        ------------
-        
-        This code requires Python 3.6+. Older versions are not supported. The C
-        extension requires CPython.
-        
-        Versioning
-        ----------
-        
-        The MaxMind DB Python module uses `Semantic Versioning <https://semver.org/>`_.
-        
-        Support
-        -------
-        
-        Please report all issues with this code using the `GitHub issue tracker
-        <https://github.com/maxmind/MaxMind-DB-Reader-python/issues>`_
-        
-        If you are having an issue with a MaxMind service that is not specific to this
-        API, please contact `MaxMind support <https://www.maxmind.com/en/support>`_ for
-        assistance.
-        
+Project-URL: Documentation, https://maxminddb.readthedocs.org/
+Project-URL: Source Code, https://github.com/maxmind/MaxMind-DB-Reader-python
+Project-URL: Issue Tracker, https://github.com/maxmind/MaxMind-DB-Reader-python/issues
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
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Internet
-Requires-Python: >=3.6
+Requires-Python: >=3.7
+License-File: LICENSE
+
+========================
+MaxMind DB Python Module
+========================
+
+Description
+-----------
+
+This is a Python module for reading MaxMind DB files. The module includes both
+a pure Python reader and an optional C extension.
+
+MaxMind DB is a binary file format that stores data indexed by IP address
+subnets (IPv4 or IPv6).
+
+Installation
+------------
+
+If you want to use the C extension, you must first install `libmaxminddb
+<https://github.com/maxmind/libmaxminddb>`_ C library installed before
+installing this extension. If the library is not available, the module will
+fall-back to a pure Python implementation. Note that when installing the C
+library from a package, you may be required to install additonal packages
+containing build requirements such as `libmaxminddb-dev` on Debian.
+
+To install maxminddb, type:
+
+.. code-block:: bash
+
+    $ pip install maxminddb
+
+If you are not able to use pip, you may also use easy_install from the
+source directory:
+
+.. code-block:: bash
+
+    $ easy_install .
+
+Usage
+-----
+
+To use this module, you must first download or create a MaxMind DB file. We
+provide `free GeoLite2 databases
+<https://dev.maxmind.com/geoip/geolocate-an-ip/databases?lang=en>`_. These
+files must be decompressed with ``gunzip``.
+
+After you have obtained a database and imported the module, call
+``open_database`` with a path, or file descriptor (in the case of ``MODE_FD``),
+to the database as the first argument. Optionally, you may pass a mode as the
+second argument. The modes are exported from ``maxminddb``. Valid modes are:
+
+* ``MODE_MMAP_EXT`` - use the C extension with memory map.
+* ``MODE_MMAP`` - read from memory map. Pure Python.
+* ``MODE_FILE`` - read database as standard file. Pure Python.
+* ``MODE_MEMORY`` - load database into memory. Pure Python.
+* ``MODE_FD`` - load database into memory from a file descriptor. Pure Python.
+* ``MODE_AUTO`` - try ``MODE_MMAP_EXT``, ``MODE_MMAP``, ``MODE_FILE`` in that
+  order. Default.
+
+**NOTE**: When using ``MODE_FD``, it is the *caller's* responsibility to be
+sure that the file descriptor gets closed properly. The caller may close the
+file descriptor immediately after the ``Reader`` object is created.
+
+The ``open_database`` function returns a ``Reader`` object. To look up an IP
+address, use the ``get`` method on this object. The method will return the
+corresponding values for the IP address from the database (e.g., a dictionary
+for GeoIP2/GeoLite2 databases). If the database does not contain a record for
+that IP address, the method will return ``None``.
+
+If you wish to also retrieve the prefix length for the record, use the
+``get_with_prefix_len`` method. This returns a tuple containing the record
+followed by the network prefix length associated with the record.
+
+Example
+-------
+
+.. code-block:: pycon
+
+    >>> import maxminddb
+    >>>
+    >>> with maxminddb.open_database('GeoLite2-City.mmdb') as reader:
+    >>>
+    >>>     reader.get('152.216.7.110')
+    {'country': ... }
+    >>>
+    >>>     reader.get_with_prefix_len('152.216.7.110')
+    ({'country': ... }, 24)
+
+Exceptions
+----------
+
+The module will return an ``InvalidDatabaseError`` if the database is corrupt
+or otherwise invalid. A ``ValueError`` will be thrown if you look up an
+invalid IP address or an IPv6 address in an IPv4 database.
+
+Requirements
+------------
+
+This code requires Python 3.7+. Older versions are not supported. The C
+extension requires CPython.
+
+Versioning
+----------
+
+The MaxMind DB Python module uses `Semantic Versioning <https://semver.org/>`_.
+
+Support
+-------
+
+Please report all issues with this code using the `GitHub issue tracker
+<https://github.com/maxmind/MaxMind-DB-Reader-python/issues>`_
+
+If you are having an issue with a MaxMind service that is not specific to this
+API, please contact `MaxMind support <https://www.maxmind.com/en/support>`_ for
+assistance.
+
+
```

### Comparing `maxminddb-2.2.0/README.rst` & `maxminddb-2.3.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 The module will return an ``InvalidDatabaseError`` if the database is corrupt
 or otherwise invalid. A ``ValueError`` will be thrown if you look up an
 invalid IP address or an IPv6 address in an IPv4 database.
 
 Requirements
 ------------
 
-This code requires Python 3.6+. Older versions are not supported. The C
+This code requires Python 3.7+. Older versions are not supported. The C
 extension requires CPython.
 
 Versioning
 ----------
 
 The MaxMind DB Python module uses `Semantic Versioning <https://semver.org/>`_.
```

### Comparing `maxminddb-2.2.0/docs/html/_sources/index.rst.txt` & `maxminddb-2.3.0/docs/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/docs/html/_static/basic.css` & `maxminddb-2.3.0/docs/html/_static/basic.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * basic.css
  * ~~~~~~~~~
  *
  * Sphinx stylesheet -- basic theme.
  *
- * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 /* -- main layout ----------------------------------------------------------- */
 
 div.clearer {
@@ -727,16 +727,17 @@
 
 .classifier {
     font-style: oblique;
 }
 
 .classifier:before {
     font-style: normal;
-    margin: 0.5em;
+    margin: 0 0.5em;
     content: ":";
+    display: inline-block;
 }
 
 abbr, acronym {
     border-bottom: dotted 1px;
     cursor: help;
 }
 
@@ -752,14 +753,15 @@
 }
 
 span.pre {
     -moz-hyphens: none;
     -ms-hyphens: none;
     -webkit-hyphens: none;
     hyphens: none;
+    white-space: nowrap;
 }
 
 div[class*="highlight-"] {
     margin: 1em 0;
 }
 
 td.linenos pre {
```

### Comparing `maxminddb-2.2.0/docs/html/_static/doctools.js` & `maxminddb-2.3.0/docs/html/_static/doctools.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * doctools.js
  * ~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for all documentation.
  *
- * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 /**
  * select a different prefix for underscore
  */
@@ -149,17 +149,15 @@
  */
 var Documentation = {
 
     init: function() {
         this.fixFirefoxAnchorBug();
         this.highlightSearchWords();
         this.initIndexTable();
-        if (DOCUMENTATION_OPTIONS.NAVIGATION_WITH_KEYS) {
-            this.initOnKeyListeners();
-        }
+        this.initOnKeyListeners();
     },
 
     /**
      * i18n support
      */
     TRANSLATIONS: {},
     PLURAL_EXPR: function(n) {
@@ -261,14 +259,24 @@
 
     /**
      * helper function to hide the search marks again
      */
     hideSearchWords: function() {
         $('#searchbox .highlight-link').fadeOut(300);
         $('span.highlighted').removeClass('highlighted');
+        var url = new URL(window.location);
+        url.searchParams.delete('highlight');
+        window.history.replaceState({}, '', url);
+    },
+
+    /**
+     * helper function to focus on search bar
+     */
+    focusSearchBar: function() {
+        $('input[name=q]').first().focus();
     },
 
     /**
      * make the url absolute
      */
     makeURL: function(relativeURL) {
         return DOCUMENTATION_OPTIONS.URL_ROOT + '/' + relativeURL;
@@ -285,35 +293,62 @@
                 parts.pop();
         });
         var url = parts.join('/');
         return path.substring(url.lastIndexOf('/') + 1, path.length - 1);
     },
 
     initOnKeyListeners: function() {
+        // only install a listener if it is really needed
+        if (!DOCUMENTATION_OPTIONS.NAVIGATION_WITH_KEYS &&
+            !DOCUMENTATION_OPTIONS.ENABLE_SEARCH_SHORTCUTS)
+            return;
+
         $(document).keydown(function(event) {
             var activeElementType = document.activeElement.tagName;
             // don't navigate when in search box, textarea, dropdown or button
             if (activeElementType !== 'TEXTAREA' && activeElementType !== 'INPUT' && activeElementType !== 'SELECT' &&
-                activeElementType !== 'BUTTON' && !event.altKey && !event.ctrlKey && !event.metaKey &&
-                !event.shiftKey) {
-                switch (event.keyCode) {
-                    case 37: // left
-                        var prevHref = $('link[rel="prev"]').prop('href');
-                        if (prevHref) {
-                            window.location.href = prevHref;
-                            return false;
-                        }
-                        break;
-                    case 39: // right
-                        var nextHref = $('link[rel="next"]').prop('href');
-                        if (nextHref) {
-                            window.location.href = nextHref;
+                activeElementType !== 'BUTTON') {
+                if (event.altKey || event.ctrlKey || event.metaKey)
+                    return;
+
+                if (!event.shiftKey) {
+                    switch (event.key) {
+                        case 'ArrowLeft':
+                            if (!DOCUMENTATION_OPTIONS.NAVIGATION_WITH_KEYS)
+                                break;
+                            var prevHref = $('link[rel="prev"]').prop('href');
+                            if (prevHref) {
+                                window.location.href = prevHref;
+                                return false;
+                            }
+                            break;
+                        case 'ArrowRight':
+                            if (!DOCUMENTATION_OPTIONS.NAVIGATION_WITH_KEYS)
+                                break;
+                            var nextHref = $('link[rel="next"]').prop('href');
+                            if (nextHref) {
+                                window.location.href = nextHref;
+                                return false;
+                            }
+                            break;
+                        case 'Escape':
+                            if (!DOCUMENTATION_OPTIONS.ENABLE_SEARCH_SHORTCUTS)
+                                break;
+                            Documentation.hideSearchWords();
                             return false;
-                        }
-                        break;
+                    }
+                }
+
+                // some keyboard layouts may need Shift to get /
+                switch (event.key) {
+                    case '/':
+                        if (!DOCUMENTATION_OPTIONS.ENABLE_SEARCH_SHORTCUTS)
+                            break;
+                        Documentation.focusSearchBar();
+                        return false;
                 }
             }
         });
     }
 };
 
 // quick alias for translations
```

### Comparing `maxminddb-2.2.0/docs/html/_static/jquery-3.5.1.js` & `maxminddb-2.3.0/docs/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/docs/html/_static/jquery.js` & `maxminddb-2.3.0/docs/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/docs/html/_static/language_data.js` & `maxminddb-2.3.0/docs/html/_static/language_data.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 /*
  * language_data.js
  * ~~~~~~~~~~~~~~~~
  *
  * This script contains the language-specific data used by searchtools.js,
  * namely the list of stopwords, stemmer, scorer and splitter.
  *
- * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 var stopwords = ["a", "and", "are", "as", "at", "be", "but", "by", "for", "if", "in", "into", "is", "it", "near", "no", "not", "of", "on", "or", "such", "that", "the", "their", "then", "there", "these", "they", "this", "to", "was", "will", "with"];
```

### Comparing `maxminddb-2.2.0/docs/html/_static/pygments.css` & `maxminddb-2.3.0/docs/html/_static/pygments.css`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-pre { line-height: 125%; margin: 0; }
-td.linenos pre { color: #000000; background-color: #f0f0f0; padding: 0 5px 0 5px; }
-span.linenos { color: #000000; background-color: #f0f0f0; padding: 0 5px 0 5px; }
-td.linenos pre.special { color: #000000; background-color: #ffffc0; padding: 0 5px 0 5px; }
-span.linenos.special { color: #000000; background-color: #ffffc0; padding: 0 5px 0 5px; }
+pre { line-height: 125%; }
+td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
+span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
+td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
+span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 .highlight .hll { background-color: #ffffcc }
 .highlight { background: #eeffcc; }
 .highlight .c { color: #408090; font-style: italic } /* Comment */
 .highlight .err { border: 1px solid #FF0000 } /* Error */
 .highlight .k { color: #007020; font-weight: bold } /* Keyword */
 .highlight .o { color: #666666 } /* Operator */
 .highlight .ch { color: #408090; font-style: italic } /* Comment.Hashbang */
```

### Comparing `maxminddb-2.2.0/docs/html/_static/searchtools.js` & `maxminddb-2.3.0/docs/html/_static/searchtools.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * searchtools.js
  * ~~~~~~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
- * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 if (!Scorer) {
     /**
      * Simple result scoring code.
@@ -176,18 +176,14 @@
 
             if ($u.indexOf(stopwords, tmp[i].toLowerCase()) != -1 || tmp[i] === "") {
                 // skip this "word"
                 continue;
             }
             // stem the word
             var word = stemmer.stemWord(tmp[i].toLowerCase());
-            // prevent stemmer from cutting word smaller than two chars
-            if (word.length < 3 && tmp[i].length >= 3) {
-                word = tmp[i];
-            }
             var toAppend;
             // select the correct list
             if (word[0] == '-') {
                 toAppend = excluded;
                 word = word.substr(1);
             } else {
                 toAppend = searchterms;
@@ -280,15 +276,15 @@
                     highlightstring + item[2]).html(item[1]));
                 if (item[3]) {
                     listItem.append($('<span> (' + item[3] + ')</span>'));
                     Search.output.append(listItem);
                     setTimeout(function() {
                         displayNextItem();
                     }, 5);
-                } else if (DOCUMENTATION_OPTIONS.HAS_SOURCE) {
+                } else if (DOCUMENTATION_OPTIONS.SHOW_SEARCH_SUMMARY) {
                     $.ajax({
                         url: requestUrl,
                         dataType: "text",
                         complete: function(jqxhr, textstatus) {
                             var data = jqxhr.responseText;
                             if (data !== '' && data !== undefined) {
                                 var summary = Search.makeSearchSummary(data, searchterms, hlterms);
@@ -299,15 +295,15 @@
                             Search.output.append(listItem);
                             setTimeout(function() {
                                 displayNextItem();
                             }, 5);
                         }
                     });
                 } else {
-                    // no source available, just display title
+                    // just display title
                     Search.output.append(listItem);
                     setTimeout(function() {
                         displayNextItem();
                     }, 5);
                 }
             }
             // search finished, update title and status message
@@ -334,29 +330,30 @@
         var objnames = this._index.objnames;
         var titles = this._index.titles;
 
         var i;
         var results = [];
 
         for (var prefix in objects) {
-            for (var name in objects[prefix]) {
+            for (var iMatch = 0; iMatch != objects[prefix].length; ++iMatch) {
+                var match = objects[prefix][iMatch];
+                var name = match[4];
                 var fullname = (prefix ? prefix + '.' : '') + name;
                 var fullnameLower = fullname.toLowerCase()
                 if (fullnameLower.indexOf(object) > -1) {
                     var score = 0;
                     var parts = fullnameLower.split('.');
                     // check for different match types: exact matches of full name or
                     // "last name" (i.e. last dotted part)
                     if (fullnameLower == object || parts[parts.length - 1] == object) {
                         score += Scorer.objNameMatch;
                         // matches in last name
                     } else if (parts[parts.length - 1].indexOf(object) > -1) {
                         score += Scorer.objPartialMatch;
                     }
-                    var match = objects[prefix][name];
                     var objname = objnames[match[1]][2];
                     var title = titles[match[0]];
                     // If more than one term searched for, we require other words to be
                     // found in the name/title/description
                     if (otherterms.length > 0) {
                         var haystack = (prefix + ' ' + name + ' ' +
                             objname + ' ' + title).toLowerCase();
```

### Comparing `maxminddb-2.2.0/docs/html/_static/sphinxdoc.css` & `maxminddb-2.3.0/docs/html/_static/sphinxdoc.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /*
  * sphinxdoc.css_t
  * ~~~~~~~~~~~~~~~
  *
  * Sphinx stylesheet -- sphinxdoc theme.  Originally created by
  * Armin Ronacher for Werkzeug.
  *
- * :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 @import url("basic.css");
 
 /* -- page layout ----------------------------------------------------------- */
```

### Comparing `maxminddb-2.2.0/docs/html/_static/underscore-1.13.1.js` & `maxminddb-2.3.0/docs/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/docs/html/_static/underscore.js` & `maxminddb-2.3.0/docs/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/docs/html/genindex.html` & `maxminddb-2.3.0/docs/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; maxminddb 2.2.0 documentation</title>
+    <title>Index &#8212; maxminddb 2.3.0 documentation</title>
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
-        <li class="nav-item nav-item-0"><a href="index.html">maxminddb 2.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">maxminddb 2.3.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -248,17 +248,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">maxminddb 2.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">maxminddb 2.3.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2013-2021, MaxMind, Inc..
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.2.0.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.5.0.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * maxminddb_2.2.0_documentation »
+    * maxminddb_2.3.0_documentation »
     * Index
 ****** Index ******
 B | C | D | G | I | L | M | N | O | R | S
 ***** B *****
     * binary_format_major_version_     * binary_format_minor_version_
       (maxminddb.reader.Metadata         (maxminddb.reader.Metadata_attribute)
       attribute)                       * build_epoch_
@@ -53,10 +53,10 @@
 ***** S *****
     * search_tree_size_(maxminddb.reader.Metadata_property)
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * maxminddb_2.2.0_documentation »
+    * maxminddb_2.3.0_documentation »
     * Index
-© Copyright 2013-2021, MaxMind, Inc.. Created using Sphinx 4.2.0.
+© Copyright 2013-2021, MaxMind, Inc.. Created using Sphinx 4.5.0.
```

### Comparing `maxminddb-2.2.0/docs/html/index.html` & `maxminddb-2.3.0/docs/html/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>MaxMind DB Python Module &#8212; maxminddb 2.2.0 documentation</title>
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+
+    <title>MaxMind DB Python Module &#8212; maxminddb 2.3.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinxdoc.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -20,36 +21,36 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">maxminddb 2.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">maxminddb 2.3.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">MaxMind DB Python Module</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
   <div class="toctree-wrapper compound">
 </div>
-<div class="section" id="maxmind-db-python-module">
+<section id="maxmind-db-python-module">
 <h1>MaxMind DB Python Module<a class="headerlink" href="#maxmind-db-python-module" title="Permalink to this headline">¶</a></h1>
-<div class="section" id="description">
+<section id="description">
 <h2>Description<a class="headerlink" href="#description" title="Permalink to this headline">¶</a></h2>
 <p>This is a Python module for reading MaxMind DB files. The module includes both
 a pure Python reader and an optional C extension.</p>
 <p>MaxMind DB is a binary file format that stores data indexed by IP address
 subnets (IPv4 or IPv6).</p>
-</div>
-<div class="section" id="installation">
+</section>
+<section id="installation">
 <h2>Installation<a class="headerlink" href="#installation" title="Permalink to this headline">¶</a></h2>
 <p>If you want to use the C extension, you must first install <a class="reference external" href="https://github.com/maxmind/libmaxminddb">libmaxminddb</a> C library installed before
 installing this extension. If the library is not available, the module will
 fall-back to a pure Python implementation. Note that when installing the C
 library from a package, you may be required to install additonal packages
 containing build requirements such as <cite>libmaxminddb-dev</cite> on Debian.</p>
 <p>To install maxminddb, type:</p>
@@ -57,16 +58,16 @@
 </pre></div>
 </div>
 <p>If you are not able to use pip, you may also use easy_install from the
 source directory:</p>
 <div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$ easy_install .
 </pre></div>
 </div>
-</div>
-<div class="section" id="usage">
+</section>
+<section id="usage">
 <h2>Usage<a class="headerlink" href="#usage" title="Permalink to this headline">¶</a></h2>
 <p>To use this module, you must first download or create a MaxMind DB file. We
 provide <a class="reference external" href="https://dev.maxmind.com/geoip/geolocate-an-ip/databases?lang=en">free GeoLite2 databases</a>. These
 files must be decompressed with <code class="docutils literal notranslate"><span class="pre">gunzip</span></code>.</p>
 <p>After you have obtained a database and imported the module, call
 <code class="docutils literal notranslate"><span class="pre">open_database</span></code> with a path, or file descriptor (in the case of <code class="docutils literal notranslate"><span class="pre">MODE_FD</span></code>),
 to the database as the first argument. Optionally, you may pass a mode as the
@@ -87,84 +88,84 @@
 address, use the <code class="docutils literal notranslate"><span class="pre">get</span></code> method on this object. The method will return the
 corresponding values for the IP address from the database (e.g., a dictionary
 for GeoIP2/GeoLite2 databases). If the database does not contain a record for
 that IP address, the method will return <code class="docutils literal notranslate"><span class="pre">None</span></code>.</p>
 <p>If you wish to also retrieve the prefix length for the record, use the
 <code class="docutils literal notranslate"><span class="pre">get_with_prefix_len</span></code> method. This returns a tuple containing the record
 followed by the network prefix length associated with the record.</p>
-</div>
-<div class="section" id="example">
+</section>
+<section id="example">
 <h2>Example<a class="headerlink" href="#example" title="Permalink to this headline">¶</a></h2>
 <div class="highlight-pycon notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">maxminddb</span>
 <span class="go">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="k">with</span> <span class="n">maxminddb</span><span class="o">.</span><span class="n">open_database</span><span class="p">(</span><span class="s1">&#39;GeoLite2-City.mmdb&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">reader</span><span class="p">:</span>
 <span class="go">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">reader</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s1">&#39;152.216.7.110&#39;</span><span class="p">)</span>
 <span class="go">{&#39;country&#39;: ... }</span>
 <span class="go">&gt;&gt;&gt;</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">reader</span><span class="o">.</span><span class="n">get_with_prefix_len</span><span class="p">(</span><span class="s1">&#39;152.216.7.110&#39;</span><span class="p">)</span>
 <span class="go">({&#39;country&#39;: ... }, 24)</span>
 </pre></div>
 </div>
-</div>
-<div class="section" id="exceptions">
+</section>
+<section id="exceptions">
 <h2>Exceptions<a class="headerlink" href="#exceptions" title="Permalink to this headline">¶</a></h2>
 <p>The module will return an <code class="docutils literal notranslate"><span class="pre">InvalidDatabaseError</span></code> if the database is corrupt
 or otherwise invalid. A <code class="docutils literal notranslate"><span class="pre">ValueError</span></code> will be thrown if you look up an
 invalid IP address or an IPv6 address in an IPv4 database.</p>
-</div>
-<div class="section" id="requirements">
+</section>
+<section id="requirements">
 <h2>Requirements<a class="headerlink" href="#requirements" title="Permalink to this headline">¶</a></h2>
-<p>This code requires Python 3.6+. Older versions are not supported. The C
+<p>This code requires Python 3.7+. Older versions are not supported. The C
 extension requires CPython.</p>
-</div>
-<div class="section" id="versioning">
+</section>
+<section id="versioning">
 <h2>Versioning<a class="headerlink" href="#versioning" title="Permalink to this headline">¶</a></h2>
 <p>The MaxMind DB Python module uses <a class="reference external" href="https://semver.org/">Semantic Versioning</a>.</p>
-</div>
-<div class="section" id="support">
+</section>
+<section id="support">
 <h2>Support<a class="headerlink" href="#support" title="Permalink to this headline">¶</a></h2>
 <p>Please report all issues with this code using the <a class="reference external" href="https://github.com/maxmind/MaxMind-DB-Reader-python/issues">GitHub issue tracker</a></p>
 <p>If you are having an issue with a MaxMind service that is not specific to this
 API, please contact <a class="reference external" href="https://www.maxmind.com/en/support">MaxMind support</a> for
 assistance.</p>
-</div>
-</div>
-<div class="section" id="module-maxminddb">
+</section>
+</section>
+<section id="module-maxminddb">
 <span id="modules"></span><h1>Modules<a class="headerlink" href="#module-maxminddb" title="Permalink to this headline">¶</a></h1>
 <dl class="py exception">
 <dt class="sig sig-object py" id="maxminddb.InvalidDatabaseError">
-<em class="property"><span class="pre">exception</span> </em><span class="sig-prename descclassname"><span class="pre">maxminddb.</span></span><span class="sig-name descname"><span class="pre">InvalidDatabaseError</span></span><a class="headerlink" href="#maxminddb.InvalidDatabaseError" title="Permalink to this definition">¶</a></dt>
-<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/exceptions.html#RuntimeError" title="(in Python v3.9)"><code class="xref py py-class docutils literal notranslate"><span class="pre">RuntimeError</span></code></a></p>
+<em class="property"><span class="pre">exception</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">maxminddb.</span></span><span class="sig-name descname"><span class="pre">InvalidDatabaseError</span></span><a class="headerlink" href="#maxminddb.InvalidDatabaseError" title="Permalink to this definition">¶</a></dt>
+<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/exceptions.html#RuntimeError" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">RuntimeError</span></code></a></p>
 <p>This error is thrown when unexpected data is found in the database.</p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="maxminddb.Reader">
-<em class="property"><span class="pre">class</span> </em><span class="sig-prename descclassname"><span class="pre">maxminddb.</span></span><span class="sig-name descname"><span class="pre">Reader</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">database</span></span><span class="p"><span class="pre">:</span></span> <span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">AnyStr</span><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/os.html#os.PathLike" title="(in Python v3.9)"><span class="pre">os.PathLike</span></a><span class="p"><span class="pre">,</span> </span><span class="pre">IO</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span> <span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a></span> <span class="o"><span class="pre">=</span></span> <span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#maxminddb.Reader" title="Permalink to this definition">¶</a></dt>
-<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.9)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">maxminddb.</span></span><span class="sig-name descname"><span class="pre">Reader</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">database</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.AnyStr" title="(in Python v3.11)"><span class="pre">AnyStr</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/os.html#os.PathLike" title="(in Python v3.11)"><span class="pre">os.PathLike</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.IO" title="(in Python v3.11)"><span class="pre">IO</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#maxminddb.Reader" title="Permalink to this definition">¶</a></dt>
+<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
 <p>Instances of this class provide a reader for the MaxMind DB format. IP
 addresses can be looked up using the <code class="docutils literal notranslate"><span class="pre">get</span></code> method.</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="maxminddb.Reader.close">
-<span class="sig-name descname"><span class="pre">close</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.9)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#maxminddb.Reader.close" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">close</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#maxminddb.Reader.close" title="Permalink to this definition">¶</a></dt>
 <dd><p>Closes the MaxMind DB file and returns the resources to the system</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="maxminddb.Reader.get">
-<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span> <span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.9)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.9)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.9)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">AnyStr</span><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.9)"><span class="pre">bool</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.9)"><span class="pre">float</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span> </span><span class="pre">RecordList</span><span class="p"><span class="pre">,</span> </span><span class="pre">RecordDict</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#maxminddb.Reader.get" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.AnyStr" title="(in Python v3.11)"><span class="pre">AnyStr</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">RecordList</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">RecordDict</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#maxminddb.Reader.get" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return the record for the ip_address in the MaxMind DB</p>
 <p>Arguments:
 ip_address – an IP address in the standard string notation</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="maxminddb.Reader.get_with_prefix_len">
-<span class="sig-name descname"><span class="pre">get_with_prefix_len</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span> <span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.9)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.9)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.9)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">AnyStr</span><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.9)"><span class="pre">bool</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.9)"><span class="pre">float</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span> </span><span class="pre">RecordList</span><span class="p"><span class="pre">,</span> </span><span class="pre">RecordDict</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#maxminddb.Reader.get_with_prefix_len" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_with_prefix_len</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Tuple" title="(in Python v3.11)"><span class="pre">Tuple</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.AnyStr" title="(in Python v3.11)"><span class="pre">AnyStr</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">RecordList</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">RecordDict</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#maxminddb.Reader.get_with_prefix_len" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return a tuple with the record and the associated prefix length</p>
 <p>Arguments:
 ip_address – an IP address in the standard string notation</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="maxminddb.Reader.metadata">
@@ -172,15 +173,15 @@
 <dd><p>Return the metadata associated with the MaxMind DB file</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="maxminddb.open_database">
-<span class="sig-prename descclassname"><span class="pre">maxminddb.</span></span><span class="sig-name descname"><span class="pre">open_database</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">database</span></span><span class="p"><span class="pre">:</span></span> <span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">AnyStr</span><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/os.html#os.PathLike" title="(in Python v3.9)"><span class="pre">os.PathLike</span></a><span class="p"><span class="pre">,</span> </span><span class="pre">IO</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span> <span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a></span> <span class="o"><span class="pre">=</span></span> <span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#maxminddb.reader.Reader" title="maxminddb.reader.Reader"><span class="pre">maxminddb.reader.Reader</span></a></span></span><a class="headerlink" href="#maxminddb.open_database" title="Permalink to this definition">¶</a></dt>
+<span class="sig-prename descclassname"><span class="pre">maxminddb.</span></span><span class="sig-name descname"><span class="pre">open_database</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">database</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.AnyStr" title="(in Python v3.11)"><span class="pre">AnyStr</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/os.html#os.PathLike" title="(in Python v3.11)"><span class="pre">os.PathLike</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.IO" title="(in Python v3.11)"><span class="pre">IO</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#maxminddb.reader.Reader" title="maxminddb.reader.Reader"><span class="pre">maxminddb.reader.Reader</span></a></span></span><a class="headerlink" href="#maxminddb.open_database" title="Permalink to this definition">¶</a></dt>
 <dd><p>Open a MaxMind DB database</p>
 <dl class="simple">
 <dt>Arguments:</dt><dd><dl class="simple">
 <dt>database – A path to a valid MaxMind DB file such as a GeoIP2 database</dt><dd><p>file, or a file descriptor in the case of MODE_FD.</p>
 </dd>
 <dt>mode – mode to open the database with. Valid mode are:</dt><dd><ul class="simple">
 <li><p>MODE_MMAP_EXT - use the C extension with memory map.</p></li>
@@ -200,199 +201,199 @@
 </ul>
 </dd>
 </dl>
 </dd>
 </dl>
 </dd></dl>
 
-<span class="target" id="module-maxminddb.errors"></span><div class="section" id="maxminddb-errors">
+<span class="target" id="module-maxminddb.errors"></span><section id="maxminddb-errors">
 <h2>maxminddb.errors<a class="headerlink" href="#maxminddb-errors" title="Permalink to this headline">¶</a></h2>
 <p>This module contains custom errors for the MaxMind DB reader</p>
 <dl class="py exception">
 <dt class="sig sig-object py" id="maxminddb.errors.InvalidDatabaseError">
-<em class="property"><span class="pre">exception</span> </em><span class="sig-prename descclassname"><span class="pre">maxminddb.errors.</span></span><span class="sig-name descname"><span class="pre">InvalidDatabaseError</span></span><a class="headerlink" href="#maxminddb.errors.InvalidDatabaseError" title="Permalink to this definition">¶</a></dt>
-<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/exceptions.html#RuntimeError" title="(in Python v3.9)"><code class="xref py py-class docutils literal notranslate"><span class="pre">RuntimeError</span></code></a></p>
+<em class="property"><span class="pre">exception</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">maxminddb.errors.</span></span><span class="sig-name descname"><span class="pre">InvalidDatabaseError</span></span><a class="headerlink" href="#maxminddb.errors.InvalidDatabaseError" title="Permalink to this definition">¶</a></dt>
+<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/exceptions.html#RuntimeError" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">RuntimeError</span></code></a></p>
 <p>This error is thrown when unexpected data is found in the database.</p>
 </dd></dl>
 
-</div>
-<span class="target" id="module-maxminddb.reader"></span><div class="section" id="maxminddb-reader">
+</section>
+<span class="target" id="module-maxminddb.reader"></span><section id="maxminddb-reader">
 <h2>maxminddb.reader<a class="headerlink" href="#maxminddb-reader" title="Permalink to this headline">¶</a></h2>
 <p>This module contains the pure Python database reader and related classes.</p>
 <dl class="py class">
 <dt class="sig sig-object py" id="maxminddb.reader.Metadata">
-<em class="property"><span class="pre">class</span> </em><span class="sig-prename descclassname"><span class="pre">maxminddb.reader.</span></span><span class="sig-name descname"><span class="pre">Metadata</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#maxminddb.reader.Metadata" title="Permalink to this definition">¶</a></dt>
-<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.9)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">maxminddb.reader.</span></span><span class="sig-name descname"><span class="pre">Metadata</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kwargs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#maxminddb.reader.Metadata" title="Permalink to this definition">¶</a></dt>
+<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
 <p>Metadata for the MaxMind DB reader</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="maxminddb.reader.Metadata.binary_format_major_version">
 <span class="sig-name descname"><span class="pre">binary_format_major_version</span></span><a class="headerlink" href="#maxminddb.reader.Metadata.binary_format_major_version" title="Permalink to this definition">¶</a></dt>
 <dd><p>The major version number of the binary format used when creating the
 database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="maxminddb.reader.Metadata.binary_format_minor_version">
 <span class="sig-name descname"><span class="pre">binary_format_minor_version</span></span><a class="headerlink" href="#maxminddb.reader.Metadata.binary_format_minor_version" title="Permalink to this definition">¶</a></dt>
 <dd><p>The minor version number of the binary format used when creating the
 database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="maxminddb.reader.Metadata.build_epoch">
 <span class="sig-name descname"><span class="pre">build_epoch</span></span><a class="headerlink" href="#maxminddb.reader.Metadata.build_epoch" title="Permalink to this definition">¶</a></dt>
 <dd><p>The Unix epoch for the build time of the database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="maxminddb.reader.Metadata.database_type">
 <span class="sig-name descname"><span class="pre">database_type</span></span><a class="headerlink" href="#maxminddb.reader.Metadata.database_type" title="Permalink to this definition">¶</a></dt>
 <dd><p>A string identifying the database type, e.g., “GeoIP2-City”.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.9)">str</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="maxminddb.reader.Metadata.description">
 <span class="sig-name descname"><span class="pre">description</span></span><a class="headerlink" href="#maxminddb.reader.Metadata.description" title="Permalink to this definition">¶</a></dt>
 <dd><p>A map from locales to text descriptions of the database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.9)">dict</a>(<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.9)">str</a>, <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.9)">str</a>)</p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.11)">dict</a>(<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a>, <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a>)</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="maxminddb.reader.Metadata.ip_version">
 <span class="sig-name descname"><span class="pre">ip_version</span></span><a class="headerlink" href="#maxminddb.reader.Metadata.ip_version" title="Permalink to this definition">¶</a></dt>
 <dd><p>The IP version of the data in a database. A value of “4” means the
 database only supports IPv4. A database with a value of “6” may support
 both IPv4 and IPv6 lookups.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="maxminddb.reader.Metadata.languages">
 <span class="sig-name descname"><span class="pre">languages</span></span><a class="headerlink" href="#maxminddb.reader.Metadata.languages" title="Permalink to this definition">¶</a></dt>
 <dd><p>A list of locale codes supported by the databse.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#list" title="(in Python v3.9)">list</a>(<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.9)">str</a>)</p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#list" title="(in Python v3.11)">list</a>(<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a>)</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="maxminddb.reader.Metadata.node_count">
 <span class="sig-name descname"><span class="pre">node_count</span></span><a class="headerlink" href="#maxminddb.reader.Metadata.node_count" title="Permalink to this definition">¶</a></dt>
 <dd><p>The number of nodes in the database.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="maxminddb.reader.Metadata.record_size">
 <span class="sig-name descname"><span class="pre">record_size</span></span><a class="headerlink" href="#maxminddb.reader.Metadata.record_size" title="Permalink to this definition">¶</a></dt>
 <dd><p>The bit size of a record in the search tree.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="maxminddb.reader.Metadata.node_byte_size">
-<em class="property"><span class="pre">property</span> </em><span class="sig-name descname"><span class="pre">node_byte_size</span></span><em class="property"><span class="pre">:</span> <a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a></em><a class="headerlink" href="#maxminddb.reader.Metadata.node_byte_size" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">node_byte_size</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></em><a class="headerlink" href="#maxminddb.reader.Metadata.node_byte_size" title="Permalink to this definition">¶</a></dt>
 <dd><p>The size of a node in bytes</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="maxminddb.reader.Metadata.search_tree_size">
-<em class="property"><span class="pre">property</span> </em><span class="sig-name descname"><span class="pre">search_tree_size</span></span><em class="property"><span class="pre">:</span> <a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a></em><a class="headerlink" href="#maxminddb.reader.Metadata.search_tree_size" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">search_tree_size</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></em><a class="headerlink" href="#maxminddb.reader.Metadata.search_tree_size" title="Permalink to this definition">¶</a></dt>
 <dd><p>The size of the search tree</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type</dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)">int</a></p>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="maxminddb.reader.Reader">
-<em class="property"><span class="pre">class</span> </em><span class="sig-prename descclassname"><span class="pre">maxminddb.reader.</span></span><span class="sig-name descname"><span class="pre">Reader</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">database</span></span><span class="p"><span class="pre">:</span></span> <span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">AnyStr</span><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/os.html#os.PathLike" title="(in Python v3.9)"><span class="pre">os.PathLike</span></a><span class="p"><span class="pre">,</span> </span><span class="pre">IO</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span> <span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a></span> <span class="o"><span class="pre">=</span></span> <span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#maxminddb.reader.Reader" title="Permalink to this definition">¶</a></dt>
-<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.9)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">maxminddb.reader.</span></span><span class="sig-name descname"><span class="pre">Reader</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">database</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.AnyStr" title="(in Python v3.11)"><span class="pre">AnyStr</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/os.html#os.PathLike" title="(in Python v3.11)"><span class="pre">os.PathLike</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.IO" title="(in Python v3.11)"><span class="pre">IO</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#maxminddb.reader.Reader" title="Permalink to this definition">¶</a></dt>
+<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
 <p>Instances of this class provide a reader for the MaxMind DB format. IP
 addresses can be looked up using the <code class="docutils literal notranslate"><span class="pre">get</span></code> method.</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="maxminddb.reader.Reader.close">
-<span class="sig-name descname"><span class="pre">close</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.9)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#maxminddb.reader.Reader.close" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">close</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#maxminddb.reader.Reader.close" title="Permalink to this definition">¶</a></dt>
 <dd><p>Closes the MaxMind DB file and returns the resources to the system</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="maxminddb.reader.Reader.get">
-<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span> <span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.9)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.9)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.9)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">AnyStr</span><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.9)"><span class="pre">bool</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.9)"><span class="pre">float</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span> </span><span class="pre">RecordList</span><span class="p"><span class="pre">,</span> </span><span class="pre">RecordDict</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#maxminddb.reader.Reader.get" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.AnyStr" title="(in Python v3.11)"><span class="pre">AnyStr</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">RecordList</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">RecordDict</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#maxminddb.reader.Reader.get" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return the record for the ip_address in the MaxMind DB</p>
 <p>Arguments:
 ip_address – an IP address in the standard string notation</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="maxminddb.reader.Reader.get_with_prefix_len">
-<span class="sig-name descname"><span class="pre">get_with_prefix_len</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span> <span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.9)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.9)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.9)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">AnyStr</span><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.9)"><span class="pre">bool</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.9)"><span class="pre">float</span></a><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span> </span><span class="pre">RecordList</span><span class="p"><span class="pre">,</span> </span><span class="pre">RecordDict</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.9)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#maxminddb.reader.Reader.get_with_prefix_len" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_with_prefix_len</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ip_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv6Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv6Address</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/ipaddress.html#ipaddress.IPv4Address" title="(in Python v3.11)"><span class="pre">ipaddress.IPv4Address</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Tuple" title="(in Python v3.11)"><span class="pre">Tuple</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Union" title="(in Python v3.11)"><span class="pre">Union</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.AnyStr" title="(in Python v3.11)"><span class="pre">AnyStr</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">RecordList</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">RecordDict</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#maxminddb.reader.Reader.get_with_prefix_len" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return a tuple with the record and the associated prefix length</p>
 <p>Arguments:
 ip_address – an IP address in the standard string notation</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="maxminddb.reader.Reader.metadata">
 <span class="sig-name descname"><span class="pre">metadata</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#maxminddb.reader.Metadata" title="maxminddb.reader.Metadata"><span class="pre">maxminddb.reader.Metadata</span></a></span></span><a class="headerlink" href="#maxminddb.reader.Reader.metadata" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return the metadata associated with the MaxMind DB file</p>
 </dd></dl>
 
 </dd></dl>
 
-</div>
-</div>
-<div class="section" id="indices-and-tables">
+</section>
+</section>
+<section id="indices-and-tables">
 <h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this headline">¶</a></h1>
 <ul class="simple">
 <li><p><a class="reference internal" href="genindex.html"><span class="std std-ref">Index</span></a></p></li>
 <li><p><a class="reference internal" href="py-modindex.html"><span class="std std-ref">Module Index</span></a></p></li>
 <li><p><a class="reference internal" href="search.html"><span class="std std-ref">Search Page</span></a></p></li>
 </ul>
 <dl class="field-list simple">
@@ -401,25 +402,26 @@
 <li><p>2013-2021 by MaxMind, Inc.</p></li>
 </ol>
 </dd>
 <dt class="field-even">license</dt>
 <dd class="field-even"><p>Apache License, Version 2.0</p>
 </dd>
 </dl>
-</div>
+</section>
 
 
             <div class="clearer"></div>
           </div>
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
-  <h3><a href="#">Table of Contents</a></h3>
-  <ul>
+  <div>
+    <h3><a href="#">Table of Contents</a></h3>
+    <ul>
 <li><a class="reference internal" href="#">MaxMind DB Python Module</a><ul>
 <li><a class="reference internal" href="#description">Description</a></li>
 <li><a class="reference internal" href="#installation">Installation</a></li>
 <li><a class="reference internal" href="#usage">Usage</a></li>
 <li><a class="reference internal" href="#example">Example</a></li>
 <li><a class="reference internal" href="#exceptions">Exceptions</a></li>
 <li><a class="reference internal" href="#requirements">Requirements</a></li>
@@ -431,14 +433,15 @@
 <li><a class="reference internal" href="#maxminddb-errors">maxminddb.errors</a></li>
 <li><a class="reference internal" href="#maxminddb-reader">maxminddb.reader</a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#indices-and-tables">Indices and tables</a></li>
 </ul>
 
+  </div>
   <div role="note" aria-label="source link">
     <h3>This Page</h3>
     <ul class="this-page-menu">
       <li><a href="_sources/index.rst.txt"
             rel="nofollow">Show Source</a></li>
     </ul>
    </div>
@@ -461,17 +464,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">maxminddb 2.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">maxminddb 2.3.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">MaxMind DB Python Module</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2013-2021, MaxMind, Inc..
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.2.0.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.5.0.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,34 +2,36 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * maxminddb_2.2.0_documentation »
+    * maxminddb_2.3.0_documentation »
     * MaxMind DB Python Module
 ****** MaxMind DB Python ModuleÂ¶ ******
 ***** DescriptionÂ¶ *****
 This is a Python module for reading MaxMind DB files. The module includes both
 a pure Python reader and an optional C extension.
 MaxMind DB is a binary file format that stores data indexed by IP address
 subnets (IPv4 or IPv6).
+
 ***** InstallationÂ¶ *****
 If you want to use the C extension, you must first install libmaxminddb C
 library installed before installing this extension. If the library is not
 available, the module will fall-back to a pure Python implementation. Note that
 when installing the C library from a package, you may be required to install
 additonal packages containing build requirements such aslibmaxminddb-devon
 Debian.
 To install maxminddb, type:
 $ pip install maxminddb
 If you are not able to use pip, you may also use easy_install from the source
 directory:
 $ easy_install .
+
 ***** UsageÂ¶ *****
 To use this module, you must first download or create a MaxMind DB file. We
 provide free_GeoLite2_databases. These files must be decompressed with gunzip.
 After you have obtained a database and imported the module, call open_database
 with a path, or file descriptor (in the case of MODE_FD), to the database as
 the first argument. Optionally, you may pass a mode as the second argument. The
 modes are exported from maxminddb. Valid modes are:
@@ -47,37 +49,43 @@
 use the get method on this object. The method will return the corresponding
 values for the IP address from the database (e.g., a dictionary for GeoIP2/
 GeoLite2 databases). If the database does not contain a record for that IP
 address, the method will return None.
 If you wish to also retrieve the prefix length for the record, use the
 get_with_prefix_len method. This returns a tuple containing the record followed
 by the network prefix length associated with the record.
+
 ***** ExampleÂ¶ *****
 >>> import maxminddb
 >>>
 >>> with maxminddb.open_database('GeoLite2-City.mmdb') as reader:
 >>>
 >>>     reader.get('152.216.7.110')
 {'country': ... }
 >>>
 >>>     reader.get_with_prefix_len('152.216.7.110')
 ({'country': ... }, 24)
+
 ***** ExceptionsÂ¶ *****
 The module will return an InvalidDatabaseError if the database is corrupt or
 otherwise invalid. A ValueError will be thrown if you look up an invalid IP
 address or an IPv6 address in an IPv4 database.
+
 ***** RequirementsÂ¶ *****
-This code requires Python 3.6+. Older versions are not supported. The C
+This code requires Python 3.7+. Older versions are not supported. The C
 extension requires CPython.
+
 ***** VersioningÂ¶ *****
 The MaxMind DB Python module uses Semantic_Versioning.
+
 ***** SupportÂ¶ *****
 Please report all issues with this code using the GitHub_issue_tracker
 If you are having an issue with a MaxMind service that is not specific to this
 API, please contact MaxMind_support for assistance.
+
 ****** ModulesÂ¶ ******
   exceptionmaxminddb.InvalidDatabaseErrorÂ¶
       Bases: RuntimeError
       This error is thrown when unexpected data is found in the database.
   classmaxminddb.Reader(database: Union[AnyStr, int, os.PathLike, IO], mode:
   int = 0)Â¶
       Bases: object
@@ -119,14 +127,15 @@
                           in that
                               order. Default mode.
 ***** maxminddb.errorsÂ¶ *****
 This module contains custom errors for the MaxMind DB reader
   exceptionmaxminddb.errors.InvalidDatabaseErrorÂ¶
       Bases: RuntimeError
       This error is thrown when unexpected data is found in the database.
+
 ***** maxminddb.readerÂ¶ *****
 This module contains the pure Python database reader and related classes.
   classmaxminddb.reader.Metadata(**kwargs)Â¶
       Bases: object
       Metadata for the MaxMind DB reader
         binary_format_major_versionÂ¶
             The major version number of the binary format used when creating
@@ -193,14 +202,15 @@
         ipaddress.IPv4Address]) &#x2192; Tuple[Optional[Union[AnyStr, bool,
         float, int, RecordList, RecordDict]], int]Â¶
             Return a tuple with the record and the associated prefix length
             Arguments: ip_address â an IP address in the standard string
             notation
         metadata() &#x2192; maxminddb.reader.MetadataÂ¶
             Return the metadata associated with the MaxMind DB file
+
 ****** Indices and tablesÂ¶ ******
     * Index
     * Module_Index
     * Search_Page
   copyright
          1. 2013-2021 by MaxMind, Inc.
   license
@@ -222,10 +232,10 @@
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * maxminddb_2.2.0_documentation »
+    * maxminddb_2.3.0_documentation »
     * MaxMind DB Python Module
-© Copyright 2013-2021, MaxMind, Inc.. Created using Sphinx 4.2.0.
+© Copyright 2013-2021, MaxMind, Inc.. Created using Sphinx 4.5.0.
```

### Comparing `maxminddb-2.2.0/docs/html/objects.inv` & `maxminddb-2.3.0/docs/html/objects.inv`

 * *Files 2% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: maxminddb
-# Version: 2.2.0
+# Version: 2.3.0
 # The remainder of this file is compressed using zlib.
 
 maxminddb py:module 0 index.html#module-$ -
 maxminddb.InvalidDatabaseError py:exception 1 index.html#$ -
 maxminddb.Reader py:class 1 index.html#$ -
 maxminddb.Reader.close py:method 1 index.html#$ -
 maxminddb.Reader.get py:method 1 index.html#$ -
```

### Comparing `maxminddb-2.2.0/docs/html/py-modindex.html` & `maxminddb-2.3.0/docs/html/py-modindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; maxminddb 2.2.0 documentation</title>
+    <title>Python Module Index &#8212; maxminddb 2.3.0 documentation</title>
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
-        <li class="nav-item nav-item-0"><a href="index.html">maxminddb 2.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">maxminddb 2.3.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -92,17 +92,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">maxminddb 2.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">maxminddb 2.3.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2013-2021, MaxMind, Inc..
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.2.0.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.5.0.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,24 +2,24 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * maxminddb_2.2.0_documentation »
+    * maxminddb_2.3.0_documentation »
     * Python Module Index
 ****** Python Module Index ******
 m
      
     m
 [-] maxminddb
         maxminddb.errors
         maxminddb.reader
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * maxminddb_2.2.0_documentation »
+    * maxminddb_2.3.0_documentation »
     * Python Module Index
-© Copyright 2013-2021, MaxMind, Inc.. Created using Sphinx 4.2.0.
+© Copyright 2013-2021, MaxMind, Inc.. Created using Sphinx 4.5.0.
```

### Comparing `maxminddb-2.2.0/docs/html/search.html` & `maxminddb-2.3.0/docs/html/search.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; maxminddb 2.2.0 documentation</title>
+    <title>Search &#8212; maxminddb 2.3.0 documentation</title>
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
-        <li class="nav-item nav-item-0"><a href="index.html">maxminddb 2.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">maxminddb 2.3.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -86,17 +86,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">maxminddb 2.2.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">maxminddb 2.3.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2013-2021, MaxMind, Inc..
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.2.0.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 4.5.0.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,19 +2,19 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * maxminddb_2.2.0_documentation »
+    * maxminddb_2.3.0_documentation »
     * Search
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
 **** Navigation ****
     * index
     * modules |
-    * maxminddb_2.2.0_documentation »
+    * maxminddb_2.3.0_documentation »
     * Search
-© Copyright 2013-2021, MaxMind, Inc.. Created using Sphinx 4.2.0.
+© Copyright 2013-2021, MaxMind, Inc.. Created using Sphinx 4.5.0.
```

### Comparing `maxminddb-2.2.0/docs/html/searchindex.js` & `maxminddb-2.3.0/docs/html/searchindex.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,67 +1,67 @@
 Search.setIndex({
     docnames: ["index"],
     envversion: {
         "sphinx.domains.c": 2,
         "sphinx.domains.changeset": 1,
         "sphinx.domains.citation": 1,
-        "sphinx.domains.cpp": 4,
+        "sphinx.domains.cpp": 5,
         "sphinx.domains.index": 1,
         "sphinx.domains.javascript": 2,
         "sphinx.domains.math": 2,
         "sphinx.domains.python": 3,
         "sphinx.domains.rst": 2,
         "sphinx.domains.std": 2,
         "sphinx.ext.intersphinx": 1,
         sphinx: 56
     },
     filenames: ["index.rst"],
     objects: {
-        "": {
-            maxminddb: [0, 0, 0, "-"]
-        },
-        "maxminddb.Reader": {
-            close: [0, 3, 1, ""],
-            get: [0, 3, 1, ""],
-            get_with_prefix_len: [0, 3, 1, ""],
-            metadata: [0, 3, 1, ""]
-        },
-        "maxminddb.errors": {
-            InvalidDatabaseError: [0, 1, 1, ""]
-        },
-        "maxminddb.reader": {
-            Metadata: [0, 2, 1, ""],
-            Reader: [0, 2, 1, ""]
-        },
-        "maxminddb.reader.Metadata": {
-            binary_format_major_version: [0, 5, 1, ""],
-            binary_format_minor_version: [0, 5, 1, ""],
-            build_epoch: [0, 5, 1, ""],
-            database_type: [0, 5, 1, ""],
-            description: [0, 5, 1, ""],
-            ip_version: [0, 5, 1, ""],
-            languages: [0, 5, 1, ""],
-            node_byte_size: [0, 6, 1, ""],
-            node_count: [0, 5, 1, ""],
-            record_size: [0, 5, 1, ""],
-            search_tree_size: [0, 6, 1, ""]
-        },
-        "maxminddb.reader.Reader": {
-            close: [0, 3, 1, ""],
-            get: [0, 3, 1, ""],
-            get_with_prefix_len: [0, 3, 1, ""],
-            metadata: [0, 3, 1, ""]
-        },
-        maxminddb: {
-            InvalidDatabaseError: [0, 1, 1, ""],
-            Reader: [0, 2, 1, ""],
-            errors: [0, 0, 0, "-"],
-            open_database: [0, 4, 1, ""],
-            reader: [0, 0, 0, "-"]
-        }
+        "": [
+            [0, 0, 0, "-", "maxminddb"]
+        ],
+        "maxminddb.Reader": [
+            [0, 3, 1, "", "close"],
+            [0, 3, 1, "", "get"],
+            [0, 3, 1, "", "get_with_prefix_len"],
+            [0, 3, 1, "", "metadata"]
+        ],
+        "maxminddb.errors": [
+            [0, 1, 1, "", "InvalidDatabaseError"]
+        ],
+        "maxminddb.reader": [
+            [0, 2, 1, "", "Metadata"],
+            [0, 2, 1, "", "Reader"]
+        ],
+        "maxminddb.reader.Metadata": [
+            [0, 5, 1, "", "binary_format_major_version"],
+            [0, 5, 1, "", "binary_format_minor_version"],
+            [0, 5, 1, "", "build_epoch"],
+            [0, 5, 1, "", "database_type"],
+            [0, 5, 1, "", "description"],
+            [0, 5, 1, "", "ip_version"],
+            [0, 5, 1, "", "languages"],
+            [0, 6, 1, "", "node_byte_size"],
+            [0, 5, 1, "", "node_count"],
+            [0, 5, 1, "", "record_size"],
+            [0, 6, 1, "", "search_tree_size"]
+        ],
+        "maxminddb.reader.Reader": [
+            [0, 3, 1, "", "close"],
+            [0, 3, 1, "", "get"],
+            [0, 3, 1, "", "get_with_prefix_len"],
+            [0, 3, 1, "", "metadata"]
+        ],
+        maxminddb: [
+            [0, 1, 1, "", "InvalidDatabaseError"],
+            [0, 2, 1, "", "Reader"],
+            [0, 0, 0, "-", "errors"],
+            [0, 4, 1, "", "open_database"],
+            [0, 0, 0, "-", "reader"]
+        ]
     },
     objnames: {
         "0": ["py", "module", "Python module"],
         "1": ["py", "exception", "Python exception"],
         "2": ["py", "class", "Python class"],
         "3": ["py", "method", "Python method"],
         "4": ["py", "function", "Python function"],
```

### Comparing `maxminddb-2.2.0/extension/maxminddb.c` & `maxminddb-2.3.0/extension/maxminddb.c`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     if (!mmdb_obj) {
         Py_XDECREF(filepath);
         free(mmdb);
         PyErr_NoMemory();
         return -1;
     }
 
-    uint16_t status = MMDB_open(filename, MMDB_MODE_MMAP, mmdb);
+    int const status = MMDB_open(filename, MMDB_MODE_MMAP, mmdb);
     Py_XDECREF(filepath);
 
     if (MMDB_SUCCESS != status) {
         free(mmdb);
         PyErr_Format(MaxMindDB_error,
                      "Error opening database file (%s). Is this a valid "
                      "MaxMind DB file?",
@@ -272,22 +272,22 @@
         return 0;
     }
 
     switch (len) {
         case 16: {
             ip_address->ss_family = AF_INET6;
             struct sockaddr_in6 *sin = (struct sockaddr_in6 *)ip_address;
-            memcpy(sin->sin6_addr.s6_addr, bytes, len);
+            memcpy(sin->sin6_addr.s6_addr, bytes, (size_t)len);
             Py_DECREF(packed);
             return 1;
         }
         case 4: {
             ip_address->ss_family = AF_INET;
             struct sockaddr_in *sin = (struct sockaddr_in *)ip_address;
-            memcpy(&(sin->sin_addr.s_addr), bytes, len);
+            memcpy(&(sin->sin_addr.s_addr), bytes, (size_t)len);
             Py_DECREF(packed);
             return 1;
         }
         default:
             PyErr_SetString(
                 PyExc_ValueError,
                 "argument 1 returned an unexpected packed length for address");
@@ -522,15 +522,15 @@
     // entry_data_list cannot start out NULL (see from_entry_data_list). We
     // check it in the loop because it may become NULL.
     // coverity[check_after_deref]
     for (i = 0; i < map_size && entry_data_list; i++) {
         *entry_data_list = (*entry_data_list)->next;
 
         PyObject *key = PyUnicode_FromStringAndSize(
-            (char *)(*entry_data_list)->entry_data.utf8_string,
+            (*entry_data_list)->entry_data.utf8_string,
             (*entry_data_list)->entry_data.data_size);
         if (!key) {
             // PyUnicode_FromStringAndSize will set an appropriate exception
             // in this case.
             return NULL;
         }
 
@@ -733,14 +733,15 @@
     Py_INCREF(&Reader_Type);
     PyModule_AddObject(m, "Reader", (PyObject *)&Reader_Type);
 
     Metadata_Type.tp_new = PyType_GenericNew;
     if (PyType_Ready(&Metadata_Type)) {
         return NULL;
     }
+    Py_INCREF(&Metadata_Type);
     PyModule_AddObject(m, "Metadata", (PyObject *)&Metadata_Type);
 
     PyObject *error_mod = PyImport_ImportModule("maxminddb.errors");
     if (error_mod == NULL) {
         return NULL;
     }
```

### Comparing `maxminddb-2.2.0/maxminddb/__init__.py` & `maxminddb-2.3.0/maxminddb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,11 +77,11 @@
     # checking purposes, pretend it is one. (Ideally this would be a subclass
     # of, or share a common parent class with, the Python Reader
     # implementation.)
     return cast(Reader, _extension.Reader(database, mode))
 
 
 __title__ = "maxminddb"
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 __author__ = "Gregory Oschwald"
 __license__ = "Apache License, Version 2.0"
 __copyright__ = "Copyright 2013-2021 MaxMind, Inc."
```

### Comparing `maxminddb-2.2.0/maxminddb/decoder.py` & `maxminddb-2.3.0/maxminddb/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,15 @@
     def _decode_array(self, size: int, offset: int) -> Tuple[List[Record], int]:
         array = []
         for _ in range(size):
             (value, offset) = self.decode(offset)
             array.append(value)
         return array, offset
 
-    def _decode_boolean(  # pylint: disable=no-self-use
-        self, size: int, offset: int
-    ) -> Tuple[bool, int]:
+    def _decode_boolean(self, size: int, offset: int) -> Tuple[bool, int]:
         return size != 0, offset
 
     def _decode_bytes(self, size: int, offset: int) -> Tuple[bytes, int]:
         new_offset = offset + size
         return self._buffer[offset:new_offset], new_offset
 
     def _decode_double(self, size: int, offset: int) -> Tuple[float, int]:
```

### Comparing `maxminddb-2.2.0/maxminddb/extension.pyi` & `maxminddb-2.3.0/maxminddb/extension.pyi`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/maxminddb/file.py` & `maxminddb-2.3.0/maxminddb/file.py`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/maxminddb/reader.py` & `maxminddb-2.3.0/maxminddb/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,17 @@
             filename = database
         elif mode in (MODE_AUTO, MODE_FILE):
             self._buffer = FileBuffer(database)  # type: ignore
             self._buffer_size = self._buffer.size()
             filename = database
         elif mode == MODE_MEMORY:
             with open(database, "rb") as db_file:  # type: ignore
-                self._buffer = db_file.read()
-                self._buffer_size = len(self._buffer)
+                buf = db_file.read()
+                self._buffer = buf
+                self._buffer_size = len(buf)
             filename = database
         elif mode == MODE_FD:
             self._buffer = database.read()  # type: ignore
             self._buffer_size = len(self._buffer)  # type: ignore
             filename = database.name  # type: ignore
         else:
             raise ValueError(
```

### Comparing `maxminddb-2.2.0/maxminddb/types.py` & `maxminddb-2.3.0/maxminddb/types.py`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/maxminddb.egg-info/PKG-INFO` & `maxminddb-2.3.0/maxminddb.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,137 +1,144 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: maxminddb
-Version: 2.2.0
+Version: 2.3.0
 Summary: Reader for the MaxMind DB format
 Home-page: http://www.maxmind.com/
 Author: Gregory Oschwald
 Author-email: goschwald@maxmind.com
 License: Apache License, Version 2.0
-Description: ========================
-        MaxMind DB Python Module
-        ========================
-        
-        Description
-        -----------
-        
-        This is a Python module for reading MaxMind DB files. The module includes both
-        a pure Python reader and an optional C extension.
-        
-        MaxMind DB is a binary file format that stores data indexed by IP address
-        subnets (IPv4 or IPv6).
-        
-        Installation
-        ------------
-        
-        If you want to use the C extension, you must first install `libmaxminddb
-        <https://github.com/maxmind/libmaxminddb>`_ C library installed before
-        installing this extension. If the library is not available, the module will
-        fall-back to a pure Python implementation. Note that when installing the C
-        library from a package, you may be required to install additonal packages
-        containing build requirements such as `libmaxminddb-dev` on Debian.
-        
-        To install maxminddb, type:
-        
-        .. code-block:: bash
-        
-            $ pip install maxminddb
-        
-        If you are not able to use pip, you may also use easy_install from the
-        source directory:
-        
-        .. code-block:: bash
-        
-            $ easy_install .
-        
-        Usage
-        -----
-        
-        To use this module, you must first download or create a MaxMind DB file. We
-        provide `free GeoLite2 databases
-        <https://dev.maxmind.com/geoip/geolocate-an-ip/databases?lang=en>`_. These
-        files must be decompressed with ``gunzip``.
-        
-        After you have obtained a database and imported the module, call
-        ``open_database`` with a path, or file descriptor (in the case of ``MODE_FD``),
-        to the database as the first argument. Optionally, you may pass a mode as the
-        second argument. The modes are exported from ``maxminddb``. Valid modes are:
-        
-        * ``MODE_MMAP_EXT`` - use the C extension with memory map.
-        * ``MODE_MMAP`` - read from memory map. Pure Python.
-        * ``MODE_FILE`` - read database as standard file. Pure Python.
-        * ``MODE_MEMORY`` - load database into memory. Pure Python.
-        * ``MODE_FD`` - load database into memory from a file descriptor. Pure Python.
-        * ``MODE_AUTO`` - try ``MODE_MMAP_EXT``, ``MODE_MMAP``, ``MODE_FILE`` in that
-          order. Default.
-        
-        **NOTE**: When using ``MODE_FD``, it is the *caller's* responsibility to be
-        sure that the file descriptor gets closed properly. The caller may close the
-        file descriptor immediately after the ``Reader`` object is created.
-        
-        The ``open_database`` function returns a ``Reader`` object. To look up an IP
-        address, use the ``get`` method on this object. The method will return the
-        corresponding values for the IP address from the database (e.g., a dictionary
-        for GeoIP2/GeoLite2 databases). If the database does not contain a record for
-        that IP address, the method will return ``None``.
-        
-        If you wish to also retrieve the prefix length for the record, use the
-        ``get_with_prefix_len`` method. This returns a tuple containing the record
-        followed by the network prefix length associated with the record.
-        
-        Example
-        -------
-        
-        .. code-block:: pycon
-        
-            >>> import maxminddb
-            >>>
-            >>> with maxminddb.open_database('GeoLite2-City.mmdb') as reader:
-            >>>
-            >>>     reader.get('152.216.7.110')
-            {'country': ... }
-            >>>
-            >>>     reader.get_with_prefix_len('152.216.7.110')
-            ({'country': ... }, 24)
-        
-        Exceptions
-        ----------
-        
-        The module will return an ``InvalidDatabaseError`` if the database is corrupt
-        or otherwise invalid. A ``ValueError`` will be thrown if you look up an
-        invalid IP address or an IPv6 address in an IPv4 database.
-        
-        Requirements
-        ------------
-        
-        This code requires Python 3.6+. Older versions are not supported. The C
-        extension requires CPython.
-        
-        Versioning
-        ----------
-        
-        The MaxMind DB Python module uses `Semantic Versioning <https://semver.org/>`_.
-        
-        Support
-        -------
-        
-        Please report all issues with this code using the `GitHub issue tracker
-        <https://github.com/maxmind/MaxMind-DB-Reader-python/issues>`_
-        
-        If you are having an issue with a MaxMind service that is not specific to this
-        API, please contact `MaxMind support <https://www.maxmind.com/en/support>`_ for
-        assistance.
-        
+Project-URL: Documentation, https://maxminddb.readthedocs.org/
+Project-URL: Source Code, https://github.com/maxmind/MaxMind-DB-Reader-python
+Project-URL: Issue Tracker, https://github.com/maxmind/MaxMind-DB-Reader-python/issues
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
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Internet
-Requires-Python: >=3.6
+Requires-Python: >=3.7
+License-File: LICENSE
+
+========================
+MaxMind DB Python Module
+========================
+
+Description
+-----------
+
+This is a Python module for reading MaxMind DB files. The module includes both
+a pure Python reader and an optional C extension.
+
+MaxMind DB is a binary file format that stores data indexed by IP address
+subnets (IPv4 or IPv6).
+
+Installation
+------------
+
+If you want to use the C extension, you must first install `libmaxminddb
+<https://github.com/maxmind/libmaxminddb>`_ C library installed before
+installing this extension. If the library is not available, the module will
+fall-back to a pure Python implementation. Note that when installing the C
+library from a package, you may be required to install additonal packages
+containing build requirements such as `libmaxminddb-dev` on Debian.
+
+To install maxminddb, type:
+
+.. code-block:: bash
+
+    $ pip install maxminddb
+
+If you are not able to use pip, you may also use easy_install from the
+source directory:
+
+.. code-block:: bash
+
+    $ easy_install .
+
+Usage
+-----
+
+To use this module, you must first download or create a MaxMind DB file. We
+provide `free GeoLite2 databases
+<https://dev.maxmind.com/geoip/geolocate-an-ip/databases?lang=en>`_. These
+files must be decompressed with ``gunzip``.
+
+After you have obtained a database and imported the module, call
+``open_database`` with a path, or file descriptor (in the case of ``MODE_FD``),
+to the database as the first argument. Optionally, you may pass a mode as the
+second argument. The modes are exported from ``maxminddb``. Valid modes are:
+
+* ``MODE_MMAP_EXT`` - use the C extension with memory map.
+* ``MODE_MMAP`` - read from memory map. Pure Python.
+* ``MODE_FILE`` - read database as standard file. Pure Python.
+* ``MODE_MEMORY`` - load database into memory. Pure Python.
+* ``MODE_FD`` - load database into memory from a file descriptor. Pure Python.
+* ``MODE_AUTO`` - try ``MODE_MMAP_EXT``, ``MODE_MMAP``, ``MODE_FILE`` in that
+  order. Default.
+
+**NOTE**: When using ``MODE_FD``, it is the *caller's* responsibility to be
+sure that the file descriptor gets closed properly. The caller may close the
+file descriptor immediately after the ``Reader`` object is created.
+
+The ``open_database`` function returns a ``Reader`` object. To look up an IP
+address, use the ``get`` method on this object. The method will return the
+corresponding values for the IP address from the database (e.g., a dictionary
+for GeoIP2/GeoLite2 databases). If the database does not contain a record for
+that IP address, the method will return ``None``.
+
+If you wish to also retrieve the prefix length for the record, use the
+``get_with_prefix_len`` method. This returns a tuple containing the record
+followed by the network prefix length associated with the record.
+
+Example
+-------
+
+.. code-block:: pycon
+
+    >>> import maxminddb
+    >>>
+    >>> with maxminddb.open_database('GeoLite2-City.mmdb') as reader:
+    >>>
+    >>>     reader.get('152.216.7.110')
+    {'country': ... }
+    >>>
+    >>>     reader.get_with_prefix_len('152.216.7.110')
+    ({'country': ... }, 24)
+
+Exceptions
+----------
+
+The module will return an ``InvalidDatabaseError`` if the database is corrupt
+or otherwise invalid. A ``ValueError`` will be thrown if you look up an
+invalid IP address or an IPv6 address in an IPv4 database.
+
+Requirements
+------------
+
+This code requires Python 3.7+. Older versions are not supported. The C
+extension requires CPython.
+
+Versioning
+----------
+
+The MaxMind DB Python module uses `Semantic Versioning <https://semver.org/>`_.
+
+Support
+-------
+
+Please report all issues with this code using the `GitHub issue tracker
+<https://github.com/maxmind/MaxMind-DB-Reader-python/issues>`_
+
+If you are having an issue with a MaxMind service that is not specific to this
+API, please contact `MaxMind support <https://www.maxmind.com/en/support>`_ for
+assistance.
+
+
```

### Comparing `maxminddb-2.2.0/maxminddb.egg-info/SOURCES.txt` & `maxminddb-2.3.0/maxminddb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 docs/html/.buildinfo
 docs/html/genindex.html
 docs/html/index.html
 docs/html/objects.inv
 docs/html/py-modindex.html
@@ -23,15 +24,14 @@
 docs/html/_static/minus.png
 docs/html/_static/navigation.png
 docs/html/_static/plus.png
 docs/html/_static/pygments.css
 docs/html/_static/searchtools.js
 docs/html/_static/sphinxdoc.css
 docs/html/_static/underscore-1.13.1.js
-docs/html/_static/underscore-1.3.1.js
 docs/html/_static/underscore.js
 extension/maxminddb.c
 maxminddb/__init__.py
 maxminddb/const.py
 maxminddb/decoder.py
 maxminddb/errors.py
 maxminddb/extension.pyi
```

### Comparing `maxminddb-2.2.0/setup.py` & `maxminddb-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import os
 import re
 import sys
 
-# This import is apparently needed for Nose on Red Hat's Python
-import multiprocessing
-
-from distutils.command.build_ext import build_ext
-from distutils.errors import CCompilerError, DistutilsExecError, DistutilsPlatformError
-
 from setuptools import setup, Extension
+from setuptools.command.build_ext import build_ext
+
+# These were only added to setuptools in 59.0.1.
+try:
+    from setuptools.errors import CCompilerError
+    from setuptools.errors import DistutilsExecError
+    from setuptools.errors import DistutilsPlatformError
+except ImportError:
+    from distutils.errors import CCompilerError
+    from distutils.errors import DistutilsExecError
+    from distutils.errors import DistutilsPlatformError
 
 cmdclass = {}
 PYPY = hasattr(sys, "pypy_version_info")
 JYTHON = sys.platform.startswith("java")
 requirements = []
 
 compile_args = ["-Wall", "-Wextra"]
@@ -29,15 +34,15 @@
 # Cargo cult code for installing extension with pure Python fallback.
 # Taken from SQLAlchemy, but this same basic code exists in many modules.
 ext_errors = (CCompilerError, DistutilsExecError, DistutilsPlatformError)
 
 
 class BuildFailed(Exception):
     def __init__(self):
-        self.cause = sys.exc_info()[1]  # work around py 2/3 different syntax
+        self.cause = sys.exc_info()[1]
 
 
 class ve_build_ext(build_ext):
     # This class allows C extension building to fail.
 
     def run(self):
         try:
@@ -48,15 +53,15 @@
     def build_extension(self, ext):
         try:
             build_ext.build_extension(self, ext)
         except ext_errors:
             raise BuildFailed()
         except ValueError:
             # this can happen on Windows 64 bit, see Python issue 7511
-            if "'path'" in str(sys.exc_info()[1]):  # works with both py 2/3
+            if "'path'" in str(sys.exc_info()[1]):
                 raise BuildFailed()
             raise
 
 
 cmdclass["build_ext"] = ve_build_ext
 
 #
@@ -105,32 +110,36 @@
         author_email="goschwald@maxmind.com",
         description="Reader for the MaxMind DB format",
         long_description=README,
         url="http://www.maxmind.com/",
         packages=find_packages("."),
         package_data={"": ["LICENSE"], "maxminddb": ["extension.pyi", "py.typed"]},
         package_dir={"maxminddb": "maxminddb"},
-        python_requires=">=3.6",
+        project_urls={
+            "Documentation": "https://maxminddb.readthedocs.org/",
+            "Source Code": "https://github.com/maxmind/MaxMind-DB-Reader-python",
+            "Issue Tracker": "https://github.com/maxmind/MaxMind-DB-Reader-python/issues",
+        },
+        python_requires=">=3.7",
         include_package_data=True,
         install_requires=requirements,
-        tests_require=["nose"],
-        test_suite="nose.collector",
         license=LICENSE,
         cmdclass=cmdclass,
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Environment :: Web Environment",
             "Intended Audience :: Developers",
             "Intended Audience :: System Administrators",
             "License :: OSI Approved :: Apache Software License",
             "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
             "Programming Language :: Python",
             "Topic :: Internet :: Proxy Servers",
             "Topic :: Internet",
         ],
         **kwargs
     )
```

### Comparing `maxminddb-2.2.0/tests/data/bad-data/maxminddb-golang/cyclic-data-structure.mmdb` & `maxminddb-2.3.0/tests/data/bad-data/maxminddb-golang/cyclic-data-structure.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/bad-data/maxminddb-golang/invalid-map-key-length.mmdb` & `maxminddb-2.3.0/tests/data/bad-data/maxminddb-golang/invalid-map-key-length.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/bad-data/maxminddb-golang/unexpected-bytes.mmdb` & `maxminddb-2.3.0/tests/data/bad-data/maxminddb-golang/unexpected-bytes.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/bad-data/maxminddb-python/bad-unicode-in-map-key.mmdb` & `maxminddb-2.3.0/tests/data/bad-data/maxminddb-python/bad-unicode-in-map-key.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-Anonymous-IP-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-Anonymous-IP-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-City-Test-Broken-Double-Format.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-City-Test-Broken-Double-Format.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-City-Test-Invalid-Node-Count.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-City-Test-Invalid-Node-Count.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-City-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-City-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-Connection-Type-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-Connection-Type-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-Country-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-Country-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-DensityIncome-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-DensityIncome-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-Domain-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-Domain-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-Enterprise-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-Enterprise-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-ISP-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-ISP-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-Precision-Enterprise-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-Precision-Enterprise-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-Static-IP-Score-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-Static-IP-Score-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoIP2-User-Count-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoIP2-User-Count-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoLite2-ASN-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoLite2-ASN-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoLite2-City-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoLite2-City-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/GeoLite2-Country-Test.mmdb` & `maxminddb-2.3.0/tests/data/test-data/GeoLite2-Country-Test.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-no-ipv4-search-tree.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-no-ipv4-search-tree.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-string-value-entries.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-string-value-entries.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-broken-pointers-24.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-broken-pointers-24.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-broken-search-tree-24.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-broken-search-tree-24.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-decoder.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-decoder.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-ipv4-24.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-ipv4-24.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-ipv4-28.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-ipv4-28.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-ipv4-32.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-ipv4-32.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-ipv6-24.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-ipv6-24.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-ipv6-28.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-ipv6-28.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-ipv6-32.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-ipv6-32.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-metadata-pointers.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-metadata-pointers.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-mixed-24.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-mixed-24.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-mixed-28.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-mixed-28.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-mixed-32.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-mixed-32.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-nested.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-nested.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/data/test-data/MaxMind-DB-test-pointer-decoder.mmdb` & `maxminddb-2.3.0/tests/data/test-data/MaxMind-DB-test-pointer-decoder.mmdb`

 * *Files identical despite different names*

### Comparing `maxminddb-2.2.0/tests/decoder_test.py` & `maxminddb-2.3.0/tests/decoder_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,14 @@
         self.validate_type_decoding("uint128", self.generate_large_uint(128))
 
     def validate_type_decoding(self, type, tests):
         for input, expected in tests.items():
             self.check_decoding(type, input, expected)
 
     def check_decoding(self, type, input, expected, name=None):
-
         name = name or expected
         db = mmap.mmap(-1, len(input))
         db.write(input)
 
         decoder = Decoder(db, pointer_test=True)
         (
             actual,
```

### Comparing `maxminddb-2.2.0/tests/reader_test.py` & `maxminddb-2.3.0/tests/reader_test.py`

 * *Files identical despite different names*

