# Comparing `tmp/django-cacheops-7.0.tar.gz` & `tmp/django-cacheops-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cacheops-7.0.tar", last modified: Wed Mar 15 10:03:10 2023, max compression
+gzip compressed data, was "django-cacheops-7.0.1.tar", last modified: Tue May  9 07:49:47 2023, max compression
```

## Comparing `django-cacheops-7.0.tar` & `django-cacheops-7.0.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-03-15 10:03:10.339889 django-cacheops-7.0/
--rw-rw-r--   0 suor      (1000) suor      (1000)      193 2021-10-19 06:04:46.000000 django-cacheops-7.0/.editorconfig
-drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-03-15 10:03:10.336556 django-cacheops-7.0/.github/
-drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-03-15 10:03:10.336556 django-cacheops-7.0/.github/workflows/
--rw-r--r--   0 suor      (1000) suor      (1000)     1794 2023-02-27 04:56:43.000000 django-cacheops-7.0/.github/workflows/ci.yml
--rw-rw-r--   0 suor      (1000) suor      (1000)       58 2021-05-24 09:36:10.000000 django-cacheops-7.0/.gitignore
--rw-r--r--   0 suor      (1000) suor      (1000)    13175 2023-03-11 09:08:54.000000 django-cacheops-7.0/CHANGELOG
--rw-rw-r--   0 suor      (1000) suor      (1000)     1533 2021-05-24 09:36:10.000000 django-cacheops-7.0/LICENSE
--rw-rw-r--   0 suor      (1000) suor      (1000)      222 2021-05-24 09:36:10.000000 django-cacheops-7.0/MANIFEST.in
--rw-r--r--   0 suor      (1000) suor      (1000)    29839 2023-03-15 10:03:10.339889 django-cacheops-7.0/PKG-INFO
--rw-r--r--   0 suor      (1000) suor      (1000)    28675 2023-03-11 09:05:57.000000 django-cacheops-7.0/README.rst
--rwxr-xr-x   0 suor      (1000) suor      (1000)     2586 2023-02-25 05:58:23.000000 django-cacheops-7.0/bench.py
-drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-03-15 10:03:10.336556 django-cacheops-7.0/cacheops/
--rw-r--r--   0 suor      (1000) suor      (1000)      241 2023-03-11 09:09:11.000000 django-cacheops-7.0/cacheops/__init__.py
--rw-r--r--   0 suor      (1000) suor      (1000)      302 2023-03-11 09:02:51.000000 django-cacheops-7.0/cacheops/apps.py
--rw-r--r--   0 suor      (1000) suor      (1000)     3526 2023-02-25 05:59:13.000000 django-cacheops-7.0/cacheops/conf.py
--rw-r--r--   0 suor      (1000) suor      (1000)     4217 2023-02-25 05:59:13.000000 django-cacheops-7.0/cacheops/getset.py
--rw-r--r--   0 suor      (1000) suor      (1000)     4009 2023-02-25 05:58:23.000000 django-cacheops-7.0/cacheops/invalidation.py
--rw-rw-r--   0 suor      (1000) suor      (1000)     2292 2021-05-24 09:36:10.000000 django-cacheops-7.0/cacheops/jinja2.py
-drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-03-15 10:03:10.336556 django-cacheops-7.0/cacheops/lua/
--rw-r--r--   0 suor      (1000) suor      (1000)     1506 2023-02-25 05:59:13.000000 django-cacheops-7.0/cacheops/lua/cache_thing.lua
--rw-r--r--   0 suor      (1000) suor      (1000)     1342 2023-02-25 05:58:23.000000 django-cacheops-7.0/cacheops/lua/cache_thing_insideout.lua
--rw-rw-r--   0 suor      (1000) suor      (1000)     1320 2021-05-24 09:36:10.000000 django-cacheops-7.0/cacheops/lua/invalidate.lua
--rw-r--r--   0 suor      (1000) suor      (1000)      681 2023-02-25 05:58:23.000000 django-cacheops-7.0/cacheops/lua/invalidate_insideout.lua
-drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-03-15 10:03:10.336556 django-cacheops-7.0/cacheops/management/
--rw-r--r--   0 suor      (1000) suor      (1000)        0 2012-02-26 04:58:36.000000 django-cacheops-7.0/cacheops/management/__init__.py
-drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-03-15 10:03:10.336556 django-cacheops-7.0/cacheops/management/commands/
--rw-r--r--   0 suor      (1000) suor      (1000)        0 2012-02-26 04:58:36.000000 django-cacheops-7.0/cacheops/management/commands/__init__.py
--rw-r--r--   0 suor      (1000) suor      (1000)      503 2018-11-09 09:54:36.000000 django-cacheops-7.0/cacheops/management/commands/cleanfilecache.py
--rw-rw-r--   0 suor      (1000) suor      (1000)     1948 2021-05-24 09:36:10.000000 django-cacheops-7.0/cacheops/management/commands/invalidate.py
--rw-r--r--   0 suor      (1000) suor      (1000)      711 2023-02-19 10:39:40.000000 django-cacheops-7.0/cacheops/management/commands/reapconjs.py
--rw-r--r--   0 suor      (1000) suor      (1000)    24928 2023-03-11 09:02:52.000000 django-cacheops-7.0/cacheops/query.py
--rw-r--r--   0 suor      (1000) suor      (1000)     2421 2023-02-19 10:39:40.000000 django-cacheops-7.0/cacheops/reaper.py
--rw-r--r--   0 suor      (1000) suor      (1000)     2132 2023-02-25 05:59:13.000000 django-cacheops-7.0/cacheops/redis.py
--rw-rw-r--   0 suor      (1000) suor      (1000)      206 2021-05-24 09:36:10.000000 django-cacheops-7.0/cacheops/serializers.py
--rw-r--r--   0 suor      (1000) suor      (1000)     1223 2017-09-15 07:08:22.000000 django-cacheops-7.0/cacheops/sharding.py
--rw-rw-r--   0 suor      (1000) suor      (1000)      144 2021-05-24 09:36:10.000000 django-cacheops-7.0/cacheops/signals.py
--rw-rw-r--   0 suor      (1000) suor      (1000)     5442 2021-05-24 09:36:10.000000 django-cacheops-7.0/cacheops/simple.py
-drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-03-15 10:03:10.336556 django-cacheops-7.0/cacheops/templatetags/
--rw-r--r--   0 suor      (1000) suor      (1000)        0 2017-05-09 04:30:00.000000 django-cacheops-7.0/cacheops/templatetags/__init__.py
--rw-rw-r--   0 suor      (1000) suor      (1000)     2311 2021-05-24 09:36:10.000000 django-cacheops-7.0/cacheops/templatetags/cacheops.py
--rw-r--r--   0 suor      (1000) suor      (1000)     4142 2022-05-27 05:04:05.000000 django-cacheops-7.0/cacheops/transaction.py
--rw-r--r--   0 suor      (1000) suor      (1000)     6382 2023-02-27 03:51:13.000000 django-cacheops-7.0/cacheops/tree.py
--rw-r--r--   0 suor      (1000) suor      (1000)     4699 2023-03-02 14:50:46.000000 django-cacheops-7.0/cacheops/utils.py
-drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-03-15 10:03:10.336556 django-cacheops-7.0/django_cacheops.egg-info/
--rw-r--r--   0 suor      (1000) suor      (1000)    29839 2023-03-15 10:03:10.000000 django-cacheops-7.0/django_cacheops.egg-info/PKG-INFO
--rw-r--r--   0 suor      (1000) suor      (1000)     1379 2023-03-15 10:03:10.000000 django-cacheops-7.0/django_cacheops.egg-info/SOURCES.txt
--rw-r--r--   0 suor      (1000) suor      (1000)        1 2023-03-15 10:03:10.000000 django-cacheops-7.0/django_cacheops.egg-info/dependency_links.txt
--rw-r--r--   0 suor      (1000) suor      (1000)        1 2014-03-04 07:12:55.000000 django-cacheops-7.0/django_cacheops.egg-info/not-zip-safe
--rw-r--r--   0 suor      (1000) suor      (1000)       47 2016-02-03 05:07:05.000000 django-cacheops-7.0/django_cacheops.egg-info/pbr.json
--rw-r--r--   0 suor      (1000) suor      (1000)       41 2023-03-15 10:03:10.000000 django-cacheops-7.0/django_cacheops.egg-info/requires.txt
--rw-r--r--   0 suor      (1000) suor      (1000)        9 2023-03-15 10:03:10.000000 django-cacheops-7.0/django_cacheops.egg-info/top_level.txt
--rwxrwxr-x   0 suor      (1000) suor      (1000)      249 2021-05-24 09:36:10.000000 django-cacheops-7.0/manage.py
--rwxr-xr-x   0 suor      (1000) suor      (1000)      294 2023-02-22 09:39:41.000000 django-cacheops-7.0/publish.sh
--rw-r--r--   0 suor      (1000) suor      (1000)       97 2023-03-11 09:05:33.000000 django-cacheops-7.0/pytest.ini
--rw-r--r--   0 suor      (1000) suor      (1000)      114 2023-03-11 09:05:33.000000 django-cacheops-7.0/requirements-test.txt
--rw-r--r--   0 suor      (1000) suor      (1000)      102 2023-03-15 10:03:10.339889 django-cacheops-7.0/setup.cfg
--rw-r--r--   0 suor      (1000) suor      (1000)     1631 2023-03-11 09:09:49.000000 django-cacheops-7.0/setup.py
-drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-03-15 10:03:10.339889 django-cacheops-7.0/tests/
--rw-r--r--   0 suor      (1000) suor      (1000)        0 2023-03-02 14:44:38.000000 django-cacheops-7.0/tests/__init__.py
--rw-rw-r--   0 suor      (1000) suor      (1000)     5693 2021-05-24 09:36:10.000000 django-cacheops-7.0/tests/bench.py
-drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-03-15 10:03:10.339889 django-cacheops-7.0/tests/fixtures/
--rw-r--r--   0 suor      (1000) suor      (1000)     1202 2017-05-09 04:30:00.000000 django-cacheops-7.0/tests/fixtures/basic.json
--rw-r--r--   0 suor      (1000) suor      (1000)     8016 2023-03-11 09:02:54.000000 django-cacheops-7.0/tests/models.py
--rw-r--r--   0 suor      (1000) suor      (1000)     3600 2023-03-11 09:05:33.000000 django-cacheops-7.0/tests/settings.py
--rw-rw-r--   0 suor      (1000) suor      (1000)     5728 2021-05-24 09:36:10.000000 django-cacheops-7.0/tests/test_extras.py
--rw-r--r--   0 suor      (1000) suor      (1000)    38367 2023-02-27 04:15:02.000000 django-cacheops-7.0/tests/tests.py
--rw-rw-r--   0 suor      (1000) suor      (1000)     1874 2021-05-24 09:36:10.000000 django-cacheops-7.0/tests/tests_sharding.py
--rw-r--r--   0 suor      (1000) suor      (1000)     4553 2022-05-27 05:04:05.000000 django-cacheops-7.0/tests/tests_transactions.py
--rw-r--r--   0 suor      (1000) suor      (1000)       17 2017-05-09 04:30:00.000000 django-cacheops-7.0/tests/urls.py
--rw-r--r--   0 suor      (1000) suor      (1000)     1911 2023-02-19 10:39:40.000000 django-cacheops-7.0/tests/utils.py
--rw-r--r--   0 suor      (1000) suor      (1000)     1324 2023-03-11 09:05:33.000000 django-cacheops-7.0/tox.ini
+drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-05-09 07:49:47.681410 django-cacheops-7.0.1/
+-rw-rw-r--   0 suor      (1000) suor      (1000)      193 2021-10-19 06:04:46.000000 django-cacheops-7.0.1/.editorconfig
+drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-05-09 07:49:47.678077 django-cacheops-7.0.1/.github/
+drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-05-09 07:49:47.678077 django-cacheops-7.0.1/.github/workflows/
+-rw-r--r--   0 suor      (1000) suor      (1000)     1794 2023-02-27 04:56:43.000000 django-cacheops-7.0.1/.github/workflows/ci.yml
+-rw-rw-r--   0 suor      (1000) suor      (1000)       58 2021-05-24 09:36:10.000000 django-cacheops-7.0.1/.gitignore
+-rw-r--r--   0 suor      (1000) suor      (1000)    13345 2023-05-09 07:41:55.000000 django-cacheops-7.0.1/CHANGELOG
+-rw-rw-r--   0 suor      (1000) suor      (1000)     1533 2021-05-24 09:36:10.000000 django-cacheops-7.0.1/LICENSE
+-rw-rw-r--   0 suor      (1000) suor      (1000)      209 2023-03-16 06:31:03.000000 django-cacheops-7.0.1/MANIFEST.in
+-rw-r--r--   0 suor      (1000) suor      (1000)    29835 2023-05-09 07:49:47.681410 django-cacheops-7.0.1/PKG-INFO
+-rw-r--r--   0 suor      (1000) suor      (1000)    28669 2023-03-17 15:09:39.000000 django-cacheops-7.0.1/README.rst
+-rwxr-xr-x   0 suor      (1000) suor      (1000)     2586 2023-02-25 05:58:23.000000 django-cacheops-7.0.1/bench.py
+drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-05-09 07:49:47.678077 django-cacheops-7.0.1/cacheops/
+-rw-r--r--   0 suor      (1000) suor      (1000)      243 2023-05-09 07:42:08.000000 django-cacheops-7.0.1/cacheops/__init__.py
+-rw-r--r--   0 suor      (1000) suor      (1000)      302 2023-03-11 09:02:51.000000 django-cacheops-7.0.1/cacheops/apps.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     3594 2023-05-05 11:51:50.000000 django-cacheops-7.0.1/cacheops/conf.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     4217 2023-02-25 05:59:13.000000 django-cacheops-7.0.1/cacheops/getset.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     4009 2023-05-05 11:40:55.000000 django-cacheops-7.0.1/cacheops/invalidation.py
+-rw-rw-r--   0 suor      (1000) suor      (1000)     2292 2021-05-24 09:36:10.000000 django-cacheops-7.0.1/cacheops/jinja2.py
+drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-05-09 07:49:47.678077 django-cacheops-7.0.1/cacheops/lua/
+-rw-r--r--   0 suor      (1000) suor      (1000)     1888 2023-04-03 11:32:23.000000 django-cacheops-7.0.1/cacheops/lua/cache_thing.lua
+-rw-r--r--   0 suor      (1000) suor      (1000)     1684 2023-04-03 11:31:30.000000 django-cacheops-7.0.1/cacheops/lua/cache_thing_insideout.lua
+-rw-rw-r--   0 suor      (1000) suor      (1000)     1320 2021-05-24 09:36:10.000000 django-cacheops-7.0.1/cacheops/lua/invalidate.lua
+-rw-r--r--   0 suor      (1000) suor      (1000)      681 2023-02-25 05:58:23.000000 django-cacheops-7.0.1/cacheops/lua/invalidate_insideout.lua
+drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-05-09 07:49:47.678077 django-cacheops-7.0.1/cacheops/management/
+-rw-r--r--   0 suor      (1000) suor      (1000)        0 2012-02-26 04:58:36.000000 django-cacheops-7.0.1/cacheops/management/__init__.py
+drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-05-09 07:49:47.681410 django-cacheops-7.0.1/cacheops/management/commands/
+-rw-r--r--   0 suor      (1000) suor      (1000)        0 2012-02-26 04:58:36.000000 django-cacheops-7.0.1/cacheops/management/commands/__init__.py
+-rw-r--r--   0 suor      (1000) suor      (1000)      503 2018-11-09 09:54:36.000000 django-cacheops-7.0.1/cacheops/management/commands/cleanfilecache.py
+-rw-rw-r--   0 suor      (1000) suor      (1000)     1948 2021-05-24 09:36:10.000000 django-cacheops-7.0.1/cacheops/management/commands/invalidate.py
+-rw-r--r--   0 suor      (1000) suor      (1000)      711 2023-02-19 10:39:40.000000 django-cacheops-7.0.1/cacheops/management/commands/reapconjs.py
+-rw-r--r--   0 suor      (1000) suor      (1000)    24842 2023-05-05 11:51:50.000000 django-cacheops-7.0.1/cacheops/query.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     2421 2023-02-19 10:39:40.000000 django-cacheops-7.0.1/cacheops/reaper.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     2444 2023-04-04 10:55:06.000000 django-cacheops-7.0.1/cacheops/redis.py
+-rw-rw-r--   0 suor      (1000) suor      (1000)      206 2021-05-24 09:36:10.000000 django-cacheops-7.0.1/cacheops/serializers.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     1223 2017-09-15 07:08:22.000000 django-cacheops-7.0.1/cacheops/sharding.py
+-rw-rw-r--   0 suor      (1000) suor      (1000)      144 2021-05-24 09:36:10.000000 django-cacheops-7.0.1/cacheops/signals.py
+-rw-rw-r--   0 suor      (1000) suor      (1000)     5442 2021-05-24 09:36:10.000000 django-cacheops-7.0.1/cacheops/simple.py
+drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-05-09 07:49:47.681410 django-cacheops-7.0.1/cacheops/templatetags/
+-rw-r--r--   0 suor      (1000) suor      (1000)        0 2017-05-09 04:30:00.000000 django-cacheops-7.0.1/cacheops/templatetags/__init__.py
+-rw-rw-r--   0 suor      (1000) suor      (1000)     2311 2021-05-24 09:36:10.000000 django-cacheops-7.0.1/cacheops/templatetags/cacheops.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     4142 2022-05-27 05:04:05.000000 django-cacheops-7.0.1/cacheops/transaction.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     6382 2023-02-27 03:51:13.000000 django-cacheops-7.0.1/cacheops/tree.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     4779 2023-05-05 11:51:50.000000 django-cacheops-7.0.1/cacheops/utils.py
+drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-05-09 07:49:47.681410 django-cacheops-7.0.1/django_cacheops.egg-info/
+-rw-r--r--   0 suor      (1000) suor      (1000)    29835 2023-05-09 07:49:47.000000 django-cacheops-7.0.1/django_cacheops.egg-info/PKG-INFO
+-rw-r--r--   0 suor      (1000) suor      (1000)     1379 2023-05-09 07:49:47.000000 django-cacheops-7.0.1/django_cacheops.egg-info/SOURCES.txt
+-rw-r--r--   0 suor      (1000) suor      (1000)        1 2023-05-09 07:49:47.000000 django-cacheops-7.0.1/django_cacheops.egg-info/dependency_links.txt
+-rw-r--r--   0 suor      (1000) suor      (1000)        1 2014-03-04 07:12:55.000000 django-cacheops-7.0.1/django_cacheops.egg-info/not-zip-safe
+-rw-r--r--   0 suor      (1000) suor      (1000)       47 2016-02-03 05:07:05.000000 django-cacheops-7.0.1/django_cacheops.egg-info/pbr.json
+-rw-r--r--   0 suor      (1000) suor      (1000)       41 2023-05-09 07:49:47.000000 django-cacheops-7.0.1/django_cacheops.egg-info/requires.txt
+-rw-r--r--   0 suor      (1000) suor      (1000)        9 2023-05-09 07:49:47.000000 django-cacheops-7.0.1/django_cacheops.egg-info/top_level.txt
+-rwxrwxr-x   0 suor      (1000) suor      (1000)      249 2021-05-24 09:36:10.000000 django-cacheops-7.0.1/manage.py
+-rwxr-xr-x   0 suor      (1000) suor      (1000)      294 2023-02-22 09:39:41.000000 django-cacheops-7.0.1/publish.sh
+-rw-r--r--   0 suor      (1000) suor      (1000)       97 2023-03-11 09:05:33.000000 django-cacheops-7.0.1/pytest.ini
+-rw-r--r--   0 suor      (1000) suor      (1000)      114 2023-03-11 09:05:33.000000 django-cacheops-7.0.1/requirements-test.txt
+-rw-r--r--   0 suor      (1000) suor      (1000)      102 2023-05-09 07:49:47.681410 django-cacheops-7.0.1/setup.cfg
+-rw-r--r--   0 suor      (1000) suor      (1000)     1633 2023-05-09 07:42:03.000000 django-cacheops-7.0.1/setup.py
+drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-05-09 07:49:47.681410 django-cacheops-7.0.1/tests/
+-rw-r--r--   0 suor      (1000) suor      (1000)        0 2023-03-02 14:44:38.000000 django-cacheops-7.0.1/tests/__init__.py
+-rw-rw-r--   0 suor      (1000) suor      (1000)     5693 2021-05-24 09:36:10.000000 django-cacheops-7.0.1/tests/bench.py
+drwxr-xr-x   0 suor      (1000) suor      (1000)        0 2023-05-09 07:49:47.681410 django-cacheops-7.0.1/tests/fixtures/
+-rw-r--r--   0 suor      (1000) suor      (1000)     1202 2017-05-09 04:30:00.000000 django-cacheops-7.0.1/tests/fixtures/basic.json
+-rw-r--r--   0 suor      (1000) suor      (1000)     8083 2023-05-05 11:51:50.000000 django-cacheops-7.0.1/tests/models.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     3600 2023-05-03 07:01:43.000000 django-cacheops-7.0.1/tests/settings.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     5837 2023-05-05 11:51:50.000000 django-cacheops-7.0.1/tests/test_extras.py
+-rw-r--r--   0 suor      (1000) suor      (1000)    38588 2023-05-05 11:51:50.000000 django-cacheops-7.0.1/tests/tests.py
+-rw-rw-r--   0 suor      (1000) suor      (1000)     1874 2021-05-24 09:36:10.000000 django-cacheops-7.0.1/tests/tests_sharding.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     4553 2022-05-27 05:04:05.000000 django-cacheops-7.0.1/tests/tests_transactions.py
+-rw-r--r--   0 suor      (1000) suor      (1000)       17 2017-05-09 04:30:00.000000 django-cacheops-7.0.1/tests/urls.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     1911 2023-02-19 10:39:40.000000 django-cacheops-7.0.1/tests/utils.py
+-rw-r--r--   0 suor      (1000) suor      (1000)     1324 2023-03-17 15:12:22.000000 django-cacheops-7.0.1/tox.ini
```

### Comparing `django-cacheops-7.0/.github/workflows/ci.yml` & `django-cacheops-7.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/CHANGELOG` & `django-cacheops-7.0.1/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+7.0.1
+- made it work with Redis 6.x and older again
+- handle abstract models better
+- some docs improvements
+
 7.0
 - support Django 4.2b and 5.0a
 - added a new insideout mode
 - made join invalidation more granular
 Backwards incompatible changes:
 - dropped Python 3.5, 3.6 and Django 2.1, 2.2, 3.0 and 3.1 support
 - removed CACHEOPS_LRU
