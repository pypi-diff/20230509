# Comparing `tmp/django-webuild_ds-0.0.1.tar.gz` & `tmp/django-webuild_ds-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webuild_ds-0.0.1.tar", last modified: Tue Jan 31 00:00:11 2023, max compression
+gzip compressed data, was "django-webuild_ds-0.0.2.tar", last modified: Tue May  9 02:04:52 2023, max compression
```

## Comparing `django-webuild_ds-0.0.1.tar` & `django-webuild_ds-0.0.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.901044 django-webuild_ds-0.0.1/
--rw-rw-rw-   0        0        0     1093 2023-01-20 02:10:20.000000 django-webuild_ds-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      270 2023-01-20 02:16:08.000000 django-webuild_ds-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3123 2023-01-31 00:00:11.901044 django-webuild_ds-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2621 2023-01-20 02:28:16.000000 django-webuild_ds-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.376267 django-webuild_ds-0.0.1/django_webuild_ds.egg-info/
--rw-rw-rw-   0        0        0     3123 2023-01-31 00:00:11.000000 django-webuild_ds-0.0.1/django_webuild_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4731 2023-01-31 00:00:11.000000 django-webuild_ds-0.0.1/django_webuild_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 00:00:11.000000 django-webuild_ds-0.0.1/django_webuild_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-01-31 00:00:11.000000 django-webuild_ds-0.0.1/django_webuild_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-01-31 00:00:11.000000 django-webuild_ds-0.0.1/django_webuild_ds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2023-01-20 02:10:20.000000 django-webuild_ds-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      750 2023-01-31 00:00:11.902083 django-webuild_ds-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-01-20 02:10:20.000000 django-webuild_ds-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.418437 django-webuild_ds-0.0.1/webuild/
--rw-rw-rw-   0        0        0        0 2023-01-20 02:10:20.000000 django-webuild_ds-0.0.1/webuild/__init__.py
--rw-rw-rw-   0        0        0       63 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/admin.py
--rw-rw-rw-   0        0        0      146 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/apps.py
--rw-rw-rw-   0        0        0      993 2023-01-30 08:36:34.000000 django-webuild_ds-0.0.1/webuild/forms.py
--rw-rw-rw-   0        0        0       57 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/models.py
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.334135 django-webuild_ds-0.0.1/webuild/static/
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.335866 django-webuild_ds-0.0.1/webuild/static/webuild/
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.425457 django-webuild_ds-0.0.1/webuild/static/webuild/css/
--rw-rw-rw-   0        0        0     7737 2023-01-20 02:12:22.000000 django-webuild_ds-0.0.1/webuild/static/webuild/css/style.css
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.441723 django-webuild_ds-0.0.1/webuild/static/webuild/img/
--rw-rw-rw-   0        0        0     1738 2023-01-20 02:10:20.000000 django-webuild_ds-0.0.1/webuild/static/webuild/img/apple-touch-icon.png
--rw-rw-rw-   0        0        0      491 2023-01-20 02:10:20.000000 django-webuild_ds-0.0.1/webuild/static/webuild/img/favicon.png
--rw-rw-rw-   0        0        0   296179 2023-01-20 02:12:22.000000 django-webuild_ds-0.0.1/webuild/static/webuild/img/hero-bg.jpg
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.454697 django-webuild_ds-0.0.1/webuild/static/webuild/js/
--rw-rw-rw-   0        0        0    89501 2023-01-30 08:36:05.000000 django-webuild_ds-0.0.1/webuild/static/webuild/js/jquery-3.6.0.min.js
--rw-rw-rw-   0        0        0     3252 2023-01-30 08:36:05.000000 django-webuild_ds-0.0.1/webuild/static/webuild/js/jquery.cookie.js
--rw-rw-rw-   0        0        0     1358 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/js/main.js
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.465968 django-webuild_ds-0.0.1/webuild/static/webuild/scss/
--rw-rw-rw-   0        0        0      454 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/scss/_footer.scss
--rw-rw-rw-   0        0        0      403 2023-01-20 02:10:55.000000 django-webuild_ds-0.0.1/webuild/static/webuild/scss/_general.scss
--rw-rw-rw-   0        0        0      892 2023-01-20 02:10:55.000000 django-webuild_ds-0.0.1/webuild/static/webuild/scss/_header.scss
--rw-rw-rw-   0        0        0     3131 2023-01-20 02:10:55.000000 django-webuild_ds-0.0.1/webuild/static/webuild/scss/_hero.scss
--rw-rw-rw-   0        0        0     2827 2023-01-20 02:10:55.000000 django-webuild_ds-0.0.1/webuild/static/webuild/scss/_sections.scss
--rw-rw-rw-   0        0        0      727 2023-01-20 02:10:55.000000 django-webuild_ds-0.0.1/webuild/static/webuild/scss/_variables.scss
--rw-rw-rw-   0        0        0      120 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/scss/style.scss
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.338489 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.337401 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.672447 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/
--rw-rw-rw-   0        0        0    71861 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0   210357 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0    53265 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0   131395 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-rw-   0        0        0    71935 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-rw-   0        0        0   210361 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-rw-   0        0        0    53340 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-rw-   0        0        0   131472 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-rw-   0        0        0     7965 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0   110875 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0     6490 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0    40331 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-rw-   0        0        0     7958 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-rw-   0        0        0   110888 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-rw-   0        0        0     6562 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-rw-   0        0        0    48693 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-rw-   0        0        0    76347 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.css
--rw-rw-rw-   0        0        0   212450 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-rw-   0        0        0    58266 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-rw-   0        0        0   131956 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-rw-   0        0        0    76214 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-rw-   0        0        0   212393 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-rw-   0        0        0    58194 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-rw-   0        0        0   131791 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-rw-   0        0        0   237950 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.css
--rw-rw-rw-   0        0        0   608300 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   194901 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   522639 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0   237528 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.css
--rw-rw-rw-   0        0        0   608144 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-rw-   0        0        0   195007 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-rw-   0        0        0   767483 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.849427 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/
--rw-rw-rw-   0        0        0   207989 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0   451770 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-rw-   0        0        0    80420 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   333078 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0   136215 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.js
--rw-rw-rw-   0        0        0   308207 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-rw-rw-   0        0        0    73978 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-rw-rw-   0        0        0   221179 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-rw-   0        0        0   145543 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.js
--rw-rw-rw-   0        0        0   309348 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.js.map
--rw-rw-rw-   0        0        0    60404 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   216913 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.min.js.map
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.482412 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap-icons/
--rw-rw-rw-   0        0        0    95609 2023-01-20 02:12:22.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap-icons/bootstrap-icons.css
--rw-rw-rw-   0        0        0    51087 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap-icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   228090 2023-01-20 02:12:22.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap-icons/bootstrap-icons.scss
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.498088 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap-icons/fonts/
--rw-rw-rw-   0        0        0   164352 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-rw-rw-   0        0        0   121296 2023-01-20 02:12:22.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.863784 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/php-email-form/
--rw-rw-rw-   0        0        0   232688 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/php-email-form/php-email-form.php
--rw-rw-rw-   0        0        0     2590 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.1/webuild/static/webuild/vendor/php-email-form/validate.js
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.338992 django-webuild_ds-0.0.1/webuild/templates/
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.896109 django-webuild_ds-0.0.1/webuild/templates/webuild/
--rw-rw-rw-   0        0        0     2188 2023-01-30 08:36:34.000000 django-webuild_ds-0.0.1/webuild/templates/webuild/_contact.html
--rw-rw-rw-   0        0        0     2059 2023-01-30 08:36:34.000000 django-webuild_ds-0.0.1/webuild/templates/webuild/_hero.html
--rw-rw-rw-   0        0        0      250 2023-01-20 04:30:42.000000 django-webuild_ds-0.0.1/webuild/templates/webuild/footer.html
--rw-rw-rw-   0        0        0      724 2023-01-30 08:36:34.000000 django-webuild_ds-0.0.1/webuild/templates/webuild/header.html
--rw-rw-rw-   0        0        0     1671 2023-01-30 08:36:34.000000 django-webuild_ds-0.0.1/webuild/templates/webuild/index.html
--rw-rw-rw-   0        0        0     1460 2023-01-20 03:07:09.000000 django-webuild_ds-0.0.1/webuild/templates/webuild/seo.html
-drwxrwxrwx   0        0        0        0 2023-01-31 00:00:11.898925 django-webuild_ds-0.0.1/webuild/templatetags/
--rw-rw-rw-   0        0        0        0 2023-01-20 03:02:18.000000 django-webuild_ds-0.0.1/webuild/templatetags/__init__.py
--rw-rw-rw-   0        0        0      951 2023-01-30 08:36:29.000000 django-webuild_ds-0.0.1/webuild/templatetags/webuild_tags.py
--rw-rw-rw-   0        0        0       60 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.1/webuild/tests.py
--rw-rw-rw-   0        0        0      221 2023-01-20 02:43:24.000000 django-webuild_ds-0.0.1/webuild/urls.py
--rw-rw-rw-   0        0        0     4649 2023-01-30 08:36:29.000000 django-webuild_ds-0.0.1/webuild/views.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.554075 django-webuild_ds-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-01-20 02:10:20.000000 django-webuild_ds-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      270 2023-01-20 02:16:08.000000 django-webuild_ds-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3123 2023-05-09 02:04:52.554075 django-webuild_ds-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2621 2023-01-20 02:28:16.000000 django-webuild_ds-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.432832 django-webuild_ds-0.0.2/django_webuild_ds.egg-info/
+-rw-rw-rw-   0        0        0     3123 2023-05-09 02:04:52.000000 django-webuild_ds-0.0.2/django_webuild_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4731 2023-05-09 02:04:52.000000 django-webuild_ds-0.0.2/django_webuild_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 02:04:52.000000 django-webuild_ds-0.0.2/django_webuild_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-05-09 02:04:52.000000 django-webuild_ds-0.0.2/django_webuild_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-09 02:04:52.000000 django-webuild_ds-0.0.2/django_webuild_ds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2023-01-20 02:10:20.000000 django-webuild_ds-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      750 2023-05-09 02:04:52.556201 django-webuild_ds-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-01-20 02:10:20.000000 django-webuild_ds-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.441338 django-webuild_ds-0.0.2/webuild/
+-rw-rw-rw-   0        0        0        0 2023-01-20 02:10:20.000000 django-webuild_ds-0.0.2/webuild/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/admin.py
+-rw-rw-rw-   0        0        0      146 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/apps.py
+-rw-rw-rw-   0        0        0      993 2023-01-30 08:36:34.000000 django-webuild_ds-0.0.2/webuild/forms.py
+-rw-rw-rw-   0        0        0       57 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/models.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.401532 django-webuild_ds-0.0.2/webuild/static/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.402597 django-webuild_ds-0.0.2/webuild/static/webuild/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.442487 django-webuild_ds-0.0.2/webuild/static/webuild/css/
+-rw-rw-rw-   0        0        0     7737 2023-01-20 02:12:22.000000 django-webuild_ds-0.0.2/webuild/static/webuild/css/style.css
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.459326 django-webuild_ds-0.0.2/webuild/static/webuild/img/
+-rw-rw-rw-   0        0        0     1738 2023-01-20 02:10:20.000000 django-webuild_ds-0.0.2/webuild/static/webuild/img/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      491 2023-01-20 02:10:20.000000 django-webuild_ds-0.0.2/webuild/static/webuild/img/favicon.png
+-rw-rw-rw-   0        0        0   296179 2023-01-20 02:12:22.000000 django-webuild_ds-0.0.2/webuild/static/webuild/img/hero-bg.jpg
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.463335 django-webuild_ds-0.0.2/webuild/static/webuild/js/
+-rw-rw-rw-   0        0        0    89501 2023-01-30 08:36:05.000000 django-webuild_ds-0.0.2/webuild/static/webuild/js/jquery-3.6.0.min.js
+-rw-rw-rw-   0        0        0     3252 2023-01-30 08:36:05.000000 django-webuild_ds-0.0.2/webuild/static/webuild/js/jquery.cookie.js
+-rw-rw-rw-   0        0        0     1358 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/js/main.js
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.469911 django-webuild_ds-0.0.2/webuild/static/webuild/scss/
+-rw-rw-rw-   0        0        0      454 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/scss/_footer.scss
+-rw-rw-rw-   0        0        0      403 2023-01-20 02:10:55.000000 django-webuild_ds-0.0.2/webuild/static/webuild/scss/_general.scss
+-rw-rw-rw-   0        0        0      892 2023-01-20 02:10:55.000000 django-webuild_ds-0.0.2/webuild/static/webuild/scss/_header.scss
+-rw-rw-rw-   0        0        0     3131 2023-01-20 02:10:55.000000 django-webuild_ds-0.0.2/webuild/static/webuild/scss/_hero.scss
+-rw-rw-rw-   0        0        0     2827 2023-01-20 02:10:55.000000 django-webuild_ds-0.0.2/webuild/static/webuild/scss/_sections.scss
+-rw-rw-rw-   0        0        0      727 2023-01-20 02:10:55.000000 django-webuild_ds-0.0.2/webuild/static/webuild/scss/_variables.scss
+-rw-rw-rw-   0        0        0      120 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/scss/style.scss
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.403910 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.403910 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.522446 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/
+-rw-rw-rw-   0        0        0    71861 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0   210357 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0    53265 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0   131395 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-rw-   0        0        0    71935 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-rw-   0        0        0   210361 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-rw-   0        0        0    53340 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-rw-   0        0        0   131472 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-rw-   0        0        0     7965 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0   110875 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0     6490 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0    40331 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-rw-   0        0        0     7958 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-rw-   0        0        0   110888 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-rw-   0        0        0     6562 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-rw-   0        0        0    48693 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-rw-   0        0        0    76347 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0   212450 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-rw-   0        0        0    58266 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-rw-   0        0        0   131956 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-rw-   0        0        0    76214 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-rw-   0        0        0   212393 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-rw-   0        0        0    58194 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-rw-   0        0        0   131791 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-rw-   0        0        0   237950 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0        0        0   608300 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   194901 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   522639 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0   237528 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-rw-rw-   0        0        0   608144 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-rw-   0        0        0   195007 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-rw-   0        0        0   767483 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.541155 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/
+-rw-rw-rw-   0        0        0   207989 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0   451770 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-rw-   0        0        0    80420 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   333078 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0   136215 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.js
+-rw-rw-rw-   0        0        0   308207 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-rw-   0        0        0    73978 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-rw-   0        0        0   221179 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-rw-   0        0        0   145543 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0        0        0   309348 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.js.map
+-rw-rw-rw-   0        0        0    60404 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0   216913 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.min.js.map
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.473284 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap-icons/
+-rw-rw-rw-   0        0        0    95609 2023-01-20 02:12:22.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-rw-rw-   0        0        0    51087 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   228090 2023-01-20 02:12:22.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap-icons/bootstrap-icons.scss
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.475901 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap-icons/fonts/
+-rw-rw-rw-   0        0        0   164352 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-rw-rw-   0        0        0   121296 2023-01-20 02:12:22.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.544461 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/php-email-form/
+-rw-rw-rw-   0        0        0   232688 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/php-email-form/php-email-form.php
+-rw-rw-rw-   0        0        0     2590 2023-01-20 02:11:08.000000 django-webuild_ds-0.0.2/webuild/static/webuild/vendor/php-email-form/validate.js
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.405017 django-webuild_ds-0.0.2/webuild/templates/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.550930 django-webuild_ds-0.0.2/webuild/templates/webuild/
+-rw-rw-rw-   0        0        0     2188 2023-01-30 08:36:34.000000 django-webuild_ds-0.0.2/webuild/templates/webuild/_contact.html
+-rw-rw-rw-   0        0        0     2059 2023-01-30 08:36:34.000000 django-webuild_ds-0.0.2/webuild/templates/webuild/_hero.html
+-rw-rw-rw-   0        0        0      340 2023-05-09 02:04:38.000000 django-webuild_ds-0.0.2/webuild/templates/webuild/footer.html
+-rw-rw-rw-   0        0        0      724 2023-01-30 08:36:34.000000 django-webuild_ds-0.0.2/webuild/templates/webuild/header.html
+-rw-rw-rw-   0        0        0     1671 2023-01-30 08:36:34.000000 django-webuild_ds-0.0.2/webuild/templates/webuild/index.html
+-rw-rw-rw-   0        0        0     1460 2023-01-20 03:07:09.000000 django-webuild_ds-0.0.2/webuild/templates/webuild/seo.html
+drwxrwxrwx   0        0        0        0 2023-05-09 02:04:52.553043 django-webuild_ds-0.0.2/webuild/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-01-20 03:02:18.000000 django-webuild_ds-0.0.2/webuild/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      951 2023-01-30 08:36:29.000000 django-webuild_ds-0.0.2/webuild/templatetags/webuild_tags.py
+-rw-rw-rw-   0        0        0       60 2023-01-20 02:12:23.000000 django-webuild_ds-0.0.2/webuild/tests.py
+-rw-rw-rw-   0        0        0      221 2023-01-20 02:43:24.000000 django-webuild_ds-0.0.2/webuild/urls.py
+-rw-rw-rw-   0        0        0     4649 2023-01-30 08:36:29.000000 django-webuild_ds-0.0.2/webuild/views.py
```

### Comparing `django-webuild_ds-0.0.1/LICENSE` & `django-webuild_ds-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/PKG-INFO` & `django-webuild_ds-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webuild_ds
-Version: 0.0.1
+Version: 0.0.2
 Summary: webuild_pro porting for django
 Home-page: https://www.demiansoft.com
 Author: hyungjin kim
 Author-email: hj3415@gmail.com
 Project-URL: Bug Tracker, https://pypi.org/project/util-demian/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-webuild_ds-0.0.1/README.md` & `django-webuild_ds-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/django_webuild_ds.egg-info/PKG-INFO` & `django-webuild_ds-0.0.2/django_webuild_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webuild-ds
