# Comparing `tmp/semantic-navigator-0.1.0.tar.gz` & `tmp/semantic-navigator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic-navigator-0.1.0.tar", last modified: Tue May  9 18:53:26 2023, max compression
+gzip compressed data, was "semantic-navigator-0.1.1.tar", last modified: Tue May  9 19:10:33 2023, max compression
```

## Comparing `semantic-navigator-0.1.0.tar` & `semantic-navigator-0.1.1.tar`

### file list

```diff
@@ -1,69 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.134715 semantic-navigator-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/.cookiecutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.122715 semantic-navigator-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.122715 semantic-navigator-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.122715 semantic-navigator-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/Justfile
--rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-09 18:53:26.134715 semantic-navigator-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.122715 semantic-navigator-0.1.0/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5511 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.122715 semantic-navigator-0.1.0/infra/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/infra/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/infra/.gcloudignore
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/infra/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/infra/Justfile
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/infra/cors.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.122715 semantic-navigator-0.1.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    93022 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/notebooks/cdp-sea-small-gen.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.122715 semantic-navigator-0.1.0/semantic_navigator/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.126715 semantic-navigator-0.1.0/semantic_navigator/app/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.126715 semantic-navigator-0.1.0/semantic_navigator/app/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/app/static/loader.css
--rw-r--r--   0 runner    (1001) docker     (123)   105911 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/app/static/protocol-components.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   324175 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/app/static/protocol-components.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    55695 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/app/static/protocol.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   179510 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/app/static/protocol.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.126715 semantic-navigator-0.1.0/semantic_navigator/app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/app/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/app/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/app/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.126715 semantic-navigator-0.1.0/semantic_navigator/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/bin/semantic_navigator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.126715 semantic-navigator-0.1.0/semantic_navigator/data/
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1609347 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/data/sem-nav-cdp-sea-small-processed-chunks.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)  5684391 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/data/sem-nav-cdp-sea-small.parquet
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.134715 semantic-navigator-0.1.0/semantic_navigator/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/semantic_navigator/tests/test_empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:53:26.126715 semantic-navigator-0.1.0/semantic_navigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-09 18:53:26.000000 semantic-navigator-0.1.0/semantic_navigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-09 18:53:26.000000 semantic-navigator-0.1.0/semantic_navigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:53:26.000000 semantic-navigator-0.1.0/semantic_navigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-09 18:53:26.000000 semantic-navigator-0.1.0/semantic_navigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:53:25.000000 semantic-navigator-0.1.0/semantic_navigator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 18:53:26.000000 semantic-navigator-0.1.0/semantic_navigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 18:53:26.000000 semantic-navigator-0.1.0/semantic_navigator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 18:53:26.134715 semantic-navigator-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 18:53:14.000000 semantic-navigator-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.cookiecutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/Justfile
+-rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5511 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/infra/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/infra/.gcloudignore
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/infra/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/infra/Justfile
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/infra/cors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/semantic_navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/semantic_navigator/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/semantic_navigator/app/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/static/loader.css
+-rw-r--r--   0 runner    (1001) docker     (123)   105911 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/static/protocol-components.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   324175 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/static/protocol-components.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    55695 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/static/protocol.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   179510 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/static/protocol.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/semantic_navigator/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/semantic_navigator/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/bin/fetch_model_for_sem_nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/bin/semantic_navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/semantic_navigator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/semantic_navigator/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/tests/test_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/semantic_navigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/setup.py
```

### Comparing `semantic-navigator-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `semantic-navigator-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `semantic-navigator-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/.github/PULL_REQUEST_TEMPLATE.md` & `semantic-navigator-0.1.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/.github/workflows/ci.yml` & `semantic-navigator-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/.github/workflows/docs.yml` & `semantic-navigator-0.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/.gitignore` & `semantic-navigator-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/CODE_OF_CONDUCT.md` & `semantic-navigator-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/CONTRIBUTING.md` & `semantic-navigator-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/Justfile` & `semantic-navigator-0.1.1/Justfile`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/LICENSE` & `semantic-navigator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/PKG-INFO` & `semantic-navigator-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-navigator
-Version: 0.1.0
+Version: 0.1.1
 Summary: An active learning approach to query and search through large archival datasets.
 Author-email: Eva Maxfield Brown <evamxb@uw.edu>, Madeleine Grunde-McLaughlin <mgrunde@uw.edu>, Isabella Pestovski <pestoi@uw.edu>, Lanyi Zhu <lanyizhu@uw.edu>
 License: MPLv2.0
 Project-URL: Homepage, https://github.com/CouncilDataProject/semantic-navigator
 Project-URL: Bug Tracker, https://github.com/CouncilDataProject/semantic-navigator/issues
 Project-URL: Documentation, https://CouncilDataProject.github.io/semantic-navigator
 Project-URL: User Support, https://github.com/CouncilDataProject/semantic-navigator/issues
```

