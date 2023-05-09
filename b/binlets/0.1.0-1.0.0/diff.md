# Comparing `tmp/binlets-0.1.0.tar.gz` & `tmp/binlets-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/binlets-0.1.0.tar", last modified: Fri Jan  3 23:18:37 2020, max compression
+gzip compressed data, was "binlets-1.0.0.tar", last modified: Tue May  9 19:06:17 2023, max compression
```

## Comparing `binlets-0.1.0.tar` & `binlets-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,29 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2020-01-03 23:18:37.000000 binlets-0.1.0/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      254 2020-01-03 23:18:37.000000 binlets-0.1.0/PKG-INFO
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2020-01-03 23:18:37.000000 binlets-0.1.0/binlets/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       28 2019-12-06 19:47:04.000000 binlets-0.1.0/binlets/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5491 2020-01-03 23:00:44.000000 binlets-0.1.0/binlets/binlets.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3357 2020-01-03 23:06:07.000000 binlets-0.1.0/binlets/modwt.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      688 2019-10-31 16:43:07.000000 binlets-0.1.0/binlets/mra.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2020-01-03 23:18:37.000000 binlets-0.1.0/binlets.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      254 2020-01-03 23:18:37.000000 binlets-0.1.0/binlets.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      233 2020-01-03 23:18:37.000000 binlets-0.1.0/binlets.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2020-01-03 23:18:37.000000 binlets-0.1.0/binlets.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       18 2020-01-03 23:18:37.000000 binlets-0.1.0/binlets.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        8 2020-01-03 23:18:37.000000 binlets-0.1.0/binlets.egg-info/top_level.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       38 2020-01-03 23:18:37.000000 binlets-0.1.0/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      347 2020-01-03 23:08:33.000000 binlets-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:06:17.282701 binlets-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:06:17.278701 binlets-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:06:17.282701 binlets-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-09 19:06:04.000000 binlets-1.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-09 19:06:04.000000 binlets-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-09 19:06:04.000000 binlets-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-09 19:06:04.000000 binlets-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 19:06:04.000000 binlets-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-09 19:06:17.282701 binlets-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-09 19:06:04.000000 binlets-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-09 19:06:04.000000 binlets-1.0.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-09 19:06:04.000000 binlets-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 19:06:04.000000 binlets-1.0.0/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 19:06:04.000000 binlets-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:06:17.282701 binlets-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:06:17.278701 binlets-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:06:17.282701 binlets-1.0.0/src/binlets/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-09 19:06:04.000000 binlets-1.0.0/src/binlets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-09 19:06:04.000000 binlets-1.0.0/src/binlets/_binlets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-09 19:06:04.000000 binlets-1.0.0/src/binlets/_modwt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:06:17.282701 binlets-1.0.0/src/binlets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-09 19:06:04.000000 binlets-1.0.0/src/binlets/tests/test_binlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-09 19:06:04.000000 binlets-1.0.0/src/binlets/tests/test_modwt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:06:17.282701 binlets-1.0.0/src/binlets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-09 19:06:17.000000 binlets-1.0.0/src/binlets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-09 19:06:17.000000 binlets-1.0.0/src/binlets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:06:17.000000 binlets-1.0.0/src/binlets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-09 19:06:17.000000 binlets-1.0.0/src/binlets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 19:06:17.000000 binlets-1.0.0/src/binlets.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

