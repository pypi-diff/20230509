# Comparing `tmp/llfuse-1.4.2.tar.gz` & `tmp/llfuse-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/llfuse-1.4.2.tar", last modified: Tue May 31 15:39:59 2022, max compression
+gzip compressed data, was "llfuse-1.4.3.tar", last modified: Tue May  9 13:15:14 2023, max compression
```

## Comparing `llfuse-1.4.2.tar` & `llfuse-1.4.3.tar`

### file list

```diff
@@ -1,148 +1,86 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/
--rw-r--r--   0 user      (1000) user      (1000)    12838 2022-05-31 15:23:32.000000 llfuse-1.4.2/Changes.rst
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/Include/
--rw-r--r--   0 user      (1000) user      (1000)     1839 2020-10-04 12:03:51.000000 llfuse-1.4.2/Include/fuse_common.pxd
--rw-r--r--   0 user      (1000) user      (1000)     7987 2020-10-04 12:03:51.000000 llfuse-1.4.2/Include/fuse_lowlevel.pxd
--rw-r--r--   0 user      (1000) user      (1000)      393 2020-10-04 12:03:51.000000 llfuse-1.4.2/Include/fuse_opt.pxd
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/Include/libc/
--rw-r--r--   0 user      (1000) user      (1000)       13 2020-10-04 12:03:51.000000 llfuse-1.4.2/Include/libc/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      546 2020-10-04 12:03:51.000000 llfuse-1.4.2/Include/libc/dirent.pxd
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/Include/libc/sys/
--rw-r--r--   0 user      (1000) user      (1000)       13 2020-10-04 12:03:51.000000 llfuse-1.4.2/Include/libc/sys/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      627 2020-10-04 12:03:51.000000 llfuse-1.4.2/Include/libc/sys/statvfs.pxd
--rw-r--r--   0 user      (1000) user      (1000)     1783 2020-10-04 12:03:51.000000 llfuse-1.4.2/Include/pthread.pxd
--rw-r--r--   0 user      (1000) user      (1000)    25960 2020-10-04 12:03:51.000000 llfuse-1.4.2/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     3205 2022-05-31 15:39:59.000000 llfuse-1.4.2/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1626 2022-05-31 15:14:28.000000 llfuse-1.4.2/README.rst
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/doc/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/doc/html/
--rw-r--r--   0 user      (1000) user      (1000)      230 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/.buildinfo
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/doc/html/.doctrees/
--rw-r--r--   0 user      (1000) user      (1000)    10698 2021-02-01 20:07:35.000000 llfuse-1.4.2/doc/html/.doctrees/about.doctree
--rw-r--r--   0 user      (1000) user      (1000)    80056 2021-02-01 20:07:35.000000 llfuse-1.4.2/doc/html/.doctrees/changes.doctree
--rw-r--r--   0 user      (1000) user      (1000)    46538 2021-02-01 20:22:37.000000 llfuse-1.4.2/doc/html/.doctrees/data.doctree
--rw-r--r--   0 user      (1000) user      (1000)  1719590 2021-02-01 20:22:38.000000 llfuse-1.4.2/doc/html/.doctrees/environment.pickle
--rw-r--r--   0 user      (1000) user      (1000)    81477 2021-02-01 20:07:35.000000 llfuse-1.4.2/doc/html/.doctrees/example.doctree
--rw-r--r--   0 user      (1000) user      (1000)    35011 2021-02-01 20:22:37.000000 llfuse-1.4.2/doc/html/.doctrees/fuse_api.doctree
--rw-r--r--   0 user      (1000) user      (1000)    20551 2021-02-01 20:07:35.000000 llfuse-1.4.2/doc/html/.doctrees/general.doctree
--rw-r--r--   0 user      (1000) user      (1000)     5491 2021-02-01 20:07:35.000000 llfuse-1.4.2/doc/html/.doctrees/gotchas.doctree
--rw-r--r--   0 user      (1000) user      (1000)     4489 2021-02-01 20:07:35.000000 llfuse-1.4.2/doc/html/.doctrees/index.doctree
--rw-r--r--   0 user      (1000) user      (1000)    19676 2021-02-01 20:07:35.000000 llfuse-1.4.2/doc/html/.doctrees/install.doctree
--rw-r--r--   0 user      (1000) user      (1000)    18796 2021-02-01 20:22:37.000000 llfuse-1.4.2/doc/html/.doctrees/lock.doctree
--rw-r--r--   0 user      (1000) user      (1000)   150519 2021-02-01 20:22:37.000000 llfuse-1.4.2/doc/html/.doctrees/operations.doctree
--rw-r--r--   0 user      (1000) user      (1000)    20870 2021-02-01 20:22:38.000000 llfuse-1.4.2/doc/html/.doctrees/util.doctree
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/doc/html/_sources/
--rw-r--r--   0 user      (1000) user      (1000)       80 2020-10-04 12:03:51.000000 llfuse-1.4.2/doc/html/_sources/about.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)       28 2020-10-04 12:03:51.000000 llfuse-1.4.2/doc/html/_sources/changes.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)     2927 2020-10-04 12:03:51.000000 llfuse-1.4.2/doc/html/_sources/data.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)      816 2020-10-04 12:03:51.000000 llfuse-1.4.2/doc/html/_sources/example.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)      327 2020-10-04 12:03:51.000000 llfuse-1.4.2/doc/html/_sources/fuse_api.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)     3226 2020-10-04 12:03:51.000000 llfuse-1.4.2/doc/html/_sources/general.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)      868 2020-10-04 12:03:51.000000 llfuse-1.4.2/doc/html/_sources/gotchas.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)      409 2020-10-04 12:03:51.000000 llfuse-1.4.2/doc/html/_sources/index.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)     2821 2020-10-04 14:42:01.000000 llfuse-1.4.2/doc/html/_sources/install.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)     2048 2020-10-04 12:03:51.000000 llfuse-1.4.2/doc/html/_sources/lock.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)      198 2020-10-04 12:03:51.000000 llfuse-1.4.2/doc/html/_sources/operations.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)      381 2020-10-04 12:03:51.000000 llfuse-1.4.2/doc/html/_sources/util.rst.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/doc/html/_static/
--rw-r--r--   0 user      (1000) user      (1000)    13647 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/_static/basic.css
--rw-r--r--   0 user      (1000) user      (1000)     4256 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/_static/classic.css
--rw-r--r--   0 user      (1000) user      (1000)       28 2020-10-09 23:15:38.000000 llfuse-1.4.2/doc/html/_static/default.css
--rw-r--r--   0 user      (1000) user      (1000)     9416 2021-01-24 17:51:41.000000 llfuse-1.4.2/doc/html/_static/doctools.js
--rw-r--r--   0 user      (1000) user      (1000)      355 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/_static/documentation_options.js
--rw-r--r--   0 user      (1000) user      (1000)      286 2020-10-09 23:15:38.000000 llfuse-1.4.2/doc/html/_static/file.png
--rw-r--r--   0 user      (1000) user      (1000)   287630 2020-10-09 23:15:38.000000 llfuse-1.4.2/doc/html/_static/jquery-3.5.1.js
--rw-r--r--   0 user      (1000) user      (1000)    89476 2020-10-09 23:15:38.000000 llfuse-1.4.2/doc/html/_static/jquery.js
--rw-r--r--   0 user      (1000) user      (1000)    10847 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/_static/language_data.js
--rw-r--r--   0 user      (1000) user      (1000)       90 2020-10-09 23:15:38.000000 llfuse-1.4.2/doc/html/_static/minus.png
--rw-r--r--   0 user      (1000) user      (1000)       90 2020-10-09 23:15:38.000000 llfuse-1.4.2/doc/html/_static/plus.png
--rw-r--r--   0 user      (1000) user      (1000)     4837 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/_static/pygments.css
--rw-r--r--   0 user      (1000) user      (1000)    16323 2021-01-24 17:51:41.000000 llfuse-1.4.2/doc/html/_static/searchtools.js
--rw-r--r--   0 user      (1000) user      (1000)     4803 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/_static/sidebar.js
--rw-r--r--   0 user      (1000) user      (1000)    35168 2020-10-09 23:15:38.000000 llfuse-1.4.2/doc/html/_static/underscore-1.3.1.js
--rw-r--r--   0 user      (1000) user      (1000)    12140 2020-10-09 23:15:38.000000 llfuse-1.4.2/doc/html/_static/underscore.js
--rw-r--r--   0 user      (1000) user      (1000)     7167 2022-05-31 15:21:24.000000 llfuse-1.4.2/doc/html/about.html
--rw-r--r--   0 user      (1000) user      (1000)    30695 2022-05-31 15:21:24.000000 llfuse-1.4.2/doc/html/changes.html
--rw-r--r--   0 user      (1000) user      (1000)    22315 2022-05-31 15:21:24.000000 llfuse-1.4.2/doc/html/data.html
--rw-r--r--   0 user      (1000) user      (1000)   183118 2022-05-31 15:21:24.000000 llfuse-1.4.2/doc/html/example.html
--rw-r--r--   0 user      (1000) user      (1000)    16936 2022-05-31 15:21:24.000000 llfuse-1.4.2/doc/html/fuse_api.html
--rw-r--r--   0 user      (1000) user      (1000)    12930 2022-05-31 15:21:24.000000 llfuse-1.4.2/doc/html/general.html
--rw-r--r--   0 user      (1000) user      (1000)    18583 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/genindex.html
--rw-r--r--   0 user      (1000) user      (1000)     8634 2022-05-31 15:21:24.000000 llfuse-1.4.2/doc/html/gotchas.html
--rw-r--r--   0 user      (1000) user      (1000)     6520 2022-05-31 15:21:24.000000 llfuse-1.4.2/doc/html/index.html
--rw-r--r--   0 user      (1000) user      (1000)     9870 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/install.html
--rw-r--r--   0 user      (1000) user      (1000)    11794 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/lock.html
--rw-r--r--   0 user      (1000) user      (1000)     1111 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/objects.inv
--rw-r--r--   0 user      (1000) user      (1000)    57525 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/operations.html
--rw-r--r--   0 user      (1000) user      (1000)     4721 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/py-modindex.html
--rw-r--r--   0 user      (1000) user      (1000)     4519 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/search.html
--rw-r--r--   0 user      (1000) user      (1000)    18408 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/searchindex.js
--rw-r--r--   0 user      (1000) user      (1000)    11682 2022-05-31 15:21:25.000000 llfuse-1.4.2/doc/html/util.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/examples/
--rwxr-xr-x   0 user      (1000) user      (1000)     5071 2021-01-21 19:35:27.000000 llfuse-1.4.2/examples/lltest.py
--rwxr-xr-x   0 user      (1000) user      (1000)    16688 2020-10-04 12:03:51.000000 llfuse-1.4.2/examples/passthroughfs.py
--rwxr-xr-x   0 user      (1000) user      (1000)    15838 2021-01-21 19:35:27.000000 llfuse-1.4.2/examples/tmpfs.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/rst/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/rst/_static/
--rw-r--r--   0 user      (1000) user      (1000)        0 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/_static/.placeholder
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/rst/_templates/
--rw-r--r--   0 user      (1000) user      (1000)       93 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/_templates/localtoc.html
--rw-r--r--   0 user      (1000) user      (1000)       80 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/about.rst
--rw-r--r--   0 user      (1000) user      (1000)       28 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/changes.rst
--rw-r--r--   0 user      (1000) user      (1000)     6947 2021-02-01 20:30:15.000000 llfuse-1.4.2/rst/conf.py
--rw-r--r--   0 user      (1000) user      (1000)     2927 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/data.rst
--rw-r--r--   0 user      (1000) user      (1000)      816 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/example.rst
--rw-r--r--   0 user      (1000) user      (1000)      327 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/fuse_api.rst
--rw-r--r--   0 user      (1000) user      (1000)     3226 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/general.rst
--rw-r--r--   0 user      (1000) user      (1000)      868 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/gotchas.rst
--rw-r--r--   0 user      (1000) user      (1000)      409 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/index.rst
--rw-r--r--   0 user      (1000) user      (1000)     2821 2020-10-04 14:42:01.000000 llfuse-1.4.2/rst/install.rst
--rw-r--r--   0 user      (1000) user      (1000)     2048 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/lock.rst
--rw-r--r--   0 user      (1000) user      (1000)      198 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/operations.rst
--rw-r--r--   0 user      (1000) user      (1000)      381 2020-10-04 12:03:51.000000 llfuse-1.4.2/rst/util.rst
--rw-r--r--   0 user      (1000) user      (1000)       87 2022-05-31 15:39:59.000000 llfuse-1.4.2/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)    10016 2022-05-31 15:23:32.000000 llfuse-1.4.2/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/src/
--rw-r--r--   0 user      (1000) user      (1000)     6145 2020-10-04 12:03:51.000000 llfuse-1.4.2/src/darwin_compat.c
--rw-r--r--   0 user      (1000) user      (1000)     1376 2020-10-04 12:03:51.000000 llfuse-1.4.2/src/darwin_compat.h
--rw-r--r--   0 user      (1000) user      (1000)    19430 2022-05-31 15:14:28.000000 llfuse-1.4.2/src/fuse_api.pxi
--rw-r--r--   0 user      (1000) user      (1000)      963 2020-10-04 12:03:51.000000 llfuse-1.4.2/src/gettime.h
--rw-r--r--   0 user      (1000) user      (1000)    23731 2020-12-08 16:48:12.000000 llfuse-1.4.2/src/handlers.pxi
--rw-r--r--   0 user      (1000) user      (1000)  2478957 2022-05-31 15:39:27.000000 llfuse-1.4.2/src/llfuse.c
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/src/llfuse.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3205 2022-05-31 15:39:58.000000 llfuse-1.4.2/src/llfuse.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     3057 2022-05-31 15:39:58.000000 llfuse-1.4.2/src/llfuse.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-05-31 15:39:58.000000 llfuse-1.4.2/src/llfuse.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2022-05-31 15:39:58.000000 llfuse-1.4.2/src/llfuse.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2021-01-21 20:47:48.000000 llfuse-1.4.2/src/llfuse.egg-info/zip-safe
--rw-r--r--   0 user      (1000) user      (1000)      924 2020-10-04 12:03:51.000000 llfuse-1.4.2/src/llfuse.h
--rw-r--r--   0 user      (1000) user      (1000)     4171 2021-01-21 19:35:27.000000 llfuse-1.4.2/src/llfuse.pyx
--rw-r--r--   0 user      (1000) user      (1000)     3893 2020-10-04 12:03:51.000000 llfuse-1.4.2/src/lock.c
--rw-r--r--   0 user      (1000) user      (1000)      383 2020-10-04 12:03:51.000000 llfuse-1.4.2/src/lock.h
--rw-r--r--   0 user      (1000) user      (1000)     1940 2020-10-04 12:03:51.000000 llfuse-1.4.2/src/macros.c
--rw-r--r--   0 user      (1000) user      (1000)    21374 2021-01-21 19:35:27.000000 llfuse-1.4.2/src/misc.pxi
--rw-r--r--   0 user      (1000) user      (1000)    19987 2020-10-04 12:03:51.000000 llfuse-1.4.2/src/operations.pxi
--rw-r--r--   0 user      (1000) user      (1000)     3500 2020-10-04 12:03:51.000000 llfuse-1.4.2/src/xattr.h
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/test/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/test/.pytest_cache/
--rw-r--r--   0 user      (1000) user      (1000)       37 2022-05-31 15:21:06.000000 llfuse-1.4.2/test/.pytest_cache/.gitignore
--rw-r--r--   0 user      (1000) user      (1000)      194 2022-05-31 15:21:06.000000 llfuse-1.4.2/test/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 user      (1000) user      (1000)      295 2022-05-31 15:21:06.000000 llfuse-1.4.2/test/.pytest_cache/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/test/.pytest_cache/v/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/test/.pytest_cache/v/cache/
--rw-r--r--   0 user      (1000) user      (1000)      525 2022-05-31 15:21:06.000000 llfuse-1.4.2/test/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 user      (1000) user      (1000)        2 2022-05-31 15:21:06.000000 llfuse-1.4.2/test/.pytest_cache/v/cache/stepwise
--rwxr-xr-x   0 user      (1000) user      (1000)       69 2022-05-31 15:23:32.000000 llfuse-1.4.2/test/ci-install.sh
--rwxr-xr-x   0 user      (1000) user      (1000)      139 2021-01-21 19:35:27.000000 llfuse-1.4.2/test/ci-test.sh
--rw-r--r--   0 user      (1000) user      (1000)     3650 2020-10-04 12:03:51.000000 llfuse-1.4.2/test/conftest.py
--rw-r--r--   0 user      (1000) user      (1000)       81 2020-12-04 19:24:11.000000 llfuse-1.4.2/test/pytest.ini
--rw-r--r--   0 user      (1000) user      (1000)     3885 2020-12-04 19:24:11.000000 llfuse-1.4.2/test/pytest_checklogs.py
--rwxr-xr-x   0 user      (1000) user      (1000)     2962 2021-01-21 19:35:27.000000 llfuse-1.4.2/test/test_api.py
--rwxr-xr-x   0 user      (1000) user      (1000)    11621 2021-01-21 19:35:27.000000 llfuse-1.4.2/test/test_examples.py
--rwxr-xr-x   0 user      (1000) user      (1000)     8337 2021-01-24 18:31:20.000000 llfuse-1.4.2/test/test_fs.py
--rwxr-xr-x   0 user      (1000) user      (1000)     1228 2021-01-31 20:24:52.000000 llfuse-1.4.2/test/test_rounding.py
--rw-r--r--   0 user      (1000) user      (1000)     3691 2021-01-21 19:35:27.000000 llfuse-1.4.2/test/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-05-31 15:39:59.000000 llfuse-1.4.2/util/
--rwxr-xr-x   0 user      (1000) user      (1000)      307 2020-10-10 00:05:54.000000 llfuse-1.4.2/util/sdist-sign
--rw-r--r--   0 user      (1000) user      (1000)     1021 2021-01-21 19:35:27.000000 llfuse-1.4.2/util/sphinx_cython.py
--rwxr-xr-x   0 user      (1000) user      (1000)      277 2020-10-10 00:05:54.000000 llfuse-1.4.2/util/upload-pypi
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.733315 llfuse-1.4.3/
+-rw-r--r--   0 tw         (501) staff       (20)    13140 2023-05-09 13:10:13.000000 llfuse-1.4.3/Changes.rst
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.716790 llfuse-1.4.3/Include/
+-rw-r--r--   0 tw         (501) staff       (20)     1839 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/fuse_common.pxd
+-rw-r--r--   0 tw         (501) staff       (20)     7987 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/fuse_lowlevel.pxd
+-rw-r--r--   0 tw         (501) staff       (20)      393 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/fuse_opt.pxd
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.717403 llfuse-1.4.3/Include/libc/
+-rw-r--r--   0 tw         (501) staff       (20)       13 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/libc/__init__.py
+-rw-r--r--   0 tw         (501) staff       (20)      546 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/libc/dirent.pxd
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.717848 llfuse-1.4.3/Include/libc/sys/
+-rw-r--r--   0 tw         (501) staff       (20)       13 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/libc/sys/__init__.py
+-rw-r--r--   0 tw         (501) staff       (20)      627 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/libc/sys/statvfs.pxd
+-rw-r--r--   0 tw         (501) staff       (20)     1783 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/pthread.pxd
+-rw-r--r--   0 tw         (501) staff       (20)    25960 2022-05-16 19:57:28.000000 llfuse-1.4.3/LICENSE
+-rw-r--r--   0 tw         (501) staff       (20)     2881 2023-05-09 13:15:14.733403 llfuse-1.4.3/PKG-INFO
+-rw-r--r--   0 tw         (501) staff       (20)     1626 2023-05-09 10:54:10.000000 llfuse-1.4.3/README.rst
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.718644 llfuse-1.4.3/examples/
+-rwxr-xr-x   0 tw         (501) staff       (20)     5071 2022-05-16 19:57:28.000000 llfuse-1.4.3/examples/lltest.py
+-rwxr-xr-x   0 tw         (501) staff       (20)    16688 2022-05-16 19:57:28.000000 llfuse-1.4.3/examples/passthroughfs.py
+-rwxr-xr-x   0 tw         (501) staff       (20)    15838 2022-05-16 19:57:28.000000 llfuse-1.4.3/examples/tmpfs.py
+-rw-r--r--   0 tw         (501) staff       (20)       81 2023-05-09 12:56:19.000000 llfuse-1.4.3/pyproject.toml
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.721472 llfuse-1.4.3/rst/
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.721658 llfuse-1.4.3/rst/_static/
+-rw-r--r--   0 tw         (501) staff       (20)        0 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/_static/.placeholder
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.721799 llfuse-1.4.3/rst/_templates/
+-rw-r--r--   0 tw         (501) staff       (20)       93 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/_templates/localtoc.html
+-rw-r--r--   0 tw         (501) staff       (20)       80 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/about.rst
+-rw-r--r--   0 tw         (501) staff       (20)       28 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/changes.rst
+-rw-r--r--   0 tw         (501) staff       (20)     6947 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/conf.py
+-rw-r--r--   0 tw         (501) staff       (20)     2927 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/data.rst
+-rw-r--r--   0 tw         (501) staff       (20)      816 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/example.rst
+-rw-r--r--   0 tw         (501) staff       (20)      327 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/fuse_api.rst
+-rw-r--r--   0 tw         (501) staff       (20)     3226 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/general.rst
+-rw-r--r--   0 tw         (501) staff       (20)      868 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/gotchas.rst
+-rw-r--r--   0 tw         (501) staff       (20)      409 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/index.rst
+-rw-r--r--   0 tw         (501) staff       (20)     2821 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/install.rst
+-rw-r--r--   0 tw         (501) staff       (20)     2048 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/lock.rst
+-rw-r--r--   0 tw         (501) staff       (20)      198 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/operations.rst
+-rw-r--r--   0 tw         (501) staff       (20)      381 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/util.rst
+-rw-r--r--   0 tw         (501) staff       (20)       87 2023-05-09 13:15:14.733704 llfuse-1.4.3/setup.cfg
+-rwxr-xr-x   0 tw         (501) staff       (20)     9886 2023-05-09 13:06:13.000000 llfuse-1.4.3/setup.py
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.728508 llfuse-1.4.3/src/
+-rw-r--r--   0 tw         (501) staff       (20)     6145 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/darwin_compat.c
+-rw-r--r--   0 tw         (501) staff       (20)     1376 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/darwin_compat.h
+-rw-r--r--   0 tw         (501) staff       (20)    19430 2023-05-09 10:54:10.000000 llfuse-1.4.3/src/fuse_api.pxi
+-rw-r--r--   0 tw         (501) staff       (20)      963 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/gettime.h
+-rw-r--r--   0 tw         (501) staff       (20)    23731 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/handlers.pxi
+-rw-r--r--   0 tw         (501) staff       (20)  2481650 2023-05-09 13:11:22.000000 llfuse-1.4.3/src/llfuse.c
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.729337 llfuse-1.4.3/src/llfuse.egg-info/
+-rw-r--r--   0 tw         (501) staff       (20)     2881 2023-05-09 13:15:14.000000 llfuse-1.4.3/src/llfuse.egg-info/PKG-INFO
+-rw-r--r--   0 tw         (501) staff       (20)     1385 2023-05-09 13:15:14.000000 llfuse-1.4.3/src/llfuse.egg-info/SOURCES.txt
+-rw-r--r--   0 tw         (501) staff       (20)        1 2023-05-09 13:15:14.000000 llfuse-1.4.3/src/llfuse.egg-info/dependency_links.txt
+-rw-r--r--   0 tw         (501) staff       (20)        7 2023-05-09 13:15:14.000000 llfuse-1.4.3/src/llfuse.egg-info/top_level.txt
+-rw-r--r--   0 tw         (501) staff       (20)        1 2022-05-16 19:58:20.000000 llfuse-1.4.3/src/llfuse.egg-info/zip-safe
+-rw-r--r--   0 tw         (501) staff       (20)      924 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/llfuse.h
+-rw-r--r--   0 tw         (501) staff       (20)     4171 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/llfuse.pyx
+-rw-r--r--   0 tw         (501) staff       (20)     3893 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/lock.c
+-rw-r--r--   0 tw         (501) staff       (20)      383 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/lock.h
+-rw-r--r--   0 tw         (501) staff       (20)     1940 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/macros.c
+-rw-r--r--   0 tw         (501) staff       (20)    21374 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/misc.pxi
+-rw-r--r--   0 tw         (501) staff       (20)    19987 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/operations.pxi
+-rw-r--r--   0 tw         (501) staff       (20)     3500 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/xattr.h
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.731336 llfuse-1.4.3/test/
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.731899 llfuse-1.4.3/test/.pytest_cache/
+-rw-r--r--   0 tw         (501) staff       (20)       37 2022-05-16 20:44:06.000000 llfuse-1.4.3/test/.pytest_cache/.gitignore
+-rw-r--r--   0 tw         (501) staff       (20)      191 2022-05-16 20:44:06.000000 llfuse-1.4.3/test/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 tw         (501) staff       (20)      302 2022-05-16 20:44:06.000000 llfuse-1.4.3/test/.pytest_cache/README.md
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.714216 llfuse-1.4.3/test/.pytest_cache/v/
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.732586 llfuse-1.4.3/test/.pytest_cache/v/cache/
+-rw-r--r--   0 tw         (501) staff       (20)       88 2022-05-16 20:50:14.000000 llfuse-1.4.3/test/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 tw         (501) staff       (20)      525 2023-05-09 13:14:27.000000 llfuse-1.4.3/test/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 tw         (501) staff       (20)        2 2023-05-09 13:14:27.000000 llfuse-1.4.3/test/.pytest_cache/v/cache/stepwise
+-rwxr-xr-x   0 tw         (501) staff       (20)       75 2023-05-09 12:56:19.000000 llfuse-1.4.3/test/ci-install.sh
+-rwxr-xr-x   0 tw         (501) staff       (20)      139 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/ci-test.sh
+-rw-r--r--   0 tw         (501) staff       (20)     3650 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/conftest.py
+-rw-r--r--   0 tw         (501) staff       (20)       81 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/pytest.ini
+-rw-r--r--   0 tw         (501) staff       (20)     3885 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/pytest_checklogs.py
+-rwxr-xr-x   0 tw         (501) staff       (20)     2962 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/test_api.py
+-rwxr-xr-x   0 tw         (501) staff       (20)    11770 2023-05-09 10:54:10.000000 llfuse-1.4.3/test/test_examples.py
+-rwxr-xr-x   0 tw         (501) staff       (20)     8337 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/test_fs.py
+-rwxr-xr-x   0 tw         (501) staff       (20)     1228 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/test_rounding.py
+-rw-r--r--   0 tw         (501) staff       (20)     3691 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/util.py
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.733141 llfuse-1.4.3/util/
+-rwxr-xr-x   0 tw         (501) staff       (20)      307 2022-05-16 19:57:28.000000 llfuse-1.4.3/util/sdist-sign
+-rw-r--r--   0 tw         (501) staff       (20)     1021 2022-05-16 19:57:28.000000 llfuse-1.4.3/util/sphinx_cython.py
+-rwxr-xr-x   0 tw         (501) staff       (20)      277 2022-05-16 19:57:28.000000 llfuse-1.4.3/util/upload-pypi
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `llfuse-1.4.2/Changes.rst` & `llfuse-1.4.3/Changes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,23 @@
  Changelog
 ===========
 
 .. currentmodule:: llfuse
 
 **WARNING**: Python-LLFUSE is no longer actively developed.
 
+Release 1.4.3 (2023-05-09)
+==========================
+
+* cythonize with Cython 0.29.34 (brings python 3.12 support)
+* also test on python 3.12-dev
+* add a minimal pyproject.toml, #70
+* fix basedir in setup.py (malfunctioned with pip install -e .)
+* tests: fix integer overflow on 32-bit architectures
+
 Release 1.4.2 (2022-05-31)
 ==========================
 
 * cythonize with Cython 0.29.30 (brings python 3.11 support)
 * also test on python 3.10 and 3.11-dev
 * remove "nonempty" default mount option, seems unsupported now.
```

