# Comparing `tmp/pyfuse3-3.2.2.tar.gz` & `tmp/pyfuse3-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyfuse3-3.2.2.tar", last modified: Wed Sep 28 00:02:23 2022, max compression
+gzip compressed data, was "dist/pyfuse3-3.2.3.tar", last modified: Tue May  9 18:44:17 2023, max compression
```

## Comparing `pyfuse3-3.2.2.tar` & `pyfuse3-3.2.3.tar`

### file list

```diff
@@ -1,131 +1,134 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/
--rw-r--r--   0 user      (1000) user      (1000)     2997 2022-09-27 23:49:26.000000 pyfuse3-3.2.2/Changes.rst
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/Include/
--rw-r--r--   0 user      (1000) user      (1000)     2676 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/Include/fuse_common.pxd
--rw-r--r--   0 user      (1000) user      (1000)     8270 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/Include/fuse_lowlevel.pxd
--rw-r--r--   0 user      (1000) user      (1000)      387 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/Include/fuse_opt.pxd
--rw-r--r--   0 user      (1000) user      (1000)     1603 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/Include/libc_extra.pxd
--rw-r--r--   0 user      (1000) user      (1000)    25960 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     3065 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1832 2022-09-27 23:49:26.000000 pyfuse3-3.2.2/README.rst
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/doc/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/doc/html/
--rw-r--r--   0 user      (1000) user      (1000)      230 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/.buildinfo
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/doc/html/_sources/
--rw-r--r--   0 user      (1000) user      (1000)       80 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/doc/html/_sources/about.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)      485 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/doc/html/_sources/asyncio.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)       28 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/doc/html/_sources/changes.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)     3953 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/doc/html/_sources/data.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)      809 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/doc/html/_sources/example.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)      583 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/doc/html/_sources/fuse_api.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)     3710 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/doc/html/_sources/general.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)      869 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/doc/html/_sources/gotchas.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)      407 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/doc/html/_sources/index.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)     2226 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/doc/html/_sources/install.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)     1257 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/doc/html/_sources/operations.rst.txt
--rw-r--r--   0 user      (1000) user      (1000)      407 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/doc/html/_sources/util.rst.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/doc/html/_static/
--rw-r--r--   0 user      (1000) user      (1000)     4418 2022-09-27 23:56:52.000000 pyfuse3-3.2.2/doc/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 user      (1000) user      (1000)    14810 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/_static/basic.css
--rw-r--r--   0 user      (1000) user      (1000)     4302 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/_static/classic.css
--rw-r--r--   0 user      (1000) user      (1000)       28 2022-09-27 23:56:52.000000 pyfuse3-3.2.2/doc/html/_static/default.css
--rw-r--r--   0 user      (1000) user      (1000)     4472 2022-09-27 23:56:52.000000 pyfuse3-3.2.2/doc/html/_static/doctools.js
--rw-r--r--   0 user      (1000) user      (1000)      420 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/_static/documentation_options.js
--rw-r--r--   0 user      (1000) user      (1000)      286 2022-09-27 23:56:52.000000 pyfuse3-3.2.2/doc/html/_static/file.png
--rw-r--r--   0 user      (1000) user      (1000)   288580 2022-09-27 23:56:52.000000 pyfuse3-3.2.2/doc/html/_static/jquery-3.6.0.js
--rw-r--r--   0 user      (1000) user      (1000)    89501 2022-09-27 23:56:52.000000 pyfuse3-3.2.2/doc/html/_static/jquery.js
--rw-r--r--   0 user      (1000) user      (1000)     4758 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/_static/language_data.js
--rw-r--r--   0 user      (1000) user      (1000)       90 2022-09-27 23:56:52.000000 pyfuse3-3.2.2/doc/html/_static/minus.png
--rw-r--r--   0 user      (1000) user      (1000)       90 2022-09-27 23:56:52.000000 pyfuse3-3.2.2/doc/html/_static/plus.png
--rw-r--r--   0 user      (1000) user      (1000)     4846 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/_static/pygments.css
--rw-r--r--   0 user      (1000) user      (1000)    18215 2022-09-27 23:56:52.000000 pyfuse3-3.2.2/doc/html/_static/searchtools.js
--rw-r--r--   0 user      (1000) user      (1000)     2540 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/_static/sidebar.js
--rw-r--r--   0 user      (1000) user      (1000)     4712 2022-09-27 23:56:52.000000 pyfuse3-3.2.2/doc/html/_static/sphinx_highlight.js
--rw-r--r--   0 user      (1000) user      (1000)    68420 2022-09-27 23:56:52.000000 pyfuse3-3.2.2/doc/html/_static/underscore-1.13.1.js
--rw-r--r--   0 user      (1000) user      (1000)    19530 2022-09-27 23:56:52.000000 pyfuse3-3.2.2/doc/html/_static/underscore.js
--rw-r--r--   0 user      (1000) user      (1000)     7703 2022-09-27 23:58:37.000000 pyfuse3-3.2.2/doc/html/about.html
--rw-r--r--   0 user      (1000) user      (1000)     6461 2022-09-27 23:58:37.000000 pyfuse3-3.2.2/doc/html/asyncio.html
--rw-r--r--   0 user      (1000) user      (1000)    12183 2022-09-27 23:58:37.000000 pyfuse3-3.2.2/doc/html/changes.html
--rw-r--r--   0 user      (1000) user      (1000)    29881 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/data.html
--rw-r--r--   0 user      (1000) user      (1000)   221890 2022-09-27 23:58:37.000000 pyfuse3-3.2.2/doc/html/example.html
--rw-r--r--   0 user      (1000) user      (1000)    27775 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/fuse_api.html
--rw-r--r--   0 user      (1000) user      (1000)    13528 2022-09-27 23:58:37.000000 pyfuse3-3.2.2/doc/html/general.html
--rw-r--r--   0 user      (1000) user      (1000)    19657 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/genindex.html
--rw-r--r--   0 user      (1000) user      (1000)     8989 2022-09-27 23:58:37.000000 pyfuse3-3.2.2/doc/html/gotchas.html
--rw-r--r--   0 user      (1000) user      (1000)     6808 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/index.html
--rw-r--r--   0 user      (1000) user      (1000)     9484 2022-09-27 23:58:37.000000 pyfuse3-3.2.2/doc/html/install.html
--rw-r--r--   0 user      (1000) user      (1000)     1166 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/objects.inv
--rw-r--r--   0 user      (1000) user      (1000)    90765 2022-09-27 23:58:38.000000 pyfuse3-3.2.2/doc/html/operations.html
--rw-r--r--   0 user      (1000) user      (1000)     4962 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/py-modindex.html
--rw-r--r--   0 user      (1000) user      (1000)     4717 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/search.html
--rw-r--r--   0 user      (1000) user      (1000)    31704 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/searchindex.js
--rw-r--r--   0 user      (1000) user      (1000)    12903 2022-09-27 23:59:28.000000 pyfuse3-3.2.2/doc/html/util.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/examples/
--rwxr-xr-x   0 user      (1000) user      (1000)     5169 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/examples/hello.py
--rwxr-xr-x   0 user      (1000) user      (1000)     5643 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/examples/hello_asyncio.py
--rwxr-xr-x   0 user      (1000) user      (1000)    17226 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/examples/passthroughfs.py
--rwxr-xr-x   0 user      (1000) user      (1000)    16707 2022-09-27 23:49:26.000000 pyfuse3-3.2.2/examples/tmpfs.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/rst/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/rst/_static/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/_static/.placeholder
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/rst/_templates/
--rw-r--r--   0 user      (1000) user      (1000)       93 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/_templates/localtoc.html
--rw-r--r--   0 user      (1000) user      (1000)       80 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/about.rst
--rw-r--r--   0 user      (1000) user      (1000)      485 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/asyncio.rst
--rw-r--r--   0 user      (1000) user      (1000)       28 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/changes.rst
--rw-r--r--   0 user      (1000) user      (1000)     6779 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/conf.py
--rw-r--r--   0 user      (1000) user      (1000)     3953 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/data.rst
--rw-r--r--   0 user      (1000) user      (1000)      809 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/example.rst
--rw-r--r--   0 user      (1000) user      (1000)      583 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/fuse_api.rst
--rw-r--r--   0 user      (1000) user      (1000)     3710 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/general.rst
--rw-r--r--   0 user      (1000) user      (1000)      869 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/gotchas.rst
--rw-r--r--   0 user      (1000) user      (1000)      407 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/index.rst
--rw-r--r--   0 user      (1000) user      (1000)     2226 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/install.rst
--rw-r--r--   0 user      (1000) user      (1000)     1257 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/operations.rst
--rw-r--r--   0 user      (1000) user      (1000)      407 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/rst/util.rst
--rw-r--r--   0 user      (1000) user      (1000)      143 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)    10105 2022-09-27 23:49:26.000000 pyfuse3-3.2.2/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/src/
--rw-r--r--   0 user      (1000) user      (1000)    24540 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/_pyfuse3.py
--rw-r--r--   0 user      (1000) user      (1000)     6145 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/darwin_compat.c
--rw-r--r--   0 user      (1000) user      (1000)     1376 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/darwin_compat.h
--rw-r--r--   0 user      (1000) user      (1000)      957 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/gettime.h
--rw-r--r--   0 user      (1000) user      (1000)    25446 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/handlers.pxi
--rw-r--r--   0 user      (1000) user      (1000)     8462 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/internal.pxi
--rw-r--r--   0 user      (1000) user      (1000)     1855 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/macros.c
--rw-r--r--   0 user      (1000) user      (1000)      806 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/macros.pxd
--rw-r--r--   0 user      (1000) user      (1000)  2447579 2022-09-27 23:52:37.000000 pyfuse3-3.2.2/src/pyfuse3.c
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/src/pyfuse3.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3065 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/src/pyfuse3.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2696 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/src/pyfuse3.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/src/pyfuse3.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       11 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/src/pyfuse3.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       33 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/src/pyfuse3.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-05-31 17:20:16.000000 pyfuse3-3.2.2/src/pyfuse3.egg-info/zip-safe
--rw-r--r--   0 user      (1000) user      (1000)      821 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/pyfuse3.h
--rw-r--r--   0 user      (1000) user      (1000)     2963 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/pyfuse3.pyi
--rw-r--r--   0 user      (1000) user      (1000)    32323 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/pyfuse3.pyx
--rw-r--r--   0 user      (1000) user      (1000)     2997 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/pyfuse3_asyncio.py
--rw-r--r--   0 user      (1000) user      (1000)     3494 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/src/xattr.h
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/test/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/test/.pytest_cache/
--rw-r--r--   0 user      (1000) user      (1000)       37 2022-05-31 17:54:44.000000 pyfuse3-3.2.2/test/.pytest_cache/.gitignore
--rw-r--r--   0 user      (1000) user      (1000)      191 2022-05-31 17:54:44.000000 pyfuse3-3.2.2/test/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 user      (1000) user      (1000)      302 2022-05-31 17:54:44.000000 pyfuse3-3.2.2/test/.pytest_cache/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/test/.pytest_cache/v/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/test/.pytest_cache/v/cache/
--rw-r--r--   0 user      (1000) user      (1000)       50 2022-05-31 19:52:11.000000 pyfuse3-3.2.2/test/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 user      (1000) user      (1000)      612 2022-05-31 19:52:11.000000 pyfuse3-3.2.2/test/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 user      (1000) user      (1000)        2 2022-05-31 19:52:11.000000 pyfuse3-3.2.2/test/.pytest_cache/v/cache/stepwise
--rwxr-xr-x   0 user      (1000) user      (1000)      346 2022-09-27 23:49:26.000000 pyfuse3-3.2.2/test/ci-install.sh
--rwxr-xr-x   0 user      (1000) user      (1000)      287 2022-09-27 23:49:26.000000 pyfuse3-3.2.2/test/ci-test.sh
--rw-r--r--   0 user      (1000) user      (1000)     3655 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/test/conftest.py
--rw-r--r--   0 user      (1000) user      (1000)       81 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/test/pytest.ini
--rw-r--r--   0 user      (1000) user      (1000)     3885 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/test/pytest_checklogs.py
--rwxr-xr-x   0 user      (1000) user      (1000)     2753 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/test/test_api.py
--rwxr-xr-x   0 user      (1000) user      (1000)    13505 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/test/test_examples.py
--rwxr-xr-x   0 user      (1000) user      (1000)     8760 2022-09-27 23:49:26.000000 pyfuse3-3.2.2/test/test_fs.py
--rwxr-xr-x   0 user      (1000) user      (1000)     1243 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/test/test_rounding.py
--rw-r--r--   0 user      (1000) user      (1000)     4302 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/test/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-28 00:02:23.000000 pyfuse3-3.2.2/util/
--rw-r--r--   0 user      (1000) user      (1000)     1038 2022-05-31 17:15:11.000000 pyfuse3-3.2.2/util/sphinx_cython.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:17.000000 pyfuse3-3.2.3/
+-rw-r--r--   0 user      (1000) user      (1000)     3543 2023-05-09 18:29:45.000000 pyfuse3-3.2.3/Changes.rst
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/Include/
+-rw-r--r--   0 user      (1000) user      (1000)     2676 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/Include/fuse_common.pxd
+-rw-r--r--   0 user      (1000) user      (1000)     8270 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/Include/fuse_lowlevel.pxd
+-rw-r--r--   0 user      (1000) user      (1000)      387 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/Include/fuse_opt.pxd
+-rw-r--r--   0 user      (1000) user      (1000)     1603 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/Include/libc_extra.pxd
+-rw-r--r--   0 user      (1000) user      (1000)    25960 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     3116 2023-05-09 18:44:17.000000 pyfuse3-3.2.3/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1832 2022-09-27 23:49:26.000000 pyfuse3-3.2.3/README.rst
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/doc/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/doc/html/
+-rw-r--r--   0 user      (1000) user      (1000)      230 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/.buildinfo
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/doc/html/_sources/
+-rw-r--r--   0 user      (1000) user      (1000)       80 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/doc/html/_sources/about.rst.txt
+-rw-r--r--   0 user      (1000) user      (1000)      485 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/doc/html/_sources/asyncio.rst.txt
+-rw-r--r--   0 user      (1000) user      (1000)       28 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/doc/html/_sources/changes.rst.txt
+-rw-r--r--   0 user      (1000) user      (1000)     3953 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/doc/html/_sources/data.rst.txt
+-rw-r--r--   0 user      (1000) user      (1000)      809 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/doc/html/_sources/example.rst.txt
+-rw-r--r--   0 user      (1000) user      (1000)      583 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/doc/html/_sources/fuse_api.rst.txt
+-rw-r--r--   0 user      (1000) user      (1000)     3710 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/doc/html/_sources/general.rst.txt
+-rw-r--r--   0 user      (1000) user      (1000)      869 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/doc/html/_sources/gotchas.rst.txt
+-rw-r--r--   0 user      (1000) user      (1000)      407 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/doc/html/_sources/index.rst.txt
+-rw-r--r--   0 user      (1000) user      (1000)     2226 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/doc/html/_sources/install.rst.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1257 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/doc/html/_sources/operations.rst.txt
+-rw-r--r--   0 user      (1000) user      (1000)      407 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/doc/html/_sources/util.rst.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/doc/html/_static/
+-rw-r--r--   0 user      (1000) user      (1000)     4418 2022-09-27 23:56:52.000000 pyfuse3-3.2.3/doc/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 user      (1000) user      (1000)    14810 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/_static/basic.css
+-rw-r--r--   0 user      (1000) user      (1000)     4302 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/_static/classic.css
+-rw-r--r--   0 user      (1000) user      (1000)       28 2022-09-27 23:56:52.000000 pyfuse3-3.2.3/doc/html/_static/default.css
+-rw-r--r--   0 user      (1000) user      (1000)     4472 2022-09-27 23:56:52.000000 pyfuse3-3.2.3/doc/html/_static/doctools.js
+-rw-r--r--   0 user      (1000) user      (1000)      420 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/_static/documentation_options.js
+-rw-r--r--   0 user      (1000) user      (1000)      286 2022-09-27 23:56:52.000000 pyfuse3-3.2.3/doc/html/_static/file.png
+-rw-r--r--   0 user      (1000) user      (1000)   288580 2022-09-27 23:56:52.000000 pyfuse3-3.2.3/doc/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 user      (1000) user      (1000)    89501 2022-09-27 23:56:52.000000 pyfuse3-3.2.3/doc/html/_static/jquery.js
+-rw-r--r--   0 user      (1000) user      (1000)     4758 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/_static/language_data.js
+-rw-r--r--   0 user      (1000) user      (1000)       90 2022-09-27 23:56:52.000000 pyfuse3-3.2.3/doc/html/_static/minus.png
+-rw-r--r--   0 user      (1000) user      (1000)       90 2022-09-27 23:56:52.000000 pyfuse3-3.2.3/doc/html/_static/plus.png
+-rw-r--r--   0 user      (1000) user      (1000)     4846 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/_static/pygments.css
+-rw-r--r--   0 user      (1000) user      (1000)    18215 2022-09-27 23:56:52.000000 pyfuse3-3.2.3/doc/html/_static/searchtools.js
+-rw-r--r--   0 user      (1000) user      (1000)     2540 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/_static/sidebar.js
+-rw-r--r--   0 user      (1000) user      (1000)     4712 2022-09-27 23:56:52.000000 pyfuse3-3.2.3/doc/html/_static/sphinx_highlight.js
+-rw-r--r--   0 user      (1000) user      (1000)    68420 2022-09-27 23:56:52.000000 pyfuse3-3.2.3/doc/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 user      (1000) user      (1000)    19530 2022-09-27 23:56:52.000000 pyfuse3-3.2.3/doc/html/_static/underscore.js
+-rw-r--r--   0 user      (1000) user      (1000)     7703 2023-05-09 18:35:21.000000 pyfuse3-3.2.3/doc/html/about.html
+-rw-r--r--   0 user      (1000) user      (1000)     6461 2023-05-09 18:35:21.000000 pyfuse3-3.2.3/doc/html/asyncio.html
+-rw-r--r--   0 user      (1000) user      (1000)    12991 2023-05-09 18:35:21.000000 pyfuse3-3.2.3/doc/html/changes.html
+-rw-r--r--   0 user      (1000) user      (1000)    29881 2023-05-09 18:36:01.000000 pyfuse3-3.2.3/doc/html/data.html
+-rw-r--r--   0 user      (1000) user      (1000)   221890 2023-05-09 18:35:21.000000 pyfuse3-3.2.3/doc/html/example.html
+-rw-r--r--   0 user      (1000) user      (1000)    27783 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/fuse_api.html
+-rw-r--r--   0 user      (1000) user      (1000)    13528 2023-05-09 18:35:21.000000 pyfuse3-3.2.3/doc/html/general.html
+-rw-r--r--   0 user      (1000) user      (1000)    19657 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/genindex.html
+-rw-r--r--   0 user      (1000) user      (1000)     8989 2023-05-09 18:35:21.000000 pyfuse3-3.2.3/doc/html/gotchas.html
+-rw-r--r--   0 user      (1000) user      (1000)     6808 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/index.html
+-rw-r--r--   0 user      (1000) user      (1000)     9484 2023-05-09 18:35:21.000000 pyfuse3-3.2.3/doc/html/install.html
+-rw-r--r--   0 user      (1000) user      (1000)     1166 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/objects.inv
+-rw-r--r--   0 user      (1000) user      (1000)    90765 2023-05-09 18:35:21.000000 pyfuse3-3.2.3/doc/html/operations.html
+-rw-r--r--   0 user      (1000) user      (1000)     4962 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/py-modindex.html
+-rw-r--r--   0 user      (1000) user      (1000)     4717 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/search.html
+-rw-r--r--   0 user      (1000) user      (1000)    32010 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/searchindex.js
+-rw-r--r--   0 user      (1000) user      (1000)    12903 2023-05-09 18:36:02.000000 pyfuse3-3.2.3/doc/html/util.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/examples/
+-rwxr-xr-x   0 user      (1000) user      (1000)     5169 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/examples/hello.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     5643 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/examples/hello_asyncio.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    17226 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/examples/passthroughfs.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    16707 2022-09-27 23:49:26.000000 pyfuse3-3.2.3/examples/tmpfs.py
+-rw-r--r--   0 user      (1000) user      (1000)       81 2023-05-09 18:26:01.000000 pyfuse3-3.2.3/pyproject.toml
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/rst/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/rst/_static/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/_static/.placeholder
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/rst/_templates/
+-rw-r--r--   0 user      (1000) user      (1000)       93 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/_templates/localtoc.html
+-rw-r--r--   0 user      (1000) user      (1000)       80 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/about.rst
+-rw-r--r--   0 user      (1000) user      (1000)      485 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/asyncio.rst
+-rw-r--r--   0 user      (1000) user      (1000)       28 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/changes.rst
+-rw-r--r--   0 user      (1000) user      (1000)     6779 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/conf.py
+-rw-r--r--   0 user      (1000) user      (1000)     3953 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/data.rst
+-rw-r--r--   0 user      (1000) user      (1000)      809 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/example.rst
+-rw-r--r--   0 user      (1000) user      (1000)      583 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/fuse_api.rst
+-rw-r--r--   0 user      (1000) user      (1000)     3710 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/general.rst
+-rw-r--r--   0 user      (1000) user      (1000)      869 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/gotchas.rst
+-rw-r--r--   0 user      (1000) user      (1000)      407 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/index.rst
+-rw-r--r--   0 user      (1000) user      (1000)     2226 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/install.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1257 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/operations.rst
+-rw-r--r--   0 user      (1000) user      (1000)      407 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/rst/util.rst
+-rw-r--r--   0 user      (1000) user      (1000)      143 2023-05-09 18:44:17.000000 pyfuse3-3.2.3/setup.cfg
+-rwxr-xr-x   0 user      (1000) user      (1000)    10107 2023-05-09 18:29:45.000000 pyfuse3-3.2.3/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/src/
+-rw-r--r--   0 user      (1000) user      (1000)    24540 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/_pyfuse3.py
+-rw-r--r--   0 user      (1000) user      (1000)     6145 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/darwin_compat.c
+-rw-r--r--   0 user      (1000) user      (1000)     1376 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/darwin_compat.h
+-rw-r--r--   0 user      (1000) user      (1000)      957 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/gettime.h
+-rw-r--r--   0 user      (1000) user      (1000)    25446 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/handlers.pxi
+-rw-r--r--   0 user      (1000) user      (1000)     8462 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/internal.pxi
+-rw-r--r--   0 user      (1000) user      (1000)     1855 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/macros.c
+-rw-r--r--   0 user      (1000) user      (1000)      806 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/macros.pxd
+-rw-r--r--   0 user      (1000) user      (1000)  2450394 2023-05-09 18:31:00.000000 pyfuse3-3.2.3/src/pyfuse3.c
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:17.000000 pyfuse3-3.2.3/src/pyfuse3.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3116 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/src/pyfuse3.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2744 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/src/pyfuse3.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/src/pyfuse3.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       11 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/src/pyfuse3.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       33 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/src/pyfuse3.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2022-05-31 17:20:16.000000 pyfuse3-3.2.3/src/pyfuse3.egg-info/zip-safe
+-rw-r--r--   0 user      (1000) user      (1000)      821 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/pyfuse3.h
+-rw-r--r--   0 user      (1000) user      (1000)     2963 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/pyfuse3.pyi
+-rw-r--r--   0 user      (1000) user      (1000)    32323 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/pyfuse3.pyx
+-rw-r--r--   0 user      (1000) user      (1000)     2997 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/pyfuse3_asyncio.py
+-rw-r--r--   0 user      (1000) user      (1000)     3494 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/src/xattr.h
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:17.000000 pyfuse3-3.2.3/test/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:17.000000 pyfuse3-3.2.3/test/.pytest_cache/
+-rw-r--r--   0 user      (1000) user      (1000)       37 2022-05-31 17:54:44.000000 pyfuse3-3.2.3/test/.pytest_cache/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)      191 2022-05-31 17:54:44.000000 pyfuse3-3.2.3/test/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 user      (1000) user      (1000)      302 2022-05-31 17:54:44.000000 pyfuse3-3.2.3/test/.pytest_cache/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:16.000000 pyfuse3-3.2.3/test/.pytest_cache/v/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:17.000000 pyfuse3-3.2.3/test/.pytest_cache/v/cache/
+-rw-r--r--   0 user      (1000) user      (1000)       50 2022-05-31 19:52:11.000000 pyfuse3-3.2.3/test/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 user      (1000) user      (1000)      612 2022-05-31 19:52:11.000000 pyfuse3-3.2.3/test/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 user      (1000) user      (1000)        2 2022-05-31 19:52:11.000000 pyfuse3-3.2.3/test/.pytest_cache/v/cache/stepwise
+-rwxr-xr-x   0 user      (1000) user      (1000)      365 2023-05-09 18:26:01.000000 pyfuse3-3.2.3/test/ci-install.sh
+-rwxr-xr-x   0 user      (1000) user      (1000)      287 2022-09-27 23:49:26.000000 pyfuse3-3.2.3/test/ci-test.sh
+-rw-r--r--   0 user      (1000) user      (1000)     3655 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/test/conftest.py
+-rw-r--r--   0 user      (1000) user      (1000)       81 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/test/pytest.ini
+-rw-r--r--   0 user      (1000) user      (1000)     3885 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/test/pytest_checklogs.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     2753 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/test/test_api.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    13654 2023-05-09 18:26:01.000000 pyfuse3-3.2.3/test/test_examples.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     8760 2022-09-27 23:49:26.000000 pyfuse3-3.2.3/test/test_fs.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     1243 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/test/test_rounding.py
+-rw-r--r--   0 user      (1000) user      (1000)     4149 2023-05-09 18:26:01.000000 pyfuse3-3.2.3/test/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 18:44:17.000000 pyfuse3-3.2.3/util/
+-rwxr-xr-x   0 user      (1000) user      (1000)      308 2023-05-09 18:43:50.000000 pyfuse3-3.2.3/util/sdist-sign
+-rw-r--r--   0 user      (1000) user      (1000)     1038 2022-05-31 17:15:11.000000 pyfuse3-3.2.3/util/sphinx_cython.py
+-rwxr-xr-x   0 user      (1000) user      (1000)      278 2023-05-09 18:43:34.000000 pyfuse3-3.2.3/util/upload-pypi
```

### Comparing `pyfuse3-3.2.2/Changes.rst` & `pyfuse3-3.2.3/Changes.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 ===========
  Changelog
 ===========
 
 .. currentmodule:: pyfuse3
 