+- removed CacheopsRedis, should inherit redis.Redis instead
 
 6.2
 - support Python 3.11 and Django 4.1
 - added command to clear stale cacheops keys (Bruno Alla)
 - fixed `invalidate_m2o` for polymorphic models (#430) (Andrey Alekseev)
 - updated README: TOC, link to the post, some explanations
```

### Comparing `django-cacheops-7.0/LICENSE` & `django-cacheops-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/PKG-INFO` & `django-cacheops-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cacheops
-Version: 7.0
+Version: 7.0.1
 Summary: A slick ORM cache with automatic granular event-driven invalidation for Django.
 Home-page: http://github.com/Suor/django-cacheops
 Author: Alexander Schepanovski
 Author-email: suor.web@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -101,15 +101,15 @@
         'locations': [('localhost', 26379)], # sentinel locations, required
         'service_name': 'mymaster',          # sentinel service name, required
         'socket_timeout': 0.1,               # connection timeout in seconds, optional
         'db': 0                              # redis database, default: 0
         ...                                  # everything else is passed to Sentinel()
     }
 
-    # Use your own redis client class, should be compatible or subclass redis.StrictRedis
+    # Use your own redis client class, should be compatible or subclass redis.Redis
     CACHEOPS_CLIENT_CLASS = 'your.redis.ClientClass'
 
     CACHEOPS = {
         # Automatically cache any User.objects.get() calls for 15 minutes
         # This also includes .first() and .last() calls,
         # as well as request.user or post.author access,
         # where Post.author is a foreign key to auth.User
```

### Comparing `django-cacheops-7.0/README.rst` & `django-cacheops-7.0.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         'locations': [('localhost', 26379)], # sentinel locations, required
         'service_name': 'mymaster',          # sentinel service name, required
         'socket_timeout': 0.1,               # connection timeout in seconds, optional
         'db': 0                              # redis database, default: 0
         ...                                  # everything else is passed to Sentinel()
     }
 
