# Comparing `tmp/pyncette-0.8.1.tar.gz` & `tmp/pyncette-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyncette-0.8.1.tar", last modified: Thu Apr  8 16:41:52 2021, max compression
+gzip compressed data, was "pyncette-0.9.0.tar", last modified: Sun Oct 17 18:41:47 2021, max compression
```

## Comparing `pyncette-0.8.1.tar` & `pyncette-0.9.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.527481 pyncette-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-04-08 16:41:41.000000 pyncette-0.8.1/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-04-08 16:41:41.000000 pyncette-0.8.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      217 2021-04-08 16:41:41.000000 pyncette-0.8.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-04-08 16:41:41.000000 pyncette-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-04-08 16:41:41.000000 pyncette-0.8.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2400 2021-04-08 16:41:41.000000 pyncette-0.8.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3084 2021-04-08 16:41:41.000000 pyncette-0.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2021-04-08 16:41:41.000000 pyncette-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      510 2021-04-08 16:41:41.000000 pyncette-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9645 2021-04-08 16:41:52.527481 pyncette-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5847 2021-04-08 16:41:41.000000 pyncette-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.519481 pyncette-0.8.1/ci/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2909 2021-04-08 16:41:41.000000 pyncette-0.8.1/ci/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-04-08 16:41:41.000000 pyncette-0.8.1/ci/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-04-08 16:41:41.000000 pyncette-0.8.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.519481 pyncette-0.8.1/docker/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2021-04-08 16:41:41.000000 pyncette-0.8.1/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)      644 2021-04-08 16:41:41.000000 pyncette-0.8.1/docker/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.519481 pyncette-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     3707 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4639 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/backends.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      567 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.523481 pyncette-0.8.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.dynamodb.rst
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.errors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.healthcheck.rst
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.model.rst
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.mysql.rst
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.postgres.rst
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.prometheus.rst
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.pyncette.rst
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.redis.rst
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.repository.rst
--rw-r--r--   0 runner    (1001) docker     (121)      471 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.rst
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.scheduler.rst
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.sqlite.rst
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.task.rst
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/reference/pyncette.utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14536 2021-04-08 16:41:41.000000 pyncette-0.8.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.523481 pyncette-0.8.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     4044 2021-04-08 16:41:41.000000 pyncette-0.8.1/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-04-08 16:41:41.000000 pyncette-0.8.1/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     5566 2021-04-08 16:41:41.000000 pyncette-0.8.1/examples/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.523481 pyncette-0.8.1/examples/data/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-04-08 16:41:41.000000 pyncette-0.8.1/examples/data/usernames.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2021-04-08 16:41:41.000000 pyncette-0.8.1/examples/delay_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2021-04-08 16:41:41.000000 pyncette-0.8.1/examples/dynamic_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2021-04-08 16:41:41.000000 pyncette-0.8.1/examples/fixtures_and_middlewares.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2021-04-08 16:41:41.000000 pyncette-0.8.1/examples/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2021-04-08 16:41:41.000000 pyncette-0.8.1/examples/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2886 2021-04-08 16:41:41.000000 pyncette-0.8.1/examples/persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)     2270 2021-04-08 16:41:41.000000 pyncette-0.8.1/examples/prometheus_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2021-04-08 16:41:52.527481 pyncette-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2896 2021-04-08 16:41:41.000000 pyncette-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.515481 pyncette-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.523481 pyncette-0.8.1/src/pyncette/
--rw-r--r--   0 runner    (1001) docker     (121)      269 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17560 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2226 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    13454 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)    11628 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/postgres.py
--rw-r--r--   0 runner    (1001) docker     (121)     8254 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    16330 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/pyncette.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.523481 pyncette-0.8.1/src/pyncette/redis/
--rw-r--r--   0 runner    (1001) docker     (121)    11312 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4540 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/redis/manage.lua
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/redis/poll_dynamic.lua
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/repository.py
--rw-r--r--   0 runner    (1001) docker     (121)    13962 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (121)     9982 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     2526 2021-04-08 16:41:41.000000 pyncette-0.8.1/src/pyncette/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.523481 pyncette-0.8.1/src/pyncette.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9645 2021-04-08 16:41:52.000000 pyncette-0.8.1/src/pyncette.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2021-04-08 16:41:52.000000 pyncette-0.8.1/src/pyncette.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-08 16:41:52.000000 pyncette-0.8.1/src/pyncette.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-08 16:41:52.000000 pyncette-0.8.1/src/pyncette.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      435 2021-04-08 16:41:52.000000 pyncette-0.8.1/src/pyncette.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-04-08 16:41:52.000000 pyncette-0.8.1/src/pyncette.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.527481 pyncette-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/test_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/test_mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (121)     7064 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/test_pyncette.py
--rw-r--r--   0 runner    (1001) docker     (121)     4491 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/test_pyncette_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)    43244 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/test_pyncette_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/test_pyncette_process.py
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/test_pyncette_prometheus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/test_redis.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/test_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 16:41:52.527481 pyncette-0.8.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/utils/fakerepository.py
--rw-r--r--   0 runner    (1001) docker     (121)     5494 2021-04-08 16:41:41.000000 pyncette-0.8.1/tests/utils/timemachine.py
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2021-04-08 16:41:41.000000 pyncette-0.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.565096 pyncette-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-10-17 18:41:36.000000 pyncette-0.9.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2021-10-17 18:41:36.000000 pyncette-0.9.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2021-10-17 18:41:36.000000 pyncette-0.9.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2021-10-17 18:41:36.000000 pyncette-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-10-17 18:41:36.000000 pyncette-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2400 2021-10-17 18:41:36.000000 pyncette-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3084 2021-10-17 18:41:36.000000 pyncette-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2021-10-17 18:41:36.000000 pyncette-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2021-10-17 18:41:36.000000 pyncette-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7943 2021-10-17 18:41:47.565096 pyncette-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5929 2021-10-17 18:41:36.000000 pyncette-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.553096 pyncette-0.9.0/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2909 2021-10-17 18:41:36.000000 pyncette-0.9.0/ci/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-10-17 18:41:36.000000 pyncette-0.9.0/ci/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2021-10-17 18:41:36.000000 pyncette-0.9.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.553096 pyncette-0.9.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2021-10-17 18:41:36.000000 pyncette-0.9.0/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2021-10-17 18:41:36.000000 pyncette-0.9.0/docker/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.557096 pyncette-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     3707 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4750 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/backends.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.557096 pyncette-0.9.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.dynamodb.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.errors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.healthcheck.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.model.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.mysql.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.postgres.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.prometheus.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.pyncette.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.redis.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.repository.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.scheduler.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.sqlite.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.task.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/reference/pyncette.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    14536 2021-10-17 18:41:36.000000 pyncette-0.9.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.561096 pyncette-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     4044 2021-10-17 18:41:36.000000 pyncette-0.9.0/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2021-10-17 18:41:36.000000 pyncette-0.9.0/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6302 2021-10-17 18:41:36.000000 pyncette-0.9.0/examples/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.561096 pyncette-0.9.0/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2021-10-17 18:41:36.000000 pyncette-0.9.0/examples/data/usernames.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2030 2021-10-17 18:41:36.000000 pyncette-0.9.0/examples/delay_queue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2034 2021-10-17 18:41:36.000000 pyncette-0.9.0/examples/dynamic_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1830 2021-10-17 18:41:36.000000 pyncette-0.9.0/examples/fixtures_and_middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2021-10-17 18:41:36.000000 pyncette-0.9.0/examples/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1629 2021-10-17 18:41:36.000000 pyncette-0.9.0/examples/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2886 2021-10-17 18:41:36.000000 pyncette-0.9.0/examples/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2270 2021-10-17 18:41:36.000000 pyncette-0.9.0/examples/prometheus_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      710 2021-10-17 18:41:47.569096 pyncette-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2947 2021-10-17 18:41:36.000000 pyncette-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.553096 pyncette-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.561096 pyncette-0.9.0/src/pyncette/
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17592 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2212 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2226 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2682 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13454 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11628 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8254 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    16330 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/pyncette.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.565096 pyncette-0.9.0/src/pyncette/redis/
+-rw-r--r--   0 runner    (1001) docker     (121)    11124 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4540 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/redis/manage.lua
+-rw-r--r--   0 runner    (1001) docker     (121)     1230 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/redis/poll_dynamic.lua
+-rw-r--r--   0 runner    (1001) docker     (121)     2168 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13962 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9982 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2526 2021-10-17 18:41:36.000000 pyncette-0.9.0/src/pyncette/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.561096 pyncette-0.9.0/src/pyncette.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7943 2021-10-17 18:41:47.000000 pyncette-0.9.0/src/pyncette.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2299 2021-10-17 18:41:47.000000 pyncette-0.9.0/src/pyncette.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-17 18:41:47.000000 pyncette-0.9.0/src/pyncette.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-17 18:41:47.000000 pyncette-0.9.0/src/pyncette.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2021-10-17 18:41:47.000000 pyncette-0.9.0/src/pyncette.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-17 18:41:47.000000 pyncette-0.9.0/src/pyncette.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.565096 pyncette-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     4396 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/test_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/test_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7064 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/test_pyncette.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4491 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/test_pyncette_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43244 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/test_pyncette_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1452 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/test_pyncette_process.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2298 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/test_pyncette_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/test_redis.py
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/test_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 18:41:47.565096 pyncette-0.9.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     2772 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/utils/fakerepository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5494 2021-10-17 18:41:36.000000 pyncette-0.9.0/tests/utils/timemachine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2025 2021-10-17 18:41:36.000000 pyncette-0.9.0/tox.ini
```

### Comparing `pyncette-0.8.1/CHANGELOG.rst` & `pyncette-0.9.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/CONTRIBUTING.rst` & `pyncette-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/LICENSE` & `pyncette-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/README.rst` & `pyncette-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/pyncette
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pyncette.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/pyncette
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/tibordp/pyncette/v0.8.1.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/tibordp/pyncette/v0.9.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/tibordp/pyncette/compare/v0.8.1...master
+    :target: https://github.com/tibordp/pyncette/compare/v0.9.0...master
 
 
 
 .. end-badges
 
 A reliable distributed scheduler with pluggable storage backends for Async Python.
 
