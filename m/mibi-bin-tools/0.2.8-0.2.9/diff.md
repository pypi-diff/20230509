# Comparing `tmp/mibi-bin-tools-0.2.8.tar.gz` & `tmp/mibi-bin-tools-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mibi-bin-tools-0.2.8.tar", last modified: Wed Mar 15 23:40:25 2023, max compression
+gzip compressed data, was "mibi-bin-tools-0.2.9.tar", last modified: Tue May  9 19:03:36 2023, max compression
```

## Comparing `mibi-bin-tools-0.2.8.tar` & `mibi-bin-tools-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:40:25.700034 mibi-bin-tools-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:40:25.688034 mibi-bin-tools-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:40:25.692034 mibi-bin-tools-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-03-15 23:40:25.700034 mibi-bin-tools-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 23:40:25.700034 mibi-bin-tools-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:40:25.688034 mibi-bin-tools-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:40:25.696034 mibi-bin-tools-0.2.8/src/mibi_bin_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/src/mibi_bin_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1055364 2023-03-15 23:40:24.000000 mibi-bin-tools-0.2.8/src/mibi_bin_tools/_extract_bin.c
--rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/src/mibi_bin_tools/_extract_bin.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    18508 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/src/mibi_bin_tools/bin_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/src/mibi_bin_tools/panel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/src/mibi_bin_tools/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:40:25.696034 mibi-bin-tools-0.2.8/src/mibi_bin_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-03-15 23:40:25.000000 mibi-bin-tools-0.2.8/src/mibi_bin_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-15 23:40:25.000000 mibi-bin-tools-0.2.8/src/mibi_bin_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 23:40:25.000000 mibi-bin-tools-0.2.8/src/mibi_bin_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-15 23:40:25.000000 mibi-bin-tools-0.2.8/src/mibi_bin_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-15 23:40:25.000000 mibi-bin-tools-0.2.8/src/mibi_bin_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:40:25.696034 mibi-bin-tools-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/tests/bin_files_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:40:25.688034 mibi-bin-tools-0.2.8/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:40:25.696034 mibi-bin-tools-0.2.8/tests/data/moly/
--rw-r--r--   0 runner    (1001) docker     (123)   652802 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/tests/data/moly/fov-1-scan-1.bin
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/tests/data/moly/fov-1-scan-1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:40:25.700034 mibi-bin-tools-0.2.8/tests/data/tissue/
--rw-r--r--   0 runner    (1001) docker     (123)   799610 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/tests/data/tissue/fov-1-scan-1.bin
--rw-r--r--   0 runner    (1001) docker     (123)    21562 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/tests/data/tissue/fov-1-scan-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   813312 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/tests/data/tissue/fov-2-scan-1.bin
--rw-r--r--   0 runner    (1001) docker     (123)    21568 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/tests/data/tissue/fov-2-scan-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/tests/panel_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-15 23:40:12.000000 mibi-bin-tools-0.2.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:03:36.414095 mibi-bin-tools-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:03:36.406095 mibi-bin-tools-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:03:36.410095 mibi-bin-tools-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-09 19:03:36.414095 mibi-bin-tools-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:03:36.414095 mibi-bin-tools-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:03:36.406095 mibi-bin-tools-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:03:36.410095 mibi-bin-tools-0.2.9/src/mibi_bin_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/src/mibi_bin_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1111918 2023-05-09 19:03:35.000000 mibi-bin-tools-0.2.9/src/mibi_bin_tools/_extract_bin.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/src/mibi_bin_tools/_extract_bin.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    18508 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/src/mibi_bin_tools/bin_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/src/mibi_bin_tools/panel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/src/mibi_bin_tools/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:03:36.410095 mibi-bin-tools-0.2.9/src/mibi_bin_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-09 19:03:36.000000 mibi-bin-tools-0.2.9/src/mibi_bin_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-09 19:03:36.000000 mibi-bin-tools-0.2.9/src/mibi_bin_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:03:36.000000 mibi-bin-tools-0.2.9/src/mibi_bin_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-09 19:03:36.000000 mibi-bin-tools-0.2.9/src/mibi_bin_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 19:03:36.000000 mibi-bin-tools-0.2.9/src/mibi_bin_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:03:36.410095 mibi-bin-tools-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/tests/bin_files_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:03:36.406095 mibi-bin-tools-0.2.9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:03:36.414095 mibi-bin-tools-0.2.9/tests/data/moly/
+-rw-r--r--   0 runner    (1001) docker     (123)   652802 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/tests/data/moly/fov-1-scan-1.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/tests/data/moly/fov-1-scan-1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:03:36.414095 mibi-bin-tools-0.2.9/tests/data/tissue/
+-rw-r--r--   0 runner    (1001) docker     (123)   799610 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/tests/data/tissue/fov-1-scan-1.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    21562 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/tests/data/tissue/fov-1-scan-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   813312 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/tests/data/tissue/fov-2-scan-1.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    21568 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/tests/data/tissue/fov-2-scan-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/tests/panel_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 19:03:18.000000 mibi-bin-tools-0.2.9/tox.ini
```

### Comparing `mibi-bin-tools-0.2.8/.github/workflows/build.yml` & `mibi-bin-tools-0.2.9/.github/workflows/build.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-name: Wheel Builder
+name: Build
 
 on:
   workflow_call:
 
 permissions:
   contents: read # to fetch code (actions/checkout)
 
 jobs:
   build_wheels:
-    name: Build  ${{ github.repository }} wheels on ${{ matrix.os }}
+    name: ${{ matrix.os }} Wheels
     runs-on: ${{ matrix.os }}
     strategy:
       # Ensure that a wheel builder finishes even if another fails
       fail-fast: false
       matrix:
-        os: [ubuntu-latest, windows-latest, macos-12]
+        os: [ubuntu-latest, windows-latest, macos-latest]
 
     steps:
       - name: Checkout ${{ github.repository }}
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up QEMU (For Linux ARM)
         if: runner.os == 'Linux'
         uses: docker/setup-qemu-action@v2
         with:
           platforms: arm64
 
       - name: Build Wheels