### Comparing `llfuse-1.4.2/Include/fuse_common.pxd` & `llfuse-1.4.3/Include/fuse_common.pxd`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/Include/fuse_lowlevel.pxd` & `llfuse-1.4.3/Include/fuse_lowlevel.pxd`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/Include/libc/dirent.pxd` & `llfuse-1.4.3/Include/libc/dirent.pxd`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/Include/libc/sys/statvfs.pxd` & `llfuse-1.4.3/Include/libc/sys/statvfs.pxd`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/Include/pthread.pxd` & `llfuse-1.4.3/Include/pthread.pxd`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/LICENSE` & `llfuse-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/PKG-INFO` & `llfuse-1.4.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,15 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: llfuse
-Version: 1.4.2
+Version: 1.4.3
 Summary: Python bindings for the low-level FUSE API
 Home-page: https://github.com/python-llfuse/python-llfuse/
 Author: Nikolaus Rath
 Author-email: Nikolaus@rath.org
 License: LGPL
-Description: ..
-          NOTE: We cannot use sophisticated ReST syntax (like
-          e.g. :file:`foo`) here because this isn't rendered correctly
-          by PyPi.
-        
-        The Python-LLFUSE Module
-        ========================
-        
-        
-        .. start-intro
-        
-        **Warning - no longer developed!**
-        
-        Python-LLFUSE is no longer actively developed and just receiving
-        community-contributed maintenance to keep it alive for some time.
-        
-        Python-LLFUSE is a set of Python bindings for the low level FUSE_
-        API. It requires at least FUSE 2.8.0 and supports both Python 2.x and
-        3.x. Like FUSE itself, Python-LLFUSE is developed for Linux systems,
-        but it should be compatible with OS-X, FreeBSD and NetBSD as well.
-        
-        Python-LLFUSE releases can be downloaded from PyPi_. The documentation
-        can be `read online`__ and is also included in the ``doc/html``
-        directory of the Python-LLFUSE tarball.
-        
-        
-        Getting Help
-        ------------
-        
-        Please report any bugs on the `issue tracker`_. For discussion and
-        questions, please use the general `FUSE mailing list`_. A searchable
-        `mailing list archive`_ is kindly provided by Gmane_.
-        
-        
-        Contributing
-        ------------
-        
-        The Python-LLFUSE source code is available on GitHub_.
-        
-        
-        .. __: http://www.rath.org/llfuse-docs/
-        .. _FUSE: http://github.com/libfuse/libfuse
-        .. _FUSE mailing list: https://lists.sourceforge.net/lists/listinfo/fuse-devel
-        .. _issue tracker: https://github.com/python-llfuse/python-llfuse/issues
-        .. _mailing list archive: http://dir.gmane.org/gmane.comp.file-systems.fuse.devel
-        .. _Gmane: http://www.gmane.org/
-        .. _PyPi: https://pypi.python.org/pypi/llfuse/
-        .. _GitHub: https://github.com/python-llfuse/python-llfuse
-        
 Keywords: FUSE,python
 Platform: Linux
 Platform: FreeBSD
 Platform: OS X
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -66,15 +17,66 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Provides: llfuse
 Requires-Python: >=3.5