+Release 3.2.3 (2023-05-09)
+==========================
+
+* cythonize with latest Cython 0.29.34 (brings Python 3.12 support)
+
+* add a minimal pyproject.toml, require setuptools
+
+* tests: fix integer overflow on 32-bit arches, fixes #47
+
+* test: Use shutil.which() instead of external which(1) program
+
+* setup.py: catch more generic OSError when searching Cython, fixes #63
+
+* setup.py: require Cython >= 0.29
+
+* fix basedir computation in setup.py (fix pip install -e .)
+
+* use sphinx < 6.0 due to compatibility issues with more recent versions
+
+
 Release 3.2.2 (2022-09-28)
 ==========================
 
 * remove support for python 3.5 (broken, out of support by python devs)
 
 * cythonize with latest Cython 0.29.x (brings Python 3.11 support)
```

### Comparing `pyfuse3-3.2.2/Include/fuse_common.pxd` & `pyfuse3-3.2.3/Include/fuse_common.pxd`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/Include/fuse_lowlevel.pxd` & `pyfuse3-3.2.3/Include/fuse_lowlevel.pxd`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/Include/libc_extra.pxd` & `pyfuse3-3.2.3/Include/libc_extra.pxd`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/LICENSE` & `pyfuse3-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/PKG-INFO` & `pyfuse3-3.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfuse3
-Version: 3.2.2
+Version: 3.2.3
 Summary: Python 3 bindings for libfuse 3 with async I/O support
 Home-page: https://github.com/libfuse/pyfuse3
 Author: Nikolaus Rath
 Author-email: Nikolaus@rath.org
 License: LGPL
 Keywords: FUSE,python
 Platform: Linux
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
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
 Classifier: Typing :: Typed
```

### Comparing `pyfuse3-3.2.2/README.rst` & `pyfuse3-3.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_sources/data.rst.txt` & `pyfuse3-3.2.3/doc/html/_sources/data.rst.txt`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_sources/example.rst.txt` & `pyfuse3-3.2.3/doc/html/_sources/example.rst.txt`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_sources/fuse_api.rst.txt` & `pyfuse3-3.2.3/doc/html/_sources/fuse_api.rst.txt`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_sources/general.rst.txt` & `pyfuse3-3.2.3/doc/html/_sources/general.rst.txt`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_sources/gotchas.rst.txt` & `pyfuse3-3.2.3/doc/html/_sources/gotchas.rst.txt`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_sources/install.rst.txt` & `pyfuse3-3.2.3/doc/html/_sources/install.rst.txt`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_sources/operations.rst.txt` & `pyfuse3-3.2.3/doc/html/_sources/operations.rst.txt`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/_sphinx_javascript_frameworks_compat.js` & `pyfuse3-3.2.3/doc/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/basic.css` & `pyfuse3-3.2.3/doc/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/classic.css` & `pyfuse3-3.2.3/doc/html/_static/classic.css`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/doctools.js` & `pyfuse3-3.2.3/doc/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/jquery-3.6.0.js` & `pyfuse3-3.2.3/doc/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/jquery.js` & `pyfuse3-3.2.3/doc/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/language_data.js` & `pyfuse3-3.2.3/doc/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/pygments.css` & `pyfuse3-3.2.3/doc/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/searchtools.js` & `pyfuse3-3.2.3/doc/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/sidebar.js` & `pyfuse3-3.2.3/doc/html/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/sphinx_highlight.js` & `pyfuse3-3.2.3/doc/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/underscore-1.13.1.js` & `pyfuse3-3.2.3/doc/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/_static/underscore.js` & `pyfuse3-3.2.3/doc/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/doc/html/about.html` & `pyfuse3-3.2.3/doc/html/about.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>About &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>About &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -34,15 +34,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="install.html" title="Installation"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="pyfuse3 Documentation"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">About</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -131,15 +131,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="install.html" title="Installation"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="pyfuse3 Documentation"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">About</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * About
 ****** AboutÂ¶ ******
 pyfuse3 is a set of Python 3 bindings for libfuse_3. It provides an
 asynchronous API compatible with Trio and asyncio, and enables you to easily
 write a full-featured Linux filesystem in Python.
 pyfuse3 releases can be downloaded from PyPi. The documentation can be read
 online and is also included in the doc/html directory of the pyfuse3 tarball.
@@ -51,10 +51,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * About
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/asyncio.html` & `pyfuse3-3.2.3/doc/html/asyncio.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>asyncio Support &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>asyncio Support &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -34,15 +34,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="fuse_api.html" title="FUSE API Functions"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="general.html" title="General Information"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">asyncio Support</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -120,15 +120,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="fuse_api.html" title="FUSE API Functions"
              >next</a> |</li>
         <li class="right" >
           <a href="general.html" title="General Information"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">asyncio Support</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * asyncio Support
 ****** asyncio SupportÂ¶ ******
 By default, pyfuse3 uses asynchronous I/O using Trio (and most of the
 documentation assumes that you are using Trio). If youâd rather use asyncio,
 import the pyfuse3_asyncio module and call its enable() function before using
 pyfuse3. For example:
 import pyfuse3
@@ -43,10 +43,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * asyncio Support
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/changes.html` & `pyfuse3-3.2.3/doc/html/changes.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Changelog &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>Changelog &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -30,26 +30,39 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="example.html" title="Example File Systems"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
   <section id="changelog">
 <h1>Changelog<a class="headerlink" href="#changelog" title="Permalink to this heading">¶</a></h1>
+<section id="release-3-2-3-2023-05-09">
+<h2>Release 3.2.3 (2023-05-09)<a class="headerlink" href="#release-3-2-3-2023-05-09" title="Permalink to this heading">¶</a></h2>
+<ul class="simple">
+<li><p>cythonize with latest Cython 0.29.34 (brings Python 3.12 support)</p></li>
+<li><p>add a minimal pyproject.toml, require setuptools</p></li>
+<li><p>tests: fix integer overflow on 32-bit arches, fixes #47</p></li>
+<li><p>test: Use shutil.which() instead of external which(1) program</p></li>
+<li><p>setup.py: catch more generic OSError when searching Cython, fixes #63</p></li>
+<li><p>setup.py: require Cython &gt;= 0.29</p></li>
+<li><p>fix basedir computation in setup.py (fix pip install -e .)</p></li>
+<li><p>use sphinx &lt; 6.0 due to compatibility issues with more recent versions</p></li>
+</ul>
+</section>
 <section id="release-3-2-2-2022-09-28">
 <h2>Release 3.2.2 (2022-09-28)<a class="headerlink" href="#release-3-2-2-2022-09-28" title="Permalink to this heading">¶</a></h2>
 <ul class="simple">
 <li><p>remove support for python 3.5 (broken, out of support by python devs)</p></li>
 <li><p>cythonize with latest Cython 0.29.x (brings Python 3.11 support)</p></li>
 <li><p>use github actions for CI, remove travis-ci</p></li>
 <li><p>update README: minimal maintenance, not developed</p></li>
