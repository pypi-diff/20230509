# Comparing `tmp/wc-django-envoyer-0.1.0.tar.gz` & `tmp/wc-django-envoyer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-envoyer-0.1.0.tar", last modified: Fri May  5 09:49:18 2023, max compression
+gzip compressed data, was "wc-django-envoyer-0.2.0.tar", last modified: Tue May  9 09:35:29 2023, max compression
```

## Comparing `wc-django-envoyer-0.1.0.tar` & `wc-django-envoyer-0.2.0.tar`

### file list

```diff
@@ -1,62 +1,73 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-05 09:49:18.380381 wc-django-envoyer-0.1.0/
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      297 2023-05-02 10:04:23.000000 wc-django-envoyer-0.1.0/CHANGELOG.md
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1072 2023-05-02 10:04:23.000000 wc-django-envoyer-0.1.0/LICENSE
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      153 2023-05-02 10:13:05.000000 wc-django-envoyer-0.1.0/MANIFEST.in
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1250 2023-05-02 10:04:23.000000 wc-django-envoyer-0.1.0/Makefile
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4863 2023-05-05 09:49:18.380381 wc-django-envoyer-0.1.0/PKG-INFO
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)     4012 2023-05-05 09:40:20.000000 wc-django-envoyer-0.1.0/README.md
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)       79 2023-05-05 09:49:18.380381 wc-django-envoyer-0.1.0/setup.cfg
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1720 2023-05-04 12:22:08.000000 wc-django-envoyer-0.1.0/setup.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-05 09:49:18.376381 wc-django-envoyer-0.1.0/tests/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1658 2023-05-05 07:23:57.000000 wc-django-envoyer-0.1.0/tests/test_run.py
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      552 2023-05-03 13:14:54.000000 wc-django-envoyer-0.1.0/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-05 09:49:18.376381 wc-django-envoyer-0.1.0/wc_django_envoyer.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4863 2023-05-05 09:49:18.000000 wc-django-envoyer-0.1.0/wc_django_envoyer.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1421 2023-05-05 09:49:18.000000 wc-django-envoyer-0.1.0/wc_django_envoyer.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-05-05 09:49:18.000000 wc-django-envoyer-0.1.0/wc_django_envoyer.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      258 2023-05-05 09:49:18.000000 wc-django-envoyer-0.1.0/wc_django_envoyer.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       12 2023-05-05 09:49:18.000000 wc-django-envoyer-0.1.0/wc_django_envoyer.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-05 09:49:18.376381 wc-django-envoyer-0.1.0/wcd_envoyer/
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      453 2023-05-05 09:41:20.000000 wc-django-envoyer-0.1.0/wcd_envoyer/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-05 09:49:18.376381 wc-django-envoyer-0.1.0/wcd_envoyer/admin/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       73 2023-05-05 04:46:14.000000 wc-django-envoyer-0.1.0/wcd_envoyer/admin/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-05-05 05:34:17.000000 wc-django-envoyer-0.1.0/wcd_envoyer/admin/channels.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      376 2023-05-05 05:29:36.000000 wc-django-envoyer-0.1.0/wcd_envoyer/admin/forms.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1604 2023-05-05 09:49:12.000000 wc-django-envoyer-0.1.0/wcd_envoyer/admin/messages.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2827 2023-05-05 07:45:51.000000 wc-django-envoyer-0.1.0/wcd_envoyer/admin/templates.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2319 2023-05-05 07:47:33.000000 wc-django-envoyer-0.1.0/wcd_envoyer/admin/utils.py
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)      322 2023-05-02 13:04:49.000000 wc-django-envoyer-0.1.0/wcd_envoyer/apps.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-05 09:49:18.376381 wc-django-envoyer-0.1.0/wcd_envoyer/channels/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      102 2023-05-04 13:50:06.000000 wc-django-envoyer-0.1.0/wcd_envoyer/channels/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     6846 2023-05-05 07:35:42.000000 wc-django-envoyer-0.1.0/wcd_envoyer/channels/backend.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-05 09:49:18.380381 wc-django-envoyer-0.1.0/wcd_envoyer/channels/backends/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-04 07:24:02.000000 wc-django-envoyer-0.1.0/wcd_envoyer/channels/backends/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1019 2023-05-05 07:23:51.000000 wc-django-envoyer-0.1.0/wcd_envoyer/channels/backends/console.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2015 2023-05-05 07:09:08.000000 wc-django-envoyer-0.1.0/wcd_envoyer/channels/backends/email.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      852 2023-05-05 05:29:56.000000 wc-django-envoyer-0.1.0/wcd_envoyer/channels/forms.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1236 2023-05-05 07:49:43.000000 wc-django-envoyer-0.1.0/wcd_envoyer/channels/registry_base.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      250 2023-05-05 08:04:59.000000 wc-django-envoyer-0.1.0/wcd_envoyer/channels/renderers.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2510 2023-05-05 08:10:12.000000 wc-django-envoyer-0.1.0/wcd_envoyer/conf.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      471 2023-05-04 07:48:09.000000 wc-django-envoyer-0.1.0/wcd_envoyer/const.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1441 2023-05-05 05:00:50.000000 wc-django-envoyer-0.1.0/wcd_envoyer/events.py
--rwxrwxrwx   0 preusx    (1000) preusx    (1000)       40 2023-05-02 10:29:47.000000 wc-django-envoyer-0.1.0/wcd_envoyer/exceptions.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-05 09:49:18.380381 wc-django-envoyer-0.1.0/wcd_envoyer/migrations/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3457 2023-05-04 07:49:17.000000 wc-django-envoyer-0.1.0/wcd_envoyer/migrations/0001_initial.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1428 2023-05-05 05:52:44.000000 wc-django-envoyer-0.1.0/wcd_envoyer/migrations/0002_auto_20230505_0852.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-03 12:44:30.000000 wc-django-envoyer-0.1.0/wcd_envoyer/migrations/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-05 09:49:18.380381 wc-django-envoyer-0.1.0/wcd_envoyer/models/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       69 2023-05-03 12:30:33.000000 wc-django-envoyer-0.1.0/wcd_envoyer/models/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      841 2023-05-05 08:12:11.000000 wc-django-envoyer-0.1.0/wcd_envoyer/models/channels.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2651 2023-05-05 08:15:18.000000 wc-django-envoyer-0.1.0/wcd_envoyer/models/messages.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-05-04 07:48:49.000000 wc-django-envoyer-0.1.0/wcd_envoyer/models/utils.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-05 09:49:18.380381 wc-django-envoyer-0.1.0/wcd_envoyer/services/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-03 13:09:31.000000 wc-django-envoyer-0.1.0/wcd_envoyer/services/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5204 2023-05-05 08:15:47.000000 wc-django-envoyer-0.1.0/wcd_envoyer/services/sender.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      784 2023-05-05 06:06:41.000000 wc-django-envoyer-0.1.0/wcd_envoyer/services/templates_resolver.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      935 2023-05-05 08:37:19.000000 wc-django-envoyer-0.1.0/wcd_envoyer/shortcuts.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-05 09:49:18.380381 wc-django-envoyer-0.1.0/wcd_envoyer/utils/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       93 2023-05-02 13:52:40.000000 wc-django-envoyer-0.1.0/wcd_envoyer/utils/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1514 2023-05-04 13:44:03.000000 wc-django-envoyer-0.1.0/wcd_envoyer/utils/functional.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1030 2023-05-04 11:22:17.000000 wc-django-envoyer-0.1.0/wcd_envoyer/utils/models.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      489 2023-05-02 13:50:44.000000 wc-django-envoyer-0.1.0/wcd_envoyer/utils/registry.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      193 2023-05-05 08:11:53.000000 wc-django-envoyer-0.1.0/wcd_envoyer/utils/types.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.430881 wc-django-envoyer-0.2.0/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      297 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/CHANGELOG.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1072 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/LICENSE
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      153 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/MANIFEST.in
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1250 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/Makefile
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     6802 2023-05-09 09:35:29.430881 wc-django-envoyer-0.2.0/PKG-INFO
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     5951 2023-05-09 09:26:34.000000 wc-django-envoyer-0.2.0/README.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-05-09 09:35:29.434881 wc-django-envoyer-0.2.0/setup.cfg
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1762 2023-05-08 11:10:01.000000 wc-django-envoyer-0.2.0/setup.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.426881 wc-django-envoyer-0.2.0/tests/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2192 2023-05-09 08:47:31.000000 wc-django-envoyer-0.2.0/tests/test_celery.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3981 2023-05-09 08:04:15.000000 wc-django-envoyer-0.2.0/tests/test_run.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      593 2023-05-09 08:31:54.000000 wc-django-envoyer-0.2.0/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.426881 wc-django-envoyer-0.2.0/wc_django_envoyer.egg-info/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     6802 2023-05-09 09:35:29.000000 wc-django-envoyer-0.2.0/wc_django_envoyer.egg-info/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1716 2023-05-09 09:35:29.000000 wc-django-envoyer-0.2.0/wc_django_envoyer.egg-info/SOURCES.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-05-09 09:35:29.000000 wc-django-envoyer-0.2.0/wc_django_envoyer.egg-info/dependency_links.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      285 2023-05-09 09:35:29.000000 wc-django-envoyer-0.2.0/wc_django_envoyer.egg-info/requires.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       12 2023-05-09 09:35:29.000000 wc-django-envoyer-0.2.0/wc_django_envoyer.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.426881 wc-django-envoyer-0.2.0/wcd_envoyer/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      453 2023-05-09 09:26:44.000000 wc-django-envoyer-0.2.0/wcd_envoyer/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.426881 wc-django-envoyer-0.2.0/wcd_envoyer/admin/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       73 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/admin/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/admin/channels.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      376 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/admin/forms.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1156 2023-05-09 09:22:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/admin/messages.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2889 2023-05-09 09:20:35.000000 wc-django-envoyer-0.2.0/wcd_envoyer/admin/templates.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2320 2023-05-09 09:20:20.000000 wc-django-envoyer-0.2.0/wcd_envoyer/admin/utils.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      322 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/apps.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.426881 wc-django-envoyer-0.2.0/wcd_envoyer/channels/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      102 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/channels/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5974 2023-05-08 08:50:13.000000 wc-django-envoyer-0.2.0/wcd_envoyer/channels/backend.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.426881 wc-django-envoyer-0.2.0/wcd_envoyer/channels/backends/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/channels/backends/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      952 2023-05-08 08:25:08.000000 wc-django-envoyer-0.2.0/wcd_envoyer/channels/backends/console.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4308 2023-05-08 12:08:11.000000 wc-django-envoyer-0.2.0/wcd_envoyer/channels/backends/django_sendmail.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      852 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/channels/forms.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1236 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/channels/registry_base.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      250 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/channels/renderers.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2510 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/conf.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      471 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/const.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.426881 wc-django-envoyer-0.2.0/wcd_envoyer/contrib/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-08 12:43:08.000000 wc-django-envoyer-0.2.0/wcd_envoyer/contrib/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.430881 wc-django-envoyer-0.2.0/wcd_envoyer/contrib/celery/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-08 12:45:33.000000 wc-django-envoyer-0.2.0/wcd_envoyer/contrib/celery/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.430881 wc-django-envoyer-0.2.0/wcd_envoyer/contrib/celery/services/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-08 12:45:44.000000 wc-django-envoyer-0.2.0/wcd_envoyer/contrib/celery/services/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1191 2023-05-09 09:14:05.000000 wc-django-envoyer-0.2.0/wcd_envoyer/contrib/celery/services/sender.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1186 2023-05-09 08:38:21.000000 wc-django-envoyer-0.2.0/wcd_envoyer/contrib/celery/shortcuts.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      640 2023-05-09 08:47:21.000000 wc-django-envoyer-0.2.0/wcd_envoyer/contrib/celery/tasks.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1441 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/events.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       40 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/exceptions.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.430881 wc-django-envoyer-0.2.0/wcd_envoyer/migrations/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3457 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/migrations/0001_initial.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1428 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/migrations/0002_auto_20230505_0852.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/migrations/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.430881 wc-django-envoyer-0.2.0/wcd_envoyer/models/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       69 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/models/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      841 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/models/channels.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2651 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/models/messages.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/models/utils.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.430881 wc-django-envoyer-0.2.0/wcd_envoyer/services/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/services/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     8341 2023-05-09 09:09:38.000000 wc-django-envoyer-0.2.0/wcd_envoyer/services/sender.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      784 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/services/templates_resolver.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      935 2023-05-08 09:18:19.000000 wc-django-envoyer-0.2.0/wcd_envoyer/shortcuts.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      129 2023-05-09 09:05:12.000000 wc-django-envoyer-0.2.0/wcd_envoyer/signals.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:35:29.430881 wc-django-envoyer-0.2.0/wcd_envoyer/utils/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       93 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/utils/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1514 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/utils/functional.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1030 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/utils/models.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      489 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/utils/registry.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      193 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.0/wcd_envoyer/utils/types.py
```

### Comparing `wc-django-envoyer-0.1.0/LICENSE` & `wc-django-envoyer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/Makefile` & `wc-django-envoyer-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/setup.py` & `wc-django-envoyer-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         'px-django-lingua>=0.1.7,<0.2.0',
         'wc-django-notifications>=0.1.3,<0.2.0',
     ],
     include_package_data=True,
     extras_require={
         'dev': [
             'pytest>=6.0,<7.0',
+            'pytest-mock>=3.10.0,<4.0.0',
             'pytest-watch>=4.2,<5.0',
             'pytest-django>=4.3,<5.0',
             'django-environ==0.4.5',
             'django-stubs',
             'django>=2.2,<4',
             'twine',
         ],
```

### Comparing `wc-django-envoyer-0.1.0/wc_django_envoyer.egg-info/SOURCES.txt` & `wc-django-envoyer-0.2.0/wc_django_envoyer.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,41 +2,49 @@
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 setup.cfg
 setup.py
 tox.ini
+tests/test_celery.py
 tests/test_run.py
 wc_django_envoyer.egg-info/PKG-INFO
 wc_django_envoyer.egg-info/SOURCES.txt
 wc_django_envoyer.egg-info/dependency_links.txt
 wc_django_envoyer.egg-info/requires.txt
 wc_django_envoyer.egg-info/top_level.txt
 wcd_envoyer/__init__.py
 wcd_envoyer/apps.py
 wcd_envoyer/conf.py
 wcd_envoyer/const.py
 wcd_envoyer/events.py
 wcd_envoyer/exceptions.py
 wcd_envoyer/shortcuts.py
+wcd_envoyer/signals.py
 wcd_envoyer/admin/__init__.py
 wcd_envoyer/admin/channels.py
 wcd_envoyer/admin/forms.py
 wcd_envoyer/admin/messages.py
 wcd_envoyer/admin/templates.py
 wcd_envoyer/admin/utils.py
 wcd_envoyer/channels/__init__.py
 wcd_envoyer/channels/backend.py
 wcd_envoyer/channels/forms.py
 wcd_envoyer/channels/registry_base.py
 wcd_envoyer/channels/renderers.py
 wcd_envoyer/channels/backends/__init__.py
 wcd_envoyer/channels/backends/console.py
-wcd_envoyer/channels/backends/email.py
+wcd_envoyer/channels/backends/django_sendmail.py
+wcd_envoyer/contrib/__init__.py
+wcd_envoyer/contrib/celery/__init__.py
+wcd_envoyer/contrib/celery/shortcuts.py
+wcd_envoyer/contrib/celery/tasks.py
+wcd_envoyer/contrib/celery/services/__init__.py
+wcd_envoyer/contrib/celery/services/sender.py
 wcd_envoyer/migrations/0001_initial.py
 wcd_envoyer/migrations/0002_auto_20230505_0852.py
 wcd_envoyer/migrations/__init__.py
 wcd_envoyer/models/__init__.py
 wcd_envoyer/models/channels.py
 wcd_envoyer/models/messages.py
 wcd_envoyer/models/utils.py
```

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/admin/messages.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/admin/messages.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,35 @@
 from django.contrib import admin
+from django.contrib.messages import INFO
 
 from wcd_envoyer.models import Message
+from wcd_envoyer.shortcuts import default_sender
+from django.utils.translation import pgettext, pgettext_lazy
 
 from .utils import JsonDataAdminMixin
 
 
 @admin.register(Message)
 class MessageAdmin(JsonDataAdminMixin, admin.ModelAdmin):
-    # actions = 'resend',
+    messages_sender = default_sender
+    actions = 'resend_action',
     list_display = 'channel', 'event', 'status', 'created_at', 'updated_at',
     list_filter = 'channel', 'event', 'status',
     readonly_fields = 'json_data', 'created_at', 'updated_at',
     date_hierarchy = 'created_at'
+    search_fields = 'channel', 'event', 'recipients', 'data', 'status',
 
-    # def resend(self, request, qs):
-    #     result = sender_service.resend(letters=qs)
-    #     if result['sent_count']:
-    #         self.message_user(
-    #             request=request,
-    #             message=(
-    #                 pgettext_lazy(
-    #                     'wcd_envour',
-    #                     'Successuly resent {} letters.'
-    #                 )
-    #                 .format(result['sent_count'])
-    #             ),
-    #             level=message_const.SUCCESS
-    #         )
-    #     if result['error_ids']:
-    #         self.message_user(
-    #             request=request,
-    #             message=(
-    #                 pgettext_lazy(
-    #                     'wcd_envour',
-    #                     'Failed reseding {} letters with id: {}.'
-    #                 )
-    #                 .format(
-    #                     len(result['error_ids']),
-    #                     ', '.join([str(pk) for pk in result['error_ids']])
-    #                 )
-    #             ),
-    #             level=message_const.ERROR
-    #         )
-    # resend.short_description = pgettext_lazy('wcd_envour', 'Resend letters')
+    def resend_action(self, request, qs):
+        messages = list(qs)
+        self.messages_sender.resend(messages)
+
+        self.message_user(
+            request=request,
+            message=(
+                pgettext('wcd_envoyer', 'Resent {} letters.')
+                .format(len(messages))
+            ),
+            level=INFO,
+        )
+    resend_action.short_description = pgettext_lazy(
+        'wcd_envoyer', 'Resend letters',
+    )
```

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/admin/templates.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/admin/templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,31 +57,32 @@
     add_fieldsets = (None, {'fields': ['channel', 'event']}),
     add_inlines = ()
     inlines = TemplateTranslationsInlineAdmin,
     list_display = 'channel', 'event', 'is_active', 'created_at', 'updated_at',
     list_filter = 'channel', 'event', 'is_active',
     date_hierarchy = 'created_at'
     readonly_fields = 'legend', 'json_data',
+    search_fields = 'channel', 'event', 'data', 'status',
 
     def get_backend_form_class(self, request, obj, backend):
         return backend.template_form_class
 
     def legend(self, obj):
         if not getattr(obj, 'pk', None):
             return '-'
 
         event = events.registry.get(obj.event)
 
         if event is None:
             return '-'
 
         data = [(
-            pgettext('wcd_envour', 'Key'),
-            pgettext('wcd_envour', 'Title'),
-            pgettext('wcd_envour', 'Description'),
+            pgettext('wcd_envoyer', 'Key'),
+            pgettext('wcd_envoyer', 'Title'),
+            pgettext('wcd_envoyer', 'Description'),
         )] + [
             (key, str(title), str(description))
             for key, title, description in event.context
         ]
 
         return mark_safe(render_html_table(data))
-    legend.short_description = pgettext_lazy('wcd_envour', 'Legend')
+    legend.short_description = pgettext_lazy('wcd_envoyer', 'Legend')
```

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/admin/utils.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/admin/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         return super().get_fieldsets(request, obj)
 
 
 class JsonDataAdminMixin:
     def json_data(self, obj):
         return mark_safe(prettify_json(getattr(obj, 'data', {})))
-    json_data.short_description = pgettext_lazy('wcd_envour', 'Json data')
+    json_data.short_description = pgettext_lazy('wcd_envoyer', 'Json data')
 
 
 def render_html_table(data: List[Tuple]) -> str:
     html = '<table style="border: 1px solid #ecf2f6;"><tbody>'
     for line in data:
         html += '<tr><td>'
         html += '</td><td>'.join(line)
```

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/channels/backend.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/channels/backend.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from typing import *
 from dataclasses import dataclass, field
 from functools import cached_property
 from typing import Any
 
 from wcd_envoyer.utils import importable_prop, KwargsInjector
-from wcd_envoyer.const import MessageStatus
 
 if TYPE_CHECKING:
     from wcd_envoyer.models import Message, Template, ChannelConfig
 
 
 __all__ = (
     'Recipient', 'Recipients',  'TemplatedMessage', 'TemplatedMessages',
+    'FailedMessages', 'SucceededFailedMessages',
     'MessageData',
     'BaseMessagesMaker', 'MessagesMaker', 'SplitRecipientsMessagesMaker',
     'MultiRecipientsMessagesMakerMixin', 'SplitRecipientsMessagesMakerMixin',
     'BaseMessagingBackend',
-    'StatusChangeMessagingBackendMixin',
 )
 
 Recipient = Dict[str, Any]
 Recipients = Sequence[Recipient]
 TemplatedMessage = Tuple['MessageData', 'Template']
 TemplatedMessages = List[TemplatedMessage]
+FailedMessages = List[Tuple['Message', Any]]
+SucceededFailedMessages = Tuple[List['Message'], FailedMessages]
 
 
 @dataclass
 class MessageData:
     channel: str
     event: str
     recipients: Recipients
@@ -189,46 +190,9 @@
         return self.messages_maker(config, templated_messages, context=context)
 
     def send(
         self,
         config: 'ChannelConfig',
         messages: Sequence['Message'],
         context: dict = {},
-    ) -> List['Message']:
+    ) -> SucceededFailedMessages:
         raise NotImplementedError()