-    # Use your own redis client class, should be compatible or subclass redis.StrictRedis
+    # Use your own redis client class, should be compatible or subclass redis.Redis
     CACHEOPS_CLIENT_CLASS = 'your.redis.ClientClass'
 
     CACHEOPS = {
         # Automatically cache any User.objects.get() calls for 15 minutes
         # This also includes .first() and .last() calls,
         # as well as request.user or post.author access,
         # where Post.author is a foreign key to auth.User
```

### Comparing `django-cacheops-7.0/bench.py` & `django-cacheops-7.0.1/bench.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/conf.py` & `django-cacheops-7.0.1/cacheops/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,15 +92,16 @@
     return model_profiles
 
 
 def model_profile(model):
     """
     Returns cacheops profile for a model
     """
-    # Django migrations these fake models, we don't want to cache them
+    assert not model._meta.abstract, "This should be handled by caller"
+    # Django migrations create lots of fake models, just skip them
     if model.__module__ == '__fake__':
         return None
 
     model_profiles = prepare_profiles()
 
     app = model._meta.app_label.lower()
     model_name = model._meta.model_name
```

### Comparing `django-cacheops-7.0/cacheops/getset.py` & `django-cacheops-7.0.1/cacheops/getset.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/invalidation.py` & `django-cacheops-7.0.1/cacheops/invalidation.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/jinja2.py` & `django-cacheops-7.0.1/cacheops/jinja2.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/lua/cache_thing.lua` & `django-cacheops-7.0.1/cacheops/lua/cache_thing.lua`

 * *Files 17% similar despite different names*

```diff
@@ -43,10 +43,20 @@
         redis.call('sadd', prefix .. 'schemes:' .. db_table, conj_schema(conj))
 
         -- Add new cache_key to list of dependencies
         local conj_key = conj_cache_key(db_table, conj)
         redis.call('sadd', conj_key, key)
         -- NOTE: an invalidator should live longer than any key it references.
         --       So we update its ttl on every key if needed.
+        -- REDIS_7
         redis.call('expire', conj_key, timeout, 'gt')
+        -- /REDIS_7
+        -- REDIS_6
+        local conj_ttl = redis.call('ttl', conj_key)
+        if conj_ttl < timeout then
+            -- We set conj_key life with a margin over key life to call expire rarer
+            -- And add few extra seconds to be extra safe
+            redis.call('expire', conj_key, timeout * 2 + 10)
+        end
+        -- /REDIS_6
     end
 end
```

### Comparing `django-cacheops-7.0/cacheops/lua/invalidate.lua` & `django-cacheops-7.0.1/cacheops/lua/invalidate.lua`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/lua/invalidate_insideout.lua` & `django-cacheops-7.0.1/cacheops/lua/invalidate_insideout.lua`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/management/commands/invalidate.py` & `django-cacheops-7.0.1/cacheops/management/commands/invalidate.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/management/commands/reapconjs.py` & `django-cacheops-7.0.1/cacheops/management/commands/reapconjs.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/query.py` & `django-cacheops-7.0.1/cacheops/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,21 +389,20 @@
         connect_first(post_delete, self._post_delete, sender=cls)
 
         # Install auto-created models as their module attributes to make them picklable
         module = sys.modules[cls.__module__]
         if not hasattr(module, cls.__name__):
             setattr(module, cls.__name__, cls)
 
-    # This is probably still needed if models are created dynamically
+    # This is probably still needed if models are created dynamically or imported late
     def contribute_to_class(self, cls, name):
         self._no_monkey.contribute_to_class(self, cls, name)
-        # Django migrations create lots of fake models, just skip them
-        # NOTE: we make it here rather then inside _install_cacheops()
+        # NOTE: we check it here rather then inside _install_cacheops()
         #       because we don't want @once_per() to hold refs to all of them.
-        if cls.__module__ != '__fake__' and family_has_profile(cls):
+        if family_has_profile(cls):
             self._install_cacheops(cls)
 
     @skip_on_no_invalidation
     def _pre_save(self, sender, instance, using, **kwargs):
         if instance.pk is not None and not instance._state.adding:
             try:
                 # TODO: do not fetch non-serializable fields
```

### Comparing `django-cacheops-7.0/cacheops/reaper.py` & `django-cacheops-7.0.1/cacheops/reaper.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/redis.py` & `django-cacheops-7.0.1/cacheops/redis.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 @LazyObject
 def redis_client():
     if settings.CACHEOPS_REDIS and settings.CACHEOPS_SENTINEL:
         raise ImproperlyConfigured("CACHEOPS_REDIS and CACHEOPS_SENTINEL are mutually exclusive")
 
-    client_class = redis.StrictRedis
+    client_class = redis.Redis
     if settings.CACHEOPS_CLIENT_CLASS:
         client_class = import_string(settings.CACHEOPS_CLIENT_CLASS)
 
     if settings.CACHEOPS_SENTINEL:
         if not {'locations', 'service_name'} <= set(settings.CACHEOPS_SENTINEL):
             raise ImproperlyConfigured("Specify locations and service_name for CACHEOPS_SENTINEL")
 
@@ -50,15 +50,26 @@
     else:
         return client_class(**settings.CACHEOPS_REDIS)
 
 
 ### Lua script loader
 
 import os.path
+import re
 
 
 @memoize
 def load_script(name):
     filename = os.path.join(os.path.dirname(__file__), 'lua/%s.lua' % name)
     with open(filename) as f:
         code = f.read()
+    if is_redis_7():
+        code = re.sub(r'REDIS_6.*?/REDIS_6', '', code, flags=re.S)
+    else:
+        code = re.sub(r'REDIS_7.*?/REDIS_7', '', code, flags=re.S)
     return redis_client.register_script(code)
+
+
+@memoize
+def is_redis_7():
+    redis_version = redis_client.info('server')['redis_version']
+    return int(redis_version.split('.')[0]) >= 7
```

### Comparing `django-cacheops-7.0/cacheops/sharding.py` & `django-cacheops-7.0.1/cacheops/sharding.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/simple.py` & `django-cacheops-7.0.1/cacheops/simple.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/templatetags/cacheops.py` & `django-cacheops-7.0.1/cacheops/templatetags/cacheops.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/transaction.py` & `django-cacheops-7.0.1/cacheops/transaction.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/tree.py` & `django-cacheops-7.0.1/cacheops/tree.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/cacheops/utils.py` & `django-cacheops-7.0.1/cacheops/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 
 from django.db import models
 from django.http import HttpRequest
 
 from .conf import model_profile
 
 
-def get_concrete_model(model):
+def get_table_model(model):
     return next((b for b in model.__mro__ if issubclass(b, models.Model) and b is not models.Model
                  and not b._meta.proxy and not b._meta.abstract), None)
 
 def model_family(model):
     """
-    Returns a list of all proxy models, including subclasess, superclasses and siblings.
+    The family is models sharing a database table, events on one should affect each other.
+
+    We simply collect a list of all proxy models, including subclasess, superclasses and siblings.
+    Two descendants of an abstract model are not family - they cannot affect each other.
     """
     def class_tree(cls):
         return [cls] + lmapcat(class_tree, cls.__subclasses__())
 
     # NOTE: we also list multitable submodels here, we just don't care.
     #       Cacheops doesn't support them anyway.
-    # NOTE: when this is called in Manager.contribute_to_class()
-    #       ._meta.concrete_model might still be None
-    return class_tree(model._meta.concrete_model or get_concrete_model(model) or model)
+    table_model = get_table_model(model)
+    return class_tree(table_model) if table_model else []
 
 
 @memoize
 def family_has_profile(cls):
     return any(model_profile, model_family(cls))
```

### Comparing `django-cacheops-7.0/django_cacheops.egg-info/PKG-INFO` & `django-cacheops-7.0.1/django_cacheops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cacheops
-Version: 7.0
+Version: 7.0.1
 Summary: A slick ORM cache with automatic granular event-driven invalidation for Django.
 Home-page: http://github.com/Suor/django-cacheops
 Author: Alexander Schepanovski
 Author-email: suor.web@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -101,15 +101,15 @@
         'locations': [('localhost', 26379)], # sentinel locations, required
         'service_name': 'mymaster',          # sentinel service name, required
         'socket_timeout': 0.1,               # connection timeout in seconds, optional
         'db': 0                              # redis database, default: 0
         ...                                  # everything else is passed to Sentinel()
     }
 
