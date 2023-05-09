# Comparing `tmp/zerobug-2.0.5.tar.gz` & `tmp/zerobug-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerobug-2.0.5.tar", last modified: Fri Apr 14 17:10:53 2023, max compression
+gzip compressed data, was "dist/zerobug-2.0.6.tar", last modified: Tue May  9 17:26:34 2023, max compression
```

## Comparing `zerobug-2.0.5.tar` & `zerobug-2.0.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.575899 zerobug-2.0.5/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2595 2023-04-14 17:10:53.575899 zerobug-2.0.5/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15608 2023-04-14 17:10:52.000000 zerobug-2.0.5/README.rst
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-14 17:10:53.575899 zerobug-2.0.5/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4102 2023-04-14 14:00:54.000000 zerobug-2.0.5/setup.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.565065 zerobug-2.0.5/zerobug/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      157 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/__main__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.575899 zerobug-2.0.5/zerobug/_travis/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1361 2023-01-27 07:10:19.000000 zerobug-2.0.5/zerobug/_travis/build_cmd
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.575899 zerobug-2.0.5/zerobug/_travis/cfg/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1126 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/coveragerc
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      690 2023-01-30 07:04:22.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      629 2023-01-30 06:58:04.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      533 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      534 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_beta.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      704 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      703 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      716 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_pr.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      122 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_shellcheck.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      152 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_shellcheck_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      132 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/_travis/cfg/travis_run_shellcheck_REDUCED.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1852 2023-04-14 14:02:41.000000 zerobug-2.0.5/zerobug/_travis/travis_after_tests_success
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    24300 2023-04-14 17:05:13.000000 zerobug-2.0.5/zerobug/_travis/travis_install_env
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    18750 2023-04-14 17:05:20.000000 zerobug-2.0.5/zerobug/_travis/travis_run_pypi_tests
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.575899 zerobug-2.0.5/zerobug/dummy/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)       47 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/dummy/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      121 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/dummy/dummylib.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.575899 zerobug-2.0.5/zerobug/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 zerobug-2.0.5/zerobug/scripts/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6398 2023-03-25 14:33:14.000000 zerobug-2.0.5/zerobug/scripts/main.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4102 2023-04-14 17:09:00.000000 zerobug-2.0.5/zerobug/scripts/setup.info
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    63946 2023-04-12 10:17:51.000000 zerobug-2.0.5/zerobug/z0testlib.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    23939 2023-03-25 14:33:10.000000 zerobug-2.0.5/zerobug/z0testrc
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      625 2023-03-25 14:33:05.000000 zerobug-2.0.5/zerobug/zerobug.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:10:53.575899 zerobug-2.0.5/zerobug.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2595 2023-04-14 17:10:53.000000 zerobug-2.0.5/zerobug.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1946 2023-04-14 17:10:53.000000 zerobug-2.0.5/zerobug.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-14 17:10:53.000000 zerobug-2.0.5/zerobug.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       91 2023-04-14 17:10:53.000000 zerobug-2.0.5/zerobug.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-09 06:43:26.000000 zerobug-2.0.5/zerobug.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       63 2023-04-14 17:10:53.000000 zerobug-2.0.5/zerobug.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        8 2023-04-14 17:10:53.000000 zerobug-2.0.5/zerobug.egg-info/top_level.txt
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/__main__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    23850 2023-05-09 16:09:43.000000 zerobug-2.0.6/zerobug/z0testrc
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug/dummy/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      121 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/dummy/dummylib.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)       47 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/dummy/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4102 2023-05-09 17:24:33.000000 zerobug-2.0.6/zerobug/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-05-09 16:09:43.000000 zerobug-2.0.6/zerobug/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/scripts/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug/_travis/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1852 2023-04-14 14:02:41.000000 zerobug-2.0.6/zerobug/_travis/travis_after_tests_success
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    18626 2023-05-09 16:09:43.000000 zerobug-2.0.6/zerobug/_travis/travis_run_pypi_tests
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug/_travis/cfg/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_pr.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      534 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1126 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/coveragerc
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      716 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      122 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_shellcheck.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      703 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      690 2023-01-30 07:04:22.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      132 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_shellcheck_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      629 2023-01-30 06:58:04.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      152 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_shellcheck_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      533 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      704 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_beta.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    24221 2023-05-09 16:09:43.000000 zerobug-2.0.6/zerobug/_travis/travis_install_env
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1361 2023-01-27 07:10:19.000000 zerobug-2.0.6/zerobug/_travis/build_cmd
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/_travis/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    63945 2023-05-09 16:09:43.000000 zerobug-2.0.6/zerobug/z0testlib.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      574 2023-05-09 16:09:43.000000 zerobug-2.0.6/zerobug/zerobug.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      157 2022-12-09 05:08:44.000000 zerobug-2.0.6/zerobug/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        8 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-09 06:43:26.000000 zerobug-2.0.6/zerobug.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       91 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1946 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       70 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2870 2023-05-09 17:26:34.000000 zerobug-2.0.6/zerobug.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-09 17:26:34.000000 zerobug-2.0.6/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4102 2023-05-09 16:09:43.000000 zerobug-2.0.6/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2870 2023-05-09 17:26:34.000000 zerobug-2.0.6/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15748 2023-05-09 17:26:33.000000 zerobug-2.0.6/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `zerobug-2.0.5/PKG-INFO` & `zerobug-2.0.6/zerobug.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,58 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: zerobug
-Version: 2.0.5
+Version: 2.0.6
 Summary: Zeroincombenze continuous testing framework and tools for python and bash programs
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
 Project-URL: Source, https://github.com/zeroincombenze/tools
+Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
+Description: 
+        This library can run unit test of target package software.
+        Supported languages are python (through z0testlib.py) and bash (through z0testrc)
+        
+        zerobug supports test automation, aggregation of tests into collections
+        and independence of the tests from the reporting framework.
+        The zerobug module provides all code that make it easy to support testing
+        both for python programs both for bash scripts.
+        zerobug shows execution test with a message like "n/tot message"
+        where n is current unit test and tot is the total unit test to execute,
+        that is a sort of advancing test progress.
+        
+        You can use z0bug_odoo that is the odoo integration to test Odoo modules.
+        
+        zerobug is built on follow concepts:
+        
+        * test main - it is a main program to executes all test runners
+        * test runner - it is a program to executes one or more test suites
+        * test suite - it is a collection of test cases
+        * test case - it is a smallest unit test
+        
+        The main file is the command zerobug of this package; it searches for test runner files
+        named `[id_]test_` where 'id' is the shor name of testing package.
+        
+        Test suite is a collection of test case named `test_[0-9]+` inside the runner file,
+        executed in sorted order.
+        
+        Every suit can contains one or more test case, the smallest unit test;
+        every unit test terminates with success or with failure.
+        
+        Because zerobug can show total number of unit test to execute, it runs tests
+        in 2 passes. In the first pass it counts the number of test, in second pass executes really
+        it. This behavior can be overridden by -0 switch.
+        
 Keywords: bash,optargs
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
-
-
-This library can run unit test of target package software.
-Supported languages are python (through z0testlib.py) and bash (through z0testrc)
-
-zerobug supports test automation, aggregation of tests into collections
-and independence of the tests from the reporting framework.
-The zerobug module provides all code that make it easy to support testing
-both for python programs both for bash scripts.
-zerobug shows execution test with a message like "n/tot message"
-where n is current unit test and tot is the total unit test to execute,
-that is a sort of advancing test progress.
-
-You can use z0bug_odoo that is the odoo integration to test Odoo modules.
-
-zerobug is built on follow concepts:
-
-* test main - it is a main program to executes all test runners
-* test runner - it is a program to executes one or more test suites
-* test suite - it is a collection of test cases
-* test case - it is a smallest unit test
-
-The main file is the command zerobug of this package; it searches for test runner files
-named `[id_]test_` where 'id' is the shor name of testing package.
-
-Test suite is a collection of test case named `test_[0-9]+` inside the runner file,
-executed in sorted order.
-
-Every suit can contains one or more test case, the smallest unit test;
-every unit test terminates with success or with failure.
-
-Because zerobug can show total number of unit test to execute, it runs tests
-in 2 passes. In the first pass it counts the number of test, in second pass executes really
-it. This behavior can be overridden by -0 switch.
-
-
```

