# Comparing `tmp/edulint-2.6.1.tar.gz` & `tmp/edulint-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-_6q2y1so/edulint-2.6.1.tar", last modified: Tue May  2 11:21:48 2023, max compression
+gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-k_9gbewx/edulint-2.6.2.tar", last modified: Tue May  9 18:06:24 2023, max compression
```

## Comparing `edulint-2.6.1.tar` & `edulint-2.6.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 11:21:37.000000 edulint-2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-02 11:21:48.000000 edulint-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-02 11:21:37.000000 edulint-2.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/config/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/config/config_translations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1873 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/explanations.py
--rw-r--r--   0 runner    (1001) docker     (123)   180321 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/explanations.toml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/linting/
--rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/linting/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/basic_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/modified_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/python_ta_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/checkers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/linting.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/process_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/linting/tweakers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/prepare_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/prepare_explanations/pylint_data/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/pylint_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15286 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/pylint_data/pylint_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint/prepare_explanations/thonny_data/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/thonny_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/thonny_data/thonny_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-02 11:21:37.000000 edulint-2.6.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 11:21:48.000000 edulint-2.6.1/edulint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-02 11:21:37.000000 edulint-2.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-02 11:21:48.000000 edulint-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-02 11:21:37.000000 edulint-2.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:21:48.000000 edulint-2.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-02 11:21:37.000000 edulint-2.6.1/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 18:06:09.000000 edulint-2.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-09 18:06:24.000000 edulint-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-09 18:06:09.000000 edulint-2.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/config/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/config/config_translations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1873 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180321 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/explanations.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/linting/
+-rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/linting/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/basic_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/modified_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/python_ta_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/checkers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/linting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/process_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/linting/tweakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/prepare_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/prepare_explanations/pylint_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/pylint_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15286 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/pylint_data/pylint_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint/prepare_explanations/thonny_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/thonny_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/thonny_data/thonny_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-09 18:06:09.000000 edulint-2.6.2/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 18:06:24.000000 edulint-2.6.2/edulint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 18:06:09.000000 edulint-2.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-09 18:06:24.000000 edulint-2.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 18:06:09.000000 edulint-2.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:06:24.000000 edulint-2.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20554 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-09 18:06:09.000000 edulint-2.6.2/tests/test_visitors.py
```

### Comparing `edulint-2.6.1/LICENSE` & `edulint-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/config/config.py` & `edulint-2.6.2/edulint/config/config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/config/config_translations.py` & `edulint-2.6.2/edulint/config/config_translations.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
          "loop-shadows-control-variable,no-repeated-op,"
          "forbidden-top-level-code,simplifiable-if-nested,simplifiable-if-seq,"
          "simplifiable-if-return-conj,simplifiable-if-assignment-conj,simplifiable-if-expr-conj,"]
     ),
     Option.PYTHON_SPECIFIC: Translation(
         Linter.PYLINT,
         ["--enable=unidiomatic-typecheck,misplaced-format-function,"
-         "unnecessary-lambda,multiple-imports,use-enumerate,consider-iterating-dictionary,"
+         "use-enumerate,consider-iterating-dictionary,"
          "consider-using-dict-items,consider-using-f-string,"
          "inconsistent-return-statements,consider-swap-variables,"
          "consider-using-join,consider-using-set-comprehension,"
          "unnecessary-comprehension,use-a-generator,use-list-literal,"
          "use-dict-literal,consider-using-in,"]
     ),
     Option.COMPLEXITY: Translation(
```

### Comparing `edulint-2.6.1/edulint/edulint.py` & `edulint-2.6.2/edulint/edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/explanations.toml` & `edulint-2.6.2/edulint/explanations.toml`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linters.py` & `edulint-2.6.2/edulint/linters.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linting/.pylintrc` & `edulint-2.6.2/edulint/linting/.pylintrc`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,15 @@
        no-self-argument,
        non-ascii-name,
        not-in-loop,
        pointless-statement,
        redefined-argument-from-local,
        redefined-builtin,
        return-in-init,
-       return-outside-function,
        self-assigning-variable,
-       singleton-comparison,
        trailing-comma-tuple,
        unnecessary-dict-index-lookup,
        unnecessary-pass,
        unneeded-not,
        unreachable,
        used-before-assignment,
        disallowed-name,
@@ -129,15 +127,14 @@
        no-loop-else,
        remove-for,
        redundant-arithmetic,
        do-not-multiply-mutable,
        redundant-elif,
        unreachable-else,
        invalid-name,
-       wrong-import-position,
        consider-using-from-import,
        wildcard-import,
        reimported,
        invalid-for-target,
        one-iteration,
        no-is-bool,
        use-ord-letter,
```

### Comparing `edulint-2.6.1/edulint/linting/checkers/basic_checker.py` & `edulint-2.6.2/edulint/linting/checkers/basic_checker.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linting/checkers/improper_loop.py` & `edulint-2.6.2/edulint/linting/checkers/improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linting/checkers/modified_listener.py` & `edulint-2.6.2/edulint/linting/checkers/modified_listener.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linting/checkers/python_ta_checkers.py` & `edulint-2.6.2/edulint/linting/checkers/python_ta_checkers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linting/checkers/short_problems.py` & `edulint-2.6.2/edulint/linting/checkers/short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linting/checkers/simplifiable_if.py` & `edulint-2.6.2/edulint/linting/checkers/simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linting/checkers/utils.py` & `edulint-2.6.2/edulint/linting/checkers/utils.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linting/linting.py` & `edulint-2.6.2/edulint/linting/linting.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linting/overrides.py` & `edulint-2.6.2/edulint/linting/overrides.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linting/problem.py` & `edulint-2.6.2/edulint/linting/problem.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linting/process_handler.py` & `edulint-2.6.2/edulint/linting/process_handler.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/linting/tweakers.py` & `edulint-2.6.2/edulint/linting/tweakers.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,22 @@
 def invalid_name_keep(self: Tweaker, problem: Problem, args: List[ImmutableArg]) -> bool:
     match = self.match(problem)
     if match.group(1).lower() == "module":
         return False
 
     name = match.group(2)
     style = match.group(3)
-    return style != "snake_case naming style" \
-        or any(ch1.islower() and ch2.isupper() for ch1, ch2 in zip(name, name[1:]))
+
+    if style == "snake_case naming style":
+        return name[0].isupper() or any(ch1.islower() and ch2.isupper() for ch1, ch2 in zip(name, name[1:]))
+
+    if style == "PascalCase naming style":
+        return name[0].islower() or "_" in name
+
+    return True
 
 
 def disallowed_name_keep(self: Tweaker, problem: Problem, args: List[ImmutableArg]) -> bool:
     if len(args) == 1 and args[0].option == Option.ALLOWED_ONECHAR_NAMES and args[0].val is not None:
         assert isinstance(args[0].val, str)
         allowed_onechar_names = args[0].val
     else:
```

### Comparing `edulint-2.6.1/edulint/options.py` & `edulint-2.6.2/edulint/options.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/prepare_explanations/__init__.py` & `edulint-2.6.2/edulint/prepare_explanations/__init__.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py` & `edulint-2.6.2/edulint/prepare_explanations/pylint_data/extract_from_pylint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/prepare_explanations/pylint_data/pylint_messages.py` & `edulint-2.6.2/edulint/prepare_explanations/pylint_data/pylint_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py` & `edulint-2.6.2/edulint/prepare_explanations/pylint_data/thonny_process_slim.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py` & `edulint-2.6.2/edulint/prepare_explanations/thonny_data/extract_from_edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/prepare_explanations/thonny_data/thonny_messages.py` & `edulint-2.6.2/edulint/prepare_explanations/thonny_data/thonny_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py` & `edulint-2.6.2/edulint/prepare_explanations/thonny_data/thonny_process_backup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/edulint.egg-info/SOURCES.txt` & `edulint-2.6.2/edulint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/setup.cfg` & `edulint-2.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/setup.py` & `edulint-2.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/tests/test_config.py` & `edulint-2.6.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/tests/test_improper_loop.py` & `edulint-2.6.2/tests/test_improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/tests/test_lint.py` & `edulint-2.6.2/tests/test_lint.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,110 @@
             lazy_problem().set_code("R1714").set_line(2),
         ])
     ])
     def test_ib111_week_custom(self, lines: List[str], args: List[Arg], expected_output: List[Problem]) -> None:
         create_apply_and_lint(lines, args, expected_output)
 
 