### Comparing `semantic-navigator-0.1.0/README.md` & `semantic-navigator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/docs/conf.py` & `semantic-navigator-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/docs/installation.rst` & `semantic-navigator-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/infra/Dockerfile` & `semantic-navigator-0.1.1/infra/Dockerfile`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/infra/Justfile` & `semantic-navigator-0.1.1/infra/Justfile`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/pyproject.toml` & `semantic-navigator-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,15 @@
   "umap-learn[plot]~=0.5.3",
 ]
 
 # entry points
 # https://peps.python.org/pep-0621/#entry-points
 [project.entry-points."console_scripts"]
 semantic-navigator = "semantic_navigator.bin.semantic_navigator:main"
+fetch-model-for-sem-nav = "semantic_navigator.bin.fetch_model_for_sem_nav:main"
 
 # build settings
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [tool.setuptools]
 zip-safe = false
 include-package-data = true
 
@@ -147,15 +148,15 @@
 ignore = [
   ".editorconfig",
   ".pre-commit-config.yaml",
   "CODE_OF_CONDUCT.md",
   "CONTRIBUTING.md",
   "Justfile",
   ".cookiecutter.yaml",
-  "*docs/*",
+  "*docs/**",
   "*notebooks/*",
   "*infra/*",
 ]
 
 [tool.mypy]
 files = "semantic_navigator/*.py"
 ignore_missing_imports = true
```

### Comparing `semantic-navigator-0.1.0/semantic_navigator/app/static/loader.css` & `semantic-navigator-0.1.1/semantic_navigator/app/static/loader.css`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/semantic_navigator/app/static/protocol-components.min.css` & `semantic-navigator-0.1.1/semantic_navigator/app/static/protocol-components.min.css`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/semantic_navigator/app/static/protocol-components.min.css.map` & `semantic-navigator-0.1.1/semantic_navigator/app/static/protocol-components.min.css.map`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/semantic_navigator/app/static/protocol.min.css` & `semantic-navigator-0.1.1/semantic_navigator/app/static/protocol.min.css`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/semantic_navigator/app/static/protocol.min.css.map` & `semantic-navigator-0.1.1/semantic_navigator/app/static/protocol.min.css.map`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/semantic_navigator/app/templates/base.html` & `semantic-navigator-0.1.1/semantic_navigator/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/semantic_navigator/app/templates/index.html` & `semantic-navigator-0.1.1/semantic_navigator/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/semantic_navigator/app/views.py` & `semantic-navigator-0.1.1/semantic_navigator/app/views.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/semantic_navigator/bin/semantic_navigator.py` & `semantic-navigator-0.1.1/semantic_navigator/bin/semantic_navigator.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/semantic_navigator/data/__init__.py` & `semantic-navigator-0.1.1/semantic_navigator/data/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Web app support package for semantic_navigator."""
 
 from __future__ import annotations
 
 import json
 import random
-import shutil
 from dataclasses import dataclass
 from datetime import datetime
 from functools import partial
 from itertools import chain
 from logging import getLogger
 from pathlib import Path
 from uuid import uuid4
@@ -16,63 +15,47 @@
 import numpy as np
 import pandas as pd
 from cdp_backend.pipeline.transcript_model import Transcript
 from dataclasses_json import DataClassJsonMixin
 from gcsfs import GCSFileSystem
 from sentence_transformers import SentenceTransformer
 
-###############################################################################
-
-DATA_DIR = Path(__file__).resolve().parent
-CDP_SEATTLE_SMALL_DATASET = DATA_DIR / "sem-nav-cdp-sea-small.parquet"
-CDP_SEATTLE_SMALL_TEXT_FILES_ARCHIVE = (
-    DATA_DIR / "sem-nav-cdp-sea-small-processed-chunks.tar.gz"
-)
+from .. import constants
 
 ###############################################################################
 
 log = getLogger(__name__)
 
 ###############################################################################
 
 
-def load_cdp_sea_small() -> pd.DataFrame:
-    # Load the dataframe at the very least
-    dataset = pd.read_parquet(CDP_SEATTLE_SMALL_DATASET)
-
-    # Unpack the archive
-    shutil.unpack_archive(CDP_SEATTLE_SMALL_TEXT_FILES_ARCHIVE)
-
-    return dataset
-
-
 @dataclass
-class TextChunkWithMeta(DataClassJsonMixin):
+class _TextChunkWithMeta(DataClassJsonMixin):
     chunk_id: str
     event_id: str
     start_time: float
     session_id: str
     session_index: int
     session_datetime: datetime
     text: str
 
 
 @dataclass
-class TextChunkingError:
+class _TextChunkingError:
     event_id: str
     session_id: str
     session_index: int
     session_datetime: datetime
     error: str
 
 
 def _get_text_chunks_from_transcript(
     session_details_row: pd.Series,
     char_count_thresh: int,
-) -> list[TextChunkWithMeta] | TextChunkingError:
+) -> list[_TextChunkWithMeta] | _TextChunkingError:
     try:
         # Read the transcript
         with open(session_details_row.transcript_path) as open_transcript:
             t = Transcript.from_json(open_transcript.read())
 
         # Store for all chunks
         completed_chunks = []
@@ -86,15 +69,15 @@
             # store the current chunk then reset
             if current_chunk_len >= char_count_thresh:
                 # Add chunk to dataset
                 chunk_id = str(uuid4())
 
                 # Add all metadata to dataset
                 completed_chunks.append(
-                    TextChunkWithMeta(
+                    _TextChunkWithMeta(
                         chunk_id=chunk_id,
                         event_id=session_details_row.event_id,
                         start_time=current_chunk_start_time,
                         session_id=session_details_row.id,
                         session_index=session_details_row.session_index,
                         session_datetime=session_details_row.session_datetime,
                         text=" ".join(current_chunk_sentences),
@@ -114,15 +97,15 @@
             current_chunk_sentences.append(sentence.text)
             current_chunk_len += len(sentence.text)
 
         return completed_chunks
 
     # If anything went wrong, raise
     except Exception as e:
-        return TextChunkingError(
+        return _TextChunkingError(
             event_id=session_details_row.event.id,
             session_id=session_details_row.id,
             session_index=session_details_row.session_index,
             session_datetime=session_details_row.session_datetime,
             error=str(e),
         )
 
@@ -155,15 +138,15 @@
     }
 
 
 def _generate_cdp_sea_dataset(
     credentials_path: str | Path,
     n: int | None = None,
     char_count_thresh: int = 1024,
-    embedding_model: str = "all-MiniLM-L12-v2",
+    embedding_model: str = constants.EMBEDDING_MODEL_NAME,
     random_seed: int = 12,
     debug: bool = False,
 ) -> str:
     from cdp_data import CDPInstances, datasets
     from tqdm.contrib.concurrent import process_map, thread_map
 
     ###############################################################
@@ -224,15 +207,15 @@
         )
     )
 
     # Remove any errors
     errors = []
     chunks = []
     for text_chunk_result in text_chunks_results:
-        if isinstance(text_chunk_result, TextChunkWithMeta):
+        if isinstance(text_chunk_result, _TextChunkWithMeta):
             chunks.append(text_chunk_result)
         else:
             errors.append(text_chunk_result)
 
     # Log errors
     if len(errors) > 0:
         if debug:
```