### Comparing `zerobug-2.0.5/README.rst` & `zerobug-2.0.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 =============
-zerobug 2.0.5
+zerobug 2.0.6
 =============
 
 
 
 |Maturity| |Build Status| |Coverage Status| |license gpl|
 
 
@@ -362,20 +362,27 @@
     ./install_tools.sh -Ud
     source /opt/odoo/devel/activate_tools
 
 
 History
 -------
 
+2.0.6 (2023-05-08)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] Now all_tests is ignored
+* [IMP] Build Odoo environment for Odoo 16.0
+
 2.0.5 (2023-03-24)
 ~~~~~~~~~~~~~~~~~~
 
 * [FIX] travis_install_env: ensure list_requirements is executable
 * [IMP] flake8 configuration
-* [IMP] coveralls and codecov are not more dependenciesple  
+* [IMP] coveralls and codecov are not more dependencies
+* [IMP] Test for Odoo 16.0
 
 2.0.4 (2022-12-08)
 ~~~~~~~~~~~~~~~~~~
 
 * [FIX] run_pypi_test: best recognition of python version
 * [FIX] build_cmd: best recognition of python version
 * [FIX] travis_install_env: ensure coverage version
@@ -447,15 +454,15 @@
 
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2023-04-14
+Last Update / Ultimo aggiornamento: 2023-05-09
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
 .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
     :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