+License-File: LICENSE
+
+..
+  NOTE: We cannot use sophisticated ReST syntax (like
+  e.g. :file:`foo`) here because this isn't rendered correctly
+  by PyPi.
+
+The Python-LLFUSE Module
+========================
+
+
+.. start-intro
+
+**Warning - no longer developed!**
+
+Python-LLFUSE is no longer actively developed and just receiving
+community-contributed maintenance to keep it alive for some time.
+
+Python-LLFUSE is a set of Python bindings for the low level FUSE_
+API. It requires at least FUSE 2.8.0 and supports both Python 2.x and
+3.x. Like FUSE itself, Python-LLFUSE is developed for Linux systems,
+but it should be compatible with OS-X, FreeBSD and NetBSD as well.
+
+Python-LLFUSE releases can be downloaded from PyPi_. The documentation
+can be `read online`__ and is also included in the ``doc/html``
+directory of the Python-LLFUSE tarball.
+
+
+Getting Help
+------------
+
+Please report any bugs on the `issue tracker`_. For discussion and
+questions, please use the general `FUSE mailing list`_. A searchable
+`mailing list archive`_ is kindly provided by Gmane_.
+
+
+Contributing
+------------
+
+The Python-LLFUSE source code is available on GitHub_.
+
+
+.. __: http://www.rath.org/llfuse-docs/
+.. _FUSE: http://github.com/libfuse/libfuse
+.. _FUSE mailing list: https://lists.sourceforge.net/lists/listinfo/fuse-devel
+.. _issue tracker: https://github.com/python-llfuse/python-llfuse/issues
+.. _mailing list archive: http://dir.gmane.org/gmane.comp.file-systems.fuse.devel
+.. _Gmane: http://www.gmane.org/
+.. _PyPi: https://pypi.python.org/pypi/llfuse/
+.. _GitHub: https://github.com/python-llfuse/python-llfuse
```

### Comparing `llfuse-1.4.2/README.rst` & `llfuse-1.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/doc/html/_sources/data.rst.txt` & `llfuse-1.4.3/rst/data.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/doc/html/_sources/example.rst.txt` & `llfuse-1.4.3/rst/example.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/doc/html/_sources/general.rst.txt` & `llfuse-1.4.3/rst/general.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/doc/html/_sources/gotchas.rst.txt` & `llfuse-1.4.3/rst/gotchas.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/doc/html/_sources/install.rst.txt` & `llfuse-1.4.3/rst/install.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/doc/html/_sources/lock.rst.txt` & `llfuse-1.4.3/rst/lock.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/examples/lltest.py` & `llfuse-1.4.3/examples/lltest.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/examples/passthroughfs.py` & `llfuse-1.4.3/examples/passthroughfs.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/examples/tmpfs.py` & `llfuse-1.4.3/examples/tmpfs.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/rst/conf.py` & `llfuse-1.4.3/rst/conf.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/setup.py` & `llfuse-1.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,24 +28,19 @@
     # We can't delete Cython.Distutils.build_ext directly,
     # because the build_ext class (that is imported from
     # the build_ext module in __init__.py) shadows the
     # build_ext module.
     module = sys.modules['Cython.Distutils.build_ext']
     del module.build_ext
 