@@ -97,15 +110,15 @@
 on the old behavior needs to be changed.</p>
 </li>
 </ul>
 </section>
 <section id="release-2-0-0">
 <h2>Release 2.0.0<a class="headerlink" href="#release-2-0-0" title="Permalink to this heading">¶</a></h2>
 <ul>
-<li><p>Changed <a class="reference external" href="https://docs.python.org/3/library/functions.html#open" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">open</span></code></a> handler to return the new <a class="reference internal" href="data.html#pyfuse3.FileInfo" title="pyfuse3.FileInfo"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FileInfo</span></code></a> struct to allow for
+<li><p>Changed <a class="reference external" href="https://docs.python.org/3/library/functions.html#open" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">open</span></code></a> handler to return the new <a class="reference internal" href="data.html#pyfuse3.FileInfo" title="pyfuse3.FileInfo"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FileInfo</span></code></a> struct to allow for
 modification of certain kernel file attributes, e.g. <code class="docutils literal notranslate"><span class="pre">direct_io</span></code>.</p>
 <p>Note that this change breaks backwards compatibility, code that depends on the old
 behavior needs to be changed.</p>
 </li>
 </ul>
 </section>
 <section id="release-1-3-1-2019-07-17">
@@ -203,15 +216,15 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="example.html" title="Example File Systems"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -5,17 +5,27 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Changelog
 ****** ChangelogÂ¶ ******
+***** Release 3.2.3 (2023-05-09)Â¶ *****
+    * cythonize with latest Cython 0.29.34 (brings Python 3.12 support)
+    * add a minimal pyproject.toml, require setuptools
+    * tests: fix integer overflow on 32-bit arches, fixes #47
+    * test: Use shutil.which() instead of external which(1) program
+    * setup.py: catch more generic OSError when searching Cython, fixes #63
+    * setup.py: require Cython >= 0.29
+    * fix basedir computation in setup.py (fix pip install -e .)
+    * use sphinx < 6.0 due to compatibility issues with more recent versions
+
 ***** Release 3.2.2 (2022-09-28)Â¶ *****
     * remove support for python 3.5 (broken, out of support by python devs)
     * cythonize with latest Cython 0.29.x (brings Python 3.11 support)
     * use github actions for CI, remove travis-ci
     * update README: minimal maintenance, not developed
     * update setup.py with tested python versions
     * examples/tmpfs.py: work around strange kernel behaviour (calling SETATTR
@@ -94,10 +104,10 @@
 Example_File_Systems
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Changelog
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/data.html` & `pyfuse3-3.2.3/doc/html/data.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Data Structures &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>Data Structures &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -34,30 +34,30 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="operations.html" title="Request Handlers"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="fuse_api.html" title="FUSE API Functions"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Data Structures</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
   <section id="data-structures">
 <h1>Data Structures<a class="headerlink" href="#data-structures" title="Permalink to this heading">¶</a></h1>
 <dl class="py data">
 <dt class="sig sig-object py" id="pyfuse3.ENOATTR">
 <span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">ENOATTR</span></span><a class="headerlink" href="#pyfuse3.ENOATTR" title="Permalink to this definition">¶</a></dt>
-<dd><p>This errorcode is unfortunately missing in the <a class="reference external" href="https://docs.python.org/3/library/errno.html#module-errno" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">errno</span></code></a> module,
+<dd><p>This errorcode is unfortunately missing in the <a class="reference external" href="https://docs.python.org/3/library/errno.html#module-errno" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">errno</span></code></a> module,
 so it is provided by pyfuse3 instead.</p>
 </dd></dl>
 
 <dl class="py data">
 <dt class="sig sig-object py" id="pyfuse3.ROOT_INODE">
 <span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">ROOT_INODE</span></span><a class="headerlink" href="#pyfuse3.ROOT_INODE" title="Permalink to this definition">¶</a></dt>
 <dd><p>The inode of the root directory, i.e. the mount point of the file
@@ -430,15 +430,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="operations.html" title="Request Handlers"
              >next</a> |</li>
         <li class="right" >
           <a href="fuse_api.html" title="FUSE API Functions"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Data Structures</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Data Structures
 ****** Data StructuresÂ¶ ******
   pyfuse3.ENOATTRÂ¶
       This errorcode is unfortunately missing in the errno module, so it is
       provided by pyfuse3 instead.
   pyfuse3.ROOT_INODEÂ¶
       The inode of the root directory, i.e. the mount point of the file system.
@@ -145,10 +145,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Data Structures
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/example.html` & `pyfuse3-3.2.3/doc/html/example.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Example File Systems &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>Example File Systems &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -34,15 +34,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changes.html" title="Changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="gotchas.html" title="Common Gotchas"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Example File Systems</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -1226,15 +1226,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changes.html" title="Changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="gotchas.html" title="Common Gotchas"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Example File Systems</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Example File Systems
 ****** Example File SystemsÂ¶ ******
 pyfuse3 comes with several example file systems in the examples directory of
 the release tarball. For completeness, these examples are also included here.
 ***** Single-file, Read-only File SystemÂ¶ *****
 (shipped as examples/lltest.py)
   1#!/usr/bin/env python3
@@ -1200,10 +1200,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Example File Systems
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/fuse_api.html` & `pyfuse3-3.2.3/doc/html/fuse_api.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>FUSE API Functions &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>FUSE API Functions &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -34,15 +34,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="data.html" title="Data Structures"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="asyncio.html" title="asyncio Support"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">FUSE API Functions</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -81,15 +81,15 @@
 <dl class="py function">
 <dt class="sig sig-object py" id="pyfuse3.terminate">
 <span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">terminate</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#pyfuse3.terminate" title="Permalink to this definition">¶</a></dt>
 <dd><p>Terminate FUSE main loop.</p>
 <p>This function gracefully terminates the FUSE main loop (resulting in the call to
 main() to return).</p>
 <p>When called by a thread different from the one that runs the main loop, the call must
-be wrapped with <a class="reference external" href="https://trio.readthedocs.io/en/stable/reference-core.html#trio.from_thread.run_sync" title="(in Trio v0.21.0)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">trio.from_thread.run_sync</span></code></a>. The necessary <em>trio_token</em> argument can
+be wrapped with <a class="reference external" href="https://trio.readthedocs.io/en/stable/reference-core.html#trio.from_thread.run_sync" title="(in Trio v0.21.0+dev)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">trio.from_thread.run_sync</span></code></a>. The necessary <em>trio_token</em> argument can
 (for convience) be retrieved from the <a class="reference internal" href="#pyfuse3.trio_token" title="pyfuse3.trio_token"><code class="xref py py-obj docutils literal notranslate"><span class="pre">trio_token</span></code></a> module attribute.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="pyfuse3.close">
 <span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">close</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">unmount</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#pyfuse3.close" title="Permalink to this definition">¶</a></dt>
 <dd><p>Clean up and ensure filesystem is unmounted</p>
@@ -115,15 +115,15 @@
 data (unless <em>attr_only</em> is True) for <em>inode</em>.</p>
 <p><strong>This operation may block</strong> if writeback caching is active and there is
 dirty data for the inode that is to be invalidated. Unfortunately there is
 no way to return control to the event loop until writeback is complete
 (leading to a deadlock if the necessary write() requests cannot be processed
 by the filesystem). Unless writeback caching is disabled, this function
 should therefore be called from a separate thread.</p>
-<p>If the operation is not supported by the kernel, raises <a class="reference external" href="https://docs.python.org/3/library/exceptions.html#OSError" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">OSError</span></code></a>
+<p>If the operation is not supported by the kernel, raises <a class="reference external" href="https://docs.python.org/3/library/exceptions.html#OSError" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">OSError</span></code></a>
 with errno ENOSYS.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="pyfuse3.invalidate_entry">
 <span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">invalidate_entry</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fuse_ino_t</span> <span class="pre">inode_p</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fuse_ino_t</span> <span class="pre">deleted=0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#pyfuse3.invalidate_entry" title="Permalink to this definition">¶</a></dt>
 <dd><p>Invalidate directory entry</p>
@@ -164,30 +164,30 @@
 logged though).</p>
 <p>The directory entries that are to be invalidated are put in an unbounded
 queue which is processed by a single thread. This means that if the entry at
 the beginning of the queue cannot be invalidated yet because a related file
 system operation is still in progress, none of the other entries will be
 processed and repeated calls to this function will result in continued
 growth of the queue.</p>
-<p>If there are errors, an exception is logged using the <a class="reference external" href="https://docs.python.org/3/library/logging.html#module-logging" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">logging</span></code></a> module.</p>
+<p>If there are errors, an exception is logged using the <a class="reference external" href="https://docs.python.org/3/library/logging.html#module-logging" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">logging</span></code></a> module.</p>
 <p>If <em>ignore_enoent</em> is True, ignore ENOENT errors (which occur if the
 kernel doesn’t actually have knowledge of the entry that is to be
 removed).</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="pyfuse3.notify_store">
 <span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">notify_store</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">offset</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">data</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#pyfuse3.notify_store" title="Permalink to this definition">¶</a></dt>
 <dd><p>Store data in kernel page cache</p>
 <p>Sends <em>data</em> for the kernel to store it in the page cache for <em>inode</em> at
 <em>offset</em>. If this provides data beyond the current file size, the file is
 automatically extended.</p>
 <p>If this function raises an exception, the store may still have completed
 partially.</p>
-<p>If the operation is not supported by the kernel, raises <a class="reference external" href="https://docs.python.org/3/library/exceptions.html#OSError" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">OSError</span></code></a>
+<p>If the operation is not supported by the kernel, raises <a class="reference external" href="https://docs.python.org/3/library/exceptions.html#OSError" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">OSError</span></code></a>
 with errno ENOSYS.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="pyfuse3.readdir_reply">
 <span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">readdir_reply</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ReaddirToken</span> <span class="pre">token</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">EntryAttributes</span> <span class="pre">attr</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">off_t</span> <span class="pre">next_id</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#pyfuse3.readdir_reply" title="Permalink to this definition">¶</a></dt>
 <dd><p>Report a directory entry in response to a <a class="reference internal" href="operations.html#pyfuse3.Operations.readdir" title="pyfuse3.Operations.readdir"><code class="xref py py-obj docutils literal notranslate"><span class="pre">readdir</span></code></a> request.</p>
@@ -210,15 +210,15 @@
 </dd></dl>
 
 <dl class="py data">
 <dt class="sig sig-object py" id="pyfuse3.trio_token">
 <span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">trio_token</span></span><a class="headerlink" href="#pyfuse3.trio_token" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set to the value returned by <code class="xref py py-obj docutils literal notranslate"><span class="pre">trio.lowlevel.current_trio_token()</span></code> while <a class="reference internal" href="#pyfuse3.main" title="pyfuse3.main"><code class="xref py py-obj docutils literal notranslate"><span class="pre">main()</span></code></a> is
 running. Can be used by other threads to run code in the main loop through
-<a class="reference external" href="https://trio.readthedocs.io/en/stable/reference-core.html#trio.from_thread.run" title="(in Trio v0.21.0)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">trio.from_thread.run</span></code></a>.</p>
+<a class="reference external" href="https://trio.readthedocs.io/en/stable/reference-core.html#trio.from_thread.run" title="(in Trio v0.21.0+dev)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">trio.from_thread.run</span></code></a>.</p>
 </dd></dl>
 
 </section>
 
 
             <div class="clearer"></div>
           </div>
@@ -275,15 +275,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="data.html" title="Data Structures"
              >next</a> |</li>
         <li class="right" >
           <a href="asyncio.html" title="asyncio Support"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">FUSE API Functions</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * FUSE API Functions
 ****** FUSE API FunctionsÂ¶ ******
   pyfuse3.init(ops, mountpoint, options=default_options)Â¶
       Initialize and mount FUSE file system
       ops has to be an instance of the Operations class (or another class
       defining the same methods).
       args has to be a set of strings. default_options provides some reasonable
@@ -151,10 +151,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * FUSE API Functions
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/general.html` & `pyfuse3-3.2.3/doc/html/general.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>General Information &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>General Information &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -34,15 +34,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="asyncio.html" title="asyncio Support"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="install.html" title="Installation"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">General Information</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -65,16 +65,16 @@
 before, please read the <a class="reference external" href="https://trio.readthedocs.io/en/latest/tutorial.html">Trio tutorial</a> first.</p>
 <p>An instance of the operations class is passed to <a class="reference internal" href="fuse_api.html#pyfuse3.init" title="pyfuse3.init"><code class="xref py py-obj docutils literal notranslate"><span class="pre">pyfuse3.init</span></code></a> to
 mount the file system. To enter the request handling loop, run
 <a class="reference internal" href="fuse_api.html#pyfuse3.main" title="pyfuse3.main"><code class="xref py py-obj docutils literal notranslate"><span class="pre">pyfuse3.main</span></code></a> in a trio event loop. This function will return when
 the file system should be unmounted again, which is done by calling
 <a class="reference internal" href="fuse_api.html#pyfuse3.close" title="pyfuse3.close"><code class="xref py py-obj docutils literal notranslate"><span class="pre">pyfuse3.close</span></code></a>.</p>
 <p>All character data (directory entry names, extended attribute names
-and values, symbolic link targets etc) are passed as <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a> and must
-be returned as <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a>.</p>
+and values, symbolic link targets etc) are passed as <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a> and must
+be returned as <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a>.</p>
 <p>For easier debugging, it is strongly recommended that applications
 using pyfuse3 also make use of the <a class="reference external" href="http://docs.python.org/3/library/faulthandler.html">faulthandler</a> module.</p>
 </section>
 <section id="lookup-counts">
 <h2>Lookup Counts<a class="headerlink" href="#lookup-counts" title="Permalink to this heading">¶</a></h2>
 <p>Most file systems need to keep track which inodes are currently known
 to the kernel. This is, for example, necessary to correctly implement
@@ -174,15 +174,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="asyncio.html" title="asyncio Support"
              >next</a> |</li>
         <li class="right" >
           <a href="install.html" title="Installation"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">General Information</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * General Information
 ****** General InformationÂ¶ ******
 ***** Getting startedÂ¶ *****
 A file system is implemented by subclassing the pyfuse3.Operations class and
 implementing the various request handlers. The handlers respond to requests
 received from the FUSE kernel module and perform functions like looking up the
 inode given a file name, looking up attributes of an inode, opening a (file)
@@ -84,10 +84,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * General Information
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/genindex.html` & `pyfuse3-3.2.3/doc/html/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>Index &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -25,15 +25,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -456,15 +456,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Index
 ****** Index ******
 A | C | D | E | F | G | I | K | L | M | N | O | P | R | S | T | U | W
 ***** A *****
     * access()_(pyfuse3.Operations     * attr_timeout_
       method)                            (pyfuse3.EntryAttributes_attribute)
 ***** C *****
@@ -139,10 +139,10 @@
     * Example_File_Systems
     * Changelog
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Index
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/gotchas.html` & `pyfuse3-3.2.3/doc/html/gotchas.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Common Gotchas &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>Common Gotchas &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -34,15 +34,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="example.html" title="Example File Systems"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="util.html" title="Utility Functions"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Common Gotchas</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -130,15 +130,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="example.html" title="Example File Systems"
              >next</a> |</li>
         <li class="right" >
           <a href="util.html" title="Utility Functions"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Common Gotchas</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Common Gotchas
 ****** Common GotchasÂ¶ ******
 This chapter lists some common gotchas that should be avoided.
 ***** Removing inodes in unlink handlerÂ¶ *****
 If your file system is mounted at mnt, the following code should complete
 without errors:
 with open('mnt/file_one', 'w+') as fh1:
@@ -51,10 +51,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Common Gotchas
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/index.html` & `pyfuse3-3.2.3/doc/html/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>pyfuse3 Documentation &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>pyfuse3 Documentation &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -30,15 +30,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="about.html" title="About"
              accesskey="N">next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">pyfuse3 Documentation</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -121,15 +121,15 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="about.html" title="About"
              >next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">pyfuse3 Documentation</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * pyfuse3 Documentation
 ****** pyfuse3 DocumentationÂ¶ ******
 ***** Table of ContentsÂ¶ *****
     * About
     * Installation
     * General_Information
     * asyncio_Support