-        uses: pypa/cibuildwheel@v2.11.4
+        uses: pypa/cibuildwheel@v2.12.3
         with:
           package-dir: .
           output-dir: wheelhouse
           config-file: "{package}/pyproject.toml"
 
       - name: Store Wheel Artifacts
         uses: actions/upload-artifact@v3
         with:
           name: distributions
           path: wheelhouse/*.whl
 
   build_sdist:
-    name: Build ${{ github.repository }} Source Distribution
+    name: Source Distribution
     runs-on: ubuntu-latest
     steps:
       - name: Checkout ${{ github.repository }}
         uses: actions/checkout@v3
 
       - name: Build sdist
         run: pipx run build --sdist
```

### Comparing `mibi-bin-tools-0.2.8/.github/workflows/ci.yml` & `mibi-bin-tools-0.2.9/.github/workflows/ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -43,16 +43,13 @@
       - name: Checkout ${{github.repository }}
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Download Coverage Artifact
         uses: actions/download-artifact@v3
-        with:
-          name: coverage
-          path: coverage
+        # if `name` is not specified, all artifacts are downloaded.
 
       - name: Upload Coverage to Coveralls
-        uses: coverallsapp/github-action@master
+        uses: coverallsapp/github-action@v2
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
-          path-to-lcov: ${{ github.workspace }}/coverage/coverage.lcov
```

### Comparing `mibi-bin-tools-0.2.8/.github/workflows/pypi_publish.yml` & `mibi-bin-tools-0.2.9/.github/workflows/pypi_publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -36,36 +36,36 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: distributions
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@release/v1.6
+      - uses: pypa/gh-action-pypi-publish@release/v1.8
         with:
           user: __token__
           password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
-          packages_dir: dist/
+          repository-url: https://test.pypi.org/legacy/
+          packages-dir: dist/
           verbose: true
 
   pypi_publish:
     name: Publish ${{ github.repository }} to to PyPI
-    needs: [test, build_wheels_sdist, test_pypi_publish]
+    needs: [test_pypi_publish]
 
     runs-on: ubuntu-latest
     # Publish when a GitHub Release is created, use the following rule:
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
       - name: Download Artifact
         uses: actions/download-artifact@v3
         with:
           name: distributions
           path: dist
 
       - name: PYPI Publish
-        uses: pypa/gh-action-pypi-publish@release/v1.6
+        uses: pypa/gh-action-pypi-publish@release/v1.8
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
-          packages_dir: dist/
+          packages-dir: dist/
           verbose: true
```

### Comparing `mibi-bin-tools-0.2.8/.github/workflows/release-drafter.yml` & `mibi-bin-tools-0.2.9/.github/workflows/release-drafter.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Release Drafter
 
 on:
   push:
     # branches to consider in the event; optional, defaults to all
-    branches: ["main"]
+    branches: [main]
   # pull_request event is required only for autolabeler
   pull_request:
     # Only following types are handled by the action, but one can default to all as well
     types: [opened, reopened, synchronize]
 
   issues:
     types: [closed]
@@ -19,14 +19,14 @@
   update_release_draft:
     runs-on: ubuntu-latest
     permissions:
       contents: write # for release-drafter/release-drafter to create a github release
       pull-requests: write # for release-drafter/release-drafter to add label to PR
     steps:
       # Drafts your next Release notes as Pull Requests are merged into "master"
-      - uses: release-drafter/release-drafter@v5.20.1
+      - uses: release-drafter/release-drafter@v5.23.0
         # Specify config name to use, relative to .github/. Default: release-drafter.yml
         with:
           config-name: release-drafter.yml
         #   disable-autolabeler: true
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `mibi-bin-tools-0.2.8/LICENSE` & `mibi-bin-tools-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mibi-bin-tools-0.2.8/PKG-INFO` & `mibi-bin-tools-0.2.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-Metadata-Version: 2.1
-Name: mibi-bin-tools
-Version: 0.2.8
-Summary: Source for extracting .bin files from the commercial MIBI.
-Author-email: Angelo Lab <theangelolab@gmail.com>
-License: Modified Apache License 2.0
-Project-URL: repository, https://github.com/angelolab/mibi-bin-tools
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
+# mibi-bin-tools
+<div align="center">
 
-[![Build Status](https://travis-ci.com/angelolab/mibi-bin-tools.svg?branch=master)](https://travis-ci.com/angelolab/mibi-bin-tools)
-[![Coverage Status](https://coveralls.io/repos/github/angelolab/mibi-bin-tools/badge.svg?branch=master)](https://coveralls.io/github/angelolab/mibi-bin-tools?branch=master)
+| | | 
+| ---        |    ---  |
+| CI / CD | [![CI](https://github.com/angelolab/mibi-bin-tools/actions/workflows/ci.yml/badge.svg)](https://github.com/angelolab/mibi-bin-tools/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/angelolab/mibi-bin-tools/badge.svg?branch=main)](https://coveralls.io/github/angelolab/mibi-bin-tools?branch=main) |
+| Package | [![PyPI - Version](https://img.shields.io/pypi/v/mibi-bin-tools.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/mibi-bin-tools/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/mibi-bin-tools.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/mibi-bin-tools/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mibi-bin-tools.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/mibi-bin-tools/) |
+|Meta | [![PyPI - License](https://img.shields.io/pypi/l/mibi-bin-tools?color=9400d3)](LICENSE) |
 
-# mibi-bin-tools
+</div>
 
 Toolbox for extracting tiff images from MIBIScope .bin files 
 
-## To install the project:
+## Installation:
+
+### PyPI
 
+```sh
+pip install mibi-bin-tools
+```
+
+### Source
 Open terminal and navigate to where you want the code stored.
 
 Then input the command:
 
-```
+```sh
 git clone https://github.com/angelolab/mibi-bin-tools.git
 ```
 
 Next, you'll need to set up a docker image with all of the required dependencies.
  - First, [download](https://hub.docker.com/?overlay=onboarding) docker desktop. 
  - Once it's sucessfully installed, make sure it is running by looking in toolbar for the Docker whale.
  - Once it's running, enter the following commands into terminal
```

### Comparing `mibi-bin-tools-0.2.8/pyproject.toml` & `mibi-bin-tools-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,65 +12,65 @@
 dependencies = [
     "Cython>=0.29.24",
     "matplotlib>=3",
     "numpy>=1.2",
     "pandas>=1.3",
     "scikit-image>=0.19",
     "alpineer>=0.1.5",
-    "xarray>=2022"
+    "xarray>=2022",
 ]
 name = "mibi-bin-tools"
-authors = [{name = "Angelo Lab", email = "theangelolab@gmail.com"}]
+authors = [{ name = "Angelo Lab", email = "theangelolab@gmail.com" }]
 description = "Source for extracting .bin files from the commercial MIBI."
 readme = "README.md"
-requires-python = ">=3.8"
-license = {text = "Modified Apache License 2.0"}
+requires-python = ">=3.9"
+license = { text = "Modified Apache License 2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Cython",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 dynamic = ["version"]
-urls = {repository = "https://github.com/angelolab/mibi-bin-tools"}
+urls = { repository = "https://github.com/angelolab/mibi-bin-tools" }
 
 [project.optional-dependencies]
 test = [
     "coveralls[toml]",
     "pytest",
     "pytest-cases",
     "pytest-cov",
     "pytest-mock",
-    "pytest-pycodestyle"
+    "pytest-pycodestyle",
 ]
 
 [tool.setuptools_scm]
 version_scheme = "release-branch-semver"
 local_scheme = "no-local-version"
 
 [tool.cibuildwheel]
-build = ["cp38-*"]
+build = ["cp39-*", "cp310-*", "cp311-*"]
 skip = [
-    "cp36-*",        # Python 3.6
-    "cp37-*",        # Python 3.7
-    "cp39-*",        # Python 3.9
-    "cp310-*",       # Python 3.10
-    "cp311-*",       # Python 3.11
-    "*-musllinux_*", # Musllinux
-    "pp*",           # PyPy wheels on all platforms
-    "*_i686",        # 32bit Linux Wheels
-    "*_s390x",       # IBM System/390, "mainframe"
-    "*-win32",       # 32bit Windows Wheels
-    "*_ppc64le",     # PowerPC
+    "cp36-*",         # Python 3.6
+    "cp37-*",         # Python 3.7
+    "cp38-*",         # Python 3.8
+    "*-musllinux_*",  # Musllinux
+    "pp*",            # PyPy wheels on all platforms
+    "*_i686",         # 32bit Linux Wheels
+    "*_s390x",        # IBM System/390, "mainframe"
+    "*-win32",        # 32bit Windows Wheels
+    "*_ppc64le",      # PowerPC
+    "cp39-win_arm64", # Windows ARM64 Python 3.9 wheels do not build.
 ]
 
 build-frontend = "build"
-build-verbosity = 3
 
 # Avoid testing on emulated architectures
 test-skip = [
     "*-win_arm64",               # Skip testing emulated arm64 biulds on Windows
     "*-*linux_aarch64",          # Skip testing emulated Linux builds
     "*-macosx_arm64",            # Skip testing emulated arm64 builds on Intel Macs
     "*-macosx_universal2:arm64", # Skip testing emulated arm64 portion of universal2 builds
```

### Comparing `mibi-bin-tools-0.2.8/setup.py` & `mibi-bin-tools-0.2.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-from os import pardir, path
-from setuptools import setup, Extension
-import numpy as np
+from pathlib import Path
 from Cython.Build import cythonize
+from Cython.Compiler.Options import get_directive_defaults
+from setuptools import Extension, setup
+import numpy as np
+
+_compiler_directives = get_directive_defaults()
 
-CYTHON_DEBUG = False
+CYTHON_PROFILE_MODE = False
 
-if CYTHON_DEBUG:
-    from Cython.Compiler.Options import get_directive_defaults
-    
-    directive_defaults = get_directive_defaults()
-    directive_defaults["linetrace"] = True
-    directive_defaults["binding"] = True
+CYTHON_MACROS: tuple[str,str] = None
 
-CYTHON_MACROS = [("CYTHON_TRACE", "1")] if CYTHON_DEBUG else None
+if CYTHON_PROFILE_MODE:
+    _compiler_directives["linetrace"] = True
+    _compiler_directives["profile"] = True
+    _compiler_directives["emit_code_comments"] = True
+    CYTHON_MACROS = [("CYTHON_TRACE", "1")]
 
-PKG_FOLDER = path.relpath(path.join(__file__, pardir))
+_compiler_directives["binding"] = True
+_compiler_directives["language_level"] = "3"
+_compiler_directives["embedsignature"] = True
 
 extensions = [
     Extension(
         name="mibi_bin_tools._extract_bin",
-        sources=[path.join(PKG_FOLDER, "src", "mibi_bin_tools", "_extract_bin.pyx")],
+        sources=[Path("src", "mibi_bin_tools", "_extract_bin.pyx").as_posix()],
         include_dirs=[np.get_include()],
         define_macros=CYTHON_MACROS
     )
 ]
 
 setup(
-    ext_modules=cythonize(extensions, compiler_directives={'language_level': "3"}),
+    ext_modules=cythonize(extensions, compiler_directives=_compiler_directives),
 )
```

### Comparing `mibi-bin-tools-0.2.8/src/mibi_bin_tools/_extract_bin.c` & `mibi-bin-tools-0.2.9/src/mibi_bin_tools/_extract_bin.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "mibi_bin_tools._extract_bin",
         "sources": [
-            "./src/mibi_bin_tools/_extract_bin.pyx"
+            "src/mibi_bin_tools/_extract_bin.pyx"
         ]
     },
     "module_name": "mibi_bin_tools._extract_bin"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -27,16 +27,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -221,15 +221,15 @@
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
@@ -260,15 +260,15 @@
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
@@ -1114,195 +1114,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1369,42 +1369,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2046,22 +2046,93 @@
 
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
 
+/* FetchCommonType.proto */
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
+
+/* CythonFunctionShared.proto */
+#define __Pyx_CyFunction_USED 1
+#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
+#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
+#define __Pyx_CYFUNCTION_CCLASS        0x04
+#define __Pyx_CyFunction_GetClosure(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_closure)
+#define __Pyx_CyFunction_GetClassObj(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_classobj)
+#define __Pyx_CyFunction_Defaults(type, f)\
+    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
+#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
+    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
+typedef struct {
+    PyCFunctionObject func;
+#if PY_VERSION_HEX < 0x030500A0
+    PyObject *func_weakreflist;
+#endif
+    PyObject *func_dict;
+    PyObject *func_name;
+    PyObject *func_qualname;
+    PyObject *func_doc;
+    PyObject *func_globals;
+    PyObject *func_code;
+    PyObject *func_closure;
+    PyObject *func_classobj;
+    void *defaults;
+    int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
+    int flags;
+    PyObject *defaults_tuple;
+    PyObject *defaults_kwdict;
+    PyObject *(*defaults_getter)(PyObject *);
+    PyObject *func_annotations;
+} __pyx_CyFunctionObject;
+static PyTypeObject *__pyx_CyFunctionType = 0;
+#define __Pyx_CyFunction_Check(obj)  (__Pyx_TypeCheck(obj, __pyx_CyFunctionType))
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *self,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
+                                                         size_t size,
+                                                         int pyobjects);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
+                                                            PyObject *tuple);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
+                                                             PyObject *dict);
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
+                                                              PyObject *dict);
+static int __pyx_CyFunction_init(void);
+
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -2436,40 +2507,48 @@
 static PyObject *__pyx_builtin_id;
 static PyObject *__pyx_builtin_IndexError;
 static const char __pyx_k_I[] = "I";
 static const char __pyx_k_O[] = "O";
 static const char __pyx_k_c[] = "c";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
+static const char __pyx_k_dst[] = "dst";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
+static const char __pyx_k_src[] = "src";
+static const char __pyx_k_tmp[] = "tmp";
 static const char __pyx_k_base[] = "base";
+static const char __pyx_k_copy[] = "copy";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
+static const char __pyx_k_self[] = "self";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ASCII[] = "ASCII";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
+static const char __pyx_k_state[] = "state";
 static const char __pyx_k_counts[] = "counts";
+static const char __pyx_k_dict_2[] = "_dict";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
+static const char __pyx_k_mslice[] = "mslice";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_uint32[] = "uint32";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
@@ -2495,43 +2574,59 @@
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_high_range[] = "high_range";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
+static const char __pyx_k_is_c_contig[] = "is_c_contig";
+static const char __pyx_k_is_f_contig[] = "is_f_contig";
+static const char __pyx_k_copy_fortran[] = "copy_fortran";
 static const char __pyx_k_pulse_counts[] = "pulse_counts";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
+static const char __pyx_k_use_setstate[] = "use_setstate";
 static const char __pyx_k_c_extract_bin[] = "c_extract_bin";
 static const char __pyx_k_pyx_getbuffer[] = "__pyx_getbuffer";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_c_total_counts[] = "c_total_counts";
 static const char __pyx_k_calc_intensity[] = "calc_intensity";
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
+static const char __pyx_k_memoryview_copy[] = "memoryview.copy";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
 static const char __pyx_k_median_pulse_height[] = "median_pulse_height";