```

### Comparing `zerobug-2.0.5/setup.py` & `zerobug-2.0.6/zerobug/scripts/setup.info`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             'os0',
             'z0lib',
         ],
     )
 
 setup(
     name='zerobug',
-    version='2.0.5',
+    version='2.0.6',
     description='Zeroincombenze continuous testing framework'
     ' and tools for python and bash programs',
     long_description="""
 This library can run unit test of target package software.
 Supported languages are python (through z0testlib.py) and bash (through z0testrc)
 
 zerobug supports test automation, aggregation of tests into collections
```

### Comparing `zerobug-2.0.5/zerobug/_travis/build_cmd` & `zerobug-2.0.6/zerobug/_travis/build_cmd`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/coveragerc` & `zerobug-2.0.6/zerobug/_travis/cfg/coveragerc`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_AVERAGE.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_NEARBY.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_flake8__init__REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_61.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_61.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_70.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_70.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_PYPI.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_beta.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_beta.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_61.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_70.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_exclude_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/cfg/travis_run_pylint_pr.cfg` & `zerobug-2.0.6/zerobug/_travis/cfg/travis_run_pylint_pr.cfg`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/travis_after_tests_success` & `zerobug-2.0.6/zerobug/_travis/travis_after_tests_success`

 * *Files identical despite different names*

### Comparing `zerobug-2.0.5/zerobug/_travis/travis_install_env` & `zerobug-2.0.6/zerobug/_travis/travis_install_env`

 * *Files 1% similar despite different names*

```diff
@@ -29,26 +29,24 @@
 [[ -z "$Z0LIBDIR" ]] && echo "Library file z0librc not found in <$PYPATH>!" && exit 72
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "Z0LIBDIR=$Z0LIBDIR"
 TESTDIR=$(findpkg "" "$TDIR . .." "tests")
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "TESTDIR=$TESTDIR"
 RUNDIR=$(readlink -e $TESTDIR/..)
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "RUNDIR=$RUNDIR"
 
-# DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
-# TCONF="$HOME/.z0tools.conf"
 CFG_init "ALL"
 link_cfg_def
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.5
+__version__=2.0.6
 
 
 run_traced() {
   [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x
   [[ -z ${Z0_STACK:+_} ]] && export Z0_STACK=0
   ((Z0_STACK=Z0_STACK+2))
   local xcmd="$1" lm="                    "
```

### Comparing `zerobug-2.0.5/zerobug/_travis/travis_run_pypi_tests` & `zerobug-2.0.6/zerobug/_travis/travis_run_pypi_tests`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # Run test in travis environment
 # This script is default script to run syntax and regression tests
 # Should be replaced by OCA maintainer-quality-tools os something like it!
 #
 # This free software is released under GNU Affero GPL3
 # author: Antonio M. Vigliotti - antoniomaria.vigliotti@gmail.com
-# (C) 2015-2022 by SHS-AV s.r.l. - http://www.shs-av.com - info@shs-av.com
+# (C) 2015-2023 by SHS-AV s.r.l. - http://www.shs-av.com - info@shs-av.com
 #
 READLINK=$(which greadlink 2>/dev/null) || READLINK=$(which readlink 2>/dev/null)
 export READLINK
 # Based on template 2.0.0
 THIS=$(basename "$0")
 TDIR=$(readlink -f $(dirname $0))
 [ $BASH_VERSINFO -lt 4 ] && echo "This script $0 requires bash 4.0+!" && exit 4