@@ -45,10 +45,10 @@
 About
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * pyfuse3 Documentation
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/install.html` & `pyfuse3-3.2.3/doc/html/install.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Installation &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>Installation &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -34,15 +34,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="general.html" title="General Information"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="about.html" title="About"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Installation</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -155,15 +155,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="general.html" title="General Information"
              >next</a> |</li>
         <li class="right" >
           <a href="about.html" title="About"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Installation</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Installation
 ****** InstallationÂ¶ ******
 ***** DependenciesÂ¶ *****
 In order to build and run pyfuse3 you need the following software:
     * Linux kernel 3.9 or newer.
     * Version 3.3.0 or newer of the libfuse library, including development
       headers (typically distributions provide them in a libfuse3-devel or
@@ -68,10 +68,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Installation
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/objects.inv` & `pyfuse3-3.2.3/doc/html/objects.inv`

 * *Files 1% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: pyfuse3
-# Version: 3.2.2
+# Version: 3.2.3
 # The remainder of this file is compressed using zlib.
 
 _pyfuse3.Operations py:class -1 operations.html#pyfuse3.Operations -
 pyfuse3 py:module 0 index.html#module-$ -
 pyfuse3.ENOATTR py:data 1 data.html#$ -
 pyfuse3.EntryAttributes py:class 1 data.html#$ -
 pyfuse3.EntryAttributes.attr_timeout py:attribute 1 data.html#$ -
```

### Comparing `pyfuse3-3.2.2/doc/html/operations.html` & `pyfuse3-3.2.3/doc/html/operations.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Request Handlers &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>Request Handlers &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -34,15 +34,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="util.html" title="Utility Functions"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="data.html" title="Data Structures"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Request Handlers</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -52,15 +52,15 @@
 <h1>Request Handlers<a class="headerlink" href="#request-handlers" title="Permalink to this heading">¶</a></h1>
 <p>(You can use the <a class="reference internal" href="genindex.html"><span class="std std-ref">Index</span></a> to directly jump to a specific handler).</p>
 <dl class="py class">
 <dt class="sig sig-object py" id="pyfuse3.Operations">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">Operations</span></span><a class="headerlink" href="#pyfuse3.Operations" title="Permalink to this definition">¶</a></dt>
 <dd><p>This class defines the request handler methods that an pyfuse3 file system
 may implement. If a particular request handler has not been implemented, it
-must raise <a class="reference internal" href="data.html#pyfuse3.FUSEError" title="pyfuse3.FUSEError"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FUSEError</span></code></a> with an errorcode of <a class="reference external" href="https://docs.python.org/3/library/errno.html#errno.ENOSYS" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">errno.ENOSYS</span></code></a>. Further requests
+must raise <a class="reference internal" href="data.html#pyfuse3.FUSEError" title="pyfuse3.FUSEError"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FUSEError</span></code></a> with an errorcode of <a class="reference external" href="https://docs.python.org/3/library/errno.html#errno.ENOSYS" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">errno.ENOSYS</span></code></a>. Further requests
 of this type will then be handled directly by the FUSE kernel module without
 calling the handler again.</p>
 <p>The only exception that request handlers are allowed to raise is
 <a class="reference internal" href="data.html#pyfuse3.FUSEError" title="pyfuse3.FUSEError"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FUSEError</span></code></a>. This will cause the specified errno to be returned by the
 syscall that is being handled.</p>
 <p>It is recommended that file systems are derived from this class and only
 overwrite the handlers that they actually implement. (The methods defined in
@@ -95,51 +95,51 @@
 <div><p>Enabling this feature implicitly turns on the
 <code class="docutils literal notranslate"><span class="pre">default_permissions</span></code> option.</p>
 </div></blockquote>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.access">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">access</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">ModeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.access" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">access</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">ModeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.access" title="Permalink to this definition">¶</a></dt>
 <dd><p>Check if requesting process has <em>mode</em> rights on <em>inode</em>.</p>
 <p><em>ctx</em> will be a <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a> instance.</p>
 <p>The method must return a boolean value.</p>
 <p>If the <code class="docutils literal notranslate"><span class="pre">default_permissions</span></code> mount option is given, this method is not
 called.</p>
 <p>When implementing this method, the <a class="reference internal" href="util.html#pyfuse3.get_sup_groups" title="pyfuse3.get_sup_groups"><code class="xref py py-obj docutils literal notranslate"><span class="pre">get_sup_groups</span></code></a> function may be
 useful.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.create">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parent_inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileNameT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">ModeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FlagT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Tuple" title="(in Python v3.10)"><span class="pre">Tuple</span></a><span class="p"><span class="pre">[</span></span><a class="reference internal" href="data.html#pyfuse3.FileInfo" title="pyfuse3.FileInfo"><span class="pre">FileInfo</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><span class="pre">EntryAttributes</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#pyfuse3.Operations.create" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parent_inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileNameT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">ModeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FlagT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Tuple" title="(in Python v3.11)"><span class="pre">Tuple</span></a><span class="p"><span class="pre">[</span></span><a class="reference internal" href="data.html#pyfuse3.FileInfo" title="pyfuse3.FileInfo"><span class="pre">FileInfo</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><span class="pre">EntryAttributes</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#pyfuse3.Operations.create" title="Permalink to this definition">¶</a></dt>
 <dd><p>Create a file with permissions <em>mode</em> and open it with <em>flags</em>.</p>
 <p><em>ctx</em> will be a <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a> instance.</p>
 <p>The method must return a tuple of the form <em>(fi, attr)</em>, where <em>fi</em> is a
 FileInfo instance handle like the one returned by <a class="reference internal" href="#pyfuse3.Operations.open" title="pyfuse3.Operations.open"><code class="xref py py-obj docutils literal notranslate"><span class="pre">open</span></code></a> and <em>attr</em> is
 an <a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><code class="xref py py-obj docutils literal notranslate"><span class="pre">EntryAttributes</span></code></a> instance with the attributes of the newly created
 directory entry.</p>
 <p>(Successful) execution of this handler increases the lookup count for
 the returned inode by one.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.flush">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">flush</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.flush" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">flush</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.flush" title="Permalink to this definition">¶</a></dt>
 <dd><p>Handle close() syscall.</p>
 <p><em>fh</em> will be an integer filehandle returned by a prior <a class="reference internal" href="#pyfuse3.Operations.open" title="pyfuse3.Operations.open"><code class="xref py py-obj docutils literal notranslate"><span class="pre">open</span></code></a> or
 <a class="reference internal" href="#pyfuse3.Operations.create" title="pyfuse3.Operations.create"><code class="xref py py-obj docutils literal notranslate"><span class="pre">create</span></code></a> call.</p>
 <p>This method is called whenever a file descriptor is closed. It may be
 called multiple times for the same open file (e.g. if the file handle
 has been duplicated).</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.forget">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">forget</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode_list</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Sequence" title="(in Python v3.10)"><span class="pre">Sequence</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Tuple" title="(in Python v3.10)"><span class="pre">Tuple</span></a><span class="p"><span class="pre">[</span></span><span class="pre">InodeT</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.forget" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">forget</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode_list</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Sequence" title="(in Python v3.11)"><span class="pre">Sequence</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Tuple" title="(in Python v3.11)"><span class="pre">Tuple</span></a><span class="p"><span class="pre">[</span></span><span class="pre">InodeT</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.forget" title="Permalink to this definition">¶</a></dt>
 <dd><p>Decrease lookup counts for inodes in <em>inode_list</em>.</p>
 <p><em>inode_list</em> is a list of <code class="docutils literal notranslate"><span class="pre">(inode,</span> <span class="pre">nlookup)</span></code> tuples. This method
 should reduce the lookup count for each <em>inode</em> by <em>nlookup</em>.</p>
 <p>If the lookup count reaches zero, the inode is currently not known to
 the kernel. In this case, the file system will typically check if there
 are still directory entries referring to this inode and, if not, remove
 the inode.</p>
@@ -150,25 +150,25 @@
 every such inode after <a class="reference internal" href="fuse_api.html#pyfuse3.main" title="pyfuse3.main"><code class="xref py py-obj docutils literal notranslate"><span class="pre">main</span></code></a> has returned).</p>
 <p>This method must not raise any exceptions (not even <a class="reference internal" href="data.html#pyfuse3.FUSEError" title="pyfuse3.FUSEError"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FUSEError</span></code></a>), since
 it is not handling a particular client request.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.fsync">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">fsync</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">datasync</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.fsync" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">fsync</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">datasync</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.fsync" title="Permalink to this definition">¶</a></dt>
 <dd><p>Flush buffers for open file <em>fh</em>.</p>
 <p>If <em>datasync</em> is true, only the file contents should be
 flushed (in contrast to the metadata about the file).</p>
 <p><em>fh</em> will be an integer filehandle returned by a prior <a class="reference internal" href="#pyfuse3.Operations.open" title="pyfuse3.Operations.open"><code class="xref py py-obj docutils literal notranslate"><span class="pre">open</span></code></a> or
 <a class="reference internal" href="#pyfuse3.Operations.create" title="pyfuse3.Operations.create"><code class="xref py py-obj docutils literal notranslate"><span class="pre">create</span></code></a> call.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.fsyncdir">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">fsyncdir</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">datasync</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.10)"><span class="pre">bool</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.fsyncdir" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">fsyncdir</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">datasync</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.fsyncdir" title="Permalink to this definition">¶</a></dt>
 <dd><p>Flush buffers for open directory <em>fh</em>.</p>
 <p>If <em>datasync</em> is true, only the directory contents should be
 flushed (in contrast to metadata about the directory itself).</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.getattr">
@@ -178,25 +178,25 @@
 <p>This method should return an <a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><code class="xref py py-obj docutils literal notranslate"><span class="pre">EntryAttributes</span></code></a> instance with the
 attributes of <em>inode</em>. The <a class="reference internal" href="data.html#pyfuse3.EntryAttributes.entry_timeout" title="pyfuse3.EntryAttributes.entry_timeout"><code class="xref py py-obj docutils literal notranslate"><span class="pre">entry_timeout</span></code></a> attribute is
 ignored in this context.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.getxattr">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">getxattr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><span class="pre">bytes</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><span class="pre">bytes</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.getxattr" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">getxattr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.getxattr" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return extended attribute <em>name</em> of <em>inode</em>.</p>
 <p><em>ctx</em> will be a <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a> instance.</p>
 <p>If the attribute does not exist, the method must raise <a class="reference internal" href="data.html#pyfuse3.FUSEError" title="pyfuse3.FUSEError"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FUSEError</span></code></a> with
-an error code of <a class="reference internal" href="data.html#pyfuse3.ENOATTR" title="pyfuse3.ENOATTR"><code class="xref py py-obj docutils literal notranslate"><span class="pre">ENOATTR</span></code></a>. <em>name</em> will be of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a>, but is
+an error code of <a class="reference internal" href="data.html#pyfuse3.ENOATTR" title="pyfuse3.ENOATTR"><code class="xref py py-obj docutils literal notranslate"><span class="pre">ENOATTR</span></code></a>. <em>name</em> will be of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a>, but is
 guaranteed not to contain zero-bytes (<code class="docutils literal notranslate"><span class="pre">\0</span></code>).</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.init">
-<span class="sig-name descname"><span class="pre">init</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.init" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">init</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.init" title="Permalink to this definition">¶</a></dt>
 <dd><p>Initialize operations.</p>
 <p>This method will be called just before the file system starts handling
 requests. It must not raise any exceptions (not even <a class="reference internal" href="data.html#pyfuse3.FUSEError" title="pyfuse3.FUSEError"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FUSEError</span></code></a>), since
 it is not handling a particular client request.</p>
 </dd></dl>
 
 <dl class="py method">
@@ -208,31 +208,31 @@
 attributes of the newly created directory entry.</p>
 <p>(Successful) execution of this handler increases the lookup count for
 the returned inode by one.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.listxattr">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">listxattr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Sequence" title="(in Python v3.10)"><span class="pre">Sequence</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><span class="pre">bytes</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#pyfuse3.Operations.listxattr" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">listxattr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Sequence" title="(in Python v3.11)"><span class="pre">Sequence</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#pyfuse3.Operations.listxattr" title="Permalink to this definition">¶</a></dt>
 <dd><p>Get list of extended attributes for <em>inode</em>.</p>
 <p><em>ctx</em> will be a <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a> instance.</p>
-<p>This method must return a sequence of <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a> objects.  The objects must
+<p>This method must return a sequence of <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a> objects.  The objects must
 not include zero-bytes (<code class="docutils literal notranslate"><span class="pre">\0</span></code>).</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.lookup">
 <em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">lookup</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parent_inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileNameT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><span class="pre">EntryAttributes</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.lookup" title="Permalink to this definition">¶</a></dt>
 <dd><p>Look up a directory entry by name and get its attributes.</p>
 <p>This method should return an <a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><code class="xref py py-obj docutils literal notranslate"><span class="pre">EntryAttributes</span></code></a> instance for the
 directory entry <em>name</em> in the directory with inode <em>parent_inode</em>.</p>
 <p>If there is no such entry, the method should either return an
 <a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><code class="xref py py-obj docutils literal notranslate"><span class="pre">EntryAttributes</span></code></a> instance with zero <code class="docutils literal notranslate"><span class="pre">st_ino</span></code> value (in which case
 the negative lookup will be cached as specified by <code class="docutils literal notranslate"><span class="pre">entry_timeout</span></code>),
-or it should raise <a class="reference internal" href="data.html#pyfuse3.FUSEError" title="pyfuse3.FUSEError"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FUSEError</span></code></a> with an errno of <a class="reference external" href="https://docs.python.org/3/library/errno.html#errno.ENOENT" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">errno.ENOENT</span></code></a> (in this
+or it should raise <a class="reference internal" href="data.html#pyfuse3.FUSEError" title="pyfuse3.FUSEError"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FUSEError</span></code></a> with an errno of <a class="reference external" href="https://docs.python.org/3/library/errno.html#errno.ENOENT" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">errno.ENOENT</span></code></a> (in this
 case the negative result will not be cached).</p>
 <p><em>ctx</em> will be a <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a> instance.</p>
 <p>The file system must be able to handle lookups for <code class="file docutils literal notranslate"><span class="pre">.</span></code> and
 <code class="file docutils literal notranslate"><span class="pre">..</span></code>, no matter if these entries are returned by <a class="reference internal" href="#pyfuse3.Operations.readdir" title="pyfuse3.Operations.readdir"><code class="xref py py-obj docutils literal notranslate"><span class="pre">readdir</span></code></a> or not.</p>
 <p>(Successful) execution of this handler increases the lookup count for
 the returned inode by one.</p>
 </dd></dl>
@@ -248,15 +248,15 @@
 attributes of the newly created directory entry.</p>
 <p>(Successful) execution of this handler increases the lookup count for
 the returned inode by one.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.mknod">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">mknod</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parent_inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileNameT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">ModeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rdev</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><span class="pre">EntryAttributes</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.mknod" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">mknod</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parent_inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileNameT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">ModeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rdev</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><span class="pre">EntryAttributes</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.mknod" title="Permalink to this definition">¶</a></dt>
 <dd><p>Create (possibly special) file.</p>
 <p>This method must create a (special or regular) file <em>name</em> in the
 directory with inode <em>parent_inode</em>. Whether the file is special or
 regular is determined by its <em>mode</em>. If the file is neither a block nor
 character device, <em>rdev</em> can be ignored. <em>ctx</em> will be a
 <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a> instance.</p>
 <p>The method must return an <a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><code class="xref py py-obj docutils literal notranslate"><span class="pre">EntryAttributes</span></code></a> instance with the attributes
@@ -267,15 +267,15 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.open">
 <em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">open</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FlagT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="data.html#pyfuse3.FileInfo" title="pyfuse3.FileInfo"><span class="pre">FileInfo</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.open" title="Permalink to this definition">¶</a></dt>
 <dd><p>Open a inode <em>inode</em> with <em>flags</em>.</p>
 <p><em>ctx</em> will be a <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a> instance.</p>
 <p><em>flags</em> will be a bitwise or of the open flags described in the
-<em class="manpage">open(2)</em> manpage and defined in the <a class="reference external" href="https://docs.python.org/3/library/os.html#module-os" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">os</span></code></a> module (with the
+<em class="manpage">open(2)</em> manpage and defined in the <a class="reference external" href="https://docs.python.org/3/library/os.html#module-os" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">os</span></code></a> module (with the
 exception of <code class="docutils literal notranslate"><span class="pre">O_CREAT</span></code>, <code class="docutils literal notranslate"><span class="pre">O_EXCL</span></code>, <code class="docutils literal notranslate"><span class="pre">O_NOCTTY</span></code> and <code class="docutils literal notranslate"><span class="pre">O_TRUNC</span></code>)</p>
 <p>This method must return a <a class="reference internal" href="data.html#pyfuse3.FileInfo" title="pyfuse3.FileInfo"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FileInfo</span></code></a> instance. The <a class="reference internal" href="data.html#pyfuse3.FileInfo.fh" title="pyfuse3.FileInfo.fh"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FileInfo.fh</span></code></a> field
 must contain an integer file handle, which will be passed to the <a class="reference internal" href="#pyfuse3.Operations.read" title="pyfuse3.Operations.read"><code class="xref py py-obj docutils literal notranslate"><span class="pre">read</span></code></a>,
 <a class="reference internal" href="#pyfuse3.Operations.write" title="pyfuse3.Operations.write"><code class="xref py py-obj docutils literal notranslate"><span class="pre">write</span></code></a>, <a class="reference internal" href="#pyfuse3.Operations.flush" title="pyfuse3.Operations.flush"><code class="xref py py-obj docutils literal notranslate"><span class="pre">flush</span></code></a>, <a class="reference internal" href="#pyfuse3.Operations.fsync" title="pyfuse3.Operations.fsync"><code class="xref py py-obj docutils literal notranslate"><span class="pre">fsync</span></code></a> and <a class="reference internal" href="#pyfuse3.Operations.release" title="pyfuse3.Operations.release"><code class="xref py py-obj docutils literal notranslate"><span class="pre">release</span></code></a> methods to identify the open
 file. The <a class="reference internal" href="data.html#pyfuse3.FileInfo" title="pyfuse3.FileInfo"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FileInfo</span></code></a> instance may also have relevant configuration
 attributes set; see the <a class="reference internal" href="data.html#pyfuse3.FileInfo" title="pyfuse3.FileInfo"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FileInfo</span></code></a> documentation for more information.</p>
 </dd></dl>
@@ -288,26 +288,26 @@
 <p>This method should return an integer file handle. The file handle will
 be passed to the <a class="reference internal" href="#pyfuse3.Operations.readdir" title="pyfuse3.Operations.readdir"><code class="xref py py-obj docutils literal notranslate"><span class="pre">readdir</span></code></a>, <a class="reference internal" href="#pyfuse3.Operations.fsyncdir" title="pyfuse3.Operations.fsyncdir"><code class="xref py py-obj docutils literal notranslate"><span class="pre">fsyncdir</span></code></a> and <a class="reference internal" href="#pyfuse3.Operations.releasedir" title="pyfuse3.Operations.releasedir"><code class="xref py py-obj docutils literal notranslate"><span class="pre">releasedir</span></code></a> methods to
 identify the directory.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.read">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">read</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">off</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">size</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.read" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">read</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">off</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">size</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.read" title="Permalink to this definition">¶</a></dt>
 <dd><p>Read <em>size</em> bytes from <em>fh</em> at position <em>off</em>.</p>
 <p><em>fh</em> will be an integer filehandle returned by a prior <a class="reference internal" href="#pyfuse3.Operations.open" title="pyfuse3.Operations.open"><code class="xref py py-obj docutils literal notranslate"><span class="pre">open</span></code></a> or
 <a class="reference internal" href="#pyfuse3.Operations.create" title="pyfuse3.Operations.create"><code class="xref py py-obj docutils literal notranslate"><span class="pre">create</span></code></a> call.</p>
 <p>This function should return exactly the number of bytes requested except
 on EOF or error, otherwise the rest of the data will be substituted with
 zeroes.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.readdir">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">readdir</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">token</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">ReaddirToken</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.readdir" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">readdir</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">token</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">ReaddirToken</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.readdir" title="Permalink to this definition">¶</a></dt>
 <dd><p>Read entries in open directory <em>fh</em>.</p>
 <p>This method should list the contents of directory <em>fh</em> (as returned by a
 prior <a class="reference internal" href="#pyfuse3.Operations.opendir" title="pyfuse3.Operations.opendir"><code class="xref py py-obj docutils literal notranslate"><span class="pre">opendir</span></code></a> call), starting at the entry identified by <em>start_id</em>.</p>
 <p>Instead of returning the directory entries directly, the method must
 call <a class="reference internal" href="fuse_api.html#pyfuse3.readdir_reply" title="pyfuse3.readdir_reply"><code class="xref py py-obj docutils literal notranslate"><span class="pre">readdir_reply</span></code></a> for each directory entry. If <a class="reference internal" href="fuse_api.html#pyfuse3.readdir_reply" title="pyfuse3.readdir_reply"><code class="xref py py-obj docutils literal notranslate"><span class="pre">readdir_reply</span></code></a>
 returns True, the file system must increase the lookup count for the
 provided directory entry by one and call <a class="reference internal" href="fuse_api.html#pyfuse3.readdir_reply" title="pyfuse3.readdir_reply"><code class="xref py py-obj docutils literal notranslate"><span class="pre">readdir_reply</span></code></a> again for the
@@ -332,49 +332,49 @@
 <em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">readlink</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">FileNameT</span></span></span><a class="headerlink" href="#pyfuse3.Operations.readlink" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return target of symbolic link <em>inode</em>.</p>
 <p><em>ctx</em> will be a <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a> instance.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.release">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">release</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.release" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">release</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.release" title="Permalink to this definition">¶</a></dt>
 <dd><p>Release open file.</p>
 <p>This method will be called when the last file descriptor of <em>fh</em> has
 been closed, i.e. when the file is no longer opened by any client
 process.</p>
 <p><em>fh</em> will be an integer filehandle returned by a prior <a class="reference internal" href="#pyfuse3.Operations.open" title="pyfuse3.Operations.open"><code class="xref py py-obj docutils literal notranslate"><span class="pre">open</span></code></a> or
 <a class="reference internal" href="#pyfuse3.Operations.create" title="pyfuse3.Operations.create"><code class="xref py py-obj docutils literal notranslate"><span class="pre">create</span></code></a> call. Once <a class="reference internal" href="#pyfuse3.Operations.release" title="pyfuse3.Operations.release"><code class="xref py py-obj docutils literal notranslate"><span class="pre">release</span></code></a> has been called, no future requests for
 <em>fh</em> will be received (until the value is re-used in the return value of
 another <a class="reference internal" href="#pyfuse3.Operations.open" title="pyfuse3.Operations.open"><code class="xref py py-obj docutils literal notranslate"><span class="pre">open</span></code></a> or <a class="reference internal" href="#pyfuse3.Operations.create" title="pyfuse3.Operations.create"><code class="xref py py-obj docutils literal notranslate"><span class="pre">create</span></code></a> call).</p>
 <p>This method may return an error by raising <a class="reference internal" href="data.html#pyfuse3.FUSEError" title="pyfuse3.FUSEError"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FUSEError</span></code></a>, but the error
 will be discarded because there is no corresponding client request.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.releasedir">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">releasedir</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.releasedir" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">releasedir</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.releasedir" title="Permalink to this definition">¶</a></dt>
 <dd><p>Release open directory.</p>
 <p>This method will be called exactly once for each <a class="reference internal" href="#pyfuse3.Operations.opendir" title="pyfuse3.Operations.opendir"><code class="xref py py-obj docutils literal notranslate"><span class="pre">opendir</span></code></a> call. After
 <em>fh</em> has been released, no further <a class="reference internal" href="#pyfuse3.Operations.readdir" title="pyfuse3.Operations.readdir"><code class="xref py py-obj docutils literal notranslate"><span class="pre">readdir</span></code></a> requests will be received
 for it (until it is opened again with <a class="reference internal" href="#pyfuse3.Operations.opendir" title="pyfuse3.Operations.opendir"><code class="xref py py-obj docutils literal notranslate"><span class="pre">opendir</span></code></a>).</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.removexattr">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">removexattr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><span class="pre">bytes</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.removexattr" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">removexattr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.removexattr" title="Permalink to this definition">¶</a></dt>
 <dd><p>Remove extended attribute <em>name</em> of <em>inode</em>.</p>
 <p><em>ctx</em> will be a <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a> instance.</p>
 <p>If the attribute does not exist, the method must raise <a class="reference internal" href="data.html#pyfuse3.FUSEError" title="pyfuse3.FUSEError"><code class="xref py py-obj docutils literal notranslate"><span class="pre">FUSEError</span></code></a> with
-an error code of <a class="reference internal" href="data.html#pyfuse3.ENOATTR" title="pyfuse3.ENOATTR"><code class="xref py py-obj docutils literal notranslate"><span class="pre">ENOATTR</span></code></a>. <em>name</em> will be of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a>, but is
+an error code of <a class="reference internal" href="data.html#pyfuse3.ENOATTR" title="pyfuse3.ENOATTR"><code class="xref py py-obj docutils literal notranslate"><span class="pre">ENOATTR</span></code></a>. <em>name</em> will be of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a>, but is
 guaranteed not to contain zero-bytes (<code class="docutils literal notranslate"><span class="pre">\0</span></code>).</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.rename">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">rename</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parent_inode_old</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name_old</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">parent_inode_new</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name_new</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FlagT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.rename" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">rename</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parent_inode_old</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name_old</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">parent_inode_new</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name_new</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FlagT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.rename" title="Permalink to this definition">¶</a></dt>
 <dd><p>Rename a directory entry.</p>
 <p>This method must rename <em>name_old</em> in the directory with inode
 <em>parent_inode_old</em> to <em>name_new</em> in the directory with inode
 <em>parent_inode_new</em>.  If <em>name_new</em> already exists, it should be
 overwritten.</p>
 <p><em>flags</em> may be <a class="reference internal" href="data.html#pyfuse3.RENAME_EXCHANGE" title="pyfuse3.RENAME_EXCHANGE"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RENAME_EXCHANGE</span></code></a> or <a class="reference internal" href="data.html#pyfuse3.RENAME_NOREPLACE" title="pyfuse3.RENAME_NOREPLACE"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RENAME_NOREPLACE</span></code></a>. If
 <a class="reference internal" href="data.html#pyfuse3.RENAME_NOREPLACE" title="pyfuse3.RENAME_NOREPLACE"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RENAME_NOREPLACE</span></code></a> is specified, the filesystem must not overwrite
@@ -393,15 +393,15 @@
 deferred to the <a class="reference internal" href="#pyfuse3.Operations.forget" title="pyfuse3.Operations.forget"><code class="xref py py-obj docutils literal notranslate"><span class="pre">forget</span></code></a> method to be carried out when the lookup count
 reaches zero (and of course only if at that point there are no more
 directory entries associated with <em>inode_deref</em> either).</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.rmdir">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">rmdir</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parent_inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileNameT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.rmdir" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">rmdir</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parent_inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileNameT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.rmdir" title="Permalink to this definition">¶</a></dt>
 <dd><p>Remove directory <em>name</em>.</p>
 <p>This method must remove the directory <em>name</em> from the direcory with
 inode <em>parent_inode</em>. <em>ctx</em> will be a <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a> instance. If
 there are still entries in the directory, the method should raise
 <code class="docutils literal notranslate"><span class="pre">FUSEError(errno.ENOTEMPTY)</span></code>.</p>
 <p>If the inode associated with <em>name</em> (i.e., not the <em>parent_inode</em>) has a
 non-zero lookup count, the file system must remove only the directory
@@ -414,47 +414,47 @@
 is not required to check if there are still other directory entries
 refering to the same inode. This conveniently avoids the ambigiouties
 associated with the <code class="docutils literal notranslate"><span class="pre">.</span></code> and <code class="docutils literal notranslate"><span class="pre">..</span></code> entries).</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.setattr">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">setattr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">attr</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><span class="pre">EntryAttributes</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">fields</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.SetattrFields" title="pyfuse3.SetattrFields"><span class="pre">SetattrFields</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.10)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><span class="pre">FileHandleT</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><span class="pre">EntryAttributes</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.setattr" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">setattr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">attr</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><span class="pre">EntryAttributes</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">fields</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.SetattrFields" title="pyfuse3.SetattrFields"><span class="pre">SetattrFields</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Optional" title="(in Python v3.11)"><span class="pre">Optional</span></a><span class="p"><span class="pre">[</span></span><span class="pre">FileHandleT</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><span class="pre">EntryAttributes</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.setattr" title="Permalink to this definition">¶</a></dt>
 <dd><p>Change attributes of <em>inode</em>.</p>
 <p><em>fields</em> will be an <a class="reference internal" href="data.html#pyfuse3.SetattrFields" title="pyfuse3.SetattrFields"><code class="xref py py-obj docutils literal notranslate"><span class="pre">SetattrFields</span></code></a> instance that specifies which
 attributes are to be updated. <em>attr</em> will be an <a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><code class="xref py py-obj docutils literal notranslate"><span class="pre">EntryAttributes</span></code></a>
 instance for <em>inode</em> that contains the new values for changed
 attributes, and undefined values for all other attributes.</p>
 <p>Most file systems will additionally set the
 <a class="reference internal" href="data.html#pyfuse3.EntryAttributes.st_ctime_ns" title="pyfuse3.EntryAttributes.st_ctime_ns"><code class="xref py py-obj docutils literal notranslate"><span class="pre">st_ctime_ns</span></code></a> attribute to the current time (to
 indicate that the inode metadata was changed).</p>
 <p>If the syscall that is being processed received a file descriptor
 argument (like e.g. <em class="manpage">ftruncate(2)</em> or <em class="manpage">fchmod(2)</em>),
 <em>fh</em> will be the file handle returned by the corresponding call to the
 <a class="reference internal" href="#pyfuse3.Operations.open" title="pyfuse3.Operations.open"><code class="xref py py-obj docutils literal notranslate"><span class="pre">open</span></code></a> handler. If the syscall was path based (like
 e.g. <em class="manpage">truncate(2)</em> or <em class="manpage">chmod(2)</em>), <em>fh</em> will be