-
-
-class StatusChangeMessagingBackendMixin:
-    def _send(
-        self,
-        config: 'ChannelConfig',
-        messages: Sequence['Message'],
-        context: dict = {},
-    ):
-        return super().send(config, messages, context=context)
-
-    def update_messages_status(
-        self, status: MessageStatus, messages: Sequence['Message']
-    ):
-        # FIXME: Circular import!
-        from wcd_envoyer.models import Message
-
-        for message in messages:
-            message.status = status
-
-        Message.objects.bulk_update(messages, fields=['status'])
-
-        return messages
-
-    def send(
-        self,
-        config: 'ChannelConfig',
-        messages: Sequence['Message'],
-        context: dict = {},
-    ):
-        self.update_messages_status(MessageStatus.PENDING, messages)
-
-        messages = self._send(config, messages, context=context)
-
-        self.update_messages_status(MessageStatus.SENT, messages)
-
-        return messages
```

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/channels/backends/console.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/channels/backends/console.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import *
 from pprint import pprint
 
 from wcd_envoyer.models import Message, ChannelConfig
 
-from ..backend import BaseMessagingBackend, StatusChangeMessagingBackendMixin
+from ..backend import BaseMessagingBackend
 
 
 def print_heading(message, l=80, s='='):
     print((message + ' ' + (s*l)).strip()[:l])
 
 
-class ConsoleBackend(StatusChangeMessagingBackendMixin, BaseMessagingBackend):
-    def _send(self, config: ChannelConfig, messages: Sequence[Message], context={}):
+class ConsoleBackend(BaseMessagingBackend):
+    def send(self, config: ChannelConfig, messages: Sequence[Message], context={}):
         print_heading('Printing %s messages' % len(messages))
 
         for message in messages:
             print_heading('', s='-')
             print('ID: %s' % message.pk)
             print('Channel: %s' % message.channel)
             print('Event: %s' % message.event)
@@ -24,8 +24,8 @@
             pprint(message.recipients, compact=True, indent=2)
             print('Data:')
             pprint(message.data, compact=True, indent=2)
             print_heading('', s='-')
 
         print_heading('')
 
-        return messages
+        return messages, []
```

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/channels/forms.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/channels/forms.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/channels/registry_base.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/channels/registry_base.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/conf.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/conf.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/events.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/events.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/migrations/0001_initial.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/migrations/0002_auto_20230505_0852.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/migrations/0002_auto_20230505_0852.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/models/channels.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/models/channels.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/models/messages.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/models/messages.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/services/templates_resolver.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/services/templates_resolver.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/shortcuts.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/shortcuts.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/utils/functional.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/utils/functional.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.1.0/wcd_envoyer/utils/models.py` & `wc-django-envoyer-0.2.0/wcd_envoyer/utils/models.py`

 * *Files identical despite different names*