-try:
-    import setuptools
-except ImportError:
-    raise SystemExit('Setuptools package not found. Please install from '
-                     'https://pypi.python.org/pypi/setuptools')
+import setuptools
 from setuptools import Extension
 from distutils.version import LooseVersion
 
-# Add util to load path
-basedir = os.path.abspath(os.path.dirname(sys.argv[0]))
+basedir = os.path.abspath(os.path.dirname(__file__))
 sys.path.insert(0, os.path.join(basedir, 'util'))
 
 # when running with DEVELOPER_MODE=1 in the environment:
 # enable all warnings, abort on some warnings.
 DEVELOPER_MODE = os.getenv('DEVELOPER_MODE', '0') == '1'
 if DEVELOPER_MODE:
     print('running in developer mode')
@@ -54,15 +49,15 @@
     # DeprecationWarning.
     warnings.simplefilter('default')
 
 # Add src to load path, important for Sphinx autodoc
 # to work properly
 sys.path.insert(0, os.path.join(basedir, 'src'))
 
-LLFUSE_VERSION = '1.4.2'
+LLFUSE_VERSION = '1.4.3'
 
 def main():
 
     try:
         from sphinx.application import Sphinx #pylint: disable-msg=W0612
     except ImportError:
         pass
@@ -131,14 +126,15 @@
                        'Programming Language :: Python :: 3.5',
                        'Programming Language :: Python :: 3.6',
                        'Programming Language :: Python :: 3.7',
                        'Programming Language :: Python :: 3.8',
                        'Programming Language :: Python :: 3.9',
                        'Programming Language :: Python :: 3.10',
                        'Programming Language :: Python :: 3.11',
