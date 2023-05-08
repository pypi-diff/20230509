# Comparing `tmp/cliconfig-0.2.2.tar.gz` & `tmp/cliconfig-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.2.2.tar", last modified: Sun May  7 20:53:12 2023, max compression
+gzip compressed data, was "cliconfig-0.3.0.tar", last modified: Mon May  8 22:58:14 2023, max compression
```

## Comparing `cliconfig-0.2.2.tar` & `cliconfig-0.3.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:53:12.555159 cliconfig-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 20:52:54.000000 cliconfig-0.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:53:12.547159 cliconfig-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:53:12.551159 cliconfig-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 20:52:54.000000 cliconfig-0.2.2/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 20:52:54.000000 cliconfig-0.2.2/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 20:52:54.000000 cliconfig-0.2.2/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 20:52:54.000000 cliconfig-0.2.2/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-07 20:52:54.000000 cliconfig-0.2.2/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 20:52:54.000000 cliconfig-0.2.2/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 20:52:54.000000 cliconfig-0.2.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 20:52:54.000000 cliconfig-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-07 20:52:54.000000 cliconfig-0.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-07 20:52:54.000000 cliconfig-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 20:52:54.000000 cliconfig-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-07 20:53:12.555159 cliconfig-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-05-07 20:52:54.000000 cliconfig-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:53:12.551159 cliconfig-0.2.2/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-07 20:52:54.000000 cliconfig-0.2.2/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 20:53:12.000000 cliconfig-0.2.2/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-07 20:52:54.000000 cliconfig-0.2.2/cliconfig/build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-07 20:52:54.000000 cliconfig-0.2.2/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-05-07 20:52:54.000000 cliconfig-0.2.2/cliconfig/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-07 20:52:54.000000 cliconfig-0.2.2/cliconfig/save_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 20:52:54.000000 cliconfig-0.2.2/cliconfig/show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:53:12.551159 cliconfig-0.2.2/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-07 20:53:12.000000 cliconfig-0.2.2/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-07 20:53:12.000000 cliconfig-0.2.2/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:53:12.000000 cliconfig-0.2.2/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 20:53:12.000000 cliconfig-0.2.2/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 20:53:12.000000 cliconfig-0.2.2/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:53:12.555159 cliconfig-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 20:52:54.000000 cliconfig-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-07 20:52:54.000000 cliconfig-0.2.2/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-07 20:52:54.000000 cliconfig-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-07 20:52:54.000000 cliconfig-0.2.2/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-07 20:52:54.000000 cliconfig-0.2.2/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-07 20:52:54.000000 cliconfig-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 20:52:54.000000 cliconfig-0.2.2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 20:52:54.000000 cliconfig-0.2.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-07 20:52:54.000000 cliconfig-0.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-07 20:52:54.000000 cliconfig-0.2.2/docs/manipulate.md
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-07 20:52:54.000000 cliconfig-0.2.2/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 20:52:54.000000 cliconfig-0.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:53:12.555159 cliconfig-0.2.2/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 20:52:54.000000 cliconfig-0.2.2/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 20:52:54.000000 cliconfig-0.2.2/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 20:52:54.000000 cliconfig-0.2.2/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 20:52:54.000000 cliconfig-0.2.2/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 20:52:54.000000 cliconfig-0.2.2/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:53:12.555159 cliconfig-0.2.2/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 20:52:54.000000 cliconfig-0.2.2/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-07 20:52:54.000000 cliconfig-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 20:52:54.000000 cliconfig-0.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 20:52:54.000000 cliconfig-0.2.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:53:12.555159 cliconfig-0.2.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 20:52:54.000000 cliconfig-0.2.2/scripts/integration-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-07 20:52:54.000000 cliconfig-0.2.2/scripts/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 20:53:12.555159 cliconfig-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 20:52:54.000000 cliconfig-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:53:12.555159 cliconfig-0.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:53:12.555159 cliconfig-0.2.2/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 20:52:54.000000 cliconfig-0.2.2/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 20:52:54.000000 cliconfig-0.2.2/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 20:52:54.000000 cliconfig-0.2.2/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 20:52:54.000000 cliconfig-0.2.2/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:53:12.555159 cliconfig-0.2.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-07 20:52:54.000000 cliconfig-0.2.2/tests/integration/integration_show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-07 20:52:54.000000 cliconfig-0.2.2/tests/test_build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-07 20:52:54.000000 cliconfig-0.2.2/tests/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-07 20:52:54.000000 cliconfig-0.2.2/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-07 20:52:54.000000 cliconfig-0.2.2/tests/test_save_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 20:52:54.000000 cliconfig-0.2.2/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.605119 cliconfig-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.597119 cliconfig-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.597119 cliconfig-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-08 22:57:58.000000 cliconfig-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 22:57:58.000000 cliconfig-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-08 22:58:14.601119 cliconfig-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-08 22:57:58.000000 cliconfig-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.597119 cliconfig-0.3.0/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-08 22:57:58.000000 cliconfig-0.3.0/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 22:58:14.000000 cliconfig-0.3.0/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-08 22:57:58.000000 cliconfig-0.3.0/cliconfig/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-08 22:57:58.000000 cliconfig-0.3.0/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-05-08 22:57:58.000000 cliconfig-0.3.0/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-05-08 22:57:58.000000 cliconfig-0.3.0/cliconfig/process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-05-08 22:57:58.000000 cliconfig-0.3.0/cliconfig/processings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-08 22:58:14.000000 cliconfig-0.3.0/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-08 22:58:14.000000 cliconfig-0.3.0/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:58:14.000000 cliconfig-0.3.0/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 22:58:14.000000 cliconfig-0.3.0/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 22:58:14.000000 cliconfig-0.3.0/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/manipulate.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 22:57:58.000000 cliconfig-0.3.0/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 22:57:58.000000 cliconfig-0.3.0/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-08 22:57:58.000000 cliconfig-0.3.0/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-08 22:57:58.000000 cliconfig-0.3.0/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-08 22:57:58.000000 cliconfig-0.3.0/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 22:57:58.000000 cliconfig-0.3.0/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-08 22:57:58.000000 cliconfig-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-08 22:57:58.000000 cliconfig-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 22:57:58.000000 cliconfig-0.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-08 22:57:58.000000 cliconfig-0.3.0/scripts/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 22:58:14.605119 cliconfig-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-08 22:57:58.000000 cliconfig-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/configs/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/test_build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/test_process_routines.py
```

### Comparing `cliconfig-0.2.2/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.3.0/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/.github/workflows/pydocstyle.yaml` & `cliconfig-0.3.0/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/.github/workflows/pylint.yaml` & `cliconfig-0.3.0/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/.github/workflows/tests.yaml` & `cliconfig-0.3.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/.pylintrc` & `cliconfig-0.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/CONTRIBUTING.md` & `cliconfig-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/LICENSE` & `cliconfig-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/PKG-INFO` & `cliconfig-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.2.2
+Version: 0.3.0
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -34,25 +34,25 @@
 
 [![Tests](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/098e9c7c53be88779ee52ef2f2bc8803/raw/cliconfig_tests.json)](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml)
 [![Documentation Status](https://readthedocs.org/projects/cliconfig/badge/?version=latest)](https://cliconfig.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
-In a new virtual environment, install the package with:
+In a new virtual environment, simply install the package with:
 
 ```bash
 pip install cliconfig
 ```
 
 ## Quick start
 
 First create a default config that can be split in multiple files that will be merged
 (from left to right in `make_config` function). There is no limit of depth for the
-configurations parameters.
+configuration parameters.
 
 ```yaml
 ---  # default1.yaml
 param1: 1
 param2: 0
 letters:
   letter1: a
@@ -71,35 +71,35 @@
 from cliconfig import make_config, show_config
 
 config = make_config('default1.yaml', 'default2.yaml')
 show_config(config)
 ```
 
 Then add one or multiple additional config files that will override the default values.
-**By default the additional config files cannot bring new parameters**.
-It is intended to prevent typos in the config files that would not be detected.
-It also improves the readability of the config files and the retro-compatibility.
-By the way, you can change this behavior with `allow_new_keys=True` in `make_config`
-(be careful).
 
 ```yaml
 ---  # first.yaml
 letters:
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
+**The additional config files cannot add new parameters that are not in
+default configs**. It is intended to prevent typos in the config files that would
+not be detected. It also improves the readability of the config files and the
+retro-compatibility.
+
 Now you can launch the program with additional configurations and parameters.
 The additional configurations are indicated with `--config` (separate with comma,
-without space) and the parameters with `--<param_name>`. The default configuration
-will be merged with the additional configurations (from left to right), then the
-parameters will be set.
+without space) and the parameters with `--<param_name>` (use dot for nested configs).
+The default configuration will be merged with the additional configurations
+(from left to right), then the parameters will be set.
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 Will show:
 
@@ -123,15 +123,15 @@
 Use lists instead if possible
 
 `None` is not recognized as a None object by YAML but as a string, you may use `null`
 or `Null` instead if you want to
 set a None object.
 
 Dicts are considered as sub-configs and so you may not be able to change the keys if
-`allow_new_keys=False` (default). If you want to modify a dict keys, you should
+`allow_new_keys=False` (default). If you want to modify or add dict keys, you should
 enclose it in a list.
 
 For instance:
 
 ```yaml
 --- default.yaml
 logging:
```

### Comparing `cliconfig-0.2.2/README.md` & `cliconfig-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,25 +22,25 @@
 
 [![Tests](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/098e9c7c53be88779ee52ef2f2bc8803/raw/cliconfig_tests.json)](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml)
 [![Documentation Status](https://readthedocs.org/projects/cliconfig/badge/?version=latest)](https://cliconfig.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
-In a new virtual environment, install the package with:
+In a new virtual environment, simply install the package with:
 
 ```bash
 pip install cliconfig
 ```
 
 ## Quick start
 
 First create a default config that can be split in multiple files that will be merged
 (from left to right in `make_config` function). There is no limit of depth for the
-configurations parameters.
+configuration parameters.
 
 ```yaml
 ---  # default1.yaml
 param1: 1
 param2: 0
 letters:
   letter1: a
@@ -59,35 +59,35 @@
 from cliconfig import make_config, show_config
 
 config = make_config('default1.yaml', 'default2.yaml')
 show_config(config)
 ```
 
 Then add one or multiple additional config files that will override the default values.
-**By default the additional config files cannot bring new parameters**.
-It is intended to prevent typos in the config files that would not be detected.
-It also improves the readability of the config files and the retro-compatibility.
-By the way, you can change this behavior with `allow_new_keys=True` in `make_config`
-(be careful).
 
 ```yaml
 ---  # first.yaml
 letters:
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
+**The additional config files cannot add new parameters that are not in
+default configs**. It is intended to prevent typos in the config files that would
+not be detected. It also improves the readability of the config files and the
+retro-compatibility.
+
 Now you can launch the program with additional configurations and parameters.
 The additional configurations are indicated with `--config` (separate with comma,
-without space) and the parameters with `--<param_name>`. The default configuration
-will be merged with the additional configurations (from left to right), then the
-parameters will be set.
+without space) and the parameters with `--<param_name>` (use dot for nested configs).
+The default configuration will be merged with the additional configurations
+(from left to right), then the parameters will be set.
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 Will show:
 
@@ -111,15 +111,15 @@
 Use lists instead if possible
 
 `None` is not recognized as a None object by YAML but as a string, you may use `null`
 or `Null` instead if you want to
 set a None object.
 
 Dicts are considered as sub-configs and so you may not be able to change the keys if
-`allow_new_keys=False` (default). If you want to modify a dict keys, you should
+`allow_new_keys=False` (default). If you want to modify or add dict keys, you should
 enclose it in a list.
 
 For instance:
 
 ```yaml
 --- default.yaml
 logging:
```

### Comparing `cliconfig-0.2.2/cliconfig/cli_parser.py` & `cliconfig-0.3.0/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.3.0/cliconfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.2.2
+Version: 0.3.0
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -34,25 +34,25 @@
 
 [![Tests](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/valentingol/098e9c7c53be88779ee52ef2f2bc8803/raw/cliconfig_tests.json)](https://github.com/valentingol/cliconfig/actions/workflows/tests.yaml)
 [![Documentation Status](https://readthedocs.org/projects/cliconfig/badge/?version=latest)](https://cliconfig.readthedocs.io/en/latest/?badge=latest)
 
 ## Installation
 
-In a new virtual environment, install the package with:
+In a new virtual environment, simply install the package with:
 
 ```bash
 pip install cliconfig
 ```
 
 ## Quick start
 
 First create a default config that can be split in multiple files that will be merged
 (from left to right in `make_config` function). There is no limit of depth for the
-configurations parameters.
+configuration parameters.
 
 ```yaml
 ---  # default1.yaml
 param1: 1
 param2: 0
 letters:
   letter1: a
@@ -71,35 +71,35 @@
 from cliconfig import make_config, show_config
 
 config = make_config('default1.yaml', 'default2.yaml')
 show_config(config)
 ```
 
 Then add one or multiple additional config files that will override the default values.
-**By default the additional config files cannot bring new parameters**.
-It is intended to prevent typos in the config files that would not be detected.
-It also improves the readability of the config files and the retro-compatibility.
-By the way, you can change this behavior with `allow_new_keys=True` in `make_config`
-(be careful).
 
 ```yaml
 ---  # first.yaml
 letters:
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
+**The additional config files cannot add new parameters that are not in
+default configs**. It is intended to prevent typos in the config files that would
+not be detected. It also improves the readability of the config files and the
+retro-compatibility.
+
 Now you can launch the program with additional configurations and parameters.
 The additional configurations are indicated with `--config` (separate with comma,
-without space) and the parameters with `--<param_name>`. The default configuration
-will be merged with the additional configurations (from left to right), then the
-parameters will be set.
+without space) and the parameters with `--<param_name>` (use dot for nested configs).
+The default configuration will be merged with the additional configurations
+(from left to right), then the parameters will be set.
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 Will show:
 
@@ -123,15 +123,15 @@
 Use lists instead if possible
 
 `None` is not recognized as a None object by YAML but as a string, you may use `null`
 or `Null` instead if you want to
 set a None object.
 
 Dicts are considered as sub-configs and so you may not be able to change the keys if
-`allow_new_keys=False` (default). If you want to modify a dict keys, you should
+`allow_new_keys=False` (default). If you want to modify or add dict keys, you should
 enclose it in a list.
 
 For instance:
 
 ```yaml
 --- default.yaml
 logging:
```

### Comparing `cliconfig-0.2.2/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.3.0/cliconfig.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 .github/workflows/pylint.yaml
 .github/workflows/ruff.yaml
 .github/workflows/tests.yaml
 cliconfig/__init__.py
 cliconfig/_version.py
 cliconfig/build_config.py
 cliconfig/cli_parser.py
-cliconfig/routines.py
-cliconfig/save_load.py
-cliconfig/show.py
+cliconfig/dict_routines.py
+cliconfig/process_routines.py
+cliconfig/processings.py
 cliconfig.egg-info/PKG-INFO
 cliconfig.egg-info/SOURCES.txt
 cliconfig.egg-info/dependency_links.txt
 cliconfig.egg-info/requires.txt
 cliconfig.egg-info/top_level.txt
 docs/Makefile
 docs/cliconfig_api.rst
@@ -41,19 +41,20 @@
 docs/requirements.txt
 github_actions_utils/__init__.py
 github_actions_utils/color.py
 github_actions_utils/pydocstyle_manager.py
 github_actions_utils/pylint_manager.py
 github_actions_utils/pytest_manager.py
 licenses_tier/FLATTEN_DICT_LICENSE
-scripts/integration-tests.sh
 scripts/pre-commit-checks.sh
+tests/__init__.py
+tests/conftest.py
 tests/test_build_config.py
 tests/test_cli_parser.py
-tests/test_routines.py
-tests/test_save_load.py
-tests/test_show.py
+tests/test_dict_routines.py
+tests/test_process_routines.py
 tests/configs/config1.yaml
 tests/configs/config2.yaml
+tests/configs/configtag1.yaml
+tests/configs/configtag2.yaml
 tests/configs/default1.yaml
-tests/configs/default2.yaml
-tests/integration/integration_show.py
+tests/configs/default2.yaml
```

### Comparing `cliconfig-0.2.2/docs/Makefile` & `cliconfig-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/docs/conf.py` & `cliconfig-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/docs/edge_cases.md` & `cliconfig-0.3.0/docs/edge_cases.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Use lists instead if possible
 
 `None` is not recognized as a None object by YAML but as a string, you may use `null`
 or `Null` instead if you want to
 set a None object.
 
 Dicts are considered as sub-configs and so you may not be able to change the keys if
-`allow_new_keys=False` (default). If you want to modify a dict keys, you should
+`allow_new_keys=False` (default). If you want to modify or add dict keys, you should
 enclose it in a list.
 
 For instance:
 
 ```yaml
 --- default.yaml
 logging:
```

### Comparing `cliconfig-0.2.2/docs/index.rst` & `cliconfig-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/docs/license.md` & `cliconfig-0.3.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/docs/make.bat` & `cliconfig-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/docs/manipulate.md` & `cliconfig-0.3.0/docs/manipulate.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/docs/quickstart.md` & `cliconfig-0.3.0/docs/quickstart.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Quick start
 
 First create a default config that can be split in multiple files that will be merged
 (from left to right in `make_config` function). There is no limit of depth for the
-configurations parameters.
+configuration parameters.
 
 ```yaml
 ---  # default1.yaml
 param1: 1
 param2: 0
 letters:
   letter1: a
@@ -25,35 +25,35 @@
 from cliconfig import make_config, show_config
 
 config = make_config('default1.yaml', 'default2.yaml')
 show_config(config)
 ```
 
 Then add one or multiple additional config files that will override the default values.
-**By default the additional config files cannot bring new parameters**.
-It is intended to prevent typos in the config files that would not be detected.
-It also improves the readability of the config files and the retro-compatibility.
-By the way, you can change this behavior with `allow_new_keys=True` in `make_config`
-(be careful).
 
 ```yaml
 ---  # first.yaml
 letters:
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
+**The additional config files cannot add new parameters that are not in
+default configs**. It is intended to prevent typos in the config files that would
+not be detected. It also improves the readability of the config files and the
+retro-compatibility.
+
 Now you can launch the program with additional configurations and parameters.
 The additional configurations are indicated with `--config` (separate with comma,
-without space) and the parameters with `--<param_name>`. The default configuration
-will be merged with the additional configurations (from left to right), then the
-parameters will be set.
+without space) and the parameters with `--<param_name>` (use dot for nested configs).
+The default configuration will be merged with the additional configurations
+(from left to right), then the parameters will be set.
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 Will show:
```

### Comparing `cliconfig-0.2.2/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.3.0/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/github_actions_utils/pylint_manager.py` & `cliconfig-0.3.0/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/github_actions_utils/pytest_manager.py` & `cliconfig-0.3.0/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.3.0/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/pyproject.toml` & `cliconfig-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/scripts/pre-commit-checks.sh` & `cliconfig-0.3.0/scripts/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/tests/test_build_config.py` & `cliconfig-0.3.0/tests/test_build_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""Tests for build_config.py."""
+"""Tests for config.py."""
 import sys
 
 import pytest
 import pytest_check as check
 
-from cliconfig.build_config import make_config
+from cliconfig.build_config import load_config, make_config
 
 
 def test_make_config(capsys: pytest.CaptureFixture) -> None:
     """Test make_config."""
     sys_argv = sys.argv.copy()
     sys.argv = [
         "tests/test_make_config.py.py",
@@ -35,26 +35,14 @@
     expected_out = (
         "[CONFIG] Merge 2 default configs, "
         "2 additional configs and 1 CLI parameter(s).\n"
     )
     check.equal(config, expected_config)
     check.equal(out, expected_out)
 
-    # No default configs
-    config = make_config(allow_new_keys=True)
-    expected_config = {
-        "param1": 4,
-        "param2": 6,
-        "letters": {
-            "letter1": "f",
-            "letter2": "e",
-        },
-    }
-    check.equal(config, expected_config)
-
     # No additional configs
     sys.argv = [
         "tests/test_make_config.py.py",
     ]
     config = make_config("tests/configs/default1.yaml", "tests/configs/default2.yaml")
     expected_config = {
         "param1": 1,
@@ -66,7 +54,39 @@
             "letter3": "c",
             "letter4": "d",
         },
     }
     check.equal(config, expected_config)
 
     sys.argv = sys_argv.copy()
+
+
+def test_load_config() -> None:
+    """Test and load_config."""
+    # With default configs
+    config = load_config(
+        "tests/configs/config2.yaml",
+        default_config_paths=[
+            "tests/configs/default1.yaml",
+            "tests/configs/default2.yaml",
+        ]
+    )
+    expected_config = {
+        "param1": 4,
+        "param2": 2,
+        "param3": 3,
+        "letters": {
+            "letter1": "a",
+            "letter2": "e",
+            "letter3": "c",
+            "letter4": "d",
+        },
+    }
+    check.equal(config, expected_config)
+    # Additional keys when allow_new_keys=False
+    with pytest.raises(ValueError, match="New parameter found 'param3'.*"):
+        load_config(
+            "tests/configs/default2.yaml",
+            default_config_paths=[
+                "tests/configs/default1.yaml",
+            ],
+        )
```

### Comparing `cliconfig-0.2.2/tests/test_cli_parser.py` & `cliconfig-0.3.0/tests/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.2/tests/test_routines.py` & `cliconfig-0.3.0/tests/test_dict_routines.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,138 @@
-"""Tests for build.py."""
+"""Tests for dict routines."""
+import os
+import shutil
+
 import pytest
 import pytest_check as check
 
-from cliconfig.routines import (
+from cliconfig.dict_routines import (
     _del_key,
     clean_pre_flat,
-    flat_config,
-    merge_config,
-    merge_config_file,
-    unflat_config,
+    flatten,
+    load_dict,
+    merge_flat,
+    merge_flat_paths,
+    save_dict,
+    show_dict,
+    unflatten,
 )
 
 
-def test_merge_config() -> None:
-    """Test merge_config."""
-    config1 = {"a.b": 1, "a": {"c": 2}}
-    config2 = {"c": 3}
-    config = merge_config(config1, config2, allow_new_keys=True)
-    check.equal(config, {"a": {"b": 1, "c": 2}, "c": 3})
+def test_flatten() -> None:
+    """Test flatten(."""
+    check.equal(
+        flatten({"a.b": 1, "a": {"c": 2}, "d": 3}),
+        {"a.b": 1, "a.c": 2, "d": 3},
+    )
+    check.equal(
+        flatten({"a.b": {"c": 1}, "a": {"b.d": 2}, "a.e": {"f.g": 3}}),
+        {"a.b.c": 1, "a.b.d": 2, "a.e.f.g": 3},
+    )
+    check.equal(
+        flatten({"a.b": 1, "a": {"c": {}}, "a.c": 3}),
+        {"a.b": 1, "a.c": 3},
+    )
+    with pytest.raises(ValueError, match="duplicated key 'a.b'"):
+        flatten({"a.b": 1, "a": {"b": 1}})
+
+
+def test_unflatten() -> None:
+    """Test unflatten."""
+    check.equal(
+        unflatten({"a.b": 1, "a.c": 2, "c": 3}),
+        {"a": {"b": 1, "c": 2}, "c": 3},
+    )
+    with pytest.raises(ValueError, match="The dict must be flatten.*"):
+        unflatten({"a.b": 1, "a": {"c": 2}})
+
+
+def test_merge_flat() -> None:
+    """Test merge_flat."""
+    dict1 = {"a.b": 1, "a": {"c": 2}}
+    dict2 = {"c": 3}
+    check.equal(
+        merge_flat(dict1, dict2, allow_new_keys=True),
+        {"a.b": 1, "a.c": 2, "c": 3},
+    )
     with pytest.raises(ValueError, match="New parameter found 'c'.*"):
-        merge_config(config1, config2, allow_new_keys=False)
-    config1 = {"a.b": 1, "a": {"b": 1, "c": 2}}
+        merge_flat(dict1, dict2, allow_new_keys=False)
+    dict1 = {"a.b": 1, "a": {"b": 1, "c": 2}}
     with pytest.raises(
         ValueError,
         match="Duplicated key found.*You may consider calling `clean_pre_flat`.*",
     ):
-        merge_config(config1, config2, allow_new_keys=True)
+        merge_flat(dict1, dict2, allow_new_keys=True)
 
 
-def test_merge_config_file() -> None:
-    """Test merge_config."""
-    config1 = {
+def test_merge_flat_paths() -> None:
+    """Test merge_flat_paths."""
+    dict1 = {
         "param1": 1,
         "param2": 2,
         "letters": {
             "letter1": "a",
             "letter2": "b",
         },
     }
-    config2 = {
+    dict2 = {
         "param3": 3,
         "letters": {
             "letter3": "c",
             "letter4": "d",
         },
     }
-    expected_config = {
+    expected_dict = {
         "param1": 1,
         "param2": 2,
         "param3": 3,
-        "letters": {
-            "letter1": "a",
-            "letter2": "b",
-            "letter3": "c",
-            "letter4": "d",
-        },
+        "letters.letter1": "a",
+        "letters.letter2": "b",
+        "letters.letter3": "c",
+        "letters.letter4": "d",
     }
 
-    config = merge_config_file(
+    flat_dict = merge_flat_paths(
         "tests/configs/default1.yaml",
         "tests/configs/default2.yaml",
         allow_new_keys=True,
     )
-    check.equal(config, expected_config)
-    config = merge_config_file(config1, config2, allow_new_keys=True)
-    check.equal(config, expected_config)
-    config = merge_config_file(
-        config1, "tests/configs/default2.yaml", allow_new_keys=True
+    check.equal(flat_dict, expected_dict)
+    flat_dict = merge_flat_paths(dict1, dict2, allow_new_keys=True)
+    check.equal(flat_dict, expected_dict)
+    flat_dict = merge_flat_paths(
+        dict1, "tests/configs/default2.yaml", allow_new_keys=True
     )
-    check.equal(config, expected_config)
+    check.equal(flat_dict, expected_dict)
     with pytest.raises(ValueError, match="New parameter found 'param3'.*"):
-        merge_config_file(
+        merge_flat_paths(
             "tests/configs/default1.yaml",
             "tests/configs/default2.yaml",
             allow_new_keys=False,
         )
 
 
-def test_flat_config() -> None:
-    """Test flat_config."""
-    check.equal(
-        flat_config({"a.b": 1, "a": {"c": 2}, "d": 3}),
-        {"a.b": 1, "a.c": 2, "d": 3},
-    )
-    check.equal(
-        flat_config({"a.b": 1, "a": {"c": {}}, "a.c": 3}),
-        {"a.b": 1, "a.c": 3},
-    )
-    with pytest.raises(ValueError, match="duplicated key 'a.b'"):
-        flat_config({"a.b": 1, "a": {"b": 1}})
-
+def test_del_key() -> None:
+    """Test _del_key."""
+    in_dict = {"a": {"b": {"c": 1}, "d": 2}, "a.e": 3, "a.b.c": 4}
+    _del_key(in_dict, "a.b.c")
+    check.equal(in_dict, {"a": {"d": 2}, "a.e": 3})
+
+    in_dict = {"a": {"b": {"c": 1}, "d": 2}, "a.e": 3, "a.b.c": 4}
+    _del_key(in_dict, "a.b.c", keep_flat=True)
+    check.equal(in_dict, {"a": {"d": 2}, "a.e": 3, "a.b.c": 4})
+
+    in_dict = {"a": {"b": {"c": 1}, "d": 2}, "a.e": 3, "a.b.c": 4}
+    _del_key(in_dict, "a.b.c", keep_unflat=True)
+    check.equal(in_dict, {"a": {"b": {"c": 1}, "d": 2}, "a.e": 3})
 
-def test_unflat_config() -> None:
-    """Test unflat_config."""
-    check.equal(
-        unflat_config({"a.b": 1, "a.c": 2, "c": 3}),
-        {"a": {"b": 1, "c": 2}, "c": 3},
-    )
-    with pytest.raises(ValueError, match="The config must be flatten.*"):
-        unflat_config({"a.b": 1, "a": {"c": 2}})
+    with pytest.raises(ValueError, match="Key 'a.b.z' not found in dict."):
+        _del_key({"a": {"b": {"c": 1}, "d": 2}, "a.e": 3, "a.b.c": 4}, "a.b.z")
+    with pytest.raises(ValueError, match="Key 'a.z.c' not found in dict."):
+        _del_key({"a": {"b": {"c": 1}, "d": 2}, "a.e": 3, "a.b.c": 4}, "a.z.c")
 
 
 def test_clean_pre_flat() -> None:
     """Test clean_pre_flat."""
     check.equal(
         clean_pre_flat({"a.b": 1, "a": {"b": 2}, "c": 3}, priority="flat"),
         {"a.b": 1, "c": 3},
@@ -119,33 +149,49 @@
             "priority argument must be one of 'flat', 'unflat' or 'error' but "
             "found 'UNKNOWN'"
         ),
     ):
         clean_pre_flat({"a.b": 1, "a": {"b": 2}, "c": 3}, priority="UNKNOWN")
 
 
-def test_del_key() -> None:
-    """Test _del_key."""
-    check.equal(
-        _del_key({"a": {"b": {"c": 1}, "d": 2}, "a.e": 3, "a.b.c": 4}, "a.b.c"),
-        {"a": {"d": 2}, "a.e": 3},
-    )
-    check.equal(
-        _del_key(
-            {"a": {"b": {"c": 1}, "d": 2}, "a.e": 3, "a.b.c": 4},
-            "a.b.c",
-            keep_flat=True,
-        ),
-        {"a": {"d": 2}, "a.e": 3, "a.b.c": 4},
-    )
-    check.equal(
-        _del_key(
-            {"a": {"b": {"c": 1}, "d": 2}, "a.e": 3, "a.b.c": 4},
-            "a.b.c",
-            keep_unflat=True,
-        ),
-        {"a": {"b": {"c": 1}, "d": 2}, "a.e": 3},
-    )
-    with pytest.raises(ValueError, match="Key 'a.b.z' not found in config."):
-        _del_key({"a": {"b": {"c": 1}, "d": 2}, "a.e": 3, "a.b.c": 4}, "a.b.z")
-    with pytest.raises(ValueError, match="Key 'a.z.c' not found in config."):
-        _del_key({"a": {"b": {"c": 1}, "d": 2}, "a.e": 3, "a.b.c": 4}, "a.z.c")
+def test_save_load_dict() -> None:
+    """Test save_dict and load_dict."""
+    config1 = {"a": 1, "b": {"c": 2}, "d": [2, 3.0], "e": [{"f": 4}]}
+    save_dict(config1, "tests/tmp/config.yaml")
+    check.is_true(os.path.isfile("tests/tmp/config.yaml"))
+    config2 = load_dict("tests/tmp/config.yaml")
+    check.equal(config1, config2)
+    shutil.rmtree("tests/tmp")
+
+
+def test_show_dict() -> None:
+    """Test show_dict."""
+    config = {
+        "model": {
+            "s1_ae_config": {
+                "in_dim": 2,
+                "out_dim": 1,
+                "layer_channels": [16, 32, 64],
+                "conv_per_layer": 1,
+                "residual": False,
+                "dropout_rate": 0.0,
+            },
+            "mask_module_dim": [6, 2],
+            "glob_module_dims": [2, 8, 2],
+            "conv_block_dims": [32, 64, 128],
+        },
+        "train": {
+            "n_epochs": 100,
+            "optimizer": {
+                "name": "Adam",
+                "lr": 0.001,
+                "weight_decay": 0.0,
+                "warmup_steps": 0,
+            },
+        },
+        "data": {
+            "dataset": "mnist",
+            "batch_size": 128,
+            "num_workers": 6,
+        },
+    }
+    show_dict(config)
```

