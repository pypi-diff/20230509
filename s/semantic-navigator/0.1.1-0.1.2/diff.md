# Comparing `tmp/semantic-navigator-0.1.1.tar.gz` & `tmp/semantic-navigator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic-navigator-0.1.1.tar", last modified: Tue May  9 19:10:33 2023, max compression
+gzip compressed data, was "semantic-navigator-0.1.2.tar", last modified: Tue May  9 19:34:06 2023, max compression
```

## Comparing `semantic-navigator-0.1.1.tar` & `semantic-navigator-0.1.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.cookiecutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/Justfile
--rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5511 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/infra/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/infra/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/infra/.gcloudignore
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/infra/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/infra/Justfile
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/infra/cors.json
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/semantic_navigator/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/semantic_navigator/app/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/semantic_navigator/app/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/static/loader.css
--rw-r--r--   0 runner    (1001) docker     (123)   105911 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/static/protocol-components.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   324175 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/static/protocol-components.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    55695 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/static/protocol.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   179510 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/static/protocol.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/semantic_navigator/app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/app/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/semantic_navigator/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/bin/fetch_model_for_sem_nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/bin/semantic_navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/semantic_navigator/data/
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/semantic_navigator/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/semantic_navigator/tests/test_empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:10:33.553526 semantic-navigator-0.1.1/semantic_navigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 19:10:33.000000 semantic-navigator-0.1.1/semantic_navigator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:10:33.557525 semantic-navigator-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 19:10:21.000000 semantic-navigator-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.693196 semantic-navigator-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/.cookiecutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.689196 semantic-navigator-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.689196 semantic-navigator-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.689196 semantic-navigator-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/Justfile
+-rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-09 19:34:06.693196 semantic-navigator-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.689196 semantic-navigator-0.1.2/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5511 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.689196 semantic-navigator-0.1.2/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/infra/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/infra/.gcloudignore
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/infra/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/infra/Justfile
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/infra/cors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.689196 semantic-navigator-0.1.2/semantic_navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.689196 semantic-navigator-0.1.2/semantic_navigator/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.693196 semantic-navigator-0.1.2/semantic_navigator/app/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/app/static/loader.css
+-rw-r--r--   0 runner    (1001) docker     (123)   105911 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/app/static/protocol-components.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   324175 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/app/static/protocol-components.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    55695 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/app/static/protocol.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   179510 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/app/static/protocol.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.693196 semantic-navigator-0.1.2/semantic_navigator/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/app/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/app/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/app/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.693196 semantic-navigator-0.1.2/semantic_navigator/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/bin/fetch_model_for_sem_nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/bin/semantic_navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.693196 semantic-navigator-0.1.2/semantic_navigator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.693196 semantic-navigator-0.1.2/semantic_navigator/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/semantic_navigator/tests/test_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:34:06.689196 semantic-navigator-0.1.2/semantic_navigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-09 19:34:06.000000 semantic-navigator-0.1.2/semantic_navigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-09 19:34:06.000000 semantic-navigator-0.1.2/semantic_navigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:34:06.000000 semantic-navigator-0.1.2/semantic_navigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 19:34:06.000000 semantic-navigator-0.1.2/semantic_navigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:34:06.000000 semantic-navigator-0.1.2/semantic_navigator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 19:34:06.000000 semantic-navigator-0.1.2/semantic_navigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 19:34:06.000000 semantic-navigator-0.1.2/semantic_navigator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:34:06.693196 semantic-navigator-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 19:33:52.000000 semantic-navigator-0.1.2/setup.py
```

### Comparing `semantic-navigator-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `semantic-navigator-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `semantic-navigator-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/.github/PULL_REQUEST_TEMPLATE.md` & `semantic-navigator-0.1.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/.github/workflows/ci.yml` & `semantic-navigator-0.1.2/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -88,7 +88,37 @@
       run: |
         python -m build
     - name: Publish to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: CouncilDataProject
         password: ${{ secrets.PYPI_TOKEN }}
+
+  # Deploy web app
+  deploy:
+    if: "success() && startsWith(github.ref, 'refs/tags/')"
+    needs: [publish]
+    runs-on: ubuntu-latest
+
+    steps:
+    - name: Sleep for a second to let PyPI get the new version
+      run: sleep 120
+
+    - uses: actions/checkout@v3
+    - name: Set up Python
+      uses: actions/setup-python@v4
+      with:
+        python-version: "3.10"
+    - uses: extractions/setup-just@v1
+      env:
+        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+    - uses: google-github-actions/auth@v1
+      with:
+        credentials_json: ${{ secrets.GOOGLE_CREDENTIALS }}
+    - name: Set up Cloud SDK
+      uses: google-github-actions/setup-gcloud@v1
+    - name: Run Deploy
+      run:
+        cd infra/
+        just deploy 
+      env:
+        GITHUB_TOKEN: ${{ secrets.GH_PAT }}
```

### Comparing `semantic-navigator-0.1.1/.github/workflows/docs.yml` & `semantic-navigator-0.1.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/.gitignore` & `semantic-navigator-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/CODE_OF_CONDUCT.md` & `semantic-navigator-0.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/CONTRIBUTING.md` & `semantic-navigator-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/Justfile` & `semantic-navigator-0.1.2/Justfile`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/LICENSE` & `semantic-navigator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/PKG-INFO` & `semantic-navigator-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-navigator
-Version: 0.1.1
+Version: 0.1.2
 Summary: An active learning approach to query and search through large archival datasets.
 Author-email: Eva Maxfield Brown <evamxb@uw.edu>, Madeleine Grunde-McLaughlin <mgrunde@uw.edu>, Isabella Pestovski <pestoi@uw.edu>, Lanyi Zhu <lanyizhu@uw.edu>
 License: MPLv2.0
 Project-URL: Homepage, https://github.com/CouncilDataProject/semantic-navigator
 Project-URL: Bug Tracker, https://github.com/CouncilDataProject/semantic-navigator/issues
 Project-URL: Documentation, https://CouncilDataProject.github.io/semantic-navigator
 Project-URL: User Support, https://github.com/CouncilDataProject/semantic-navigator/issues
```

