# Comparing `tmp/happi-2.1.1.tar.gz` & `tmp/happi-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happi-2.1.1.tar", last modified: Sat Apr  8 00:01:07 2023, max compression
+gzip compressed data, was "happi-2.2.0.tar", last modified: Tue May  9 00:02:29 2023, max compression
```

## Comparing `happi-2.1.1.tar` & `happi-2.2.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.074400 happi-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-04-08 00:00:46.000000 happi-2.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)      973 2023-04-08 00:00:46.000000 happi-2.1.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-08 00:00:46.000000 happi-2.1.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-08 00:00:46.000000 happi-2.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.058400 happi-2.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-08 00:00:46.000000 happi-2.1.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-04-08 00:00:46.000000 happi-2.1.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.058400 happi-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-04-08 00:00:46.000000 happi-2.1.1/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-04-08 00:00:46.000000 happi-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-08 00:00:46.000000 happi-2.1.1/.landscape.yml
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-04-08 00:00:46.000000 happi-2.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-08 00:00:46.000000 happi-2.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-04-08 00:00:46.000000 happi-2.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-08 00:00:46.000000 happi-2.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-08 00:00:46.000000 happi-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-08 00:01:07.074400 happi-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-04-08 00:00:46.000000 happi-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.058400 happi-2.1.1/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-04-08 00:00:46.000000 happi-2.1.1/conda-recipe/activate.sh
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-08 00:00:46.000000 happi-2.1.1/conda-recipe/deactivate.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-04-08 00:00:46.000000 happi-2.1.1/conda-recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      430 2023-04-08 00:00:46.000000 happi-2.1.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.058400 happi-2.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-08 00:00:46.000000 happi-2.1.1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (122)      901 2023-04-08 00:00:46.000000 happi-2.1.1/docs/pre-release-notes.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3431 2023-04-08 00:00:46.000000 happi-2.1.1/docs/release_notes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.062399 happi-2.1.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-04-08 00:00:46.000000 happi-2.1.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-08 00:00:46.000000 happi-2.1.1/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7422 2023-04-08 00:00:46.000000 happi-2.1.1/docs/source/client.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-04-08 00:00:46.000000 happi-2.1.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)    10012 2023-04-08 00:00:46.000000 happi-2.1.1/docs/source/containers.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-04-08 00:00:46.000000 happi-2.1.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    22702 2023-04-08 00:00:46.000000 happi-2.1.1/docs/source/releases.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-04-08 00:00:46.000000 happi-2.1.1/docs/source/upcoming_changes.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.062399 happi-2.1.1/docs/source/upcoming_release_notes/
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-04-08 00:00:46.000000 happi-2.1.1/docs/source/upcoming_release_notes/template-full.rst
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-04-08 00:00:46.000000 happi-2.1.1/docs/source/upcoming_release_notes/template-short.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.062399 happi-2.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      929 2023-04-08 00:00:46.000000 happi-2.1.1/examples/db.json
--rw-r--r--   0 runner    (1001) docker     (122)     3493 2023-04-08 00:00:46.000000 happi-2.1.1/examples/launch_edl.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.062399 happi-2.1.1/examples/qt/
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-04-08 00:00:46.000000 happi-2.1.1/examples/qt/listview.py
--rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-04-08 00:00:46.000000 happi-2.1.1/examples/qt/treeview.py
--rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-04-08 00:00:46.000000 happi-2.1.1/github_deploy_key_pcdshub_happi.enc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.066400 happi-2.1.1/happi/
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-08 00:00:46.000000 happi-2.1.1/happi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-08 00:00:46.000000 happi-2.1.1/happi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-08 00:01:06.000000 happi-2.1.1/happi/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-04-08 00:00:46.000000 happi-2.1.1/happi/audit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.070400 happi-2.1.1/happi/backends/
--rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-04-08 00:00:46.000000 happi-2.1.1/happi/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-04-08 00:00:46.000000 happi-2.1.1/happi/backends/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-04-08 00:00:46.000000 happi-2.1.1/happi/backends/json_db.py
--rw-r--r--   0 runner    (1001) docker     (122)     7266 2023-04-08 00:00:46.000000 happi-2.1.1/happi/backends/mongo_db.py
--rw-r--r--   0 runner    (1001) docker     (122)     5325 2023-04-08 00:00:46.000000 happi-2.1.1/happi/backends/multi_db.py
--rw-r--r--   0 runner    (1001) docker     (122)    15490 2023-04-08 00:00:46.000000 happi-2.1.1/happi/backends/qs_db.py
--rw-r--r--   0 runner    (1001) docker     (122)    38591 2023-04-08 00:00:46.000000 happi-2.1.1/happi/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    29883 2023-04-08 00:00:46.000000 happi-2.1.1/happi/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6967 2023-04-08 00:00:46.000000 happi-2.1.1/happi/containers.py
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-04-08 00:00:46.000000 happi-2.1.1/happi/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-04-08 00:00:46.000000 happi-2.1.1/happi/item.py
--rw-r--r--   0 runner    (1001) docker     (122)    14097 2023-04-08 00:00:46.000000 happi-2.1.1/happi/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     7221 2023-04-08 00:00:46.000000 happi-2.1.1/happi/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.070400 happi-2.1.1/happi/qt/
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-04-08 00:00:46.000000 happi-2.1.1/happi/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6252 2023-04-08 00:00:46.000000 happi-2.1.1/happi/qt/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.070400 happi-2.1.1/happi/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-08 00:00:46.000000 happi-2.1.1/happi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19157 2023-04-08 00:00:46.000000 happi-2.1.1/happi/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-04-08 00:00:46.000000 happi-2.1.1/happi/tests/test_audit.py
--rw-r--r--   0 runner    (1001) docker     (122)     9058 2023-04-08 00:00:46.000000 happi-2.1.1/happi/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)    24416 2023-04-08 00:00:46.000000 happi-2.1.1/happi/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    12850 2023-04-08 00:00:46.000000 happi-2.1.1/happi/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-04-08 00:00:46.000000 happi-2.1.1/happi/tests/test_happi_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     5762 2023-04-08 00:00:46.000000 happi-2.1.1/happi/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-04-08 00:00:46.000000 happi-2.1.1/happi/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (122)     3452 2023-04-08 00:00:46.000000 happi-2.1.1/happi/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-04-08 00:00:46.000000 happi-2.1.1/happi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 00:01:07.066400 happi-2.1.1/happi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-08 00:01:06.000000 happi-2.1.1/happi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-04-08 00:01:07.000000 happi-2.1.1/happi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-08 00:01:06.000000 happi-2.1.1/happi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-08 00:01:06.000000 happi-2.1.1/happi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-08 00:01:07.000000 happi-2.1.1/happi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-08 00:01:07.000000 happi-2.1.1/happi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-08 00:00:46.000000 happi-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-08 00:00:46.000000 happi-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-08 00:01:07.074400 happi-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.753220 happi-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-09 00:02:12.000000 happi-2.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2023-05-09 00:02:12.000000 happi-2.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-09 00:02:12.000000 happi-2.2.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-09 00:02:12.000000 happi-2.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.733220 happi-2.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-05-09 00:02:12.000000 happi-2.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-05-09 00:02:12.000000 happi-2.2.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.733220 happi-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-05-09 00:02:12.000000 happi-2.2.0/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-05-09 00:02:12.000000 happi-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-05-09 00:02:12.000000 happi-2.2.0/.landscape.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-05-09 00:02:12.000000 happi-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-09 00:02:12.000000 happi-2.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-05-09 00:02:12.000000 happi-2.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-05-09 00:02:12.000000 happi-2.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-09 00:02:12.000000 happi-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-05-09 00:02:29.753220 happi-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-05-09 00:02:12.000000 happi-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.737220 happi-2.2.0/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-05-09 00:02:12.000000 happi-2.2.0/conda-recipe/activate.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-09 00:02:12.000000 happi-2.2.0/conda-recipe/deactivate.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-05-09 00:02:12.000000 happi-2.2.0/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-05-09 00:02:12.000000 happi-2.2.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.737220 happi-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-09 00:02:12.000000 happi-2.2.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (122)      901 2023-05-09 00:02:12.000000 happi-2.2.0/docs/pre-release-notes.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3431 2023-05-09 00:02:12.000000 happi-2.2.0/docs/release_notes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.741220 happi-2.2.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7422 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/client.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10012 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    23277 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/upcoming_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.741220 happi-2.2.0/docs/source/upcoming_release_notes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/upcoming_release_notes/template-full.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/upcoming_release_notes/template-short.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.741220 happi-2.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      929 2023-05-09 00:02:12.000000 happi-2.2.0/examples/db.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3493 2023-05-09 00:02:12.000000 happi-2.2.0/examples/launch_edl.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.741220 happi-2.2.0/examples/qt/
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-05-09 00:02:12.000000 happi-2.2.0/examples/qt/listview.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-05-09 00:02:12.000000 happi-2.2.0/examples/qt/treeview.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-05-09 00:02:12.000000 happi-2.2.0/github_deploy_key_pcdshub_happi.enc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.745220 happi-2.2.0/happi/
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-09 00:02:12.000000 happi-2.2.0/happi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-09 00:02:12.000000 happi-2.2.0/happi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-09 00:02:29.000000 happi-2.2.0/happi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-05-09 00:02:12.000000 happi-2.2.0/happi/audit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.749220 happi-2.2.0/happi/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-05-09 00:02:12.000000 happi-2.2.0/happi/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-05-09 00:02:12.000000 happi-2.2.0/happi/backends/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-05-09 00:02:12.000000 happi-2.2.0/happi/backends/json_db.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7266 2023-05-09 00:02:12.000000 happi-2.2.0/happi/backends/mongo_db.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5325 2023-05-09 00:02:12.000000 happi-2.2.0/happi/backends/multi_db.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15490 2023-05-09 00:02:12.000000 happi-2.2.0/happi/backends/qs_db.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38591 2023-05-09 00:02:12.000000 happi-2.2.0/happi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29883 2023-05-09 00:02:12.000000 happi-2.2.0/happi/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6967 2023-05-09 00:02:12.000000 happi-2.2.0/happi/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-05-09 00:02:12.000000 happi-2.2.0/happi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-05-09 00:02:12.000000 happi-2.2.0/happi/item.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14512 2023-05-09 00:02:12.000000 happi-2.2.0/happi/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7221 2023-05-09 00:02:12.000000 happi-2.2.0/happi/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.749220 happi-2.2.0/happi/qt/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-05-09 00:02:12.000000 happi-2.2.0/happi/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6352 2023-05-09 00:02:12.000000 happi-2.2.0/happi/qt/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.753220 happi-2.2.0/happi/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19157 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_audit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9058 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24416 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12850 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_happi_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6602 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3452 2023-05-09 00:02:12.000000 happi-2.2.0/happi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-09 00:02:12.000000 happi-2.2.0/happi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.749220 happi-2.2.0/happi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-05-09 00:02:29.000000 happi-2.2.0/happi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-05-09 00:02:29.000000 happi-2.2.0/happi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 00:02:29.000000 happi-2.2.0/happi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-09 00:02:29.000000 happi-2.2.0/happi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-09 00:02:29.000000 happi-2.2.0/happi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-09 00:02:29.000000 happi-2.2.0/happi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-09 00:02:12.000000 happi-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-09 00:02:12.000000 happi-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 00:02:29.753220 happi-2.2.0/setup.cfg
```

### Comparing `happi-2.1.1/.flake8` & `happi-2.2.0/.flake8`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/.github/ISSUE_TEMPLATE.md` & `happi-2.2.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/.github/PULL_REQUEST_TEMPLATE.md` & `happi-2.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/.github/workflows/standard.yml` & `happi-2.2.0/.github/workflows/standard.yml`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/.gitignore` & `happi-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/.pre-commit-config.yaml` & `happi-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/CONTRIBUTING.rst` & `happi-2.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/LICENSE.md` & `happi-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/PKG-INFO` & `happi-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happi
-Version: 2.1.1
+Version: 2.2.0
 Summary: Happi Database Access for LCLS Beamline Devices
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: happi Version: 2.1.1 Summary: Happi Database Access
+Metadata-Version: 2.1 Name: happi Version: 2.2.0 Summary: Happi Database Access
 for LCLS Beamline Devices Author: SLAC National Accelerator Laboratory License:
 Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
 University, through SLAC National Accelerator Laboratory (subject to receipt of
 any required approvals from the U.S. Dept. of Energy). All rights reserved.
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: (1)
 Redistributions of source code must retain the above copyright notice, this