-<a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code></a>.</p>
+<a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code></a>.</p>
 <p><em>ctx</em> will be a <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a> instance.</p>
 <p>The method should return an <a class="reference internal" href="data.html#pyfuse3.EntryAttributes" title="pyfuse3.EntryAttributes"><code class="xref py py-obj docutils literal notranslate"><span class="pre">EntryAttributes</span></code></a> instance (containing both
 the changed and unchanged values).</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.setxattr">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">setxattr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><span class="pre">bytes</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><span class="pre">bytes</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.setxattr" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">setxattr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.setxattr" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set extended attribute <em>name</em> of <em>inode</em> to <em>value</em>.</p>
 <p><em>ctx</em> will be a <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a> instance.</p>
 <p>The attribute may or may not exist already. Both <em>name</em> and <em>value</em> will
-be of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a>. <em>name</em> is guaranteed not to contain zero-bytes
+be of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a>. <em>name</em> is guaranteed not to contain zero-bytes
 (<code class="docutils literal notranslate"><span class="pre">\0</span></code>).</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.stacktrace">
-<span class="sig-name descname"><span class="pre">stacktrace</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.stacktrace" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">stacktrace</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.stacktrace" title="Permalink to this definition">¶</a></dt>
 <dd><p>Asynchronous debugging.</p>
 <p>This method will be called when the <code class="docutils literal notranslate"><span class="pre">fuse_stacktrace</span></code> extended
 attribute is set on the mountpoint. The default implementation logs the
 current stack trace of every running Python thread. This can be quite
 useful to debug file system deadlocks.</p>
 </dd></dl>
 
@@ -477,15 +477,15 @@
 of the newly created directory entry.</p>
 <p>(Successful) execution of this handler increases the lookup count for
 the returned inode by one.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.unlink">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">unlink</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parent_inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileNameT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.10)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.unlink" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">unlink</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parent_inode</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">InodeT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileNameT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ctx</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><span class="pre">RequestContext</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.unlink" title="Permalink to this definition">¶</a></dt>
 <dd><p>Remove a (possibly special) file.</p>
 <p>This method must remove the (special or regular) file <em>name</em> from the
 direcory with inode <em>parent_inode</em>.  <em>ctx</em> will be a <a class="reference internal" href="data.html#pyfuse3.RequestContext" title="pyfuse3.RequestContext"><code class="xref py py-obj docutils literal notranslate"><span class="pre">RequestContext</span></code></a>
 instance.</p>
 <p>If the inode associated with <em>file</em> (i.e., not the <em>parent_inode</em>) has a
 non-zero lookup count, or if there are still other directory entries
 referring to this inode (due to hardlinks), the file system must remove
@@ -496,15 +496,15 @@
 the <a class="reference internal" href="#pyfuse3.Operations.forget" title="pyfuse3.Operations.forget"><code class="xref py py-obj docutils literal notranslate"><span class="pre">forget</span></code></a> method to be carried out when the lookup count reaches zero
 (and of course only if at that point there are no more directory entries
 associated with the inode either).</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="pyfuse3.Operations.write">
-<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">write</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">off</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">buf</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><span class="pre">bytes</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.10)"><span class="pre">int</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.write" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">coroutine</span> </em><span class="sig-name descname"><span class="pre">write</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fh</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">FileHandleT</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">off</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">buf</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></span><a class="headerlink" href="#pyfuse3.Operations.write" title="Permalink to this definition">¶</a></dt>
 <dd><p>Write <em>buf</em> into <em>fh</em> at <em>off</em>.</p>
 <p><em>fh</em> will be an integer filehandle returned by a prior <a class="reference internal" href="#pyfuse3.Operations.open" title="pyfuse3.Operations.open"><code class="xref py py-obj docutils literal notranslate"><span class="pre">open</span></code></a> or
 <a class="reference internal" href="#pyfuse3.Operations.create" title="pyfuse3.Operations.create"><code class="xref py py-obj docutils literal notranslate"><span class="pre">create</span></code></a> call.</p>
 <p>This method must return the number of bytes written. However, unless the
 file system has been mounted with the <code class="docutils literal notranslate"><span class="pre">direct_io</span></code> option, the file
 system <em>must</em> always write <em>all</em> the provided data (i.e., return
 <code class="docutils literal notranslate"><span class="pre">len(buf)</span></code>).</p>
