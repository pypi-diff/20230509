# Comparing `tmp/django-gesha-0.1a0.tar.gz` & `tmp/django-gesha-0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-gesha-0.1a0.tar", last modified: Fri Apr 21 00:49:51 2023, max compression
+gzip compressed data, was "django-gesha-0.1a1.tar", last modified: Mon May  8 22:20:13 2023, max compression
```

## Comparing `django-gesha-0.1a0.tar` & `django-gesha-0.1a1.tar`

### file list

```diff
@@ -1,69 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.437011 django-gesha-0.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-21 00:49:38.000000 django-gesha-0.1a0/.eslintrc.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.425011 django-gesha-0.1a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.429011 django-gesha-0.1a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-21 00:49:38.000000 django-gesha-0.1a0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-21 00:49:38.000000 django-gesha-0.1a0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-21 00:49:38.000000 django-gesha-0.1a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-21 00:49:38.000000 django-gesha-0.1a0/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-21 00:49:38.000000 django-gesha-0.1a0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:38.000000 django-gesha-0.1a0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-21 00:49:38.000000 django-gesha-0.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-21 00:49:51.437011 django-gesha-0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-21 00:49:38.000000 django-gesha-0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.429011 django-gesha-0.1a0/django_gesha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-21 00:49:51.000000 django-gesha-0.1a0/django_gesha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-21 00:49:51.000000 django-gesha-0.1a0/django_gesha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:49:51.000000 django-gesha-0.1a0/django_gesha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-21 00:49:51.000000 django-gesha-0.1a0/django_gesha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 00:49:51.000000 django-gesha-0.1a0/django_gesha.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.433011 django-gesha-0.1a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-21 00:49:38.000000 django-gesha-0.1a0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-21 00:49:38.000000 django-gesha-0.1a0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-21 00:49:38.000000 django-gesha-0.1a0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-21 00:49:38.000000 django-gesha-0.1a0/docs/user_guide.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.433011 django-gesha-0.1a0/gesha/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 00:49:38.000000 django-gesha-0.1a0/gesha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-21 00:49:38.000000 django-gesha-0.1a0/gesha/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-21 00:49:38.000000 django-gesha-0.1a0/gesha/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.425011 django-gesha-0.1a0/gesha/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.425011 django-gesha-0.1a0/gesha/static/gesha/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.425011 django-gesha-0.1a0/gesha/static/gesha/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.433011 django-gesha-0.1a0/gesha/static/gesha/dist/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-21 00:49:38.000000 django-gesha-0.1a0/gesha/static/gesha/dist/js/django-gesha.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-21 00:49:38.000000 django-gesha-0.1a0/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.433011 django-gesha-0.1a0/gesha/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:38.000000 django-gesha-0.1a0/gesha/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-21 00:49:38.000000 django-gesha-0.1a0/gesha/templatetags/gesha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-21 00:49:38.000000 django-gesha-0.1a0/gulpfile.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.433011 django-gesha-0.1a0/js_src/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-21 00:49:38.000000 django-gesha-0.1a0/js_src/context.ts
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-21 00:49:38.000000 django-gesha-0.1a0/js_src/main.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.433011 django-gesha-0.1a0/js_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-21 00:49:38.000000 django-gesha-0.1a0/js_tests/context.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-21 00:49:38.000000 django-gesha-0.1a0/js_tests/helpers.ts
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-21 00:49:38.000000 django-gesha-0.1a0/js_tests/main.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-21 00:49:38.000000 django-gesha-0.1a0/js_tests/test.html
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-21 00:49:38.000000 django-gesha-0.1a0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)   342194 2023-04-21 00:49:38.000000 django-gesha-0.1a0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-21 00:49:38.000000 django-gesha-0.1a0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-21 00:49:38.000000 django-gesha-0.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 00:49:51.437011 django-gesha-0.1a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.437011 django-gesha-0.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.437011 django-gesha-0.1a0/tests/fake_project/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.437011 django-gesha-0.1a0/tests/fake_project/fake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tests/fake_project/fake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tests/fake_project/fake/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tests/fake_project/fake/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:49:51.437011 django-gesha-0.1a0/tests/fake_project/fake/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tests/fake_project/fake/templates/test.html
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tests/fake_project/fake/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tests/fake_project/fake/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tests/fake_project/fake/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tests/fake_project/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tests/test_jscontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tests/test_package_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 00:49:38.000000 django-gesha-0.1a0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.469610 django-gesha-0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-08 22:20:01.000000 django-gesha-0.1a1/.eslintrc.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.449609 django-gesha-0.1a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.457610 django-gesha-0.1a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-08 22:20:01.000000 django-gesha-0.1a1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-08 22:20:01.000000 django-gesha-0.1a1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-08 22:20:01.000000 django-gesha-0.1a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-08 22:20:01.000000 django-gesha-0.1a1/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-08 22:20:01.000000 django-gesha-0.1a1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-08 22:20:01.000000 django-gesha-0.1a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 22:20:01.000000 django-gesha-0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-08 22:20:13.469610 django-gesha-0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-08 22:20:01.000000 django-gesha-0.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.457610 django-gesha-0.1a1/django_gesha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-08 22:20:13.000000 django-gesha-0.1a1/django_gesha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-08 22:20:13.000000 django-gesha-0.1a1/django_gesha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:20:13.000000 django-gesha-0.1a1/django_gesha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-08 22:20:13.000000 django-gesha-0.1a1/django_gesha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 22:20:13.000000 django-gesha-0.1a1/django_gesha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.461609 django-gesha-0.1a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:01.000000 django-gesha-0.1a1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-08 22:20:01.000000 django-gesha-0.1a1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-08 22:20:01.000000 django-gesha-0.1a1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-08 22:20:01.000000 django-gesha-0.1a1/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.461609 django-gesha-0.1a1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-08 22:20:01.000000 django-gesha-0.1a1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-08 22:20:01.000000 django-gesha-0.1a1/docs/user_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.461609 django-gesha-0.1a1/gesha/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.449609 django-gesha-0.1a1/gesha/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.449609 django-gesha-0.1a1/gesha/static/gesha/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.449609 django-gesha-0.1a1/gesha/static/gesha/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.461609 django-gesha-0.1a1/gesha/static/gesha/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/static/gesha/dist/js/django-gesha.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.465610 django-gesha-0.1a1/gesha/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/templatetags/gesha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gulpfile.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.465610 django-gesha-0.1a1/js_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_src/context.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_src/converters.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_src/main.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_src/urls.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.465610 django-gesha-0.1a1/js_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_tests/context.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_tests/converters.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_tests/helpers.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_tests/main.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_tests/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_tests/urls.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-08 22:20:01.000000 django-gesha-0.1a1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   342194 2023-05-08 22:20:01.000000 django-gesha-0.1a1/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-08 22:20:01.000000 django-gesha-0.1a1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-08 22:20:01.000000 django-gesha-0.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 22:20:13.469610 django-gesha-0.1a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.465610 django-gesha-0.1a1/test_project/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.469610 django-gesha-0.1a1/test_project/fake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.469610 django-gesha-0.1a1/test_project/fake/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.469610 django-gesha-0.1a1/test_project/fake/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/management/commands/printtestpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.469610 django-gesha-0.1a1/test_project/fake/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/templates/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.469610 django-gesha-0.1a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tests/test_jscontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tests/test_package_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tsconfig.json
```

### Comparing `django-gesha-0.1a0/.github/workflows/python-publish.yml` & `django-gesha-0.1a1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a0/.github/workflows/test.yml` & `django-gesha-0.1a1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a0/.gitignore` & `django-gesha-0.1a1/.gitignore`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a0/LICENSE` & `django-gesha-0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a0/docs/installation.md` & `django-gesha-0.1a1/docs/installation.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,47 @@
 ## Install to Python environment using pip
 
-```sh
-pip install django-gesha
+``` console
+$ pip install django-gesha
 ```
 
 ## Install app in Django project
 