@@ -142,15 +142,15 @@
 ==================
 
 Pyncette comes with an implementation for the following backends (used for persistence and coordination) out-of-the-box:
 
 - SQLite (included)
 - Redis (``pip install pyncette[redis]``)
 - PostgreSQL (``pip install pyncette[postgres]``)
-- MySQL 8.0+ (``pip install pyncette[mysql]``)
+- MySQL 8.0+ (``pip install pyncette[mysql]`` - [does not work on Python 3.10](https://github.com/aio-libs/aiomysql/issues/624))
 - Amazon DynamoDB (``pip install pyncette[dynamodb]``)
 
 Pyncette imposes few requirements on the underlying datastores, so it can be extended to support other databases or
 custom storage formats / integrations with existing systems. For best results, the backend needs to provide:
 
 - Some sort of serialization mechanism, e.g. traditional transactions, atomic stored procedures or compare-and-swap
 - Efficient range queries over a secondary index, which can be eventually consistent
```

### Comparing `pyncette-0.8.1/ci/bootstrap.py` & `pyncette-0.9.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/docker/entrypoint.py` & `pyncette-0.9.0/docker/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/docs/advanced_usage.rst` & `pyncette-0.9.0/docs/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/docs/backends.rst` & `pyncette-0.9.0/docs/backends.rst`

 * *Files 10% similar despite different names*

```diff
@@ -80,14 +80,16 @@
         mysql_user="pyncette",
         mysql_password="password",
         mysql_table_name='pyncette_tasks'
     )
 
 The table will be automatically initialized on startup if it does not exists unless ``mysql_skip_table_create`` is set to ``True``.
 
+.. caution:: MySQL backend currently does not work with Python 3.10 due to an issue with an upstream library.
+
 
 Amazon DynamoDB
 ---------------
 
 Amazon DynamoDB backend can be configured with :meth:`~pyncette.dynamodb.dynamodb_repository`. 
 
 .. code-block:: py
```

### Comparing `pyncette-0.8.1/docs/conf.py` & `pyncette-0.9.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "Pyncette"
 year = "2019"
 author = "Tibor Djurica Potpara"
 copyright = "{0}, {1}".format(year, author)
-version = release = "0.8.1"
+version = release = "0.9.0"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/tibordp/pyncette/issues/%s", "#"),
     "pr": ("https://github.com/tibordp/pyncette/pull/%s", "PR #"),
 }