@@ -570,15 +570,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="util.html" title="Utility Functions"
              >next</a> |</li>
         <li class="right" >
           <a href="data.html" title="Data Structures"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Request Handlers</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Request Handlers
 ****** Request HandlersÂ¶ ******
 (You can use the Index to directly jump to a specific handler).
   classpyfuse3.OperationsÂ¶
       This class defines the request handler methods that an pyfuse3 file
       system may implement. If a particular request handler has not been
       implemented, it must raise FUSEError with an errorcode of errno.ENOSYS.
@@ -380,10 +380,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Request Handlers
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/py-modindex.html` & `pyfuse3-3.2.3/doc/html/py-modindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>Python Module Index &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -32,15 +32,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -104,15 +104,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Python Module Index
 ****** Python Module Index ******
 p
   
  p
  pyfuse3
 **** Table_Of_Contents ****
@@ -27,10 +27,10 @@
     * Example_File_Systems
     * Changelog
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Python Module Index
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/search.html` & `pyfuse3-3.2.3/doc/html/search.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>Search &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -31,15 +31,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -105,15 +105,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Search
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
 **** Table_Of_Contents ****
     * About
@@ -24,10 +24,10 @@
     * Utility_Functions
     * Common_Gotchas
     * Example_File_Systems
     * Changelog
 **** Navigation ****
     * index
     * modules |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Search
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/doc/html/searchindex.js` & `pyfuse3-3.2.3/doc/html/searchindex.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -41,21 +41,21 @@
         "html": 0,
         "directori": [0, 3, 4, 5, 6, 10, 11],
         "tarbal": [0, 4, 9],
         "pleas": [0, 6],
         "report": [0, 5, 9, 10],
         "ani": [0, 3, 4, 5, 6, 10],
         "bug": [0, 2, 9],
-        "issu": [0, 9],
+        "issu": [0, 2, 9],
         "tracker": [0, 9],
         "For": [0, 1, 4, 5, 6, 11],
         "discuss": 0,
         "question": 0,
         "us": [0, 1, 2, 3, 4, 5, 6, 10, 11],
-        "gener": [0, 3, 4, 5, 8],
+        "gener": [0, 2, 3, 4, 5, 8],
         "fuse": [0, 4, 8, 9, 10, 11],
         "mail": [0, 9],
         "list": [0, 5, 6, 7, 9, 10],
         "A": [0, 3, 4, 5, 6, 9],
         "searchabl": 0,
         "archiv": 0,
         "kindli": 0,
@@ -235,15 +235,15 @@
         "rename_exchang": [3, 10],
         "flag": [3, 4, 10],
         "must": [3, 5, 6, 10],
         "atom": [3, 10],
         "exchang": [3, 10],
         "two": [3, 4, 6, 10],
         "path": [3, 4, 10, 11],
-        "which": [3, 5, 6, 10],
+        "which": [2, 3, 5, 6, 10],
         "both": [3, 4, 10],
         "exist": [3, 4, 10],
         "rename_noreplac": [3, 10],
         "replac": 3,
         "target": [3, 4, 6, 10],
         "default_opt": [3, 4, 5],
         "recommend": [3, 5, 6, 10],
@@ -332,15 +332,15 @@
         "st_size": [3, 4],
         "st_blksize": [3, 4],
         "st_block": [3, 4],
         "st_atime_n": [3, 4],
         "time": [3, 4, 6, 10, 11],
         "last": [3, 10],
         "access": [3, 4, 5, 10],
-        "integ": [3, 4, 5, 10],
+        "integ": [2, 3, 4, 5, 10],
         "st_ctime_n": [3, 4, 10],
         "st_mtime_n": [3, 4],
         "fuse_file_info": 3,
         "relev": [3, 10],
         "fh": [3, 4, 10],
         "uint64_t": 3,
         "bool": [3, 10],
@@ -374,15 +374,15 @@
         "usr": 4,
         "bin": 4,
         "env": 4,
         "python3": [4, 9],
         "utf": 4,
         "8": [4, 5],
         "hello": 4,
-        "program": 4,
+        "program": [2, 4],
         "present": 4,
         "static": 4,
         "copyright": 4,
         "2015": 4,
         "nikolau": 4,
         "rath": 4,
         "org": [4, 9],
@@ -448,15 +448,15 @@
         "connect": [4, 5],
         "WITH": 4,
         "sy": [4, 5],
         "we": 4,
         "run": [4, 5, 6, 9, 10],
         "try": 4,
         "load": 4,
-        "basedir": 4,
+        "basedir": [2, 4],
         "abspath": 4,
         "join": 4,
         "dirnam": 4,
         "argv": 4,
         "0": [4, 5, 7, 9, 10],
         "src": 4,
         "pyx": 4,
@@ -671,15 +671,15 @@
         "lastrowid": 4,
         "offset": [4, 5],
         "length": 4,
         "buf": [4, 10],
         "del": 4,
         "__str__": 4,
         "queri": 4,
-        "more": [4, 9, 10],
+        "more": [2, 4, 9, 10],
         "than": [4, 10],
         "produc": 4,
         "discard": [4, 5, 10],
         "mirror": 4,
         "tree": 4,
         "caveat": 4,
         "through": [4, 5],
@@ -722,15 +722,15 @@
         "forget": [4, 5, 6, 7, 10],
         "inode_list": [4, 10],
         "nlookup": [4, 10],
         "continu": [4, 5],
         "_getattr": 4,
         "fd": 4,
         "lstat": 4,
-        "oserror": [4, 5],
+        "oserror": [2, 4, 5],
         "listdir": [4, 7, 11],
         "append": 4,
         "start": [4, 5, 10],
         "same": [4, 5, 6, 10, 11],
         "between": 4,
         "cannot": [4, 5],
         "simpli": 4,
@@ -872,15 +872,15 @@
         "readdirtoken": [5, 10],
         "off_t": 5,
         "next_id": [5, 10],
         "respons": [5, 10],
         "each": [5, 10],
         "receiv": [5, 6, 10],
         "64": 5,
-        "bit": [5, 9],
+        "bit": [2, 5, 9],
         "identifi": [5, 10],
         "posit": [5, 10],
         "back": 5,
         "later": 5,
         "robust": 5,
         "presenc": 5,
         "creation": 5,
@@ -935,33 +935,33 @@
         "dup": 7,
         "fileno": 7,
         "foobar": 7,
         "re": [7, 10, 11],
         "probabl": 7,
         "did": 7,
         "mistak": 7,
-        "instal": 8,
+        "instal": [2, 8],
         "structur": 8,
         "util": 8,
         "common": 8,
         "gotcha": 8,
         "changelog": 8,
         "index": [8, 10],
-        "search": 8,
+        "search": [2, 8],
         "build": 9,
         "9": 9,
         "newer": 9,
         "librari": [9, 11],
         "header": 9,
         "typic": [9, 10],
         "libfuse3": 9,
         "devel": 9,
         "packag": 9,
         "7": 9,
-        "setuptool": 9,
+        "setuptool": [2, 9],
         "pkg": 9,
         "config": 9,
         "tool": 9,
         "compil": 9,
         "unpack": 9,
         "http": 9,
         "build_ext": 9,
@@ -970,17 +970,17 @@
         "pytest": 9,
         "ask": 9,
         "wide": 9,
         "sudo": 9,
         "local": 9,
         "unstabl": 9,
         "effort": 9,
-        "requir": [9, 10],
+        "requir": [2, 9, 10],
         "28": 9,
-        "sphinx": 9,
+        "sphinx": [2, 9],
         "build_cython": 9,
         "build_sphinx": 9,
         "directli": 10,
         "jump": 10,
         "further": 10,
         "caus": 10,
         "being": 10,
@@ -1083,15 +1083,15 @@
         "stack": 10,
         "trace": 10,
         "quit": 10,
         "statist": 10,
         "appropri": 10,
         "fill": 10,
         "symbolink": 10,
-        "due": 10,
+        "due": [2, 10],
         "written": 10,
         "necessarili": 11,
         "translat": 11,
         "namespac": 11,
         "surrog": 11,
         "freebsd": 11,
         "platform": 11,
@@ -1113,15 +1113,30 @@
         "pep": 11,
         "383": 11,
         "supplementari": 11,
         "group": 11,
         "rel": 11,
         "expens": 11,
         "proc": 11,