```

### Comparing `happi-2.1.1/README.md` & `happi-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/conda-recipe/meta.yaml` & `happi-2.2.0/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/docs/Makefile` & `happi-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/docs/pre-release-notes.sh` & `happi-2.2.0/docs/pre-release-notes.sh`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/docs/release_notes.py` & `happi-2.2.0/docs/release_notes.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/docs/source/api.rst` & `happi-2.2.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/docs/source/client.rst` & `happi-2.2.0/docs/source/client.rst`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/docs/source/conf.py` & `happi-2.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/docs/source/containers.rst` & `happi-2.2.0/docs/source/containers.rst`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/docs/source/index.rst` & `happi-2.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/docs/source/releases.rst` & `happi-2.2.0/docs/source/releases.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,34 @@
 Release History
 ###############
 
 
+v2.2.0 (2023-05-08)
+===================
+
+Features
+--------
+- Adds a hook in ``happi.loader.from_container`` that runs the method
+  ``post_happi_md`` on an instantiated object after the metadata
+  container has been attached.
+  This allows a clear method for objects to interact with
+  happi metadata if desired.
+
+Maintenance
+-----------
+- Makes ``HappiDeviceTreeView`` more tolerant of items with missing metadata keys.
+  Items missing the key used to group the tree view will be organized
+  into a catch-all "[KEY NOT FOUND]" group.
+
+Contributors
+------------
+- tangkong
+
+
+
 v2.1.0 (2023-04-03)
 ===================
 
 Features
 --------
 - Adds ``happi repair`` command, for synchronizing backend database with fields expected by container.
   Adds a corresponding audit function.
```