+                       'Programming Language :: Python :: 3.12',
                        'Topic :: Software Development :: Libraries :: Python Modules',
                        'Topic :: System :: Filesystems',
                        'License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)',
                        'Operating System :: POSIX :: Linux',
                        'Operating System :: MacOS :: MacOS X',
                        'Operating System :: POSIX :: BSD :: FreeBSD'],
           platforms=[ 'Linux', 'FreeBSD', 'OS X' ],
@@ -224,15 +220,15 @@
                                               universal_newlines=True,
                                               stderr=subprocess.STDOUT)
         except OSError:
             raise SystemExit('Cython needs to be installed for this command')
 
         hit = re.match('^Cython version (.+)$', version)
         if not hit or LooseVersion(hit.group(1)) < "0.29":
-            # in fact, we need a very recent Cython version (like 0.29.21) to support py39
+            # in fact, we need a very recent Cython version to support the latest pythons
             raise SystemExit('Need Cython 0.29 or newer, found ' + version)
 
         cmd = ['cython', '-Wextra', '--force', '-3', '--fast-fail',
                '--directive', 'embedsignature=True', '--include-dir',
                os.path.join(basedir, 'Include'), '--verbose' ]
         if DEVELOPER_MODE:
             cmd.append('-Werror')
```

### Comparing `llfuse-1.4.2/src/darwin_compat.c` & `llfuse-1.4.3/src/darwin_compat.c`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/src/darwin_compat.h` & `llfuse-1.4.3/src/darwin_compat.h`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/src/fuse_api.pxi` & `llfuse-1.4.3/src/fuse_api.pxi`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/src/gettime.h` & `llfuse-1.4.3/src/gettime.h`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/src/handlers.pxi` & `llfuse-1.4.3/src/handlers.pxi`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/src/llfuse.c` & `llfuse-1.4.3/src/llfuse.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.30 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_30"
-#define CYTHON_HEX_VERSION 0x001D1EF0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -82,20 +83,21 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -128,18 +130,64 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -151,15 +199,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -190,15 +238,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -500,35 +548,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1382,26 +1430,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1681,20 +1729,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* decode_c_string_utf16.proto */
 static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
     int byteorder = 0;
     return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
 }
@@ -29803,15 +29859,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Lock, (type(self), 0xd41d8cd, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Lock__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6llfuse___pyx_unpickle_Lock__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Lock, (type(self), 0xd41d8cd, state)
@@ -30411,15 +30467,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_NoLockManager, (type(self), 0xd41d8cd, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_NoLockManager__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6llfuse___pyx_unpickle_NoLockManager__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_NoLockManager, (type(self), 0xd41d8cd, state)
@@ -31744,15 +31800,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_RequestContext, (type(self), 0x223b7a8, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_RequestContext__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6llfuse___pyx_unpickle_RequestContext__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_RequestContext, (type(self), 0x223b7a8, state)
@@ -37091,15 +37147,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_NotifyRequest, (type(self), 0x822d368, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_NotifyRequest__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6llfuse___pyx_unpickle_NotifyRequest__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_NotifyRequest, (type(self), 0x822d368, state)
@@ -44867,19 +44923,19 @@
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
-    goto __pyx_L20;
+    goto __pyx_L21;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L1_error;
-    __pyx_L20:;
+    __pyx_L21:;
   }
 
   /* "src/fuse_api.pxi":615
  *         else:
  *             raise RuntimeError("Unable to parse %s" % fh.name)
  *     gids = set()             # <<<<<<<<<<<<<<
  *     for x in line.split()[1:]:
@@ -45237,15 +45293,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Lock.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Lock__set_state(<Lock> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Lock__set_state(Lock __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_f_6llfuse___pyx_unpickle_Lock__set_state(((struct __pyx_obj_6llfuse_Lock *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(4, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = Lock.__new__(__pyx_type)
@@ -45620,15 +45676,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = NoLockManager.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_NoLockManager__set_state(<NoLockManager> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_NoLockManager__set_state(NoLockManager __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_f_6llfuse___pyx_unpickle_NoLockManager__set_state(((struct __pyx_obj_6llfuse_NoLockManager *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(4, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = NoLockManager.__new__(__pyx_type)
@@ -46003,15 +46059,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = RequestContext.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_RequestContext__set_state(<RequestContext> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_RequestContext__set_state(RequestContext __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_f_6llfuse___pyx_unpickle_RequestContext__set_state(((struct __pyx_obj_6llfuse_RequestContext *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(4, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x223b7a8, 0xe56624f, 0x8a019cd) = (gid, pid, uid, umask))" % __pyx_checksum)
  *     __pyx_result = RequestContext.__new__(__pyx_type)
@@ -46434,15 +46490,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = NotifyRequest.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_NotifyRequest__set_state(<NotifyRequest> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_NotifyRequest__set_state(NotifyRequest __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(4, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_f_6llfuse___pyx_unpickle_NotifyRequest__set_state(((struct __pyx_obj_6llfuse_NotifyRequest *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(4, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x822d368, 0x6efe08a, 0xd633613) = (attr_only, ino, kind, name))" % __pyx_checksum)
  *     __pyx_result = NotifyRequest.__new__(__pyx_type)
@@ -49536,15 +49592,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(5, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(5, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(5, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(5, 1, __pyx_L1_error)
   __pyx_int_5 = PyInt_FromLong(5); if (unlikely(!__pyx_int_5)) __PYX_ERR(5, 1, __pyx_L1_error)
   __pyx_int_30 = PyInt_FromLong(30); if (unlikely(!__pyx_int_30)) __PYX_ERR(5, 1, __pyx_L1_error)
   __pyx_int_1000 = PyInt_FromLong(1000); if (unlikely(!__pyx_int_1000)) __PYX_ERR(5, 1, __pyx_L1_error)
   __pyx_int_35895208 = PyInt_FromLong(35895208L); if (unlikely(!__pyx_int_35895208)) __PYX_ERR(5, 1, __pyx_L1_error)
   __pyx_int_116383882 = PyInt_FromLong(116383882L); if (unlikely(!__pyx_int_116383882)) __PYX_ERR(5, 1, __pyx_L1_error)
@@ -49710,17 +49766,17 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
@@ -49909,15 +49965,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(5, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(5, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(5, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(5, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(5, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(5, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(5, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_llfuse) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(5, 1, __pyx_L1_error)
@@ -51456,28 +51512,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -51586,15 +51642,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -51731,18 +51787,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* RaiseNoneIterError */
 static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
 }
 
@@ -52230,17 +52284,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -53341,17 +53393,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -53551,15 +53608,15 @@
         uval = NULL;
         if (uoffset > 0) {
             prepend_sign = !!prepend_sign;
             if (uoffset > prepend_sign) {
                 padding = PyUnicode_FromOrdinal(padding_char);
                 if (likely(padding) && uoffset > prepend_sign + 1) {
                     PyObject *tmp;
-                    PyObject *repeat = PyInt_FromSize_t(uoffset - prepend_sign);
+                    PyObject *repeat = PyInt_FromSsize_t(uoffset - prepend_sign);
                     if (unlikely(!repeat)) goto done_or_error;
                     tmp = PyNumber_Multiply(padding, repeat);
                     Py_DECREF(repeat);
                     Py_DECREF(padding);
                     padding = tmp;
                 }
                 if (unlikely(!padding)) goto done_or_error;
@@ -53968,44 +54025,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -54243,15 +54318,15 @@
 #else
     return PyObject_Call((PyObject*)&PyFrozenSet_Type, __pyx_empty_tuple, NULL);
 #endif
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `llfuse-1.4.2/src/llfuse.egg-info/PKG-INFO` & `llfuse-1.4.3/src/llfuse.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,15 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: llfuse
-Version: 1.4.2
+Version: 1.4.3
 Summary: Python bindings for the low-level FUSE API
 Home-page: https://github.com/python-llfuse/python-llfuse/
 Author: Nikolaus Rath
 Author-email: Nikolaus@rath.org
 License: LGPL