+static const char __pyx_k_Enum___reduce_cython[] = "Enum.__reduce_cython__";
 static const char __pyx_k_c_extract_histograms[] = "c_extract_histograms";
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
+static const char __pyx_k_array___reduce_cython[] = "array.__reduce_cython__";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
+static const char __pyx_k_Enum___setstate_cython[] = "Enum.__setstate_cython__";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
+static const char __pyx_k_memoryview_is_c_contig[] = "memoryview.is_c_contig";
+static const char __pyx_k_memoryview_is_f_contig[] = "memoryview.is_f_contig";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
+static const char __pyx_k_array___setstate_cython[] = "array.__setstate_cython__";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
+static const char __pyx_k_memoryview_copy_fortran[] = "memoryview.copy_fortran";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
+static const char __pyx_k_memoryview___reduce_cython[] = "memoryview.__reduce_cython__";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_mibi_bin_tools__extract_bin[] = "mibi_bin_tools._extract_bin";
+static const char __pyx_k_memoryview___setstate_cython[] = "memoryview.__setstate_cython__";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
+static const char __pyx_k_memoryviewslice___reduce_cython[] = "_memoryviewslice.__reduce_cython__";
+static const char __pyx_k_memoryviewslice___setstate_cyth[] = "_memoryviewslice.__setstate_cython__";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_src_mibi_bin_tools__extract_bin[] = "src/mibi_bin_tools/_extract_bin.pyx";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
@@ -2549,14 +2644,16 @@
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
+static PyObject *__pyx_n_s_Enum___reduce_cython;
+static PyObject *__pyx_n_s_Enum___setstate_cython;
 static PyObject *__pyx_n_u_I;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
@@ -2567,29 +2664,35 @@
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_s_allocate_buffer;
+static PyObject *__pyx_n_s_array___reduce_cython;
+static PyObject *__pyx_n_s_array___setstate_cython;
 static PyObject *__pyx_n_s_asarray;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_c;
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_n_s_c_extract_bin;
 static PyObject *__pyx_n_s_c_extract_histograms;
 static PyObject *__pyx_n_s_c_pulse_height_vs_positive_pixel;
 static PyObject *__pyx_n_s_c_total_counts;
 static PyObject *__pyx_n_s_calc_intensity;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
+static PyObject *__pyx_n_s_copy;
+static PyObject *__pyx_n_s_copy_fortran;
 static PyObject *__pyx_n_s_counts;
 static PyObject *__pyx_n_s_dict;
+static PyObject *__pyx_n_s_dict_2;
+static PyObject *__pyx_n_s_dst;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_dtype_is_object;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_enumerate;
 static PyObject *__pyx_n_s_error;
 static PyObject *__pyx_n_s_filename;
 static PyObject *__pyx_n_s_flags;
@@ -2598,23 +2701,34 @@
 static PyObject *__pyx_n_u_fortran;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_kp_s_got_differing_extents_in_dimensi;
 static PyObject *__pyx_n_s_high_range;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_intensity;
+static PyObject *__pyx_n_s_is_c_contig;
+static PyObject *__pyx_n_s_is_f_contig;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
 static PyObject *__pyx_n_s_low_range;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_mean_pp;
 static PyObject *__pyx_n_s_median_pulse_height;
+static PyObject *__pyx_n_s_memoryview___reduce_cython;
+static PyObject *__pyx_n_s_memoryview___setstate_cython;
+static PyObject *__pyx_n_s_memoryview_copy;
+static PyObject *__pyx_n_s_memoryview_copy_fortran;
+static PyObject *__pyx_n_s_memoryview_is_c_contig;
+static PyObject *__pyx_n_s_memoryview_is_f_contig;
+static PyObject *__pyx_n_s_memoryviewslice___reduce_cython;
+static PyObject *__pyx_n_s_memoryviewslice___setstate_cyth;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_mibi_bin_tools__extract_bin;
 static PyObject *__pyx_n_s_mode;
+static PyObject *__pyx_n_s_mslice;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_n_s_ndim;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
@@ -2633,33 +2747,38 @@
 static PyObject *__pyx_n_s_pyx_unpickle_Enum;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_reshape;
+static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_n_s_size;
+static PyObject *__pyx_n_s_src;
 static PyObject *__pyx_kp_s_src_mibi_bin_tools__extract_bin;
 static PyObject *__pyx_n_s_start;
+static PyObject *__pyx_n_s_state;
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_kp_s_strided_and_direct;
 static PyObject *__pyx_kp_s_strided_and_direct_or_indirect;
 static PyObject *__pyx_kp_s_strided_and_indirect;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_test;
+static PyObject *__pyx_n_s_tmp;
 static PyObject *__pyx_n_s_uint32;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
+static PyObject *__pyx_n_s_use_setstate;
 static PyObject *__pyx_n_s_widths;
 static PyObject *__pyx_pf_14mibi_bin_tools_12_extract_bin_c_extract_bin(CYTHON_UNUSED PyObject *__pyx_self, char *__pyx_v_filename, __Pyx_memviewslice __pyx_v_low_range, __Pyx_memviewslice __pyx_v_high_range, __Pyx_memviewslice __pyx_v_calc_intensity); /* proto */
 static PyObject *__pyx_pf_14mibi_bin_tools_12_extract_bin_2c_extract_histograms(CYTHON_UNUSED PyObject *__pyx_self, char *__pyx_v_filename, __pyx_t_14mibi_bin_tools_12_extract_bin_DTYPE_t __pyx_v_low_range, __pyx_t_14mibi_bin_tools_12_extract_bin_DTYPE_t __pyx_v_high_range); /* proto */
 static PyObject *__pyx_pf_14mibi_bin_tools_12_extract_bin_4c_pulse_height_vs_positive_pixel(CYTHON_UNUSED PyObject *__pyx_self, char *__pyx_v_filename, __pyx_t_14mibi_bin_tools_12_extract_bin_DTYPE_t __pyx_v_low_range, __pyx_t_14mibi_bin_tools_12_extract_bin_DTYPE_t __pyx_v_high_range); /* proto */
 static PyObject *__pyx_pf_14mibi_bin_tools_12_extract_bin_6c_total_counts(CYTHON_UNUSED PyObject *__pyx_self, char *__pyx_v_filename); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
@@ -2736,24 +2855,48 @@
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_tuple__30;
-static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__32;
-static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__34;
-static PyObject *__pyx_tuple__35;
+static PyObject *__pyx_tuple__36;
+static PyObject *__pyx_tuple__38;
+static PyObject *__pyx_tuple__39;
+static PyObject *__pyx_tuple__40;
+static PyObject *__pyx_tuple__41;
+static PyObject *__pyx_tuple__42;
+static PyObject *__pyx_tuple__43;
+static PyObject *__pyx_tuple__45;
+static PyObject *__pyx_tuple__47;
+static PyObject *__pyx_tuple__49;
+static PyObject *__pyx_tuple__51;
+static PyObject *__pyx_tuple__53;
+static PyObject *__pyx_tuple__55;
+static PyObject *__pyx_tuple__57;
+static PyObject *__pyx_tuple__59;
 static PyObject *__pyx_codeobj__23;
 static PyObject *__pyx_codeobj__25;
 static PyObject *__pyx_codeobj__27;
 static PyObject *__pyx_codeobj__29;
-static PyObject *__pyx_codeobj__36;
+static PyObject *__pyx_codeobj__31;
+static PyObject *__pyx_codeobj__33;
+static PyObject *__pyx_codeobj__35;
+static PyObject *__pyx_codeobj__37;
+static PyObject *__pyx_codeobj__44;
+static PyObject *__pyx_codeobj__46;
+static PyObject *__pyx_codeobj__48;
+static PyObject *__pyx_codeobj__50;
+static PyObject *__pyx_codeobj__52;
+static PyObject *__pyx_codeobj__54;
+static PyObject *__pyx_codeobj__56;
+static PyObject *__pyx_codeobj__58;
+static PyObject *__pyx_codeobj__60;
 /* Late includes */
 
 /* "mibi_bin_tools/_extract_bin.pyx":20
  * @wraparound(False)  # Deactivate negative indexing
  * @cdivision(True) # Ignore modulo/divide by zero warning
  * cdef inline int _minimum_larger_value_in_sorted(const DTYPE_t[:] low_range, DTYPE_t val) nogil:             # <<<<<<<<<<<<<<
  *     """ minimal bianry search impl
@@ -5184,15 +5327,16 @@
  * def c_extract_bin(char* filename, DTYPE_t[:] low_range,             # <<<<<<<<<<<<<<
  *                   DTYPE_t[:] high_range, SMALL_t[:] calc_intensity):
  *     return np.asarray(
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14mibi_bin_tools_12_extract_bin_1c_extract_bin(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_14mibi_bin_tools_12_extract_bin_1c_extract_bin = {"c_extract_bin", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14mibi_bin_tools_12_extract_bin_1c_extract_bin, METH_VARARGS|METH_KEYWORDS, 0};
+static char __pyx_doc_14mibi_bin_tools_12_extract_bin_c_extract_bin[] = "c_extract_bin(char *filename, DTYPE_t[:] low_range, DTYPE_t[:] high_range, SMALL_t[:] calc_intensity)";
+static PyMethodDef __pyx_mdef_14mibi_bin_tools_12_extract_bin_1c_extract_bin = {"c_extract_bin", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14mibi_bin_tools_12_extract_bin_1c_extract_bin, METH_VARARGS|METH_KEYWORDS, __pyx_doc_14mibi_bin_tools_12_extract_bin_c_extract_bin};
 static PyObject *__pyx_pw_14mibi_bin_tools_12_extract_bin_1c_extract_bin(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   char *__pyx_v_filename;
   __Pyx_memviewslice __pyx_v_low_range = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_high_range = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_calc_intensity = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -5365,15 +5509,16 @@
  * def c_extract_histograms(char* filename, DTYPE_t low_range,             # <<<<<<<<<<<<<<
  *                          DTYPE_t high_range):
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14mibi_bin_tools_12_extract_bin_3c_extract_histograms(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_14mibi_bin_tools_12_extract_bin_3c_extract_histograms = {"c_extract_histograms", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14mibi_bin_tools_12_extract_bin_3c_extract_histograms, METH_VARARGS|METH_KEYWORDS, 0};
+static char __pyx_doc_14mibi_bin_tools_12_extract_bin_2c_extract_histograms[] = "c_extract_histograms(char *filename, DTYPE_t low_range, DTYPE_t high_range)";
+static PyMethodDef __pyx_mdef_14mibi_bin_tools_12_extract_bin_3c_extract_histograms = {"c_extract_histograms", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14mibi_bin_tools_12_extract_bin_3c_extract_histograms, METH_VARARGS|METH_KEYWORDS, __pyx_doc_14mibi_bin_tools_12_extract_bin_2c_extract_histograms};
 static PyObject *__pyx_pw_14mibi_bin_tools_12_extract_bin_3c_extract_histograms(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   char *__pyx_v_filename;
   __pyx_t_14mibi_bin_tools_12_extract_bin_DTYPE_t __pyx_v_low_range;
   __pyx_t_14mibi_bin_tools_12_extract_bin_DTYPE_t __pyx_v_high_range;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -5650,15 +5795,16 @@
  * def c_pulse_height_vs_positive_pixel(char* filename, DTYPE_t low_range, DTYPE_t high_range):             # <<<<<<<<<<<<<<
  *     cdef MAXINDEX_t median_pulse_height = 0
  *     cdef double mean_pp = 0.0
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14mibi_bin_tools_12_extract_bin_5c_pulse_height_vs_positive_pixel(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_14mibi_bin_tools_12_extract_bin_5c_pulse_height_vs_positive_pixel = {"c_pulse_height_vs_positive_pixel", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14mibi_bin_tools_12_extract_bin_5c_pulse_height_vs_positive_pixel, METH_VARARGS|METH_KEYWORDS, 0};
+static char __pyx_doc_14mibi_bin_tools_12_extract_bin_4c_pulse_height_vs_positive_pixel[] = "c_pulse_height_vs_positive_pixel(char *filename, DTYPE_t low_range, DTYPE_t high_range)";
+static PyMethodDef __pyx_mdef_14mibi_bin_tools_12_extract_bin_5c_pulse_height_vs_positive_pixel = {"c_pulse_height_vs_positive_pixel", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14mibi_bin_tools_12_extract_bin_5c_pulse_height_vs_positive_pixel, METH_VARARGS|METH_KEYWORDS, __pyx_doc_14mibi_bin_tools_12_extract_bin_4c_pulse_height_vs_positive_pixel};
 static PyObject *__pyx_pw_14mibi_bin_tools_12_extract_bin_5c_pulse_height_vs_positive_pixel(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   char *__pyx_v_filename;
   __pyx_t_14mibi_bin_tools_12_extract_bin_DTYPE_t __pyx_v_low_range;
   __pyx_t_14mibi_bin_tools_12_extract_bin_DTYPE_t __pyx_v_high_range;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -5822,15 +5968,16 @@
  * def c_total_counts(char* filename):             # <<<<<<<<<<<<<<
  *     counts = _extract_total_counts(filename)
  *     return int(counts)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14mibi_bin_tools_12_extract_bin_7c_total_counts(PyObject *__pyx_self, PyObject *__pyx_arg_filename); /*proto*/