@@ -31,26 +31,24 @@
 [[ -z "$Z0LIBDIR" ]] && echo "Library file z0librc not found in <$PYPATH>!" && exit 72
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "Z0LIBDIR=$Z0LIBDIR"
 TRAVISLIBDIR=$(findpkg travisrc "$PYPATH" "travis_emulator")
 [[ -z "$TRAVISLIBDIR" ]] && echo "Library file travisrc not found!" && exit 72
 . $TRAVISLIBDIR
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "TRAVISLIBDIR=$TRAVISLIBDIR"
 
-# DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
-# TCONF="$HOME/.z0tools.conf"
 CFG_init "ALL"
 link_cfg_def
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.5
+__version__=2.0.6
 
 
 travis_test_bash() {
     echo "======== Testing test_bash   ========"
     local s sts
     sts=0
     if [ ${opt_dry_run:-0} -eq 0 ]; then
@@ -218,30 +216,29 @@
     local s sts
     sts=0
     if [ ${opt_dry_run:-0} -eq 0 ]; then
         [[ $TRAVIS_PDB == "true" ]] && opts="${opts}B"
         [[ $TRAVIS_DEBUG_MODE =~ [89] ]] && opts="${opts}n"
         OPTS=$(inherits_travis_opts "$opts" "T")
         coverage_set
-        # coverage_ensure_installed
-        if [[ -f ./tests/all_tests.py ]]; then
-            if [[ ${opt_dprj:-0} -gt 0 ]]; then
-                run_traced "cd $PRJPATH; DEV_ENVIRONMENT=$PRJNAME coverage run -a --rcfile $COVERAGE_PROCESS_START ./tests/all_tests.py $OPTS"
-            else
-                run_traced "cd $PRJPATH/tests; DEV_ENVIRONMENT=$PRJNAME coverage run -a --rcfile $COVERAGE_PROCESS_START all_tests.py $OPTS"
-            fi
-            s=$?; [ ${s-1} -eq 0 -o $sts -ne 0 ] || sts=$s
-        elif [[ -f ./tests/all_tests && ${opt_pyth:-0} -eq 0 ]]; then
-            if [ ${opt_dprj:-0} -gt 0 ]; then
-                run_traced "$PRJPATH/tests/all_tests $OPTS"
-            else
-                run_traced "cd $PRJPATH/tests; ./all_tests $OPTS"
-            fi
-            s=$?; [ ${s-1} -eq 0 -o $sts -ne 0 ] || sts=$s
-        elif [[ -f ./tests/test_$PRJNAME.py ]]; then
+#        if [[ -f ./tests/all_tests.py ]]; then
+#            if [[ ${opt_dprj:-0} -gt 0 ]]; then
+#                run_traced "cd $PRJPATH; DEV_ENVIRONMENT=$PRJNAME coverage run -a --rcfile $COVERAGE_PROCESS_START ./tests/all_tests.py $OPTS"
+#            else
+#                run_traced "cd $PRJPATH/tests; DEV_ENVIRONMENT=$PRJNAME coverage run -a --rcfile $COVERAGE_PROCESS_START all_tests.py $OPTS"
+#            fi
+#            s=$?; [ ${s-1} -eq 0 -o $sts -ne 0 ] || sts=$s
+#        elif [[ -f ./tests/all_tests && ${opt_pyth:-0} -eq 0 ]]; then
+#            if [ ${opt_dprj:-0} -gt 0 ]; then
+#                run_traced "$PRJPATH/tests/all_tests $OPTS"
+#            else
+#                run_traced "cd $PRJPATH/tests; ./all_tests $OPTS"
+#            fi
+#            s=$?; [ ${s-1} -eq 0 -o $sts -ne 0 ] || sts=$s
+        if [[ -f ./tests/test_$PRJNAME.py ]]; then
             if [ ${opt_dprj:-0} -gt 0 ]; then
                 run_traced "cd $PRJPATH; DEV_ENVIRONMENT=$PRJNAME coverage run -a --rcfile $COVERAGE_PROCESS_START ./tests/test_$PRJNAME.py $OPTS"
             else
                 run_traced "cd $PRJPATH/tests; DEV_ENVIRONMENT=$PRJNAME coverage run -a --rcfile $COVERAGE_PROCESS_START test_$PRJNAME.py $OPTS"
             fi
             s=$?; [ ${s-1} -eq 0 -o $sts -ne 0 ] || sts=$s
         else
@@ -370,28 +367,27 @@
 parseoptargs "$@"
 if [[ "$opt_version" ]]; then
     echo "$__version__"
     exit 0
 fi
 if [[ $opt_help -gt 0 ]]; then
     print_help "Run test in travis environment" \
-               "(C) 2015-2022 by zeroincombenze(R)\nhttp://wiki.zeroincombenze.org/en/Linux/dev\nAuthor: antoniomaria.vigliotti@gmail.com"
+               "(C) 2015-2023 by zeroincombenze(R)\nhttp://wiki.zeroincombenze.org/en/Linux/dev\nAuthor: antoniomaria.vigliotti@gmail.com"
     exit 0
 fi
 
 [ "${MQT_DRY_RUN:-0}" == "1" ] && opt_dry_run=1
 [ "${MQT_VERBOSE_MODE:-0}" == "1" ] && opt_verbose=1
 [ "${MQT_VERBOSE_MODE:-1}" == "0" ] && opt_verbose=0
 [ ${TRAVIS_DEBUG_MODE:-0} -ne 0 ] && opt_verbose=1
 
 opts_travis
 conf_default
 [[ $opt_verbose -gt 2 ]] && set -x
 init_travis
-# prepare_env_travis
 prepare_env_travis
 
 sts=0
 if [ $test_mode -gt 0 ]; then
     do_chkconfig
     exit 0
 fi
```

### Comparing `zerobug-2.0.5/zerobug/scripts/main.py` & `zerobug-2.0.6/zerobug/scripts/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# template 20
+# template 21
 """
 Python supplemental features
 ----------------------------
 
 python_plus adds various features to python 2 and python 3 programs.
 It is designed to be used as integration of pypi future to help to port your code
 from Python 2 to Python 3 and still have it run on Python 2.
@@ -20,15 +20,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
@@ -104,20 +104,28 @@
                             else:
                                 fd.write(help_text)
                         if verbose:
                             print("$ gzip -c %s > %s" % (full_fn, tgt_fn))
                         continue
                     if lib_path:
                         tgt_fn = os.path.join(lib_path, base)
-                        try:
-                            shutil.copy(full_fn, tgt_fn)
-                            if verbose:
-                                print("$ cp %s %s" % (full_fn, tgt_fn))
-                        except shutil.SameFileError:
-                            pass
+                        if sys.version_info[0] == 3:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except shutil.SameFileError:
+                                pass
+                        else:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except BaseException:
+                                pass
                     # TODO> compatibility mode
                     tgt_fn = os.path.join(bin_path, base)
                     if os.path.isfile(tgt_fn):
                         os.unlink(tgt_fn)
                     if not os.path.exists(tgt_fn):
                         if verbose:
                             print("$ ln -s %s %s" % (full_fn, tgt_fn))
```

### Comparing `zerobug-2.0.5/zerobug/scripts/setup.info` & `zerobug-2.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             'os0',
             'z0lib',
         ],
     )
 
 setup(
     name='zerobug',
-    version='2.0.5',
+    version='2.0.6',
     description='Zeroincombenze continuous testing framework'
     ' and tools for python and bash programs',
     long_description="""
 This library can run unit test of target package software.
 Supported languages are python (through z0testlib.py) and bash (through z0testrc)
 
 zerobug supports test automation, aggregation of tests into collections
```

### Comparing `zerobug-2.0.5/zerobug/z0testlib.py` & `zerobug-2.0.6/zerobug/z0testlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from subprocess import PIPE, Popen
 
 import magic
 
 from os0 import os0
 from python_plus import _c
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 # return code
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 if os.name == "posix":
     RED = "\033[1;31m"
     GREEN = "\033[1;32m"
@@ -420,16 +420,16 @@
             del sys.path[ix]
         sys.path.insert(0, this_pkg_dir)
 
         if not id:
             if this.startswith('test_'):
                 id = this[5:]
             elif (
-                this.startswith('all_tests')
-                or this.startswith('zerobug')
+                # this.startswith('all_tests')
+                this.startswith('zerobug')
                 or this == '__main__'
             ):
                 id = os.path.basename(self.rundir)
             else:
                 id = this
             if id[-3:] >= '_00' and id[-3:] <= '_99':
                 id = id[0:-3]
```

### Comparing `zerobug-2.0.5/zerobug/z0testrc` & `zerobug-2.0.6/zerobug/z0testrc`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 #
 # Zeroincombenze® continuous testing framework and tools for bash scripts
 # This library can run unit test of target package software.
 # Use z0testlib.py for python programs.
 #
 # Package, test environment and deployment are:
 #   ./pkg                   $RUNDIR - Package directory (may be pypi packge or Odoo module);
-#   ./pkg/tests             $TESTDIR - Unit test directory (must contains one of 'all_tests' or 'test_PKG');
+#   ./pkg/tests             $TESTDIR - Unit test directory (must contains 'test_PKG');
 #   ./pkg/tests/z0testrc    $Z0TLIBDIR - This unit test bash script library; usually does not exist;
 #                           may be a real file (when is under test), or a link to ~/dev/z0testrc,
 #                           or a link to $PYTHONPATH/zerobug/z0testrc;
 #                           on github.com project must be a real file;
 # .../pkg/z0librc           $Z0LIBDIR - Local bash script library; usually does not exist
 #                           may be a real file (when is under test), or a link to ~/dev/z0librc,
 #                           usually it is /etc/z0librc;
 # .../pkg/_travis           $TRAVISDIR - Interface to travis emulator; usually is a link to ~/dev/_travis
 #                           on github.com become a directory with copies of travis interface files
 #                           in future, on github, could be become a test project for all packages.
 #
 # Unit test can run in package directory or in ./tests directory of package
-# Main unit test (all_tests script) calls sequentially all unit test scripts
 # Every unit test check for cmdline which is:
 # > unit_test [-hek][-l file][-Nnq][-s number][-Vv][-z number][-0]
 # where:
 # -h             this help
 # -b             run tests in debug mode
 # -e             enable echoing even if not interactive tty
 # -f             RESERVED TO --failfast (stop on first failure)
@@ -59,15 +58,15 @@
 # WLOGCMD:        oveerride opt_echo; may be None, 'echo', 'echo-1' or 'echo-0'
 #
 # This free software is released under GNU Affero GPL3
 # author: Antonio M. Vigliotti - antoniomaria.vigliotti@gmail.com
 # (C) 2015-2023 by SHS-AV s.r.l. - http://www.shs-av.com - info@shs-av.com
 #
 
-__version__=2.0.5
+__version__=2.0.6
 
 export opt_dry_run
 export ctr
 export opt_verbose
 export max_test
 export min_test
 export opt_noctr
@@ -373,16 +372,16 @@
 
 Z0BUG_init() {
     export teststs=0
     export Z0BUG_on_error=""
     export Z0BUG_run_autotest=0
     if [ "${THIS:0:5}" == "test_" ]; then
       module_id=${THIS:5}
-    elif [ "$THIS" == "all_tests" ]; then
-      module_id=$(basename $RUNDIR)
+    # elif [ "$THIS" == "all_tests" ]; then
+    #   module_id=$(basename $RUNDIR)
     else
       module_id=$THIS
     fi
     if [[ $module_id =~ _[0-9][0-9]$ ]]; then
       module_id=${module_id:0: -3}
     fi
     if [ "${module_id: -5}" == "_test" ]; then
@@ -705,15 +704,15 @@
     local odoo_home os_tree script h v w x y path
     local odoo_vid=$1
     local hy=$2
     x=$(echo $odoo_vid | grep --color=never -Eo "VENV[_-]([0-9]{3,10})?/?" | tail -n1)
     [[ -n $x ]] && x=$(echo $odoo_vid | grep --color=never -Eo "^.*$x")
     [[ -n $x ]] && w=${odoo_vid/$x/} || w=$odoo_vid
     [[ $odoo_vid =~ ^($HOME/)?VENV ]] && h="$odoo_vid/odoo" || h=$odoo_vid
-    v=$(echo $w|grep --color=never -Eo "(6|7|8|9|10|11|12|13|14)"|head -n1)
+    v=$(echo $w|grep --color=never -Eo "(6|7|8|9|10|11|12|13|14|15|16)"|head -n1)
     if [[ -n $v ]]; then
         [ $v -ge 10 ] && odoo_home="$h/odoo" || odoo_home="$h/openerp"
         [[ $hy == "tree" ]] && odoo_home="$odoo_vid/odoo/odoo"
         [[ $hy == "server" || $odoo_vid =~ (v6|v7) ]] && odoo_home="$odoo_vid/server/openerp"
         [ $v -ge 10 ] && script="odoo-bin" || script="openerp-server"
     else
         echo "Invalid Odoo odoo_version $odoo_vid!"
```

### Comparing `zerobug-2.0.5/zerobug/zerobug.py` & `zerobug-2.0.6/zerobug/zerobug.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2015-2023 SHS-AV s.r.l. (<http://www.zeroincombenze.org>)
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 """
     Zeroincombenze® unit test library for python programs Regression Test Suite
-    You can use this file as main all_tests.py too
 """
 import sys
 from . import z0test
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 def version():
     return __version__
 
 
 def main(cli_args=None):
```

### Comparing `zerobug-2.0.5/zerobug.egg-info/PKG-INFO` & `zerobug-2.0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,58 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: zerobug
-Version: 2.0.5
+Version: 2.0.6
 Summary: Zeroincombenze continuous testing framework and tools for python and bash programs
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
 Project-URL: Source, https://github.com/zeroincombenze/tools
+Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
+Description: 
+        This library can run unit test of target package software.
+        Supported languages are python (through z0testlib.py) and bash (through z0testrc)
+        
+        zerobug supports test automation, aggregation of tests into collections
+        and independence of the tests from the reporting framework.
+        The zerobug module provides all code that make it easy to support testing
+        both for python programs both for bash scripts.
+        zerobug shows execution test with a message like "n/tot message"
+        where n is current unit test and tot is the total unit test to execute,
+        that is a sort of advancing test progress.
+        
+        You can use z0bug_odoo that is the odoo integration to test Odoo modules.
+        
+        zerobug is built on follow concepts:
+        
+        * test main - it is a main program to executes all test runners
+        * test runner - it is a program to executes one or more test suites
+        * test suite - it is a collection of test cases
+        * test case - it is a smallest unit test
+        
+        The main file is the command zerobug of this package; it searches for test runner files
+        named `[id_]test_` where 'id' is the shor name of testing package.
+        
+        Test suite is a collection of test case named `test_[0-9]+` inside the runner file,
+        executed in sorted order.
+        
+        Every suit can contains one or more test case, the smallest unit test;
+        every unit test terminates with success or with failure.
+        
+        Because zerobug can show total number of unit test to execute, it runs tests
+        in 2 passes. In the first pass it counts the number of test, in second pass executes really
+        it. This behavior can be overridden by -0 switch.
+        
 Keywords: bash,optargs
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
-
-
-This library can run unit test of target package software.
-Supported languages are python (through z0testlib.py) and bash (through z0testrc)
-
-zerobug supports test automation, aggregation of tests into collections
-and independence of the tests from the reporting framework.
-The zerobug module provides all code that make it easy to support testing
-both for python programs both for bash scripts.
-zerobug shows execution test with a message like "n/tot message"
-where n is current unit test and tot is the total unit test to execute,
-that is a sort of advancing test progress.
-
-You can use z0bug_odoo that is the odoo integration to test Odoo modules.
-
-zerobug is built on follow concepts:
-
-* test main - it is a main program to executes all test runners
-* test runner - it is a program to executes one or more test suites
-* test suite - it is a collection of test cases
-* test case - it is a smallest unit test
-
-The main file is the command zerobug of this package; it searches for test runner files
-named `[id_]test_` where 'id' is the shor name of testing package.
-
-Test suite is a collection of test case named `test_[0-9]+` inside the runner file,
-executed in sorted order.
-
-Every suit can contains one or more test case, the smallest unit test;
-every unit test terminates with success or with failure.
-
-Because zerobug can show total number of unit test to execute, it runs tests
-in 2 passes. In the first pass it counts the number of test, in second pass executes really
-it. This behavior can be overridden by -0 switch.
-
-
```

### Comparing `zerobug-2.0.5/zerobug.egg-info/SOURCES.txt` & `zerobug-2.0.6/zerobug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