-        "statu": 11
+        "statu": 11,
+        "34": 2,
+        "pyproject": 2,
+        "toml": 2,
+        "overflow": 2,
+        "32": 2,
+        "arch": 2,
+        "47": 2,
+        "shutil": 2,
+        "extern": 2,
+        "catch": 2,
+        "63": 2,
+        "comput": 2,
+        "pip": 2,
+        "6": 2,
+        "recent": 2
     },
     "objects": {
         "": [
             [8, 0, 0, "-", "pyfuse3"]
         ],
         "pyfuse3": [
             [3, 1, 1, "", "ENOATTR"],
@@ -1322,15 +1337,16 @@
         "content": 8,
         "indic": 8,
         "instal": 9,
         "depend": 9,
         "stabl": 9,
         "version": 9,
         "request": 10,
-        "util": 11
+        "util": 11,
+        "2023": 2
     },
     "envversion": {
         "sphinx.domains.c": 2,
         "sphinx.domains.changeset": 1,
         "sphinx.domains.citation": 1,
         "sphinx.domains.cpp": 8,
         "sphinx.domains.index": 1,
@@ -1357,14 +1373,17 @@
         ],
         "asyncio Support": [
             [1, "asyncio-support"]
         ],
         "Changelog": [
             [2, "changelog"]
         ],
+        "Release 3.2.3 (2023-05-09)": [
+            [2, "release-3-2-3-2023-05-09"]
+        ],
         "Release 3.2.2 (2022-09-28)": [
             [2, "release-3-2-2-2022-09-28"]
         ],
         "Release 3.2.1 (2021-09-17)": [
             [2, "release-3-2-1-2021-09-17"]
         ],
         "Release 3.2.0 (2020-12-30)": [
```

### Comparing `pyfuse3-3.2.2/doc/html/util.html` & `pyfuse3-3.2.3/doc/html/util.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Utility Functions &#8212; pyfuse3 3.2.2 documentation</title>
+    <title>Utility Functions &#8212; pyfuse3 3.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/classic.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -34,15 +34,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="gotchas.html" title="Common Gotchas"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="operations.html" title="Request Handlers"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Utility Functions</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -53,47 +53,47 @@
 <p>The following functions do not necessarily translate to calls to the
 FUSE library. They are provided because they’re potentially useful
 when implementing file systems in Python.</p>
 <dl class="py function">
 <dt class="sig sig-object py" id="pyfuse3.setxattr">
 <span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">setxattr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">path</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">namespace</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'user'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#pyfuse3.setxattr" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set extended attribute</p>
-<p><em>path</em> and <em>name</em> have to be of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">str</span></code></a>. In Python 3.x, they may
-contain surrogates. <em>value</em> has to be of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a>.</p>
+<p><em>path</em> and <em>name</em> have to be of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">str</span></code></a>. In Python 3.x, they may
+contain surrogates. <em>value</em> has to be of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a>.</p>
 <p>Under FreeBSD, the <em>namespace</em> parameter may be set to <em>system</em> or <em>user</em> to
 select the namespace for the extended attribute. For other platforms, this
 parameter is ignored.</p>
-<p>In contrast to the <a class="reference external" href="https://docs.python.org/3/library/os.html#os.setxattr" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">os.setxattr</span></code></a> function from the standard library, the
+<p>In contrast to the <a class="reference external" href="https://docs.python.org/3/library/os.html#os.setxattr" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">os.setxattr</span></code></a> function from the standard library, the
 method provided by pyfuse3 is also available for non-Linux systems.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="pyfuse3.getxattr">
 <span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">getxattr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">path</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">size_t</span> <span class="pre">size_guess=128</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">namespace=u'user'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#pyfuse3.getxattr" title="Permalink to this definition">¶</a></dt>
 <dd><p>Get extended attribute</p>
-<p><em>path</em> and <em>name</em> have to be of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">str</span></code></a>. In Python 3.x, they may
-contain surrogates. Returns a value of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a>.</p>
+<p><em>path</em> and <em>name</em> have to be of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">str</span></code></a>. In Python 3.x, they may
+contain surrogates. Returns a value of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">bytes</span></code></a>.</p>
 <p>If the caller knows the approximate size of the attribute value,
 it should be supplied in <em>size_guess</em>. If the guess turns out
 to be wrong, the system call has to be carried out three times
 (the first call will fail, the second determines the size and
 the third finally gets the value).</p>
 <p>Under FreeBSD, the <em>namespace</em> parameter may be set to <em>system</em> or <em>user</em> to
 select the namespace for the extended attribute. For other platforms, this
 parameter is ignored.</p>
-<p>In contrast to the <a class="reference external" href="https://docs.python.org/3/library/os.html#os.getxattr" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">os.getxattr</span></code></a> function from the standard library, the
+<p>In contrast to the <a class="reference external" href="https://docs.python.org/3/library/os.html#os.getxattr" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">os.getxattr</span></code></a> function from the standard library, the
 method provided by pyfuse3 is also available for non-Linux systems.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="pyfuse3.listdir">
 <span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">listdir</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">path</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#pyfuse3.listdir" title="Permalink to this definition">¶</a></dt>
-<dd><p>Like <a class="reference external" href="https://docs.python.org/3/library/os.html#os.listdir" title="(in Python v3.10)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">os.listdir</span></code></a>, but releases the GIL.</p>
+<dd><p>Like <a class="reference external" href="https://docs.python.org/3/library/os.html#os.listdir" title="(in Python v3.11)"><code class="xref py py-obj docutils literal notranslate"><span class="pre">os.listdir</span></code></a>, but releases the GIL.</p>
 <p>This function returns an iterator over the directory entries in <em>path</em>.</p>
-<p>The returned values are of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#textseq" title="(in Python v3.10)"><span class="xref std std-ref">str</span></a>. Surrogate
+<p>The returned values are of type <a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#textseq" title="(in Python v3.11)"><span class="xref std std-ref">str</span></a>. Surrogate
 escape coding (cf.  <a class="reference external" href="http://www.python.org/dev/peps/pep-0383/">PEP 383</a>)
 is used for directory names that do not have a string representation.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="pyfuse3.get_sup_groups">
 <span class="sig-prename descclassname"><span class="pre">pyfuse3.</span></span><span class="sig-name descname"><span class="pre">get_sup_groups</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">pid</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#pyfuse3.get_sup_groups" title="Permalink to this definition">¶</a></dt>
@@ -170,15 +170,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="gotchas.html" title="Common Gotchas"
              >next</a> |</li>
         <li class="right" >
           <a href="operations.html" title="Request Handlers"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">pyfuse3 3.2.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Utility Functions</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2015, Nikolaus Rath.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.2.2.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Utility Functions
 ****** Utility FunctionsÂ¶ ******
 The following functions do not necessarily translate to calls to the FUSE
 library. They are provided because theyâre potentially useful when
 implementing file systems in Python.
   pyfuse3.setxattr(path, name, value, namespace='user')Â¶
       Set extended attribute
@@ -74,10 +74,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * pyfuse3_3.2.2_documentation »
+    * pyfuse3_3.2.3_documentation »
     * Utility Functions
 © Copyright 2010-2015, Nikolaus Rath. Created using Sphinx 5.2.2.
```

### Comparing `pyfuse3-3.2.2/examples/hello.py` & `pyfuse3-3.2.3/examples/hello.py`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/examples/hello_asyncio.py` & `pyfuse3-3.2.3/examples/hello_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/examples/passthroughfs.py` & `pyfuse3-3.2.3/examples/passthroughfs.py`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/examples/tmpfs.py` & `pyfuse3-3.2.3/examples/tmpfs.py`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/rst/conf.py` & `pyfuse3-3.2.3/rst/conf.py`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/rst/data.rst` & `pyfuse3-3.2.3/rst/data.rst`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/rst/example.rst` & `pyfuse3-3.2.3/rst/example.rst`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/rst/fuse_api.rst` & `pyfuse3-3.2.3/rst/fuse_api.rst`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/rst/general.rst` & `pyfuse3-3.2.3/rst/general.rst`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/rst/gotchas.rst` & `pyfuse3-3.2.3/rst/gotchas.rst`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/rst/install.rst` & `pyfuse3-3.2.3/rst/install.rst`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/rst/operations.rst` & `pyfuse3-3.2.3/rst/operations.rst`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/setup.py` & `pyfuse3-3.2.3/setup.py`

 * *Files 3% similar despite different names*

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
 
 # When running from Git repo, enable all warnings
 DEVELOPER_MODE = os.path.exists(os.path.join(basedir, 'MANIFEST.in'))
 if DEVELOPER_MODE:
     print('found MANIFEST.in, running in developer mode')
     warnings.resetwarnings()
@@ -53,15 +48,15 @@
     # DeprecationWarning.
     warnings.simplefilter('default')
 
 # Add src to load path, important for Sphinx autodoc
 # to work properly
 sys.path.insert(0, os.path.join(basedir, 'src'))
 
-PYFUSE3_VERSION = '3.2.2'
+PYFUSE3_VERSION = '3.2.3'
 
 def main():
 
     try:
         from sphinx.application import Sphinx #pylint: disable-msg=W0612
     except ImportError:
         pass
@@ -130,14 +125,15 @@
                        'Programming Language :: Python :: 3',
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
                        'Operating System :: POSIX :: BSD :: FreeBSD',
                        'Typing :: Typed'],
@@ -222,22 +218,23 @@
     def run(self):
         cython = None
         for c in ('cython3', 'cython'):
             try:
                 version = subprocess.check_output([c, '--version'],
                                               universal_newlines=True, stderr=subprocess.STDOUT)
                 cython = c
-            except FileNotFoundError:
+            except OSError:  # file not found, permission denied, ..., see issue #63
                 pass
         if cython is None:
             raise SystemExit('Cython needs to be installed for this command') from None
 
         hit = re.match('^Cython version (.+)$', version)
-        if not hit or LooseVersion(hit.group(1)) < "0.24":
-            raise SystemExit('Need Cython 0.24 or newer, found ' + version)
+        if not hit or LooseVersion(hit.group(1)) < "0.29":
+            # in fact we need a very recent Cython 0.29.x to support recent Pythons
+            raise SystemExit('Need Cython 0.29 or newer, found ' + version)
 
         cmd = [cython, '-Wextra', '--force', '-3', '--fast-fail',
                '--directive', 'embedsignature=True', '--include-dir',
                os.path.join(basedir, 'Include'), '--verbose' ]
         if DEVELOPER_MODE:
             cmd.append('-Werror')
```

### Comparing `pyfuse3-3.2.2/src/_pyfuse3.py` & `pyfuse3-3.2.3/src/_pyfuse3.py`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/src/darwin_compat.c` & `pyfuse3-3.2.3/src/darwin_compat.c`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/src/darwin_compat.h` & `pyfuse3-3.2.3/src/darwin_compat.h`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/src/gettime.h` & `pyfuse3-3.2.3/src/gettime.h`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/src/handlers.pxi` & `pyfuse3-3.2.3/src/handlers.pxi`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/src/internal.pxi` & `pyfuse3-3.2.3/src/internal.pxi`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/src/macros.c` & `pyfuse3-3.2.3/src/macros.c`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/src/macros.pxd` & `pyfuse3-3.2.3/src/macros.pxd`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/src/pyfuse3.c` & `pyfuse3-3.2.3/src/pyfuse3.c`

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
@@ -2025,26 +2073,26 @@
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
 
@@ -2426,20 +2474,28 @@
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
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
@@ -27481,15 +27537,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle__WorkerData, (type(self), 0xe8d9c4e, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle__WorkerData__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(0, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_7pyfuse3___pyx_unpickle__WorkerData__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle__WorkerData, (type(self), 0xe8d9c4e, state)
@@ -29851,15 +29907,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_RequestContext, (type(self), 0x223b7a8, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_RequestContext__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(0, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_7pyfuse3___pyx_unpickle_RequestContext__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_RequestContext, (type(self), 0x223b7a8, state)
@@ -40909,19 +40965,19 @@
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
 
   /* "pyfuse3.pyx":1021
  *         else:
  *             raise RuntimeError("Unable to parse %s" % fh.name)
  *     gids = set()             # <<<<<<<<<<<<<<
  *     for x in line.split()[1:]:
@@ -41553,15 +41609,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = _WorkerData.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle__WorkerData__set_state(<_WorkerData> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle__WorkerData__set_state(_WorkerData __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(0, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(0, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_f_7pyfuse3___pyx_unpickle__WorkerData__set_state(((struct __pyx_obj_7pyfuse3__WorkerData *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe8d9c4e, 0x2a8cfde, 0x9365cf3) = (active_readers, read_lock, task_count, task_serial))" % __pyx_checksum)
  *     __pyx_result = _WorkerData.__new__(__pyx_type)
@@ -41983,15 +42039,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = RequestContext.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_RequestContext__set_state(<RequestContext> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_RequestContext__set_state(RequestContext __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(0, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(0, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_f_7pyfuse3___pyx_unpickle_RequestContext__set_state(((struct __pyx_obj_7pyfuse3_RequestContext *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x223b7a8, 0xe56624f, 0x8a019cd) = (gid, pid, uid, umask))" % __pyx_checksum)
  *     __pyx_result = RequestContext.__new__(__pyx_type)
@@ -49412,15 +49468,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(3, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(3, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(3, 1, __pyx_L1_error)
   __pyx_int_35895208 = PyInt_FromLong(35895208L); if (unlikely(!__pyx_int_35895208)) __PYX_ERR(3, 1, __pyx_L1_error)
   __pyx_int_44617694 = PyInt_FromLong(44617694L); if (unlikely(!__pyx_int_44617694)) __PYX_ERR(3, 1, __pyx_L1_error)
   __pyx_int_144710093 = PyInt_FromLong(144710093L); if (unlikely(!__pyx_int_144710093)) __PYX_ERR(3, 1, __pyx_L1_error)
   __pyx_int_154557683 = PyInt_FromLong(154557683L); if (unlikely(!__pyx_int_154557683)) __PYX_ERR(3, 1, __pyx_L1_error)
   __pyx_int_240542287 = PyInt_FromLong(240542287L); if (unlikely(!__pyx_int_240542287)) __PYX_ERR(3, 1, __pyx_L1_error)
@@ -49843,17 +49899,17 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
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
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
@@ -50043,15 +50099,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(3, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(3, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(3, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(3, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pyfuse3) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main_2) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
@@ -51383,28 +51439,28 @@
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
@@ -51552,15 +51608,15 @@
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
@@ -51640,17 +51696,15 @@
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
@@ -53432,15 +53486,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030500B2 || defined(PyCoro_CheckExact)
     if (PyCoro_CheckExact(obj)) {
         return __Pyx_NewRef(obj);
     } else
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && defined(CO_ITERABLE_COROUTINE)
+#if PY_VERSION_HEX >= 0x030C00A6
+    if (PyGen_CheckExact(obj) && (PyGen_GetCode(obj)->co_flags & CO_ITERABLE_COROUTINE)) {
+#else
     if (PyGen_CheckExact(obj) && ((PyGenObject*)obj)->gi_code && ((PyCodeObject *)((PyGenObject*)obj)->gi_code)->co_flags & CO_ITERABLE_COROUTINE) {
+#endif
         return __Pyx_NewRef(obj);
     } else
 #endif
     {
         PyObject *method = NULL;
         int is_method = __Pyx_PyObject_GetMethod(obj, __pyx_n_s_await, &method);
         if (likely(is_method)) {
@@ -53482,15 +53540,15 @@
                  "object %.100s can't be used in 'await' expression",
                  Py_TYPE(obj)->tp_name);
 bad:
     return NULL;
 }
 
 /* CoroutineYieldFrom */
-static PyObject* __Pyx__Coroutine_Yield_From_Generic(__pyx_CoroutineObject *gen, PyObject *source) {
+  static PyObject* __Pyx__Coroutine_Yield_From_Generic(__pyx_CoroutineObject *gen, PyObject *source) {
     PyObject *retval;
     PyObject *source_gen = __Pyx__Coroutine_GetAwaitableIter(source);
     if (unlikely(!source_gen)) {
         return NULL;
     }
     if (__Pyx_Coroutine_Check(source_gen)) {
         retval = __Pyx_Generator_Next(source_gen);
@@ -53529,28 +53587,28 @@
         Py_INCREF(source);
         gen->yieldfrom = source;
     }
     return retval;
 }
 
 /* ExtTypeTest */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+  static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     if (likely(__Pyx_TypeCheck(obj, type)))
         return 1;
     PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
                  Py_TYPE(obj)->tp_name, type->tp_name);
     return 0;
 }
 
 /* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
+  #if CYTHON_FAST_THREAD_STATE
 static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
     for (i=0; i<n; i++) {
         if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
     }
@@ -53567,15 +53625,15 @@
     if (unlikely(PyTuple_Check(err)))
         return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
     return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
 }
 #endif
 
 /* GetException */
-#if CYTHON_FAST_THREAD_STATE
+  #if CYTHON_FAST_THREAD_STATE
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
 #endif
 {
     PyObject *local_type, *local_value, *local_tb;
 #if CYTHON_FAST_THREAD_STATE
@@ -53641,15 +53699,15 @@
     Py_XDECREF(local_type);
     Py_XDECREF(local_value);
     Py_XDECREF(local_tb);
     return -1;
 }
 
 /* BytesEquals */
-static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+  static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
 #if CYTHON_COMPILING_IN_PYPY
     return PyObject_RichCompareBool(s1, s2, equals);
 #else
     if (s1 == s2) {
         return (equals == Py_EQ);
     } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
         const char *ps1, *ps2;
@@ -53688,15 +53746,15 @@
         Py_DECREF(py_result);
         return result;
     }
 #endif
 }
 
 /* UnicodeEquals */
-static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+  static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
 #if CYTHON_COMPILING_IN_PYPY
     return PyObject_RichCompareBool(s1, s2, equals);
 #else
 #if PY_MAJOR_VERSION < 3
     PyObject* owned_ref = NULL;
 #endif
     int s1_is_unicode, s2_is_unicode;
@@ -53790,22 +53848,22 @@
     Py_XDECREF(owned_ref);
     #endif
     return (equals == Py_NE);
 #endif
 }
 
 /* StringJoin */
-#if !CYTHON_COMPILING_IN_CPYTHON
+  #if !CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyBytes_Join(PyObject* sep, PyObject* values) {
     return PyObject_CallMethodObjArgs(sep, __pyx_n_s_join, values, NULL);
 }
 #endif
 
 /* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+  static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
@@ -53884,28 +53942,28 @@
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* RaiseTooManyValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
+  static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
     PyErr_Format(PyExc_ValueError,
                  "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
 }
 
 /* RaiseNeedMoreValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
+  static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
     PyErr_Format(PyExc_ValueError,
                  "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
                  index, (index == 1) ? "" : "s");
 }
 
 /* IterFinish */
-static CYTHON_INLINE int __Pyx_IterFinish(void) {
+  static CYTHON_INLINE int __Pyx_IterFinish(void) {
 #if CYTHON_FAST_THREAD_STATE
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject* exc_type = tstate->curexc_type;
     if (unlikely(exc_type)) {
         if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) {
             PyObject *exc_value, *exc_tb;
             exc_value = tstate->curexc_value;
@@ -53932,27 +53990,25 @@
         }
     }
     return 0;
 #endif
 }
 
 /* UnpackItemEndCheck */
-static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
+  static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
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
 
 /* KeywordStringCheck */
-static int __Pyx_CheckKeywordStrings(
+  static int __Pyx_CheckKeywordStrings(
     PyObject *kwdict,
     const char* function_name,
     int kw_allowed)
 {
     PyObject* key = 0;
     Py_ssize_t pos = 0;
 #if CYTHON_COMPILING_IN_PYPY
@@ -53984,43 +54040,43 @@
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
     return 0;
 }
 
 /* GetAttr */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
+  static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
 #if CYTHON_USE_TYPE_SLOTS
 #if PY_MAJOR_VERSION >= 3
     if (likely(PyUnicode_Check(n)))
 #else
     if (likely(PyString_Check(n)))
 #endif
         return __Pyx_PyObject_GetAttrStr(o, n);
 #endif
     return PyObject_GetAttr(o, n);
 }
 
 /* GetAttr3 */
-static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
+  static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         return NULL;
     __Pyx_PyErr_Clear();
     Py_INCREF(d);
     return d;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
     PyObject *r = __Pyx_GetAttr(o, n);
     return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
 }
 
 /* ReturnWithStopIteration */
-static void __Pyx__ReturnWithStopIteration(PyObject* value) {
+  static void __Pyx__ReturnWithStopIteration(PyObject* value) {
     PyObject *exc, *args;
 #if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_PYSTON
     __Pyx_PyThreadState_declare
     if ((PY_VERSION_HEX >= 0x03030000 && PY_VERSION_HEX < 0x030500B1)
             || unlikely(PyTuple_Check(value) || PyExceptionInstance_Check(value))) {
         args = PyTuple_New(1);
         if (unlikely(!args)) return;
@@ -54054,15 +54110,15 @@
     if (unlikely(!exc)) return;
 #endif
     PyErr_SetObject(PyExc_StopIteration, exc);
     Py_DECREF(exc);
 }
 
 /* FastTypeChecks */
-#if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = a->tp_base;
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
@@ -54154,15 +54210,15 @@
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* PyObjectCallMethod0 */
-static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
+  static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
     PyObject *method = NULL, *result = NULL;
     int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
     if (likely(is_method)) {
         result = __Pyx_PyObject_CallOneArg(method, obj);
         Py_DECREF(method);
         return result;
     }
@@ -54170,31 +54226,31 @@
     result = __Pyx_PyObject_CallNoArg(method);
     Py_DECREF(method);
 bad:
     return result;
 }
 
 /* RaiseNoneIterError */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
+  static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
 }
 
 /* UnpackTupleError */
-static void __Pyx_UnpackTupleError(PyObject *t, Py_ssize_t index) {
+  static void __Pyx_UnpackTupleError(PyObject *t, Py_ssize_t index) {
     if (t == Py_None) {
       __Pyx_RaiseNoneNotIterableError();
     } else if (PyTuple_GET_SIZE(t) < index) {
       __Pyx_RaiseNeedMoreValuesError(PyTuple_GET_SIZE(t));
     } else {
       __Pyx_RaiseTooManyValuesError(index);
     }
 }
 
 /* UnpackTuple2 */
-static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
+  static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
         PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2, int decref_tuple) {
     PyObject *value1 = NULL, *value2 = NULL;
 #if CYTHON_COMPILING_IN_PYPY
     value1 = PySequence_ITEM(tuple, 0);  if (unlikely(!value1)) goto bad;
     value2 = PySequence_ITEM(tuple, 1);  if (unlikely(!value2)) goto bad;
 #else
     value1 = PyTuple_GET_ITEM(tuple, 0);  Py_INCREF(value1);
@@ -54238,15 +54294,15 @@
     Py_XDECREF(value1);
     Py_XDECREF(value2);
     if (decref_tuple) { Py_XDECREF(tuple); }
     return -1;
 }
 
 /* dict_iter */
-static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* iterable, int is_dict, PyObject* method_name,
+  static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* iterable, int is_dict, PyObject* method_name,
                                                    Py_ssize_t* p_orig_length, int* p_source_is_dict) {
     is_dict = is_dict || likely(PyDict_CheckExact(iterable));
     *p_source_is_dict = is_dict;
     if (is_dict) {
 #if !CYTHON_COMPILING_IN_PYPY
         *p_orig_length = PyDict_Size(iterable);
         Py_INCREF(iterable);
@@ -54351,34 +54407,34 @@
     } else {
         *pvalue = next_item;
     }
     return 1;
 }
 
 /* PyObjectSetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
+  #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_setattro))
         return tp->tp_setattro(obj, attr_name, value);
 #if PY_MAJOR_VERSION < 3
     if (likely(tp->tp_setattr))
         return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
 #endif
     return PyObject_SetAttr(obj, attr_name, value);
 }
 #endif
 
 /* None */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
+  static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
     PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
 }
 
 /* SliceObject */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(PyObject* obj,
+  static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(PyObject* obj,
         Py_ssize_t cstart, Py_ssize_t cstop,
         PyObject** _py_start, PyObject** _py_stop, PyObject** _py_slice,
         int has_cstart, int has_cstop, CYTHON_UNUSED int wraparound) {
 #if CYTHON_USE_TYPE_SLOTS
     PyMappingMethods* mp;
 #if PY_MAJOR_VERSION < 3
     PySequenceMethods* ms = Py_TYPE(obj)->tp_as_sequence;
@@ -54467,15 +54523,15 @@
     PyErr_Format(PyExc_TypeError,
         "'%.200s' object is unsliceable", Py_TYPE(obj)->tp_name);
 bad:
     return NULL;
 }
 
 /* Import */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+  static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
     PyObject *empty_list = 0;
     PyObject *module = 0;
     PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
     PyObject *list;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
@@ -54532,29 +54588,29 @@
     #endif
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* ImportFrom */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
+  static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
     PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
     if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Format(PyExc_ImportError,
         #if PY_MAJOR_VERSION < 3
             "cannot import name %.230s", PyString_AS_STRING(name));
         #else
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
 /* HasAttr */
-static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
+  static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
     PyObject *r;
     if (unlikely(!__Pyx_PyBaseString_Check(n))) {
         PyErr_SetString(PyExc_TypeError,
                         "hasattr(): attribute name must be string");
         return -1;
     }
     r = __Pyx_GetAttr(o, n);
@@ -54564,25 +54620,25 @@
     } else {
         Py_DECREF(r);
         return 1;
     }
 }
 
 /* PyObject_GenericGetAttr */
-#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+  #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name) {
     if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
-static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+  static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
@@ -54596,15 +54652,15 @@
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
 }
 
 /* SetupReduce */
-static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
+  static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
   name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name_2);
   if (likely(name_attr)) {
       ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
   } else {
       ret = -1;
@@ -54700,15 +54756,15 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* SetVTable */
-static int __Pyx_SetVtable(PyObject *dict, void *vtable) {
+  static int __Pyx_SetVtable(PyObject *dict, void *vtable) {
 #if PY_VERSION_HEX >= 0x02070000
     PyObject *ob = PyCapsule_New(vtable, 0, 0);
 #else
     PyObject *ob = PyCObject_FromVoidPtr(vtable, 0);
 #endif
     if (!ob)
         goto bad;
@@ -54718,47 +54774,65 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
+  #ifndef __PYX_HAVE_RT_ImportType
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
@@ -54779,15 +54853,15 @@
 bad:
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* decode_c_string */
-static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
+  static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
     Py_ssize_t length;
     if (unlikely((start < 0) | (stop < 0))) {
         size_t slen = strlen(cstring);
         if (unlikely(slen > (size_t) PY_SSIZE_T_MAX)) {
@@ -54812,15 +54886,15 @@
         return decode_func(cstring, length, errors);
     } else {
         return PyUnicode_Decode(cstring, length, encoding, errors);
     }
 }
 
 /* Globals */
-static PyObject* __Pyx_Globals(void) {
+  static PyObject* __Pyx_Globals(void) {
     Py_ssize_t i;
     PyObject *names;
     PyObject *globals = __pyx_d;
     Py_INCREF(globals);
     names = PyObject_Dir(__pyx_m);
     if (!names)
         goto bad;
@@ -54857,15 +54931,15 @@
 bad:
     Py_XDECREF(names);
     Py_XDECREF(globals);
     return NULL;
 }
 
 /* pyfrozenset_new */
-static CYTHON_INLINE PyObject* __Pyx_PyFrozenSet_New(PyObject* it) {
+  static CYTHON_INLINE PyObject* __Pyx_PyFrozenSet_New(PyObject* it) {
     if (it) {
         PyObject* result;
 #if CYTHON_COMPILING_IN_PYPY
         PyObject* args;
         args = PyTuple_Pack(1, it);
         if (unlikely(!args))
             return NULL;
@@ -54889,16 +54963,16 @@
     return PyFrozenSet_Type.tp_new(&PyFrozenSet_Type, __pyx_empty_tuple, NULL);
 #else
     return PyObject_Call((PyObject*)&PyFrozenSet_Type, __pyx_empty_tuple, NULL);
 #endif
 }
 
 /* CLineInTraceback */
-#ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+  #ifndef CYTHON_CLINE_IN_TRACEBACK
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -54931,15 +55005,15 @@
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+  static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -55011,15 +55085,15 @@
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
-#include "compile.h"
+  #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
@@ -55118,15 +55192,15 @@
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 /* CIntFromPyVerify */
-#define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
         func_type value = func_value;\
         if (sizeof(target_type) < sizeof(func_type)) {\
@@ -55140,15 +55214,15 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -55178,15 +55252,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+  static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -55374,15 +55448,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_gid_t(gid_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_gid_t(gid_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const gid_t neg_one = (gid_t) -1, const_zero = (gid_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -55412,15 +55486,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(gid_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE gid_t __Pyx_PyInt_As_gid_t(PyObject *x) {
+  static CYTHON_INLINE gid_t __Pyx_PyInt_As_gid_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const gid_t neg_one = (gid_t) -1, const_zero = (gid_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -55608,15 +55682,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to gid_t");
     return (gid_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_pid_t(pid_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_pid_t(pid_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const pid_t neg_one = (pid_t) -1, const_zero = (pid_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -55646,15 +55720,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(pid_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE pid_t __Pyx_PyInt_As_pid_t(PyObject *x) {
+  static CYTHON_INLINE pid_t __Pyx_PyInt_As_pid_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const pid_t neg_one = (pid_t) -1, const_zero = (pid_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -55842,15 +55916,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to pid_t");
     return (pid_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uid_t(uid_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uid_t(uid_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const uid_t neg_one = (uid_t) -1, const_zero = (uid_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -55880,15 +55954,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(uid_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE uid_t __Pyx_PyInt_As_uid_t(PyObject *x) {
+  static CYTHON_INLINE uid_t __Pyx_PyInt_As_uid_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const uid_t neg_one = (uid_t) -1, const_zero = (uid_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -56076,15 +56150,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to uid_t");
     return (uid_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_mode_t(mode_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_mode_t(mode_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const mode_t neg_one = (mode_t) -1, const_zero = (mode_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -56114,15 +56188,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(mode_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE mode_t __Pyx_PyInt_As_mode_t(PyObject *x) {
+  static CYTHON_INLINE mode_t __Pyx_PyInt_As_mode_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const mode_t neg_one = (mode_t) -1, const_zero = (mode_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -56310,15 +56384,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to mode_t");
     return (mode_t) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
+  static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const size_t neg_one = (size_t) -1, const_zero = (size_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -56506,15 +56580,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to size_t");
     return (size_t) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE fuse_ino_t __Pyx_PyInt_As_fuse_ino_t(PyObject *x) {
+  static CYTHON_INLINE fuse_ino_t __Pyx_PyInt_As_fuse_ino_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const fuse_ino_t neg_one = (fuse_ino_t) -1, const_zero = (fuse_ino_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -56702,15 +56776,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to fuse_ino_t");
     return (fuse_ino_t) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE off_t __Pyx_PyInt_As_off_t(PyObject *x) {
+  static CYTHON_INLINE off_t __Pyx_PyInt_As_off_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const off_t neg_one = (off_t) -1, const_zero = (off_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -56898,15 +56972,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to off_t");
     return (off_t) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+  static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -57094,15 +57168,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const unsigned int neg_one = (unsigned int) -1, const_zero = (unsigned int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -57132,15 +57206,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(unsigned int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_fuse_ino_t(fuse_ino_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_fuse_ino_t(fuse_ino_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const fuse_ino_t neg_one = (fuse_ino_t) -1, const_zero = (fuse_ino_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -57170,15 +57244,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(fuse_ino_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint64_t(uint64_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint64_t(uint64_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const uint64_t neg_one = (uint64_t) -1, const_zero = (uint64_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -57208,15 +57282,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(uint64_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_dev_t(dev_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_dev_t(dev_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const dev_t neg_one = (dev_t) -1, const_zero = (dev_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -57246,15 +57320,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(dev_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_off_t(off_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_off_t(off_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const off_t neg_one = (off_t) -1, const_zero = (off_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -57284,15 +57358,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(off_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE uint64_t __Pyx_PyInt_As_uint64_t(PyObject *x) {
+  static CYTHON_INLINE uint64_t __Pyx_PyInt_As_uint64_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const uint64_t neg_one = (uint64_t) -1, const_zero = (uint64_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -57480,15 +57554,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to uint64_t");
     return (uint64_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -57518,15 +57592,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE ino_t __Pyx_PyInt_As_ino_t(PyObject *x) {
+  static CYTHON_INLINE ino_t __Pyx_PyInt_As_ino_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const ino_t neg_one = (ino_t) -1, const_zero = (ino_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -57714,15 +57788,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to ino_t");
     return (ino_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_nlink_t(nlink_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_nlink_t(nlink_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const nlink_t neg_one = (nlink_t) -1, const_zero = (nlink_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -57752,15 +57826,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(nlink_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE nlink_t __Pyx_PyInt_As_nlink_t(PyObject *x) {
+  static CYTHON_INLINE nlink_t __Pyx_PyInt_As_nlink_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const nlink_t neg_one = (nlink_t) -1, const_zero = (nlink_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -57948,15 +58022,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to nlink_t");
     return (nlink_t) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE dev_t __Pyx_PyInt_As_dev_t(PyObject *x) {
+  static CYTHON_INLINE dev_t __Pyx_PyInt_As_dev_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const dev_t neg_one = (dev_t) -1, const_zero = (dev_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -58144,15 +58218,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to dev_t");
     return (dev_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_blkcnt_t(blkcnt_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_blkcnt_t(blkcnt_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const blkcnt_t neg_one = (blkcnt_t) -1, const_zero = (blkcnt_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -58182,15 +58256,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(blkcnt_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE blkcnt_t __Pyx_PyInt_As_blkcnt_t(PyObject *x) {
+  static CYTHON_INLINE blkcnt_t __Pyx_PyInt_As_blkcnt_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const blkcnt_t neg_one = (blkcnt_t) -1, const_zero = (blkcnt_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -58378,15 +58452,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to blkcnt_t");
     return (blkcnt_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_blksize_t(blksize_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_blksize_t(blksize_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const blksize_t neg_one = (blksize_t) -1, const_zero = (blksize_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -58416,15 +58490,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(blksize_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE blksize_t __Pyx_PyInt_As_blksize_t(PyObject *x) {
+  static CYTHON_INLINE blksize_t __Pyx_PyInt_As_blksize_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const blksize_t neg_one = (blksize_t) -1, const_zero = (blksize_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -58612,15 +58686,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to blksize_t");
     return (blksize_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_time_t(time_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_time_t(time_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const time_t neg_one = (time_t) -1, const_zero = (time_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -58650,15 +58724,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(time_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE time_t __Pyx_PyInt_As_time_t(PyObject *x) {
+  static CYTHON_INLINE time_t __Pyx_PyInt_As_time_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const time_t neg_one = (time_t) -1, const_zero = (time_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -58846,15 +58920,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to time_t");
     return (time_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_long(unsigned long value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_long(unsigned long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const unsigned long neg_one = (unsigned long) -1, const_zero = (unsigned long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -58884,15 +58958,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(unsigned long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE unsigned long __Pyx_PyInt_As_unsigned_long(PyObject *x) {
+  static CYTHON_INLINE unsigned long __Pyx_PyInt_As_unsigned_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const unsigned long neg_one = (unsigned long) -1, const_zero = (unsigned long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -59080,15 +59154,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to unsigned long");
     return (unsigned long) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_fsblkcnt_t(fsblkcnt_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_fsblkcnt_t(fsblkcnt_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const fsblkcnt_t neg_one = (fsblkcnt_t) -1, const_zero = (fsblkcnt_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -59118,15 +59192,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(fsblkcnt_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE fsblkcnt_t __Pyx_PyInt_As_fsblkcnt_t(PyObject *x) {
+  static CYTHON_INLINE fsblkcnt_t __Pyx_PyInt_As_fsblkcnt_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const fsblkcnt_t neg_one = (fsblkcnt_t) -1, const_zero = (fsblkcnt_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -59314,15 +59388,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to fsblkcnt_t");
     return (fsblkcnt_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_fsfilcnt_t(fsfilcnt_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_fsfilcnt_t(fsfilcnt_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const fsfilcnt_t neg_one = (fsfilcnt_t) -1, const_zero = (fsfilcnt_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -59352,15 +59426,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(fsfilcnt_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE fsfilcnt_t __Pyx_PyInt_As_fsfilcnt_t(PyObject *x) {
+  static CYTHON_INLINE fsfilcnt_t __Pyx_PyInt_As_fsfilcnt_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const fsfilcnt_t neg_one = (fsfilcnt_t) -1, const_zero = (fsfilcnt_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -59548,15 +59622,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to fsfilcnt_t");
     return (fsfilcnt_t) -1;
 }
 
 /* CheckBinaryVersion */
-static int __Pyx_check_binary_version(void) {
+  static int __Pyx_check_binary_version(void) {
     char ctversion[5];
     int same=1, i, found_dot;
     const char* rt_from_call = Py_GetVersion();
     PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
     found_dot = 0;
     for (i = 0; i < 4; i++) {
         if (!ctversion[i]) {
@@ -59586,15 +59660,15 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
-static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+  static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
         #if PY_MAJOR_VERSION < 3
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
```

### Comparing `pyfuse3-3.2.2/src/pyfuse3.egg-info/PKG-INFO` & `pyfuse3-3.2.3/src/pyfuse3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfuse3
-Version: 3.2.2
+Version: 3.2.3
 Summary: Python 3 bindings for libfuse 3 with async I/O support
 Home-page: https://github.com/libfuse/pyfuse3
 Author: Nikolaus Rath
 Author-email: Nikolaus@rath.org
 License: LGPL
 Keywords: FUSE,python
 Platform: Linux
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
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
 Classifier: Typing :: Typed
```

### Comparing `pyfuse3-3.2.2/src/pyfuse3.egg-info/SOURCES.txt` & `pyfuse3-3.2.3/src/pyfuse3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Changes.rst
 LICENSE
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 Include/fuse_common.pxd
 Include/fuse_lowlevel.pxd
 Include/fuse_opt.pxd
 Include/libc_extra.pxd
 doc/html/.buildinfo
@@ -106,8 +107,10 @@
 test/util.py
 test/.pytest_cache/.gitignore
 test/.pytest_cache/CACHEDIR.TAG
 test/.pytest_cache/README.md
 test/.pytest_cache/v/cache/lastfailed
 test/.pytest_cache/v/cache/nodeids
 test/.pytest_cache/v/cache/stepwise
-util/sphinx_cython.py
+util/sdist-sign
+util/sphinx_cython.py
+util/upload-pypi
```

### Comparing `pyfuse3-3.2.2/src/pyfuse3.h` & `pyfuse3-3.2.3/src/pyfuse3.h`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/src/pyfuse3.pyi` & `pyfuse3-3.2.3/src/pyfuse3.pyi`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/src/pyfuse3.pyx` & `pyfuse3-3.2.3/src/pyfuse3.pyx`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/src/pyfuse3_asyncio.py` & `pyfuse3-3.2.3/src/pyfuse3_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/src/xattr.h` & `pyfuse3-3.2.3/src/xattr.h`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/test/.pytest_cache/v/cache/nodeids` & `pyfuse3-3.2.3/test/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/test/conftest.py` & `pyfuse3-3.2.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/test/pytest_checklogs.py` & `pyfuse3-3.2.3/test/pytest_checklogs.py`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/test/test_api.py` & `pyfuse3-3.2.3/test/test_api.py`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/test/test_examples.py` & `pyfuse3-3.2.3/test/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,16 +358,18 @@
 
 
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

### Comparing `pyfuse3-3.2.2/test/test_fs.py` & `pyfuse3-3.2.3/test/test_fs.py`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/test/test_rounding.py` & `pyfuse3-3.2.3/test/test_rounding.py`

 * *Files identical despite different names*

### Comparing `pyfuse3-3.2.2/test/util.py` & `pyfuse3-3.2.3/test/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 This file is part of pyfuse3. This work may be distributed under
 the terms of the GNU LGPL.
 '''
 
 import os
 import platform
 import pytest
+import shutil
 import stat
 import subprocess
 import time
 
 def fuse_test_marker():
     '''Return a pytest.marker that indicates FUSE availability
 
@@ -25,19 +26,16 @@
     '''
 
     if platform.system() == 'Darwin':
         # No working autodetection, just assume it will work.
         return
     skip = lambda x: pytest.mark.skip(reason=x)
 
-    with subprocess.Popen(['which', 'fusermount'], stdout=subprocess.PIPE,
-                           universal_newlines=True) as which:
-        fusermount_path = which.communicate()[0].strip()
-
-    if not fusermount_path or which.returncode != 0:
+    fusermount_path = shutil.which('fusermount')
+    if fusermount_path is None:
         return skip("Can't find fusermount executable")
 
     if not os.path.exists('/dev/fuse'):
         return skip("FUSE kernel module does not seem to be loaded")
 
     if os.getuid() == 0:
         return pytest.mark.uses_fuse()
```

### Comparing `pyfuse3-3.2.2/util/sphinx_cython.py` & `pyfuse3-3.2.3/util/sphinx_cython.py`

 * *Files identical despite different names*