-    # Use your own redis client class, should be compatible or subclass redis.StrictRedis
+    # Use your own redis client class, should be compatible or subclass redis.Redis
     CACHEOPS_CLIENT_CLASS = 'your.redis.ClientClass'
 
     CACHEOPS = {
         # Automatically cache any User.objects.get() calls for 15 minutes
         # This also includes .first() and .last() calls,
         # as well as request.user or post.author access,
         # where Post.author is a foreign key to auth.User
```

### Comparing `django-cacheops-7.0/django_cacheops.egg-info/SOURCES.txt` & `django-cacheops-7.0.1/django_cacheops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/setup.py` & `django-cacheops-7.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Remove build status
 README = open('README.rst').read().replace('|Build Status|', '', 1)
 
 
 setup(
     name='django-cacheops',
-    version='7.0',
+    version='7.0.1',
     author='Alexander Schepanovski',
     author_email='suor.web@gmail.com',
 
     description='A slick ORM cache with automatic granular event-driven invalidation for Django.',
     long_description=README,
     url='http://github.com/Suor/django-cacheops',
     license='BSD',
```

### Comparing `django-cacheops-7.0/tests/bench.py` & `django-cacheops-7.0.1/tests/bench.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/tests/fixtures/basic.json` & `django-cacheops-7.0.1/tests/fixtures/basic.json`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/tests/models.py` & `django-cacheops-7.0.1/tests/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,7 +303,12 @@
 
             return _curried
 
         super().__init__(*args, **kwargs)
         setattr(self, '_get_private_data', curry(sum, [1, 2, 3, 4]))
 
     name = models.CharField(max_length=255)
+
+
+class Abs(models.Model):
+    class Meta:
+        abstract = True
```

### Comparing `django-cacheops-7.0/tests/settings.py` & `django-cacheops-7.0.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/tests/test_extras.py` & `django-cacheops-7.0.1/tests/test_extras.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from django.test import TestCase, override_settings
 
 from cacheops import cached_as, no_invalidation, invalidate_obj, invalidate_model, invalidate_all
 from cacheops.conf import settings
 from cacheops.signals import cache_read, cache_invalidated
 
 from .utils import BaseTestCase, make_inc
-from .models import Post, Category, Local, DbAgnostic, DbBinded
+from .models import Post, Category, Local, DbAgnostic, DbBinded, Abs
 
 
 class SettingsTests(TestCase):
     def test_context_manager(self):
         self.assertTrue(settings.CACHEOPS_ENABLED)
 
         with self.settings(CACHEOPS_ENABLED=False):
@@ -100,15 +100,15 @@
         results = []
         locked = threading.Event()
         thread = [None]
 
         def second_thread():
             def _target():
                 try:
-                    with before('redis.StrictRedis.brpoplpush', lambda *a, **kw: locked.set()):
+                    with before('redis.Redis.brpoplpush', lambda *a, **kw: locked.set()):
                         results.append(func())
                 except Exception:
                     locked.set()
                     raise
 
             thread[0] = ThreadWithReturnValue(target=_target)
             thread[0].start()
@@ -179,7 +179,13 @@
             list(DbAgnostic.objects.cache().using('slave'))
 
     def test_db_agnostic_disabled(self):
         list(DbBinded.objects.cache())
 
         with self.assertNumQueries(1, using='slave'):
             list(DbBinded.objects.cache().using('slave'))
+
+
+def test_abstract_family():
+    from cacheops.utils import model_family
+
+    assert model_family(Abs) == []
```

### Comparing `django-cacheops-7.0/tests/tests.py` & `django-cacheops-7.0.1/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -957,14 +957,21 @@
         media = NonCachedMedia.objects.create(title='Pulp Fiction')
         MediaProxy.objects.cache().get(title=media.title)
         NonCachedMedia.objects.get(id=media.id).delete()
 
         with self.assertRaises(NonCachedMedia.DoesNotExist):
             MediaProxy.objects.cache().get(title=media.title)
 
+    def test_siblings(self):
+        list(VideoProxy.objects.cache())
+        NonCachedVideoProxy.objects.create(title='Pulp Fiction')
+
+        with self.assertNumQueries(1):
+            list(VideoProxy.objects.cache())
+
     def test_proxy_caching(self):
         video = Video.objects.create(title='Pulp Fiction')
         self.assertEqual(type(Video.objects.cache().get(pk=video.pk)),
                          Video)
         self.assertEqual(type(VideoProxy.objects.cache().get(pk=video.pk)),
                          VideoProxy)
```

### Comparing `django-cacheops-7.0/tests/tests_sharding.py` & `django-cacheops-7.0.1/tests/tests_sharding.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/tests/tests_transactions.py` & `django-cacheops-7.0.1/tests/tests_transactions.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/tests/utils.py` & `django-cacheops-7.0.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-cacheops-7.0/tox.ini` & `django-cacheops-7.0.1/tox.ini`

 * *Files identical despite different names*