-Description: ..
-          NOTE: We cannot use sophisticated ReST syntax (like
-          e.g. :file:`foo`) here because this isn't rendered correctly
-          by PyPi.
-        
-        The Python-LLFUSE Module
-        ========================
-        
-        
-        .. start-intro
-        
-        **Warning - no longer developed!**
-        
-        Python-LLFUSE is no longer actively developed and just receiving
-        community-contributed maintenance to keep it alive for some time.
-        
-        Python-LLFUSE is a set of Python bindings for the low level FUSE_
-        API. It requires at least FUSE 2.8.0 and supports both Python 2.x and
-        3.x. Like FUSE itself, Python-LLFUSE is developed for Linux systems,
-        but it should be compatible with OS-X, FreeBSD and NetBSD as well.
-        
-        Python-LLFUSE releases can be downloaded from PyPi_. The documentation
-        can be `read online`__ and is also included in the ``doc/html``
-        directory of the Python-LLFUSE tarball.
-        
-        
-        Getting Help
-        ------------
-        
-        Please report any bugs on the `issue tracker`_. For discussion and
-        questions, please use the general `FUSE mailing list`_. A searchable
-        `mailing list archive`_ is kindly provided by Gmane_.
-        
-        
-        Contributing
-        ------------
-        
-        The Python-LLFUSE source code is available on GitHub_.
-        
-        
-        .. __: http://www.rath.org/llfuse-docs/
-        .. _FUSE: http://github.com/libfuse/libfuse
-        .. _FUSE mailing list: https://lists.sourceforge.net/lists/listinfo/fuse-devel
-        .. _issue tracker: https://github.com/python-llfuse/python-llfuse/issues
-        .. _mailing list archive: http://dir.gmane.org/gmane.comp.file-systems.fuse.devel
-        .. _Gmane: http://www.gmane.org/
-        .. _PyPi: https://pypi.python.org/pypi/llfuse/
-        .. _GitHub: https://github.com/python-llfuse/python-llfuse
-        
 Keywords: FUSE,python
 Platform: Linux
 Platform: FreeBSD
 Platform: OS X
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -66,15 +17,66 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Provides: llfuse
 Requires-Python: >=3.5