-static PyMethodDef __pyx_mdef_14mibi_bin_tools_12_extract_bin_7c_total_counts = {"c_total_counts", (PyCFunction)__pyx_pw_14mibi_bin_tools_12_extract_bin_7c_total_counts, METH_O, 0};
+static char __pyx_doc_14mibi_bin_tools_12_extract_bin_6c_total_counts[] = "c_total_counts(char *filename)";
+static PyMethodDef __pyx_mdef_14mibi_bin_tools_12_extract_bin_7c_total_counts = {"c_total_counts", (PyCFunction)__pyx_pw_14mibi_bin_tools_12_extract_bin_7c_total_counts, METH_O, __pyx_doc_14mibi_bin_tools_12_extract_bin_6c_total_counts};
 static PyObject *__pyx_pw_14mibi_bin_tools_12_extract_bin_7c_total_counts(PyObject *__pyx_self, PyObject *__pyx_arg_filename) {
   char *__pyx_v_filename;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5901,15 +6048,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5918,29 +6065,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5951,15 +6098,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5968,29 +6115,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6001,15 +6148,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6018,29 +6165,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6051,15 +6198,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6068,29 +6215,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6101,15 +6248,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6118,29 +6265,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6151,212 +6298,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6372,15 +6519,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6388,53 +6535,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
@@ -6442,30 +6589,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6480,15 +6627,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6504,15 +6651,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6520,53 +6667,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
@@ -6574,30 +6721,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6612,15 +6759,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6636,15 +6783,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6652,53 +6799,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
@@ -6706,30 +6853,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6744,176 +6891,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8725,14 +8872,16 @@
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw___pyx_array_1__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc___pyx_array___reduce_cython__[] = "array.__reduce_cython__(self)";
+static PyMethodDef __pyx_mdef___pyx_array_1__reduce_cython__ = {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_array_1__reduce_cython__, METH_NOARGS, __pyx_doc___pyx_array___reduce_cython__};
 static PyObject *__pyx_pw___pyx_array_1__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   __pyx_r = __pyx_pf___pyx_array___reduce_cython__(((struct __pyx_array_obj *)__pyx_v_self));
 
   /* function exit code */
@@ -8782,14 +8931,16 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw___pyx_array_3__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc___pyx_array_2__setstate_cython__[] = "array.__setstate_cython__(self, __pyx_state)";
+static PyMethodDef __pyx_mdef___pyx_array_3__setstate_cython__ = {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_array_3__setstate_cython__, METH_O, __pyx_doc___pyx_array_2__setstate_cython__};
 static PyObject *__pyx_pw___pyx_array_3__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   __pyx_r = __pyx_pf___pyx_array_2__setstate_cython__(((struct __pyx_array_obj *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
@@ -9159,14 +9310,16 @@
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw___pyx_MemviewEnum_1__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc___pyx_MemviewEnum___reduce_cython__[] = "Enum.__reduce_cython__(self)";
+static PyMethodDef __pyx_mdef___pyx_MemviewEnum_1__reduce_cython__ = {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_1__reduce_cython__, METH_NOARGS, __pyx_doc___pyx_MemviewEnum___reduce_cython__};
 static PyObject *__pyx_pw___pyx_MemviewEnum_1__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   __pyx_r = __pyx_pf___pyx_MemviewEnum___reduce_cython__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self));
 
   /* function exit code */
@@ -9394,14 +9547,16 @@
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw___pyx_MemviewEnum_3__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc___pyx_MemviewEnum_2__setstate_cython__[] = "Enum.__setstate_cython__(self, __pyx_state)";
+static PyMethodDef __pyx_mdef___pyx_MemviewEnum_3__setstate_cython__ = {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_3__setstate_cython__, METH_O, __pyx_doc___pyx_MemviewEnum_2__setstate_cython__};
 static PyObject *__pyx_pw___pyx_MemviewEnum_3__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   __pyx_r = __pyx_pf___pyx_MemviewEnum_2__setstate_cython__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
@@ -13285,14 +13440,16 @@
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
 /* Python wrapper */
 static PyObject *__pyx_memoryview_is_c_contig(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_15View_dot_MemoryView_10memoryview_16is_c_contig[] = "memoryview.is_c_contig(self)";
+static PyMethodDef __pyx_mdef_15View_dot_MemoryView_10memoryview_17is_c_contig = {"is_c_contig", (PyCFunction)__pyx_memoryview_is_c_contig, METH_NOARGS, __pyx_doc_15View_dot_MemoryView_10memoryview_16is_c_contig};
 static PyObject *__pyx_memoryview_is_c_contig(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_c_contig (wrapper)", 0);
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_16is_c_contig(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
@@ -13361,14 +13518,16 @@
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
 /* Python wrapper */
 static PyObject *__pyx_memoryview_is_f_contig(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_15View_dot_MemoryView_10memoryview_18is_f_contig[] = "memoryview.is_f_contig(self)";
+static PyMethodDef __pyx_mdef_15View_dot_MemoryView_10memoryview_19is_f_contig = {"is_f_contig", (PyCFunction)__pyx_memoryview_is_f_contig, METH_NOARGS, __pyx_doc_15View_dot_MemoryView_10memoryview_18is_f_contig};
 static PyObject *__pyx_memoryview_is_f_contig(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_f_contig (wrapper)", 0);
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_18is_f_contig(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
@@ -13437,14 +13596,16 @@
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
 /* Python wrapper */
 static PyObject *__pyx_memoryview_copy(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_15View_dot_MemoryView_10memoryview_20copy[] = "memoryview.copy(self)";
+static PyMethodDef __pyx_mdef_15View_dot_MemoryView_10memoryview_21copy = {"copy", (PyCFunction)__pyx_memoryview_copy, METH_NOARGS, __pyx_doc_15View_dot_MemoryView_10memoryview_20copy};
 static PyObject *__pyx_memoryview_copy(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("copy (wrapper)", 0);
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_20copy(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
@@ -13531,14 +13692,16 @@
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
 /* Python wrapper */
 static PyObject *__pyx_memoryview_copy_fortran(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_15View_dot_MemoryView_10memoryview_22copy_fortran[] = "memoryview.copy_fortran(self)";
+static PyMethodDef __pyx_mdef_15View_dot_MemoryView_10memoryview_23copy_fortran = {"copy_fortran", (PyCFunction)__pyx_memoryview_copy_fortran, METH_NOARGS, __pyx_doc_15View_dot_MemoryView_10memoryview_22copy_fortran};
 static PyObject *__pyx_memoryview_copy_fortran(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("copy_fortran (wrapper)", 0);
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_22copy_fortran(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
@@ -13624,14 +13787,16 @@
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw___pyx_memoryview_1__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc___pyx_memoryview___reduce_cython__[] = "memoryview.__reduce_cython__(self)";
+static PyMethodDef __pyx_mdef___pyx_memoryview_1__reduce_cython__ = {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_memoryview_1__reduce_cython__, METH_NOARGS, __pyx_doc___pyx_memoryview___reduce_cython__};
 static PyObject *__pyx_pw___pyx_memoryview_1__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   __pyx_r = __pyx_pf___pyx_memoryview___reduce_cython__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
@@ -13681,14 +13846,16 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw___pyx_memoryview_3__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc___pyx_memoryview_2__setstate_cython__[] = "memoryview.__setstate_cython__(self, __pyx_state)";
+static PyMethodDef __pyx_mdef___pyx_memoryview_3__setstate_cython__ = {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_memoryview_3__setstate_cython__, METH_O, __pyx_doc___pyx_memoryview_2__setstate_cython__};
 static PyObject *__pyx_pw___pyx_memoryview_3__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   __pyx_r = __pyx_pf___pyx_memoryview_2__setstate_cython__(((struct __pyx_memoryview_obj *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
@@ -16525,14 +16692,16 @@
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw___pyx_memoryviewslice_1__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc___pyx_memoryviewslice___reduce_cython__[] = "_memoryviewslice.__reduce_cython__(self)";
+static PyMethodDef __pyx_mdef___pyx_memoryviewslice_1__reduce_cython__ = {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_memoryviewslice_1__reduce_cython__, METH_NOARGS, __pyx_doc___pyx_memoryviewslice___reduce_cython__};
 static PyObject *__pyx_pw___pyx_memoryviewslice_1__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   __pyx_r = __pyx_pf___pyx_memoryviewslice___reduce_cython__(((struct __pyx_memoryviewslice_obj *)__pyx_v_self));
 
   /* function exit code */
@@ -16582,14 +16751,16 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw___pyx_memoryviewslice_3__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc___pyx_memoryviewslice_2__setstate_cython__[] = "_memoryviewslice.__setstate_cython__(self, __pyx_state)";
+static PyMethodDef __pyx_mdef___pyx_memoryviewslice_3__setstate_cython__ = {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_memoryviewslice_3__setstate_cython__, METH_O, __pyx_doc___pyx_memoryviewslice_2__setstate_cython__};
 static PyObject *__pyx_pw___pyx_memoryviewslice_3__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   __pyx_r = __pyx_pf___pyx_memoryviewslice_2__setstate_cython__(((struct __pyx_memoryviewslice_obj *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
@@ -19785,15 +19956,16 @@
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_15View_dot_MemoryView_1__pyx_unpickle_Enum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_15View_dot_MemoryView_1__pyx_unpickle_Enum = {"__pyx_unpickle_Enum", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_15View_dot_MemoryView_1__pyx_unpickle_Enum, METH_VARARGS|METH_KEYWORDS, 0};
+static char __pyx_doc_15View_dot_MemoryView___pyx_unpickle_Enum[] = "__pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state)";
+static PyMethodDef __pyx_mdef_15View_dot_MemoryView_1__pyx_unpickle_Enum = {"__pyx_unpickle_Enum", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_15View_dot_MemoryView_1__pyx_unpickle_Enum, METH_VARARGS|METH_KEYWORDS, __pyx_doc_15View_dot_MemoryView___pyx_unpickle_Enum};
 static PyObject *__pyx_pw_15View_dot_MemoryView_1__pyx_unpickle_Enum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -20252,16 +20424,16 @@
 
 static PyObject *__pyx_getprop___pyx_array_memview(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_15View_dot_MemoryView_5array_7memview_1__get__(o);
 }
 
 static PyMethodDef __pyx_methods_array[] = {
   {"__getattr__", (PyCFunction)__pyx_array___getattr__, METH_O|METH_COEXIST, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_array_1__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_array_3__setstate_cython__, METH_O, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_array_1__reduce_cython__, METH_NOARGS, __pyx_doc___pyx_array___reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_array_3__setstate_cython__, METH_O, __pyx_doc___pyx_array_2__setstate_cython__},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_array[] = {
   {(char *)"memview", __pyx_getprop___pyx_array_memview, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
@@ -20415,16 +20587,16 @@
   tmp = ((PyObject*)p->name);
   p->name = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
 static PyMethodDef __pyx_methods_Enum[] = {
-  {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_1__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_3__setstate_cython__, METH_O, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_1__reduce_cython__, METH_NOARGS, __pyx_doc___pyx_MemviewEnum___reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_3__setstate_cython__, METH_O, __pyx_doc___pyx_MemviewEnum_2__setstate_cython__},
   {0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type___pyx_MemviewEnum = {
   PyVarObject_HEAD_INIT(0, 0)
   "mibi_bin_tools._extract_bin.Enum", /*tp_name*/
   sizeof(struct __pyx_MemviewEnum_obj), /*tp_basicsize*/
@@ -20451,15 +20623,15 @@
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
-  0, /*tp_doc*/
+  "Enum(name)", /*tp_doc*/
   __pyx_tp_traverse_Enum, /*tp_traverse*/
   __pyx_tp_clear_Enum, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_Enum, /*tp_methods*/
@@ -20626,20 +20798,20 @@
 }
 
 static PyObject *__pyx_getprop___pyx_memoryview_size(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_15View_dot_MemoryView_10memoryview_4size_1__get__(o);
 }
 
 static PyMethodDef __pyx_methods_memoryview[] = {
-  {"is_c_contig", (PyCFunction)__pyx_memoryview_is_c_contig, METH_NOARGS, 0},
-  {"is_f_contig", (PyCFunction)__pyx_memoryview_is_f_contig, METH_NOARGS, 0},
-  {"copy", (PyCFunction)__pyx_memoryview_copy, METH_NOARGS, 0},
-  {"copy_fortran", (PyCFunction)__pyx_memoryview_copy_fortran, METH_NOARGS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_memoryview_1__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_memoryview_3__setstate_cython__, METH_O, 0},
+  {"is_c_contig", (PyCFunction)__pyx_memoryview_is_c_contig, METH_NOARGS, __pyx_doc_15View_dot_MemoryView_10memoryview_16is_c_contig},
+  {"is_f_contig", (PyCFunction)__pyx_memoryview_is_f_contig, METH_NOARGS, __pyx_doc_15View_dot_MemoryView_10memoryview_18is_f_contig},
+  {"copy", (PyCFunction)__pyx_memoryview_copy, METH_NOARGS, __pyx_doc_15View_dot_MemoryView_10memoryview_20copy},
+  {"copy_fortran", (PyCFunction)__pyx_memoryview_copy_fortran, METH_NOARGS, __pyx_doc_15View_dot_MemoryView_10memoryview_22copy_fortran},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_memoryview_1__reduce_cython__, METH_NOARGS, __pyx_doc___pyx_memoryview___reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_memoryview_3__setstate_cython__, METH_O, __pyx_doc___pyx_memoryview_2__setstate_cython__},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_memoryview[] = {
   {(char *)"T", __pyx_getprop___pyx_memoryview_T, 0, (char *)0, 0},
   {(char *)"base", __pyx_getprop___pyx_memoryview_base, 0, (char *)0, 0},
   {(char *)"shape", __pyx_getprop___pyx_memoryview_shape, 0, (char *)0, 0},
@@ -20815,16 +20987,16 @@
 }
 
 static PyObject *__pyx_getprop___pyx_memoryviewslice_base(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_15View_dot_MemoryView_16_memoryviewslice_4base_1__get__(o);
 }
 
 static PyMethodDef __pyx_methods__memoryviewslice[] = {
-  {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_memoryviewslice_1__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_memoryviewslice_3__setstate_cython__, METH_O, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_memoryviewslice_1__reduce_cython__, METH_NOARGS, __pyx_doc___pyx_memoryviewslice___reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_memoryviewslice_3__setstate_cython__, METH_O, __pyx_doc___pyx_memoryviewslice_2__setstate_cython__},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets__memoryviewslice[] = {
   {(char *)"base", __pyx_getprop___pyx_memoryviewslice_base, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
@@ -20959,14 +21131,16 @@
   {&__pyx_kp_s_Buffer_view_does_not_expose_stri, __pyx_k_Buffer_view_does_not_expose_stri, sizeof(__pyx_k_Buffer_view_does_not_expose_stri), 0, 0, 1, 0},
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
+  {&__pyx_n_s_Enum___reduce_cython, __pyx_k_Enum___reduce_cython, sizeof(__pyx_k_Enum___reduce_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_Enum___setstate_cython, __pyx_k_Enum___setstate_cython, sizeof(__pyx_k_Enum___setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_u_I, __pyx_k_I, sizeof(__pyx_k_I), 0, 1, 0, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
@@ -20977,29 +21151,35 @@
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
+  {&__pyx_n_s_array___reduce_cython, __pyx_k_array___reduce_cython, sizeof(__pyx_k_array___reduce_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_array___setstate_cython, __pyx_k_array___setstate_cython, sizeof(__pyx_k_array___setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_asarray, __pyx_k_asarray, sizeof(__pyx_k_asarray), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_n_s_c_extract_bin, __pyx_k_c_extract_bin, sizeof(__pyx_k_c_extract_bin), 0, 0, 1, 1},
   {&__pyx_n_s_c_extract_histograms, __pyx_k_c_extract_histograms, sizeof(__pyx_k_c_extract_histograms), 0, 0, 1, 1},
   {&__pyx_n_s_c_pulse_height_vs_positive_pixel, __pyx_k_c_pulse_height_vs_positive_pixel, sizeof(__pyx_k_c_pulse_height_vs_positive_pixel), 0, 0, 1, 1},
   {&__pyx_n_s_c_total_counts, __pyx_k_c_total_counts, sizeof(__pyx_k_c_total_counts), 0, 0, 1, 1},
   {&__pyx_n_s_calc_intensity, __pyx_k_calc_intensity, sizeof(__pyx_k_calc_intensity), 0, 0, 1, 1},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
+  {&__pyx_n_s_copy, __pyx_k_copy, sizeof(__pyx_k_copy), 0, 0, 1, 1},
+  {&__pyx_n_s_copy_fortran, __pyx_k_copy_fortran, sizeof(__pyx_k_copy_fortran), 0, 0, 1, 1},
   {&__pyx_n_s_counts, __pyx_k_counts, sizeof(__pyx_k_counts), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
+  {&__pyx_n_s_dict_2, __pyx_k_dict_2, sizeof(__pyx_k_dict_2), 0, 0, 1, 1},
+  {&__pyx_n_s_dst, __pyx_k_dst, sizeof(__pyx_k_dst), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
   {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
   {&__pyx_n_s_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 0, 1, 1},
   {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
@@ -21008,23 +21188,34 @@
   {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 0, 1, 0},
   {&__pyx_n_s_high_range, __pyx_k_high_range, sizeof(__pyx_k_high_range), 0, 0, 1, 1},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_intensity, __pyx_k_intensity, sizeof(__pyx_k_intensity), 0, 0, 1, 1},
+  {&__pyx_n_s_is_c_contig, __pyx_k_is_c_contig, sizeof(__pyx_k_is_c_contig), 0, 0, 1, 1},
+  {&__pyx_n_s_is_f_contig, __pyx_k_is_f_contig, sizeof(__pyx_k_is_f_contig), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
   {&__pyx_n_s_low_range, __pyx_k_low_range, sizeof(__pyx_k_low_range), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_mean_pp, __pyx_k_mean_pp, sizeof(__pyx_k_mean_pp), 0, 0, 1, 1},
   {&__pyx_n_s_median_pulse_height, __pyx_k_median_pulse_height, sizeof(__pyx_k_median_pulse_height), 0, 0, 1, 1},
+  {&__pyx_n_s_memoryview___reduce_cython, __pyx_k_memoryview___reduce_cython, sizeof(__pyx_k_memoryview___reduce_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_memoryview___setstate_cython, __pyx_k_memoryview___setstate_cython, sizeof(__pyx_k_memoryview___setstate_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_memoryview_copy, __pyx_k_memoryview_copy, sizeof(__pyx_k_memoryview_copy), 0, 0, 1, 1},
+  {&__pyx_n_s_memoryview_copy_fortran, __pyx_k_memoryview_copy_fortran, sizeof(__pyx_k_memoryview_copy_fortran), 0, 0, 1, 1},
+  {&__pyx_n_s_memoryview_is_c_contig, __pyx_k_memoryview_is_c_contig, sizeof(__pyx_k_memoryview_is_c_contig), 0, 0, 1, 1},
+  {&__pyx_n_s_memoryview_is_f_contig, __pyx_k_memoryview_is_f_contig, sizeof(__pyx_k_memoryview_is_f_contig), 0, 0, 1, 1},
+  {&__pyx_n_s_memoryviewslice___reduce_cython, __pyx_k_memoryviewslice___reduce_cython, sizeof(__pyx_k_memoryviewslice___reduce_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_memoryviewslice___setstate_cyth, __pyx_k_memoryviewslice___setstate_cyth, sizeof(__pyx_k_memoryviewslice___setstate_cyth), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_mibi_bin_tools__extract_bin, __pyx_k_mibi_bin_tools__extract_bin, sizeof(__pyx_k_mibi_bin_tools__extract_bin), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
+  {&__pyx_n_s_mslice, __pyx_k_mslice, sizeof(__pyx_k_mslice), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
@@ -21043,33 +21234,38 @@
   {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_reshape, __pyx_k_reshape, sizeof(__pyx_k_reshape), 0, 0, 1, 1},
+  {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
+  {&__pyx_n_s_src, __pyx_k_src, sizeof(__pyx_k_src), 0, 0, 1, 1},
   {&__pyx_kp_s_src_mibi_bin_tools__extract_bin, __pyx_k_src_mibi_bin_tools__extract_bin, sizeof(__pyx_k_src_mibi_bin_tools__extract_bin), 0, 0, 1, 0},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
+  {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_kp_s_strided_and_direct, __pyx_k_strided_and_direct, sizeof(__pyx_k_strided_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_direct_or_indirect, __pyx_k_strided_and_direct_or_indirect, sizeof(__pyx_k_strided_and_direct_or_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+  {&__pyx_n_s_tmp, __pyx_k_tmp, sizeof(__pyx_k_tmp), 0, 0, 1, 1},
   {&__pyx_n_s_uint32, __pyx_k_uint32, sizeof(__pyx_k_uint32), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
+  {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_widths, __pyx_k_widths, sizeof(__pyx_k_widths), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 66, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
@@ -21084,26 +21280,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-80pvlkff/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-se2yldt4/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
@@ -21349,78 +21545,210 @@
  *     return int(counts)
  */
   __pyx_tuple__28 = PyTuple_Pack(3, __pyx_n_s_filename, __pyx_n_s_filename, __pyx_n_s_counts); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
   __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_mibi_bin_tools__extract_bin, __pyx_n_s_c_total_counts, 405, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 405, __pyx_L1_error)
 
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(2, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ */
+  __pyx_tuple__32 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(2, 3, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
+ */
+  __pyx_tuple__34 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(2, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_Enum__set_state(self, __pyx_state)
+ */
+  __pyx_tuple__36 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(2, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(2, 16, __pyx_L1_error)
+
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(2, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__38);
+  __Pyx_GIVEREF(__pyx_tuple__38);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(2, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(2, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__40);
+  __Pyx_GIVEREF(__pyx_tuple__40);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(2, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__41 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(2, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_tuple__42 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__42);
+  __Pyx_GIVEREF(__pyx_tuple__42);
+
+  /* "View.MemoryView":621
+ * 
+ * 
+ *     def is_c_contig(self):             # <<<<<<<<<<<<<<
+ *         cdef __Pyx_memviewslice *mslice
+ *         cdef __Pyx_memviewslice tmp
+ */
+  __pyx_tuple__43 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_mslice, __pyx_n_s_tmp); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(2, 621, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__43);
+  __Pyx_GIVEREF(__pyx_tuple__43);
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_is_c_contig, 621, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(2, 621, __pyx_L1_error)
+
+  /* "View.MemoryView":627
+ *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
+ * 
+ *     def is_f_contig(self):             # <<<<<<<<<<<<<<
+ *         cdef __Pyx_memviewslice *mslice
+ *         cdef __Pyx_memviewslice tmp
+ */
+  __pyx_tuple__45 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_mslice, __pyx_n_s_tmp); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(2, 627, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__45);
+  __Pyx_GIVEREF(__pyx_tuple__45);
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_is_f_contig, 627, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(2, 627, __pyx_L1_error)
+
+  /* "View.MemoryView":633
+ *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
+ * 
+ *     def copy(self):             # <<<<<<<<<<<<<<
+ *         cdef __Pyx_memviewslice mslice
+ *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
+ */
+  __pyx_tuple__47 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_mslice, __pyx_n_s_flags); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(2, 633, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__47);
+  __Pyx_GIVEREF(__pyx_tuple__47);
+  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_copy, 633, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(2, 633, __pyx_L1_error)
+
+  /* "View.MemoryView":645
+ *         return memoryview_copy_from_slice(self, &mslice)
+ * 
+ *     def copy_fortran(self):             # <<<<<<<<<<<<<<
+ *         cdef __Pyx_memviewslice src, dst
+ *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
+ */
+  __pyx_tuple__49 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_src, __pyx_n_s_dst, __pyx_n_s_flags); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(2, 645, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__49);
+  __Pyx_GIVEREF(__pyx_tuple__49);
+  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_copy_fortran, 645, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(2, 645, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_tuple__51 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__51);
+  __Pyx_GIVEREF(__pyx_tuple__51);
+  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(2, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ */
+  __pyx_tuple__53 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__53);
+  __Pyx_GIVEREF(__pyx_tuple__53);
+  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(2, 3, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_tuple__55 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__55);
+  __Pyx_GIVEREF(__pyx_tuple__55);
+  __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(2, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ */
+  __pyx_tuple__57 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__57);
+  __Pyx_GIVEREF(__pyx_tuple__57);
+  __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(2, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__35 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__35);
-  __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__59 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__59);
+  __Pyx_GIVEREF(__pyx_tuple__59);
+  __pyx_codeobj__60 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__60)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -21548,52 +21876,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
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
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -21832,51 +22175,51 @@
   /* "mibi_bin_tools/_extract_bin.pyx":372
  *     return counts
  * 
  * def c_extract_bin(char* filename, DTYPE_t[:] low_range,             # <<<<<<<<<<<<<<
  *                   DTYPE_t[:] high_range, SMALL_t[:] calc_intensity):
  *     return np.asarray(
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14mibi_bin_tools_12_extract_bin_1c_extract_bin, NULL, __pyx_n_s_mibi_bin_tools__extract_bin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_14mibi_bin_tools_12_extract_bin_1c_extract_bin, 0, __pyx_n_s_c_extract_bin, NULL, __pyx_n_s_mibi_bin_tools__extract_bin, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_c_extract_bin, __pyx_t_1) < 0) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "mibi_bin_tools/_extract_bin.pyx":379
  * 
  * 
  * def c_extract_histograms(char* filename, DTYPE_t low_range,             # <<<<<<<<<<<<<<
  *                          DTYPE_t high_range):
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14mibi_bin_tools_12_extract_bin_3c_extract_histograms, NULL, __pyx_n_s_mibi_bin_tools__extract_bin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_14mibi_bin_tools_12_extract_bin_3c_extract_histograms, 0, __pyx_n_s_c_extract_histograms, NULL, __pyx_n_s_mibi_bin_tools__extract_bin, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_c_extract_histograms, __pyx_t_1) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "mibi_bin_tools/_extract_bin.pyx":398
  *     )
  * 
  * def c_pulse_height_vs_positive_pixel(char* filename, DTYPE_t low_range, DTYPE_t high_range):             # <<<<<<<<<<<<<<
  *     cdef MAXINDEX_t median_pulse_height = 0
  *     cdef double mean_pp = 0.0
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14mibi_bin_tools_12_extract_bin_5c_pulse_height_vs_positive_pixel, NULL, __pyx_n_s_mibi_bin_tools__extract_bin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_14mibi_bin_tools_12_extract_bin_5c_pulse_height_vs_positive_pixel, 0, __pyx_n_s_c_pulse_height_vs_positive_pixel, NULL, __pyx_n_s_mibi_bin_tools__extract_bin, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_c_pulse_height_vs_positive_pixel, __pyx_t_1) < 0) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "mibi_bin_tools/_extract_bin.pyx":405
  *     return int(median_pulse_height), float(mean_pp)
  * 
  * def c_total_counts(char* filename):             # <<<<<<<<<<<<<<
  *     counts = _extract_total_counts(filename)
  *     return int(counts)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14mibi_bin_tools_12_extract_bin_7c_total_counts, NULL, __pyx_n_s_mibi_bin_tools__extract_bin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_14mibi_bin_tools_12_extract_bin_7c_total_counts, 0, __pyx_n_s_c_total_counts, NULL, __pyx_n_s_mibi_bin_tools__extract_bin, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_c_total_counts, __pyx_t_1) < 0) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "mibi_bin_tools/_extract_bin.pyx":1
  * from cython.view cimport array as cvarray             # <<<<<<<<<<<<<<
  * from cython cimport cdivision, boundscheck, wraparound
@@ -21896,78 +22239,122 @@
  */
   __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 210, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_array_type);
 
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef___pyx_array_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_array___reduce_cython, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_1) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef___pyx_array_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_array___setstate_cython, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_1) < 0) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef___pyx_MemviewEnum_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Enum___reduce_cython, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_MemviewEnum_type->tp_dict, __pyx_n_s_reduce_cython, __pyx_t_1) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  PyType_Modified(__pyx_MemviewEnum_type);
+
+  /* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_Enum__set_state(self, __pyx_state)
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef___pyx_MemviewEnum_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Enum___setstate_cython, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_MemviewEnum_type->tp_dict, __pyx_n_s_setstate_cython, __pyx_t_1) < 0) __PYX_ERR(2, 16, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  PyType_Modified(__pyx_MemviewEnum_type);
+
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__41, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__42, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":317
@@ -22005,33 +22392,127 @@
  */
   __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 551, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 551, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryview_type);
 
+  /* "View.MemoryView":621
+ * 
+ * 
+ *     def is_c_contig(self):             # <<<<<<<<<<<<<<
+ *         cdef __Pyx_memviewslice *mslice
+ *         cdef __Pyx_memviewslice tmp
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_15View_dot_MemoryView_10memoryview_17is_c_contig, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_memoryview_is_c_contig, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 621, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_is_c_contig, __pyx_t_1) < 0) __PYX_ERR(2, 621, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  PyType_Modified(__pyx_memoryview_type);
+
+  /* "View.MemoryView":627
+ *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
+ * 
+ *     def is_f_contig(self):             # <<<<<<<<<<<<<<
+ *         cdef __Pyx_memviewslice *mslice
+ *         cdef __Pyx_memviewslice tmp
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_15View_dot_MemoryView_10memoryview_19is_f_contig, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_memoryview_is_f_contig, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 627, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_is_f_contig, __pyx_t_1) < 0) __PYX_ERR(2, 627, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  PyType_Modified(__pyx_memoryview_type);
+
+  /* "View.MemoryView":633
+ *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
+ * 
+ *     def copy(self):             # <<<<<<<<<<<<<<
+ *         cdef __Pyx_memviewslice mslice
+ *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_15View_dot_MemoryView_10memoryview_21copy, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_memoryview_copy, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 633, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_copy, __pyx_t_1) < 0) __PYX_ERR(2, 633, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  PyType_Modified(__pyx_memoryview_type);
+
+  /* "View.MemoryView":645
+ *         return memoryview_copy_from_slice(self, &mslice)
+ * 
+ *     def copy_fortran(self):             # <<<<<<<<<<<<<<
+ *         cdef __Pyx_memviewslice src, dst
+ *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_15View_dot_MemoryView_10memoryview_23copy_fortran, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_memoryview_copy_fortran, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 645, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_copy_fortran, __pyx_t_1) < 0) __PYX_ERR(2, 645, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  PyType_Modified(__pyx_memoryview_type);
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef___pyx_memoryview_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_memoryview___reduce_cython, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_1) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef___pyx_memoryview_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_memoryview___setstate_cython, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__54)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_1) < 0) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
   /* "View.MemoryView":997
  *         return self.from_object
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 997, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryviewslice_type);
 
   /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef___pyx_memoryviewslice_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_memoryviewslice___reduce_cython, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__56)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_1) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef___pyx_memoryviewslice_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_memoryviewslice___setstate_cyth, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__58)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_1) < 0) __PYX_ERR(2, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_15View_dot_MemoryView_1__pyx_unpickle_Enum, NULL, __pyx_n_s_View_MemoryView); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_15View_dot_MemoryView_1__pyx_unpickle_Enum, 0, __pyx_n_s_pyx_unpickle_Enum, NULL, __pyx_n_s_View_MemoryView, __pyx_d, ((PyObject *)__pyx_codeobj__60)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Enum, __pyx_t_1) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  *     return __pyx_result
@@ -23054,28 +23535,28 @@
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
@@ -24029,44 +24510,62 @@
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
@@ -24086,14 +24585,682 @@
     return (PyTypeObject *)result;
 bad:
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
+/* FetchCommonType */
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+    PyObject* fake_module;
+    PyTypeObject* cached_type = NULL;
+    fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
+    if (!fake_module) return NULL;
+    Py_INCREF(fake_module);
+    cached_type = (PyTypeObject*) PyObject_GetAttrString(fake_module, type->tp_name);
+    if (cached_type) {
+        if (!PyType_Check((PyObject*)cached_type)) {
+            PyErr_Format(PyExc_TypeError,
+                "Shared Cython type %.200s is not a type object",
+                type->tp_name);
+            goto bad;
+        }
+        if (cached_type->tp_basicsize != type->tp_basicsize) {
+            PyErr_Format(PyExc_TypeError,
+                "Shared Cython type %.200s has the wrong size, try recompiling",
+                type->tp_name);
+            goto bad;
+        }
+    } else {
+        if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+        PyErr_Clear();
+        if (PyType_Ready(type) < 0) goto bad;
+        if (PyObject_SetAttrString(fake_module, type->tp_name, (PyObject*) type) < 0)
+            goto bad;
+        Py_INCREF(type);
+        cached_type = type;
+    }
+done:
+    Py_DECREF(fake_module);
+    return cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+
+/* CythonFunctionShared */
+#include <structmember.h>
+static PyObject *
+__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *closure)
+{
+    if (unlikely(op->func_doc == NULL)) {
+        if (op->func.m_ml->ml_doc) {
+#if PY_MAJOR_VERSION >= 3
+            op->func_doc = PyUnicode_FromString(op->func.m_ml->ml_doc);
+#else
+            op->func_doc = PyString_FromString(op->func.m_ml->ml_doc);
+#endif
+            if (unlikely(op->func_doc == NULL))
+                return NULL;
+        } else {
+            Py_INCREF(Py_None);
+            return Py_None;
+        }
+    }
+    Py_INCREF(op->func_doc);
+    return op->func_doc;
+}
+static int
+__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, CYTHON_UNUSED void *context)
+{
+    PyObject *tmp = op->func_doc;
+    if (value == NULL) {
+        value = Py_None;
+    }
+    Py_INCREF(value);
+    op->func_doc = value;
+    Py_XDECREF(tmp);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *context)
+{
+    if (unlikely(op->func_name == NULL)) {
+#if PY_MAJOR_VERSION >= 3
+        op->func_name = PyUnicode_InternFromString(op->func.m_ml->ml_name);
+#else
+        op->func_name = PyString_InternFromString(op->func.m_ml->ml_name);
+#endif
+        if (unlikely(op->func_name == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_name);
+    return op->func_name;
+}
+static int
+__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, CYTHON_UNUSED void *context)
+{
+    PyObject *tmp;
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
+    }
+    tmp = op->func_name;
+    Py_INCREF(value);
+    op->func_name = value;
+    Py_XDECREF(tmp);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *context)
+{
+    Py_INCREF(op->func_qualname);
+    return op->func_qualname;
+}
+static int
+__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, CYTHON_UNUSED void *context)
+{
+    PyObject *tmp;
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    tmp = op->func_qualname;
+    Py_INCREF(value);
+    op->func_qualname = value;
+    Py_XDECREF(tmp);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_self(__pyx_CyFunctionObject *m, CYTHON_UNUSED void *closure)
+{
+    PyObject *self;
+    self = m->func_closure;
+    if (self == NULL)
+        self = Py_None;
+    Py_INCREF(self);
+    return self;
+}
+static PyObject *
+__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *context)
+{
+    if (unlikely(op->func_dict == NULL)) {
+        op->func_dict = PyDict_New();
+        if (unlikely(op->func_dict == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_dict);
+    return op->func_dict;
+}
+static int
+__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, CYTHON_UNUSED void *context)
+{
+    PyObject *tmp;
+    if (unlikely(value == NULL)) {
+        PyErr_SetString(PyExc_TypeError,
+               "function's dictionary may not be deleted");
+        return -1;
+    }
+    if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+               "setting function's dictionary to a non-dict");
+        return -1;
+    }
+    tmp = op->func_dict;
+    Py_INCREF(value);
+    op->func_dict = value;
+    Py_XDECREF(tmp);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *context)
+{
+    Py_INCREF(op->func_globals);
+    return op->func_globals;
+}
+static PyObject *
+__Pyx_CyFunction_get_closure(CYTHON_UNUSED __pyx_CyFunctionObject *op, CYTHON_UNUSED void *context)
+{
+    Py_INCREF(Py_None);
+    return Py_None;
+}
+static PyObject *
+__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *context)
+{
+    PyObject* result = (op->func_code) ? op->func_code : Py_None;
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
+    int result = 0;
+    PyObject *res = op->defaults_getter((PyObject *) op);
+    if (unlikely(!res))
+        return -1;
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
+    Py_INCREF(op->defaults_tuple);
+    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
+    Py_INCREF(op->defaults_kwdict);
+    #else
+    op->defaults_tuple = PySequence_ITEM(res, 0);
+    if (unlikely(!op->defaults_tuple)) result = -1;
+    else {
+        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        if (unlikely(!op->defaults_kwdict)) result = -1;
+    }
+    #endif
+    Py_DECREF(res);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, CYTHON_UNUSED void *context) {
+    PyObject* tmp;
+    if (!value) {
+        value = Py_None;
+    } else if (value != Py_None && !PyTuple_Check(value)) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__defaults__ must be set to a tuple object");
+        return -1;
+    }
+    Py_INCREF(value);
+    tmp = op->defaults_tuple;
+    op->defaults_tuple = value;
+    Py_XDECREF(tmp);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *context) {
+    PyObject* result = op->defaults_tuple;
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (__Pyx_CyFunction_init_defaults(op) < 0) return NULL;
+            result = op->defaults_tuple;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, CYTHON_UNUSED void *context) {
+    PyObject* tmp;
+    if (!value) {
+        value = Py_None;
+    } else if (value != Py_None && !PyDict_Check(value)) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__kwdefaults__ must be set to a dict object");
+        return -1;
+    }
+    Py_INCREF(value);
+    tmp = op->defaults_kwdict;
+    op->defaults_kwdict = value;
+    Py_XDECREF(tmp);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *context) {
+    PyObject* result = op->defaults_kwdict;
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (__Pyx_CyFunction_init_defaults(op) < 0) return NULL;
+            result = op->defaults_kwdict;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, CYTHON_UNUSED void *context) {
+    PyObject* tmp;
+    if (!value || value == Py_None) {
+        value = NULL;
+    } else if (!PyDict_Check(value)) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__annotations__ must be set to a dict object");
+        return -1;
+    }
+    Py_XINCREF(value);
+    tmp = op->func_annotations;
+    op->func_annotations = value;
+    Py_XDECREF(tmp);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *context) {
+    PyObject* result = op->func_annotations;
+    if (unlikely(!result)) {
+        result = PyDict_New();
+        if (unlikely(!result)) return NULL;
+        op->func_annotations = result;
+    }
+    Py_INCREF(result);
+    return result;
+}
+static PyGetSetDef __pyx_CyFunction_getsets[] = {
+    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
+    {(char *) "__self__", (getter)__Pyx_CyFunction_get_self, 0, 0, 0},
+    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
+    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
+    {0, 0, 0, 0, 0}
+};
+static PyMemberDef __pyx_CyFunction_members[] = {
+    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), PY_WRITE_RESTRICTED, 0},
+    {0, 0, 0,  0, 0}
+};
+static PyObject *
+__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, CYTHON_UNUSED PyObject *args)
+{
+#if PY_MAJOR_VERSION >= 3
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
+#else
+    return PyString_FromString(m->func.m_ml->ml_name);
+#endif
+}
+static PyMethodDef __pyx_CyFunction_methods[] = {
+    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
+    {0, 0, 0, 0}
+};
+#if PY_VERSION_HEX < 0x030500A0
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
+#else
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func.m_weakreflist)
+#endif
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    if (unlikely(op == NULL))
+        return NULL;
+    op->flags = flags;
+    __Pyx_CyFunction_weakreflist(op) = NULL;
+    op->func.m_ml = ml;
+    op->func.m_self = (PyObject *) op;
+    Py_XINCREF(closure);
+    op->func_closure = closure;
+    Py_XINCREF(module);
+    op->func.m_module = module;
+    op->func_dict = NULL;
+    op->func_name = NULL;
+    Py_INCREF(qualname);
+    op->func_qualname = qualname;
+    op->func_doc = NULL;
+    op->func_classobj = NULL;
+    op->func_globals = globals;
+    Py_INCREF(op->func_globals);
+    Py_XINCREF(code);
+    op->func_code = code;
+    op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
+    op->defaults = NULL;
+    op->defaults_tuple = NULL;
+    op->defaults_kwdict = NULL;
+    op->defaults_getter = NULL;
+    op->func_annotations = NULL;
+    return (PyObject *) op;
+}
+static int
+__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
+{
+    Py_CLEAR(m->func_closure);
+    Py_CLEAR(m->func.m_module);
+    Py_CLEAR(m->func_dict);
+    Py_CLEAR(m->func_name);
+    Py_CLEAR(m->func_qualname);
+    Py_CLEAR(m->func_doc);
+    Py_CLEAR(m->func_globals);
+    Py_CLEAR(m->func_code);
+    Py_CLEAR(m->func_classobj);
+    Py_CLEAR(m->defaults_tuple);
+    Py_CLEAR(m->defaults_kwdict);
+    Py_CLEAR(m->func_annotations);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_XDECREF(pydefaults[i]);
+        PyObject_Free(m->defaults);
+        m->defaults = NULL;
+    }
+    return 0;
+}
+static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    if (__Pyx_CyFunction_weakreflist(m) != NULL)
+        PyObject_ClearWeakRefs((PyObject *) m);
+    __Pyx_CyFunction_clear(m);
+    PyObject_GC_Del(m);
+}
+static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    PyObject_GC_UnTrack(m);
+    __Pyx__CyFunction_dealloc(m);
+}
+static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
+{
+    Py_VISIT(m->func_closure);
+    Py_VISIT(m->func.m_module);
+    Py_VISIT(m->func_dict);
+    Py_VISIT(m->func_name);
+    Py_VISIT(m->func_qualname);
+    Py_VISIT(m->func_doc);
+    Py_VISIT(m->func_globals);
+    Py_VISIT(m->func_code);
+    Py_VISIT(m->func_classobj);
+    Py_VISIT(m->defaults_tuple);
+    Py_VISIT(m->defaults_kwdict);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_VISIT(pydefaults[i]);
+    }
+    return 0;
+}
+static PyObject *__Pyx_CyFunction_descr_get(PyObject *func, PyObject *obj, PyObject *type)
+{
+#if PY_MAJOR_VERSION < 3
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    if (m->flags & __Pyx_CYFUNCTION_STATICMETHOD) {
+        Py_INCREF(func);
+        return func;
+    }
+    if (m->flags & __Pyx_CYFUNCTION_CLASSMETHOD) {
+        if (type == NULL)
+            type = (PyObject *)(Py_TYPE(obj));
+        return __Pyx_PyMethod_New(func, type, (PyObject *)(Py_TYPE(type)));
+    }
+    if (obj == Py_None)
+        obj = NULL;
+#endif
+    return __Pyx_PyMethod_New(func, obj, type);
+}
+static PyObject*
+__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
+{
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromFormat("<cyfunction %U at %p>",
+                                op->func_qualname, (void *)op);
+#else
+    return PyString_FromFormat("<cyfunction %s at %p>",
+                               PyString_AsString(op->func_qualname), (void *)op);
+#endif
+}
+static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+    PyCFunctionObject* f = (PyCFunctionObject*)func;
+    PyCFunction meth = f->m_ml->ml_meth;
+    Py_ssize_t size;
+    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    case METH_VARARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0))
+            return (*meth)(self, arg);
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
+    case METH_NOARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 0))
+                return (*meth)(self, NULL);
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    case METH_O:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 1)) {
+                PyObject *result, *arg0;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                arg0 = PyTuple_GET_ITEM(arg, 0);
+                #else
+                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                #endif
+                result = (*meth)(self, arg0);
+                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+                Py_DECREF(arg0);
+                #endif
+                return result;
+            }
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags in "
+                        "__Pyx_CyFunction_Call. METH_OLDARGS is no "
+                        "longer supported!");
+        return NULL;
+    }
+    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
+                 f->m_ml->ml_name);
+    return NULL;
+}
+static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+}
+static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
+    PyObject *result;
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        Py_ssize_t argc;
+        PyObject *new_args;
+        PyObject *self;
+        argc = PyTuple_GET_SIZE(args);
+        new_args = PyTuple_GetSlice(args, 1, argc);
+        if (unlikely(!new_args))
+            return NULL;
+        self = PyTuple_GetItem(args, 0);
+        if (unlikely(!self)) {
+            Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
+            return NULL;
+        }
+        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
+        Py_DECREF(new_args);
+    } else {
+        result = __Pyx_CyFunction_Call(func, args, kw);
+    }
+    return result;
+}
+static PyTypeObject __pyx_CyFunctionType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+    (destructor) __Pyx_CyFunction_dealloc,
+    0,
+    0,
+    0,
+#if PY_MAJOR_VERSION < 3
+    0,
+#else
+    0,
+#endif
+    (reprfunc) __Pyx_CyFunction_repr,
+    0,
+    0,
+    0,
+    0,
+    __Pyx_CyFunction_CallAsMethod,
+    0,
+    0,
+    0,
+    0,
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,
+    0,
+    (traverseproc) __Pyx_CyFunction_traverse,
+    (inquiry) __Pyx_CyFunction_clear,
+    0,
+#if PY_VERSION_HEX < 0x030500A0
+    offsetof(__pyx_CyFunctionObject, func_weakreflist),
+#else
+    offsetof(PyCFunctionObject, m_weakreflist),
+#endif
+    0,
+    0,
+    __pyx_CyFunction_methods,
+    __pyx_CyFunction_members,
+    __pyx_CyFunction_getsets,
+    0,
+    0,
+    __Pyx_CyFunction_descr_get,
+    0,
+    offsetof(__pyx_CyFunctionObject, func_dict),
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+    0,
+#endif
+};
+static int __pyx_CyFunction_init(void) {
+    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
+    if (unlikely(__pyx_CyFunctionType == NULL)) {
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults = PyObject_Malloc(size);
+    if (unlikely(!m->defaults))
+        return PyErr_NoMemory();
+    memset(m->defaults, 0, size);
+    m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
+    return m->defaults;
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_tuple = tuple;
+    Py_INCREF(tuple);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_kwdict = dict;
+    Py_INCREF(dict);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->func_annotations = dict;
+    Py_INCREF(dict);
+}
+
+/* CythonFunction */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
```

### Comparing `mibi-bin-tools-0.2.8/src/mibi_bin_tools/_extract_bin.pyx` & `mibi-bin-tools-0.2.9/src/mibi_bin_tools/_extract_bin.pyx`

 * *Files identical despite different names*

### Comparing `mibi-bin-tools-0.2.8/src/mibi_bin_tools/bin_files.py` & `mibi-bin-tools-0.2.9/src/mibi_bin_tools/bin_files.py`

 * *Files identical despite different names*

### Comparing `mibi-bin-tools-0.2.8/src/mibi_bin_tools/panel_utils.py` & `mibi-bin-tools-0.2.9/src/mibi_bin_tools/panel_utils.py`

 * *Files identical despite different names*

### Comparing `mibi-bin-tools-0.2.8/src/mibi_bin_tools.egg-info/PKG-INFO` & `mibi-bin-tools-0.2.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 Metadata-Version: 2.1
 Name: mibi-bin-tools
-Version: 0.2.8
+Version: 0.2.9
 Summary: Source for extracting .bin files from the commercial MIBI.
 Author-email: Angelo Lab <theangelolab@gmail.com>
 License: Modified Apache License 2.0
 Project-URL: repository, https://github.com/angelolab/mibi-bin-tools
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-[![Build Status](https://travis-ci.com/angelolab/mibi-bin-tools.svg?branch=master)](https://travis-ci.com/angelolab/mibi-bin-tools)
-[![Coverage Status](https://coveralls.io/repos/github/angelolab/mibi-bin-tools/badge.svg?branch=master)](https://coveralls.io/github/angelolab/mibi-bin-tools?branch=master)
-
 # mibi-bin-tools
+<div align="center">
+
+| | | 
+| ---        |    ---  |
+| CI / CD | [![CI](https://github.com/angelolab/mibi-bin-tools/actions/workflows/ci.yml/badge.svg)](https://github.com/angelolab/mibi-bin-tools/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/angelolab/mibi-bin-tools/badge.svg?branch=main)](https://coveralls.io/github/angelolab/mibi-bin-tools?branch=main) |
+| Package | [![PyPI - Version](https://img.shields.io/pypi/v/mibi-bin-tools.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/mibi-bin-tools/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/mibi-bin-tools.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/mibi-bin-tools/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mibi-bin-tools.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/mibi-bin-tools/) |
+|Meta | [![PyPI - License](https://img.shields.io/pypi/l/mibi-bin-tools?color=9400d3)](LICENSE) |
+
+</div>
 
 Toolbox for extracting tiff images from MIBIScope .bin files 
 
-## To install the project:
+## Installation:
+
+### PyPI
 
+```sh
+pip install mibi-bin-tools
+```
+
+### Source
 Open terminal and navigate to where you want the code stored.
 
 Then input the command:
 
-```
+```sh
 git clone https://github.com/angelolab/mibi-bin-tools.git
 ```
 
 Next, you'll need to set up a docker image with all of the required dependencies.
  - First, [download](https://hub.docker.com/?overlay=onboarding) docker desktop. 
  - Once it's sucessfully installed, make sure it is running by looking in toolbar for the Docker whale.
  - Once it's running, enter the following commands into terminal
```

### Comparing `mibi-bin-tools-0.2.8/src/mibi_bin_tools.egg-info/SOURCES.txt` & `mibi-bin-tools-0.2.9/src/mibi_bin_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 .gitignore
 LICENSE
 README.md
 conftest.py
 pyproject.toml
 setup.py
 tox.ini
-./src/mibi_bin_tools/_extract_bin.c
 .github/workflows/build.yml
 .github/workflows/ci.yml
 .github/workflows/pypi_publish.yml
 .github/workflows/release-drafter.yml
 .github/workflows/test.yml
 src/mibi_bin_tools/__init__.py
+src/mibi_bin_tools/_extract_bin.c
 src/mibi_bin_tools/_extract_bin.pyx
 src/mibi_bin_tools/bin_files.py
 src/mibi_bin_tools/panel_utils.py
 src/mibi_bin_tools/type_utils.py
 src/mibi_bin_tools.egg-info/PKG-INFO
 src/mibi_bin_tools.egg-info/SOURCES.txt
 src/mibi_bin_tools.egg-info/dependency_links.txt
```

### Comparing `mibi-bin-tools-0.2.8/tests/bin_files_test.py` & `mibi-bin-tools-0.2.9/tests/bin_files_test.py`

 * *Files identical despite different names*

### Comparing `mibi-bin-tools-0.2.8/tests/data/moly/fov-1-scan-1.bin` & `mibi-bin-tools-0.2.9/tests/data/moly/fov-1-scan-1.bin`

 * *Files identical despite different names*

### Comparing `mibi-bin-tools-0.2.8/tests/data/moly/fov-1-scan-1.json` & `mibi-bin-tools-0.2.9/tests/data/moly/fov-1-scan-1.json`

 * *Files identical despite different names*

### Comparing `mibi-bin-tools-0.2.8/tests/data/tissue/fov-1-scan-1.bin` & `mibi-bin-tools-0.2.9/tests/data/tissue/fov-1-scan-1.bin`

 * *Files identical despite different names*

### Comparing `mibi-bin-tools-0.2.8/tests/data/tissue/fov-1-scan-1.json` & `mibi-bin-tools-0.2.9/tests/data/tissue/fov-1-scan-1.json`

 * *Files identical despite different names*

### Comparing `mibi-bin-tools-0.2.8/tests/data/tissue/fov-2-scan-1.bin` & `mibi-bin-tools-0.2.9/tests/data/tissue/fov-2-scan-1.bin`

 * *Files identical despite different names*

### Comparing `mibi-bin-tools-0.2.8/tests/data/tissue/fov-2-scan-1.json` & `mibi-bin-tools-0.2.9/tests/data/tissue/fov-2-scan-1.json`

 * *Files identical despite different names*

### Comparing `mibi-bin-tools-0.2.8/tests/panel_utils_test.py` & `mibi-bin-tools-0.2.9/tests/panel_utils_test.py`

 * *Files identical despite different names*