-Version: 0.0.1
+Version: 0.0.2
 Summary: webuild_pro porting for django
 Home-page: https://www.demiansoft.com
 Author: hyungjin kim
 Author-email: hj3415@gmail.com
 Project-URL: Bug Tracker, https://pypi.org/project/util-demian/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-webuild_ds-0.0.1/django_webuild_ds.egg-info/SOURCES.txt` & `django-webuild_ds-0.0.2/django_webuild_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/setup.cfg` & `django-webuild_ds-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 7765 6275 696c   = django-webuil
 00000020: 645f 6473 0d0a 7665 7273 696f 6e20 3d20  d_ds..version = 
-00000030: 302e 302e 310d 0a61 7574 686f 7220 3d20  0.0.1..author = 
+00000030: 302e 302e 320d 0a61 7574 686f 7220 3d20  0.0.2..author = 
 00000040: 6879 756e 676a 696e 206b 696d 0d0a 6175  hyungjin kim..au
 00000050: 7468 6f72 5f65 6d61 696c 203d 2068 6a33  thor_email = hj3
 00000060: 3431 3540 676d 6169 6c2e 636f 6d0d 0a64  415@gmail.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2077 6562  escription = web
 00000080: 7569 6c64 5f70 726f 2070 6f72 7469 6e67  uild_pro porting
 00000090: 2066 6f72 2064 6a61 6e67 6f0d 0a6c 6f6e   for django..lon
 000000a0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description =