+License-File: LICENSE
+
+..
+  NOTE: We cannot use sophisticated ReST syntax (like
+  e.g. :file:`foo`) here because this isn't rendered correctly
+  by PyPi.
+
+The Python-LLFUSE Module
+========================
+
+
+.. start-intro
+
+**Warning - no longer developed!**
+
+Python-LLFUSE is no longer actively developed and just receiving
+community-contributed maintenance to keep it alive for some time.
+
+Python-LLFUSE is a set of Python bindings for the low level FUSE_
+API. It requires at least FUSE 2.8.0 and supports both Python 2.x and
+3.x. Like FUSE itself, Python-LLFUSE is developed for Linux systems,
+but it should be compatible with OS-X, FreeBSD and NetBSD as well.
+
+Python-LLFUSE releases can be downloaded from PyPi_. The documentation
+can be `read online`__ and is also included in the ``doc/html``
+directory of the Python-LLFUSE tarball.
+
+
+Getting Help
+------------
+
+Please report any bugs on the `issue tracker`_. For discussion and
+questions, please use the general `FUSE mailing list`_. A searchable
+`mailing list archive`_ is kindly provided by Gmane_.
+
+
+Contributing
+------------
+
+The Python-LLFUSE source code is available on GitHub_.
+
+
+.. __: http://www.rath.org/llfuse-docs/
+.. _FUSE: http://github.com/libfuse/libfuse
+.. _FUSE mailing list: https://lists.sourceforge.net/lists/listinfo/fuse-devel
+.. _issue tracker: https://github.com/python-llfuse/python-llfuse/issues
+.. _mailing list archive: http://dir.gmane.org/gmane.comp.file-systems.fuse.devel
+.. _Gmane: http://www.gmane.org/
+.. _PyPi: https://pypi.python.org/pypi/llfuse/
+.. _GitHub: https://github.com/python-llfuse/python-llfuse
```

### Comparing `llfuse-1.4.2/src/llfuse.h` & `llfuse-1.4.3/src/llfuse.h`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/src/llfuse.pyx` & `llfuse-1.4.3/src/llfuse.pyx`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/src/lock.c` & `llfuse-1.4.3/src/lock.c`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/src/macros.c` & `llfuse-1.4.3/src/macros.c`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/src/misc.pxi` & `llfuse-1.4.3/src/misc.pxi`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/src/operations.pxi` & `llfuse-1.4.3/src/operations.pxi`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/src/xattr.h` & `llfuse-1.4.3/src/xattr.h`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/test/.pytest_cache/v/cache/nodeids` & `llfuse-1.4.3/test/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/test/conftest.py` & `llfuse-1.4.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/test/pytest_checklogs.py` & `llfuse-1.4.3/test/pytest_checklogs.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/test/test_api.py` & `llfuse-1.4.3/test/test_api.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/test/test_examples.py` & `llfuse-1.4.3/test/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,16 +336,18 @@
     checked_unlink(filename, mnt_dir, isdir=True)
 
 def tst_rounding(mnt_dir, ns_tol=0):
     filename = os.path.join(mnt_dir, name_generator())
     os.mkdir(filename)
     fstat = os.lstat(filename)
 
-    # Approximately 100 years
-    secs = 100 * 365 * 24 * 3600 + 999
+    # Approximately 67 years, ending in 999.
+    # Note: 67 years were chosen to avoid y2038 issues (1970 + 67 = 2037).
+    #       Testing these is **not** in scope of this test.
+    secs = 67 * 365 * 24 * 3600 + 999
     # Max nanos
     nanos = _NANOS_PER_SEC - 1
 
     # seconds+ns and ns_tol as a float in seconds 
     secs_f = secs + nanos / _NANOS_PER_SEC
     secs_tol = ns_tol / _NANOS_PER_SEC
```

### Comparing `llfuse-1.4.2/test/test_fs.py` & `llfuse-1.4.3/test/test_fs.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/test/test_rounding.py` & `llfuse-1.4.3/test/test_rounding.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/test/util.py` & `llfuse-1.4.3/test/util.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.2/util/sphinx_cython.py` & `llfuse-1.4.3/util/sphinx_cython.py`

 * *Files identical despite different names*