```

### Comparing `pyncette-0.8.1/docs/installation.rst` & `pyncette-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/docs/usage.rst` & `pyncette-0.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/examples/README.md` & `pyncette-0.9.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/examples/benchmark.py` & `pyncette-0.9.0/examples/benchmark.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from multiprocessing import Process
 from multiprocessing.sharedctypes import RawValue  # type: ignore
 from typing import Any
 from typing import List
 from typing import Optional
 
 import coloredlogs
-import uvloop
 
 from pyncette import Context
 from pyncette import ExecutionMode
 from pyncette import Pyncette
 from pyncette.redis import redis_repository
 
 logger = logging.getLogger(__name__)
@@ -80,35 +79,52 @@
                 logger.info(f"Scheduled {i+1} tasks")
 
         await asyncio.gather(*tasks)
         logger.info("DONE!")
 
 
 async def run(
-    hit_count: RawValue,
-    staleness: RawValue,
+    hit_count: Any,
+    staleness: Any,
     enabled_partitions: Optional[List[int]],
 ) -> None:
 
     async with app.create() as app_context:
         app_context.add_to_context("hit_count", hit_count)
         app_context.add_to_context("staleness", staleness)
         benchmark_task.enabled_partitions = enabled_partitions
 
         logger.info(f"Starting to poll following partitions {enabled_partitions}")
         await app_context.run()
 
 