### Comparing `semantic-navigator-0.1.1/README.md` & `semantic-navigator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/docs/conf.py` & `semantic-navigator-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/docs/installation.rst` & `semantic-navigator-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/infra/Dockerfile` & `semantic-navigator-0.1.2/infra/Dockerfile`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/infra/Justfile` & `semantic-navigator-0.1.2/infra/Justfile`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # get and store user
 USER := env_var("USER")
 
 # default params
 default_region := "us-central1"
 default_key_dir := ".keys/"
 default_key := ".keys/sem-nav-dev.json"
-default_project := "cdp-sem-nav-proto"
+default_project := "sem-nav-eva-005"
 
 # run gcloud login
 login:
     gcloud auth login
     gcloud auth application-default login
 
 # generate a service account JSON
@@ -56,30 +56,26 @@
 
 # deploy the web app
 deploy project=default_project region=default_region:
     just enable-services
     -gsutil mb gs://{{project}}
     gsutil cors set cors.json gs://{{project}}
     gsutil defacl ch -u AllUsers:R gs://{{project}}
+    gcloud builds submit --tag gcr.io/{{project}}/semanticnavigator
+    gcloud run deploy semanticnavigator \
+        --image gcr.io/{{project}}/semanticnavigator \
+        --region {{region}} \
+        --allow-unauthenticated \
+        --memory 4Gi
 
 # fully teardown project
 destroy project:
     gcloud projects delete {{project}}
     rm -f {{default_key_dir}}{{project}}.json
 
 # build docker image locally
 build-docker:
 	docker build --tag semantic-navigator {{justfile_directory()}}
 
 # run docker image locally
 run-docker:
-	docker run --rm -p 9090:8080 -e PORT=8080 semantic-navigator
-
-# deploy the web app
-deploy project=default_project region=default_region:
-	just enable-services
-	gcloud builds submit --tag gcr.io/{{project}}/paperswithoutcode
-	gcloud run deploy paperswithoutcode \
-		--image gcr.io/{{project}}/paperswithoutcode \
-		--region {{region}} \
-		--allow-unauthenticated \
-		--memory 4Gi
+	docker run --rm -p 9090:8080 -e PORT=8080 semantic-navigator
```

### Comparing `semantic-navigator-0.1.1/pyproject.toml` & `semantic-navigator-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator/app/static/loader.css` & `semantic-navigator-0.1.2/semantic_navigator/app/static/loader.css`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator/app/static/protocol-components.min.css` & `semantic-navigator-0.1.2/semantic_navigator/app/static/protocol-components.min.css`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator/app/static/protocol-components.min.css.map` & `semantic-navigator-0.1.2/semantic_navigator/app/static/protocol-components.min.css.map`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator/app/static/protocol.min.css` & `semantic-navigator-0.1.2/semantic_navigator/app/static/protocol.min.css`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator/app/static/protocol.min.css.map` & `semantic-navigator-0.1.2/semantic_navigator/app/static/protocol.min.css.map`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator/app/templates/base.html` & `semantic-navigator-0.1.2/semantic_navigator/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator/app/templates/index.html` & `semantic-navigator-0.1.2/semantic_navigator/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator/app/views.py` & `semantic-navigator-0.1.2/semantic_navigator/app/views.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator/bin/fetch_model_for_sem_nav.py` & `semantic-navigator-0.1.2/semantic_navigator/bin/fetch_model_for_sem_nav.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator/bin/semantic_navigator.py` & `semantic-navigator-0.1.2/semantic_navigator/bin/semantic_navigator.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator/data/__init__.py` & `semantic-navigator-0.1.2/semantic_navigator/data/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator/tests/conftest.py` & `semantic-navigator-0.1.2/semantic_navigator/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `semantic-navigator-0.1.1/semantic_navigator.egg-info/PKG-INFO` & `semantic-navigator-0.1.2/semantic_navigator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-navigator
-Version: 0.1.1
+Version: 0.1.2
 Summary: An active learning approach to query and search through large archival datasets.
 Author-email: Eva Maxfield Brown <evamxb@uw.edu>, Madeleine Grunde-McLaughlin <mgrunde@uw.edu>, Isabella Pestovski <pestoi@uw.edu>, Lanyi Zhu <lanyizhu@uw.edu>
 License: MPLv2.0
 Project-URL: Homepage, https://github.com/CouncilDataProject/semantic-navigator
 Project-URL: Bug Tracker, https://github.com/CouncilDataProject/semantic-navigator/issues
 Project-URL: Documentation, https://CouncilDataProject.github.io/semantic-navigator
 Project-URL: User Support, https://github.com/CouncilDataProject/semantic-navigator/issues
```

### Comparing `semantic-navigator-0.1.1/semantic_navigator.egg-info/SOURCES.txt` & `semantic-navigator-0.1.2/semantic_navigator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