### Comparing `semantic-navigator-0.1.0/semantic_navigator/tests/conftest.py` & `semantic-navigator-0.1.1/semantic_navigator/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.0/semantic_navigator.egg-info/PKG-INFO` & `semantic-navigator-0.1.1/semantic_navigator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-navigator
-Version: 0.1.0
+Version: 0.1.1
 Summary: An active learning approach to query and search through large archival datasets.
 Author-email: Eva Maxfield Brown <evamxb@uw.edu>, Madeleine Grunde-McLaughlin <mgrunde@uw.edu>, Isabella Pestovski <pestoi@uw.edu>, Lanyi Zhu <lanyizhu@uw.edu>
 License: MPLv2.0
 Project-URL: Homepage, https://github.com/CouncilDataProject/semantic-navigator
 Project-URL: Bug Tracker, https://github.com/CouncilDataProject/semantic-navigator/issues
 Project-URL: Documentation, https://CouncilDataProject.github.io/semantic-navigator
 Project-URL: User Support, https://github.com/CouncilDataProject/semantic-navigator/issues
```

### Comparing `semantic-navigator-0.1.0/semantic_navigator.egg-info/SOURCES.txt` & `semantic-navigator-0.1.1/semantic_navigator.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 docs/index.rst
 docs/installation.rst
 infra/.dockerignore
 infra/.gcloudignore
 infra/Dockerfile
 infra/Justfile
 infra/cors.json
-notebooks/cdp-sea-small-gen.ipynb
 semantic_navigator/__init__.py
+semantic_navigator/constants.py
 semantic_navigator/py.typed
 semantic_navigator.egg-info/PKG-INFO
 semantic_navigator.egg-info/SOURCES.txt
 semantic_navigator.egg-info/dependency_links.txt
 semantic_navigator.egg-info/entry_points.txt
 semantic_navigator.egg-info/not-zip-safe
 semantic_navigator.egg-info/requires.txt
@@ -40,13 +40,12 @@
 semantic_navigator/app/static/protocol-components.min.css
 semantic_navigator/app/static/protocol-components.min.css.map
 semantic_navigator/app/static/protocol.min.css
 semantic_navigator/app/static/protocol.min.css.map
 semantic_navigator/app/templates/base.html
 semantic_navigator/app/templates/index.html
 semantic_navigator/bin/__init__.py
+semantic_navigator/bin/fetch_model_for_sem_nav.py
 semantic_navigator/bin/semantic_navigator.py
 semantic_navigator/data/__init__.py
-semantic_navigator/data/sem-nav-cdp-sea-small-processed-chunks.tar.gz
-semantic_navigator/data/sem-nav-cdp-sea-small.parquet
 semantic_navigator/tests/conftest.py
 semantic_navigator/tests/test_empty.py
```