-def _run(*args: Any, **kwargs: Any) -> None:
+def _run(log_level: str, *args: Any, **kwargs: Any) -> None:
+    # On Windows we need to setup logging again as forking is not supported
+    setup(log_level)
     asyncio.run(run(*args, **kwargs))
 
 
+def setup(log_level: str) -> None:
+    # Make sure that this module logger always logs no matter what
+    # the selected level is.
+    coloredlogs.install(level="DEBUG", milliseconds=True)
+    logging.getLogger().setLevel(log_level)
+    logger.setLevel("INFO")
+
+    try:
+        import uvloop
+
+        uvloop.install()
+    except ImportError:
+        logger.info("uvloop is not available, ignoring.")
+
+
 async def report(
-    hit_counts: List[RawValue],
-    stalenesses: List[RawValue],
+    hit_counts: List[Any],
+    stalenesses: List[Any],
 ) -> None:
     previous_hit_count = 0
     previous_sample = time.perf_counter()
 
     while True:
         await asyncio.sleep(5)
 
@@ -154,31 +170,40 @@
         "--partition-count",
         type=int,
         default=PARTITION_COUNT,
         help="How many partitions each process should poll",
     )
 
     options = parser.parse_args()
-    coloredlogs.install(level="INFO", milliseconds=True, logger=logger)
-    coloredlogs.install(level=options.log_level, milliseconds=True)
-    uvloop.install()
+    setup(options.log_level)
 
     if options.command == "run":
         hit_count = [RawValue("l", 0) for _ in range(options.processes)]
         staleness = [RawValue("f", 0) for _ in range(options.processes)]
 