### Comparing `happi-2.1.1/docs/source/upcoming_release_notes/template-full.rst` & `happi-2.2.0/docs/source/upcoming_release_notes/template-full.rst`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/examples/db.json` & `happi-2.2.0/examples/db.json`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/examples/launch_edl.py` & `happi-2.2.0/examples/launch_edl.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/examples/qt/listview.py` & `happi-2.2.0/examples/qt/listview.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/examples/qt/treeview.py` & `happi-2.2.0/examples/qt/treeview.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/github_deploy_key_pcdshub_happi.enc` & `happi-2.2.0/github_deploy_key_pcdshub_happi.enc`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/audit.py` & `happi-2.2.0/happi/audit.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/backends/__init__.py` & `happi-2.2.0/happi/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/backends/core.py` & `happi-2.2.0/happi/backends/core.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/backends/json_db.py` & `happi-2.2.0/happi/backends/json_db.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/backends/mongo_db.py` & `happi-2.2.0/happi/backends/mongo_db.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/backends/multi_db.py` & `happi-2.2.0/happi/backends/multi_db.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/backends/qs_db.py` & `happi-2.2.0/happi/backends/qs_db.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/cli.py` & `happi-2.2.0/happi/cli.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/client.py` & `happi-2.2.0/happi/client.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/containers.py` & `happi-2.2.0/happi/containers.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/errors.py` & `happi-2.2.0/happi/errors.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/item.py` & `happi-2.2.0/happi/item.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/loader.py` & `happi-2.2.0/happi/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         )
     return filled
 
 
 def from_container(
     item: HappiItem,
     attach_md: bool = True,
+    run_post_attach_hook: bool = True,
     use_cache: bool = True,
     threaded: bool = False,
 ) -> Any:
     """
     Load an object (or "device") from a compatible HappiItem.
 
     The item container is queried for the ``device_class``, ``args``, and
@@ -118,14 +119,17 @@
 
     Parameters
     ----------
     item : happi.HappiItem
         The item to load.
     attach_md : bool, optional
         Attach the container to the instantiated object as ``md``.
+    run_post_attach_hook : bool, optional
+        Run ``post_happi_md`` method on the device after attaching the container
+        if possible.
     use_cache : bool, optional
         When devices are loaded they are stored in the ``happi.cache``
         dictionary. This means that repeated attempts to load the device will
         return the same object. This prevents unnecessary EPICS connections
         from being initialized in the same process. If a new object is
         needed, set ``use_cache`` to `False` and a new object will be created,
         overriding the current cached object. An object with matching name
@@ -197,14 +201,20 @@
     # Attach the metadata to the object
     if attach_md:
         try:
             setattr(obj, 'md', item)
         except Exception:
             logger.warning("Unable to attach metadata dictionary to device")
 
+        if run_post_attach_hook and hasattr(obj, 'post_happi_md'):
+            try:
+                obj.post_happi_md()
+            except Exception as ex:
+                logger.warning(f"Unable to run {obj}.post_happi_md: {ex}")
+
     # Store the device in the cache
     cache[item.name] = obj
     return obj
 
 
 def import_class(device_class: str):
     """