+@pytest.mark.parametrize("lines,expected_output", [
+    ([
+        "class A:",
+        "    pass"
+    ], []),
+    ([
+        "class _:",
+        "    pass"
+    ], []),
+    ([
+        "class a:",
+        "    pass"
+    ], [lazy_problem().set_line(1)]),
+    ([
+        "class class_name:",
+        "    pass"
+    ], [lazy_problem().set_line(1)]),
+    ([
+        "class CLASS_NAME:",
+        "    pass"
+    ], [lazy_problem().set_line(1)]),
+    ([
+        "def fun():",
+        "    a = 5"
+    ], []),
+    ([
+        "def fun():",
+        "    local_variable = 5"
+    ], []),
+    ([
+        "def fun():",
+        "    _ = 5"
+    ], []),
+    ([
+        "def fun():",
+        "    A = 5"
+    ], [lazy_problem().set_line(2)]),
+    ([
+        "def fun():",
+        "    LOCAL_VARIABLE = 5"
+    ], [lazy_problem().set_line(2)]),
+    ([
+        "def fun():",
+        "    localVariable = 5"
+    ], [lazy_problem().set_line(2)]),
+    ([
+        "def f():",
+        "    pass"
+    ], []),
+    ([
+        "def just_fun():",
+        "    pass"
+    ], []),
+    ([
+        "def _():",
+        "    pass"
+    ], []),
+    ([
+        "def F():",
+        "    pass"
+    ], [lazy_problem().set_line(1)]),
+    ([
+        "def JUST_FUN():",
+        "    pass"
+    ], [lazy_problem().set_line(1)]),
+    ([
+        "def JustFun():",
+        "    pass"
+    ], [lazy_problem().set_line(1)]),
+    ([
+        "A = 5"
+    ], []),
+    ([
+        "GLOBAL_VARIABLE = 1"
+    ], []),
+    ([
+        "TypeAlias = int"
+    ], []),
+    ([
+        "_ = int"
+    ], []),
+    ([
+        "a = 1"
+    ], [lazy_problem().set_line(1)]),
+    ([
+        "global_variable = 1"
+    ], [lazy_problem().set_line(1)]),
+])
+def test_invalid_name_custom(lines: List[str], expected_output: List[Problem]) -> None:
+    create_apply_and_lint(
+        lines,
+        [Arg(Option.PYLINT, "--disable=all"), Arg(Option.PYLINT, "--enable=invalid-name"), Arg(Option.NO_FLAKE8, "on")],
+        expected_output
+    )
+
+
 @pytest.mark.parametrize("filename,args,expected_output", [
     ("014186-p2_nested.py", [Arg(Option.PYTHON_SPECIFIC, "on")], [
         lazy_problem().set_code("C0103").set_line(20),
         lazy_problem().set_code("C0103").set_line(21),
         lazy_problem().set_code("C0103").set_line(27),
         lazy_problem().set_code("C0103").set_line(28),
         lazy_problem().set_code("C0103").set_line(31),
```

### Comparing `edulint-2.6.1/tests/test_main.py` & `edulint-2.6.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/tests/test_short_problems.py` & `edulint-2.6.2/tests/test_short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/tests/test_simplifiable_if.py` & `edulint-2.6.2/tests/test_simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.6.1/tests/test_visitors.py` & `edulint-2.6.2/tests/test_visitors.py`

 * *Files identical despite different names*