+        if options.partition_count * options.processes < PARTITION_COUNT:
+            logger.warning(
+                f"partition_count * processes < {PARTITION_COUNT}. Not all partitions will be processed."
+            )
+
         for i in range(options.processes):
             enabled_partitions = sorted(
-                (i + j) % PARTITION_COUNT for j in range(options.partition_count)
+                (i * options.partition_count + j) % PARTITION_COUNT
+                for j in range(options.partition_count)
             )
 
             job = Process(
                 target=_run,
                 name=str(i),
-                args=(hit_count[i], staleness[i], list(enabled_partitions)),
+                args=(
+                    options.log_level,
+                    hit_count[i],
+                    staleness[i],
+                    list(enabled_partitions),
+                ),
             )
             job.start()
 
         asyncio.run(report(hit_count, staleness))
 
     elif options.command == "populate":
-        asyncio.run(populate(options.number, options.parallel))
+        asyncio.run(populate(options.number, options.parallelism))
```

### Comparing `pyncette-0.8.1/examples/delay_queue.py` & `pyncette-0.9.0/examples/delay_queue.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/examples/dynamic_tasks.py` & `pyncette-0.9.0/examples/dynamic_tasks.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/examples/fixtures_and_middlewares.py` & `pyncette-0.9.0/examples/fixtures_and_middlewares.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/examples/healthcheck.py` & `pyncette-0.9.0/examples/healthcheck.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/examples/heartbeat.py` & `pyncette-0.9.0/examples/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/examples/persistence.py` & `pyncette-0.9.0/examples/persistence.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/examples/prometheus_metrics.py` & `pyncette-0.9.0/examples/prometheus_metrics.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/setup.cfg` & `pyncette-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/setup.py` & `pyncette-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,25 +20,25 @@
     with io.open(
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 extras = {
-    "redis": ["aioredis>=1.3.1"],
-    "prometheus": ["prometheus_client>=0.8.0"],
-    "postgres": ["asyncpg>=0.20.1"],
-    "dynamodb": ["aioboto3>=8.3.0"],
+    "redis": ["aioredis>=2.0.0"],
+    "prometheus": ["prometheus_client>=0.11.0"],
+    "postgres": ["asyncpg>=0.24.0"],
+    "dynamodb": ["aioboto3>=9.2.2"],
     "mysql": ["aiomysql>=0.0.21", "cryptography>=3.4.7"],
-    "uvloop": ["uvloop>=0.15.2"],
+    "uvloop": ["uvloop>=0.16.0"],
 }
 
 setup(
     name="pyncette",
-    version="0.8.1",
+    version="0.9.0",
     license="MIT",
     description="A reliable distributed scheduler with pluggable storage backends",
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
@@ -61,32 +61,33 @@
         "Operating System :: Unix",
         "Operating System :: POSIX",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Utilities",
     ],
     project_urls={
         "Documentation": "https://pyncette.readthedocs.io/",
         "Changelog": "https://pyncette.readthedocs.io/en/latest/changelog.html",
         "Issue Tracker": "https://github.com/tibordp/pyncette/issues",
     },
     keywords=[
         # eg: 'keyword1', 'keyword2', 'keyword3',
     ],
     python_requires=">=3.7",
     install_requires=[
         "typing-extensions>=3.7.4.2",
-        "croniter>=0.3.34",
-        "aiosqlite>=0.13.0",
-        "aiohttp>=3.6.2",
-        "python-dateutil>=2.8.1",
+        "croniter>=1.0.15",
+        "aiosqlite>=0.17.0",
+        "aiohttp>=3.7.4",
+        "python-dateutil>=2.8.2",
         "coloredlogs",
     ],
     extras_require={
         **extras,
         # A convenience all extras
         "all": list(itertools.chain(*extras.values())),
     },
```

### Comparing `pyncette-0.8.1/src/pyncette/dynamodb.py` & `pyncette-0.9.0/src/pyncette/dynamodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,15 +444,16 @@
     dynamodb_endpoint: Optional[str] = None,
     dynamodb_region_name: Optional[str] = None,
     dynamodb_skip_table_create: bool = False,
     dynamodb_partition_prefix: str = "",
     **kwargs: Any,
 ) -> AsyncIterator[DynamoDBRepository]:
     """Factory context manager for Redis repository that initializes the connection to Redis"""