```

### Comparing `django-webuild_ds-0.0.1/webuild/forms.py` & `django-webuild_ds-0.0.2/webuild/forms.py`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/css/style.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/css/style.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/img/apple-touch-icon.png` & `django-webuild_ds-0.0.2/webuild/static/webuild/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/img/hero-bg.jpg` & `django-webuild_ds-0.0.2/webuild/static/webuild/img/hero-bg.jpg`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/js/jquery-3.6.0.min.js` & `django-webuild_ds-0.0.2/webuild/static/webuild/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/js/jquery.cookie.js` & `django-webuild_ds-0.0.2/webuild/static/webuild/js/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/js/main.js` & `django-webuild_ds-0.0.2/webuild/static/webuild/js/main.js`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/scss/_header.scss` & `django-webuild_ds-0.0.2/webuild/static/webuild/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/scss/_hero.scss` & `django-webuild_ds-0.0.2/webuild/static/webuild/scss/_hero.scss`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/scss/_sections.scss` & `django-webuild_ds-0.0.2/webuild/static/webuild/scss/_sections.scss`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/scss/_variables.scss` & `django-webuild_ds-0.0.2/webuild/static/webuild/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.min.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.min.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.min.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.js` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.js` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.js.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.min.js` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.js` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.js.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.min.js` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap/js/bootstrap.min.js.map` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap-icons/bootstrap-icons.css` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap-icons/bootstrap-icons.json` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap-icons/bootstrap-icons.scss` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/php-email-form/php-email-form.php` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/static/webuild/vendor/php-email-form/validate.js` & `django-webuild_ds-0.0.2/webuild/static/webuild/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/templates/webuild/_contact.html` & `django-webuild_ds-0.0.2/webuild/templates/webuild/_contact.html`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/templates/webuild/_hero.html` & `django-webuild_ds-0.0.2/webuild/templates/webuild/_hero.html`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/templates/webuild/header.html` & `django-webuild_ds-0.0.2/webuild/templates/webuild/header.html`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/templates/webuild/index.html` & `django-webuild_ds-0.0.2/webuild/templates/webuild/index.html`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/templates/webuild/seo.html` & `django-webuild_ds-0.0.2/webuild/templates/webuild/seo.html`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/templatetags/webuild_tags.py` & `django-webuild_ds-0.0.2/webuild/templatetags/webuild_tags.py`

 * *Files identical despite different names*

### Comparing `django-webuild_ds-0.0.1/webuild/views.py` & `django-webuild_ds-0.0.2/webuild/views.py`

 * *Files identical despite different names*