-Add `gesha` to [`INSTALLED_APPS`](https://docs.djangoproject.com/en/4.2/ref/settings/#installed-apps) in your Django project's
-[settings](https://docs.djangoproject.com/en/4.2/topics/settings/):
-```py
+Add `gesha` to
+[`INSTALLED_APPS`](https://docs.djangoproject.com/en/stable/ref/settings/#installed-apps)
+in your Django project's
+[settings](https://docs.djangoproject.com/en/stable/topics/settings/):
+
+``` py title="settings.py" hl_lines="3"
 INSTALLED_APPS = [
     ...
     "gesha",
 ]
 ```
 
 ## Collect JavaScript assets
 
-Run the
-[`collectstatic`](https://docs.djangoproject.com/en/4.2/ref/contrib/staticfiles/#collectstatic)
-management command to collect django-gesha's JavaScript files. Django should locate
-them automatically once the [app is installed](#install-app-in-django-project).
-```sh
-python manage.py collectstatic
+Run [`collectstatic`](https://docs.djangoproject.com/en/stable/ref/contrib/staticfiles/#collectstatic)
+to collect **django-gesha**'s JavaScript files.
+
+``` console
+$ python manage.py collectstatic
 ```
+
+??? tip "Static file discovery"
+
+    Django should locate **django-gesha**'s JavaScript files automatically once the
+    [app is installed](#install-app-in-django-project).
+
+    To check that the JavaScript bundle has been collected:
+
+    === "POSIX"
+
+        ``` console
+        $ python manage.py findstatic gesha/dist/js/django-gesha.bundle.min.js
+        ```
+
+    === "Windows"
+
+        ``` doscon
+        C:\> python manage.py findstatic gesha\dist\js\django-gesha.bundle.min.js
+        ```
```

### Comparing `django-gesha-0.1a0/gesha/templatetags/gesha.py` & `django-gesha-0.1a1/gesha/templatetags/gesha.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 import typing
 
 from django import template
 from django.utils.html import json_script
 
-from gesha.settings import get_js_context_key
+from gesha.conf import get_setting
 
 logger = logging.getLogger(__name__)
 register = template.Library()
 
 
 @register.simple_tag(takes_context=True)
 def jscontext(context: typing.Mapping) -> str:
-    js_context_key = get_js_context_key()
+    js_context_key = get_setting("GESHA_JSCONTEXT_KEY")
     try:
         js_context = context[js_context_key]
     except KeyError:
         logger.warning(
             "Template tag 'gesha' used, but context dict did not contain key "
             f"'{js_context_key}'."
         )
```

### Comparing `django-gesha-0.1a0/gulpfile.js` & `django-gesha-0.1a1/gulpfile.js`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a0/js_tests/helpers.ts` & `django-gesha-0.1a1/js_tests/helpers.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a0/package-lock.json` & `django-gesha-0.1a1/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8999922744128555%*

 * *Differences: {"'packages'": "{'': {'version': '0.1.0-alpha1'}}", "'version'": "'0.1.0-alpha1'"}*

```diff
@@ -23,15 +23,15 @@
                 "typescript": "^5.0.4",
                 "vinyl-buffer": "^1.0.1",
                 "vinyl-source-stream": "^2.0.0",
                 "watchify": "^4.0.0"
             },
             "license": "MIT",
             "name": "django-gesha",
-            "version": "0.1.0-alpha0"
+            "version": "0.1.0-alpha1"
         },
         "node_modules/@cspotcode/source-map-support": {
             "dependencies": {
                 "@jridgewell/trace-mapping": "0.3.9"
             },
             "dev": true,
             "engines": {
@@ -9298,9 +9298,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "0.1.0-alpha0"
+    "version": "0.1.0-alpha1"
 }
```

### Comparing `django-gesha-0.1a0/package.json` & `django-gesha-0.1a1/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.1.0-alpha1'"}*

```diff
@@ -37,9 +37,9 @@
         "type": "git",
         "url": "git+https://github.com/ely-as/django-gesha.git"
     },
     "scripts": {
         "lint": "eslint ./js_*/**/*.ts",
         "test": "mocha"
     },
-    "version": "0.1.0-alpha0"
+    "version": "0.1.0-alpha1"
 }
```

### Comparing `django-gesha-0.1a0/pyproject.toml` & `django-gesha-0.1a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
     {name = "elyas", email = "elyas@ely.as"},
 ]
 description = "JavaScript utilities for Django projects."
 requires-python = ">=3.8"
 keywords = ["django", "javascript"]
 license = {text = "MIT"}
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
+    "Programming Language :: JavaScript",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
@@ -62,29 +63,29 @@
     "pytest>=7",      # >=7 required for pythonpath option
     "pytest-cov",
     "pytest-django",
     "ruff",
 ]
 
 [tool.coverage.run]
-omit = ["tests/fake_project/*"]
+omit = ["test_project/*"]
 
 [tool.mypy]
 warn_unused_configs = true
 ignore_missing_imports = true
 files = [
     "gesha/**/*.py",
     "tests/**/*.py",
 ]
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "fake.settings"
 pythonpath = [
   ".",
-  "tests/fake_project",
+  "test_project",
 ]
 
 [tool.ruff]
 select = [
     "F",     # Pyflakes
     "E",     # pycodestyle errors
     "W",     # pycodestyle warnings
```

### Comparing `django-gesha-0.1a0/tests/fake_project/fake/settings.py` & `django-gesha-0.1a1/test_project/fake/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 BASE_DIR = Path(__file__).resolve().parent.parent
 
 SECRET_KEY = get_random_secret_key()
 
 DEBUG = True
 
+ALLOWED_HOSTS = ["*"]
+
 
 # Application definition
 
 INSTALLED_APPS = [
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
```

### Comparing `django-gesha-0.1a0/tests/fake_project/manage.py` & `django-gesha-0.1a1/test_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a0/tests/test_jscontext.py` & `django-gesha-0.1a1/tests/test_jscontext.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a0/tests/test_package_json.py` & `django-gesha-0.1a1/tests/test_package_json.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a0/tox.ini` & `django-gesha-0.1a1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -26,12 +26,12 @@
     py39-django22: Django>=2.2.17
     py39-django30: Django>=3.0.11
     py39-django31: Django>=3.1.3
     py310-django32: Django>=3.2.9
     py311-django41: Django>=4.1.3
 commands =
     format: black {toxinidir} {posargs}
-    format: ruff check --fix {toxinidir} {posargs}
+    format: ruff check --select I --fix {toxinidir} {posargs}
     lint: black {toxinidir} --check --diff {posargs}
     lint: ruff check {toxinidir} {posargs}
     test: pytest --cov={toxinidir} --cov-report=term --cov-report=xml {posargs}
     type: mypy {posargs}
```