-    async with aioboto3.resource(
+    session = aioboto3.Session()
+    async with session.resource(
         "dynamodb",
         region_name=dynamodb_region_name,
         endpoint_url=dynamodb_endpoint,
     ) as dynamo_resource:
         repository = DynamoDBRepository(
             dynamo_resource,
             skip_table_create=dynamodb_skip_table_create,
```

### Comparing `pyncette-0.8.1/src/pyncette/executor.py` & `pyncette-0.9.0/src/pyncette/executor.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette/healthcheck.py` & `pyncette-0.9.0/src/pyncette/healthcheck.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette/model.py` & `pyncette-0.9.0/src/pyncette/model.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette/mysql.py` & `pyncette-0.9.0/src/pyncette/mysql.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette/postgres.py` & `pyncette-0.9.0/src/pyncette/postgres.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette/prometheus.py` & `pyncette-0.9.0/src/pyncette/prometheus.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette/pyncette.py` & `pyncette-0.9.0/src/pyncette/pyncette.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette/redis/__init__.py` & `pyncette-0.9.0/src/pyncette/redis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,21 +51,18 @@
         args: List[Any] = [],
     ) -> Any:
         if self._sha is None:
             await self.register(client)
 
         for _ in range(3):
             try:
-                return await client.evalsha(self._sha, keys=keys, args=args)
-            except aioredis.ReplyError as err:
-                if str(err).startswith("NOSCRIPT"):
-                    logger.warning("We seem to have lost the LUA script, reloading...")
-                    await self.register(client)
-                else:
-                    raise
+                return await client.evalsha(self._sha, len(keys), *keys, *args)
+            except aioredis.exceptions.NoScriptError:
+                logger.warning("We seem to have lost the LUA script, reloading...")
+                await self.register(client)
 
         raise PyncetteException("Could not reload the Lua script.")
 
 
 @dataclass
 class _ManageScriptResponse:
     result: ResultType
@@ -290,15 +287,11 @@
         index_name = f"index:{task.canonical_name}" if task else "index"
         return f"pyncette:{self._namespace}:{index_name}"
 
 
 @contextlib.asynccontextmanager
 async def redis_repository(**kwargs: Any) -> AsyncIterator[RedisRepository]:
     """Factory context manager for Redis repository that initializes the connection to Redis"""
-    redis_pool = await aioredis.create_redis_pool(kwargs["redis_url"])
-    try:
+    async with aioredis.from_url(kwargs["redis_url"]) as redis_pool:
         repository = RedisRepository(redis_pool, **kwargs)
         await repository.register_scripts()
         yield repository
-    finally:
-        redis_pool.close()
-        await redis_pool.wait_closed()
```

### Comparing `pyncette-0.8.1/src/pyncette/redis/manage.lua` & `pyncette-0.9.0/src/pyncette/redis/manage.lua`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette/redis/poll_dynamic.lua` & `pyncette-0.9.0/src/pyncette/redis/poll_dynamic.lua`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette/repository.py` & `pyncette-0.9.0/src/pyncette/repository.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette/sqlite.py` & `pyncette-0.9.0/src/pyncette/sqlite.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette/task.py` & `pyncette-0.9.0/src/pyncette/task.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette/utils.py` & `pyncette-0.9.0/src/pyncette/utils.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/src/pyncette.egg-info/SOURCES.txt` & `pyncette-0.9.0/src/pyncette.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/tests/conftest.py` & `pyncette-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/tests/test_dynamodb.py` & `pyncette-0.9.0/tests/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/tests/test_mysql.py` & `pyncette-0.9.0/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/tests/test_postgres.py` & `pyncette-0.9.0/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/tests/test_pyncette.py` & `pyncette-0.9.0/tests/test_pyncette.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/tests/test_pyncette_healthcheck.py` & `pyncette-0.9.0/tests/test_pyncette_healthcheck.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/tests/test_pyncette_integration.py` & `pyncette-0.9.0/tests/test_pyncette_integration.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/tests/test_pyncette_process.py` & `pyncette-0.9.0/tests/test_pyncette_process.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/tests/test_pyncette_prometheus.py` & `pyncette-0.9.0/tests/test_pyncette_prometheus.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/tests/test_redis.py` & `pyncette-0.9.0/tests/test_redis.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 
 @pytest.mark.asyncio
 @pytest.mark.integration
 async def test_script_reload(monkeypatch):
     monkeypatch.setattr(redis, "read_text", lambda *args: 'return { "SUCCESS" }')
 
     redis_url = os.environ.get("REDIS_URL", "redis://localhost")
-    redis_pool = await aioredis.create_redis_pool(redis_url)
+    redis_pool = aioredis.from_url(redis_url)
 
     lua_script = redis._LuaScript("dummy")
     result = await lua_script.register(redis_pool)
-    await redis_pool.execute("SCRIPT", "FLUSH", "SYNC")
+    await redis_pool.execute_command("SCRIPT", "FLUSH", "SYNC")
 
     result = await lua_script.execute(redis_pool, [], [])
 
     assert result == [b"SUCCESS"]
 
 
 @pytest.mark.asyncio
 @pytest.mark.integration
 async def test_script_register(monkeypatch):
     monkeypatch.setattr(redis, "read_text", lambda *args: 'return { "SUCCESS" }')
 
     redis_url = os.environ.get("REDIS_URL", "redis://localhost")
-    redis_pool = await aioredis.create_redis_pool(redis_url)
+    redis_pool = aioredis.from_url(redis_url)
 
     lua_script = redis._LuaScript("dummy")
     result = await lua_script.execute(redis_pool, [], [])
 
     assert result == [b"SUCCESS"]
```

### Comparing `pyncette-0.8.1/tests/utils/fakerepository.py` & `pyncette-0.9.0/tests/utils/fakerepository.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/tests/utils/timemachine.py` & `pyncette-0.9.0/tests/utils/timemachine.py`

 * *Files identical despite different names*

### Comparing `pyncette-0.8.1/tox.ini` & `pyncette-0.9.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,25 @@
     *
 
 [tox]
 envlist =
     clean,
     check,
     docs,
-    {py37,py38,py39},
+    {py37,py38,py39,py310},
     integration,
     report
 ignore_basepython_conflict = true
 
 [testenv]
 basepython =
     py37: {env:TOXPYTHON:python3.7}
     py38: {env:TOXPYTHON:python3.8}
     py39: {env:TOXPYTHON:python3.9}
+    py310: {env:TOXPYTHON:python3.10}
     {integration,docs}: {env:TOXPYTHON:python3}
     {bootstrap,clean,check,report,fmt}: {env:TOXPYTHON:python3}
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
@@ -55,14 +56,17 @@
     check-manifest
     black
     flake8
     readme-renderer
     pygments
     mypy
     isort
+    types-python-dateutil
+    types-croniter
+    types-PyMySQL
 skip_install = true
 commands =
     python setup.py check --strict --metadata --restructuredtext
     check-manifest {toxinidir}
     flake8 src tests examples setup.py
     mypy src examples
     isort --verbose --check-only --diff --recursive src tests examples setup.py
```