```

### Comparing `happi-2.1.1/happi/prompt.py` & `happi-2.2.0/happi/prompt.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/qt/model.py` & `happi-2.2.0/happi/qt/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,18 +166,20 @@
         entry_group = collections.defaultdict(list)
 
         for entry in self.entries():
             try:
                 field_val = get_happi_entry_value(entry.item, field)
                 entry_group[field_val].append(entry.item)
             except ValueError:
-                logger.exception(
+                logger.debug(
                     'Could not retrieve value for field %s at entry %s',
                     field, entry
                 )
+                field_val = '[KEY NOT FOUND]'
+                entry_group[field_val].append(entry.item)
 
         for idx, (key_value, entries) in enumerate(entry_group.items()):
             root = QtGui.QStandardItem(key_value)
             # Disable edit
             root.setFlags(root.flags() & ~QtCore.Qt.ItemIsEditable)
 
             if len(entries) == 1 and entries[0].name == key_value:
```

### Comparing `happi-2.1.1/happi/tests/conftest.py` & `happi-2.2.0/happi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/tests/test_audit.py` & `happi-2.2.0/happi/tests/test_audit.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/tests/test_backends.py` & `happi-2.2.0/happi/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/tests/test_cli.py` & `happi-2.2.0/happi/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/tests/test_client.py` & `happi-2.2.0/happi/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/tests/test_happi_item.py` & `happi-2.2.0/happi/tests/test_happi_item.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/tests/test_loader.py` & `happi-2.2.0/happi/tests/test_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any
+from unittest.mock import patch
 
 import pytest
 
 from happi import EntryInfo, OphydItem, cache
 from happi.item import HappiItem
 from happi.loader import fill_template, from_container, load_devices
 from happi.utils import create_alias
@@ -145,7 +146,32 @@
     item_jinja._info_attrs['kwargs'].include_default_as_kwarg = False
     filtered_dev = from_container(item_jinja, use_cache=False)
 
     assert filtered_dev.blank == 'None'
     assert getattr(filtered_dev, 'blank_exclude', 'DNE') == 'DNE'
     for bl in blanks:
         assert getattr(filtered_dev, bl, 'DNE') == 'DNE'
+
+
+class PostDevice:
+    def post_happi_md(self):
+        print('post_happi_md hook run')
+
+
+@pytest.fixture
+def item_post_md_hook():
+    item = HappiItem(name='post_test',
+                     device_class='happi.tests.test_loader.PostDevice')
+    return item
+
+
+def test_post_happi_md(item_post_md_hook: HappiItem):
+    with patch('happi.tests.test_loader.PostDevice.post_happi_md') as mock:
+        dev = from_container(item_post_md_hook, use_cache=False)
+        assert isinstance(dev, PostDevice)
+        mock.assert_called_once()
+
+    with patch('happi.tests.test_loader.PostDevice.post_happi_md') as mock:
+        dev = from_container(item_post_md_hook, run_post_attach_hook=False,
+                             use_cache=False)
+        assert isinstance(dev, PostDevice)
+        mock.assert_not_called()
```

### Comparing `happi-2.1.1/happi/tests/test_prompt.py` & `happi-2.2.0/happi/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/utils.py` & `happi-2.2.0/happi/utils.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi/version.py` & `happi-2.2.0/happi/version.py`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/happi.egg-info/PKG-INFO` & `happi-2.2.0/happi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happi
-Version: 2.1.1
+Version: 2.2.0
 Summary: Happi Database Access for LCLS Beamline Devices
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: happi Version: 2.1.1 Summary: Happi Database Access
+Metadata-Version: 2.1 Name: happi Version: 2.2.0 Summary: Happi Database Access
 for LCLS Beamline Devices Author: SLAC National Accelerator Laboratory License:
 Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
 University, through SLAC National Accelerator Laboratory (subject to receipt of
 any required approvals from the U.S. Dept. of Energy). All rights reserved.
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: (1)
 Redistributions of source code must retain the above copyright notice, this
```

### Comparing `happi-2.1.1/happi.egg-info/SOURCES.txt` & `happi-2.2.0/happi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `happi-2.1.1/pyproject.toml` & `happi-2.2.0/pyproject.toml`

 * *Files identical despite different names*

