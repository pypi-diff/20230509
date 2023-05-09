# Comparing `tmp/django-mentor_ds_myenglish-1.0.0.tar.gz` & `tmp/django-mentor_ds_myenglish-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mentor_ds_myenglish-1.0.0.tar", last modified: Tue Feb  7 07:28:31 2023, max compression
+gzip compressed data, was "django-mentor_ds_myenglish-1.0.1.tar", last modified: Tue May  9 01:36:46 2023, max compression
```

## Comparing `django-mentor_ds_myenglish-1.0.0.tar` & `django-mentor_ds_myenglish-1.0.1.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.654206 django-mentor_ds_myenglish-1.0.0/
--rw-rw-rw-   0        0        0     1093 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      267 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2817 2023-02-07 07:28:31.655207 django-mentor_ds_myenglish-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2307 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.464096 django-mentor_ds_myenglish-1.0.0/django_mentor_ds_myenglish.egg-info/
--rw-rw-rw-   0        0        0     2817 2023-02-07 07:28:31.000000 django-mentor_ds_myenglish-1.0.0/django_mentor_ds_myenglish.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6362 2023-02-07 07:28:31.000000 django-mentor_ds_myenglish-1.0.0/django_mentor_ds_myenglish.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 07:28:31.000000 django-mentor_ds_myenglish-1.0.0/django_mentor_ds_myenglish.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-02-07 07:28:31.000000 django-mentor_ds_myenglish-1.0.0/django_mentor_ds_myenglish.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-02-07 07:28:31.000000 django-mentor_ds_myenglish-1.0.0/django_mentor_ds_myenglish.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.474099 django-mentor_ds_myenglish-1.0.0/mentor/
--rw-rw-rw-   0        0        0        0 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/__init__.py
--rw-rw-rw-   0        0        0       66 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/admin.py
--rw-rw-rw-   0        0        0      150 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/apps.py
--rw-rw-rw-   0        0        0     1178 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/forms.py
--rw-rw-rw-   0        0        0       60 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/models.py
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.429858 django-mentor_ds_myenglish-1.0.0/mentor/static/
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.430750 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.475103 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/js/
--rw-rw-rw-   0        0        0     4545 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/js/main.js
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.484775 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/
--rw-rw-rw-   0        0        0     3301 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_footer.scss
--rw-rw-rw-   0        0        0     2019 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_general.scss
--rw-rw-rw-   0        0        0     1012 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_header.scss
--rw-rw-rw-   0        0        0     1462 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_hero.scss
--rw-rw-rw-   0        0        0     3743 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_nav.scss
--rw-rw-rw-   0        0        0    17426 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_sections.scss
--rw-rw-rw-   0        0        0      498 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_variables.scss
--rw-rw-rw-   0        0        0      136 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/style.scss
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.438371 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.490261 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/animate.css/
--rw-rw-rw-   0        0        0    70607 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/animate.css/animate.compat.css
--rw-rw-rw-   0        0        0    95374 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/animate.css/animate.css
--rw-rw-rw-   0        0        0    71750 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/animate.css/animate.min.css
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.493286 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/aos/
--rw-rw-rw-   0        0        0    26053 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/aos/aos.css
--rw-rw-rw-   0        0        0    14690 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/aos/aos.js
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.435290 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.557716 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/
--rw-rw-rw-   0        0        0    71861 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0   210292 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0    53265 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0   131408 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-rw-   0        0        0    71935 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-rw-   0        0        0   210296 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-rw-   0        0        0    53340 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-rw-   0        0        0   131485 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-rw-   0        0        0     7965 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0   110811 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0     6490 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0    40345 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-rw-   0        0        0     7958 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-rw-   0        0        0   110824 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-rw-   0        0        0     6562 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-rw-   0        0        0    48707 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-rw-   0        0        0    74135 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.css
--rw-rw-rw-   0        0        0   196370 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-rw-   0        0        0    56365 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-rw-   0        0        0   115601 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-rw-   0        0        0    74002 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-rw-   0        0        0   196313 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-rw-   0        0        0    56293 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-rw-   0        0        0   115436 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-rw-   0        0        0   237872 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.css
--rw-rw-rw-   0        0        0   606249 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   194699 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   521459 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0   237386 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.css
--rw-rw-rw-   0        0        0   606069 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-rw-   0        0        0   194803 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-rw-   0        0        0   765329 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.581741 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/
--rw-rw-rw-   0        0        0   207083 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0   448881 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-rw-   0        0        0    79790 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   330849 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0   135367 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.js
--rw-rw-rw-   0        0        0   306814 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-rw-rw-   0        0        0    73539 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-rw-rw-   0        0        0   220143 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-rw-   0        0        0   144701 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.js
--rw-rw-rw-   0        0        0   307954 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.js.map
--rw-rw-rw-   0        0        0    60104 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   215897 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.min.js.map
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.499464 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/
--rw-rw-rw-   0        0        0    88585 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/bootstrap-icons.css
--rw-rw-rw-   0        0        0    47187 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   211136 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/bootstrap-icons.scss
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.502801 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/fonts/
--rw-rw-rw-   0        0        0   150592 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-rw-rw-   0        0        0   112440 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-rw-rw-   0        0        0   218010 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/index.html
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.436293 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.588490 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/css/
--rw-rw-rw-   0        0        0     7522 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/css/animations.css
--rw-rw-rw-   0        0        0    92272 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/css/boxicons.css
--rw-rw-rw-   0        0        0    66571 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/css/boxicons.min.css
--rw-rw-rw-   0        0        0      683 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/css/transformations.css
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.598401 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/fonts/
--rw-rw-rw-   0        0        0   396413 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/fonts/boxicons.eot
--rw-rw-rw-   0        0        0  1216389 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/fonts/boxicons.svg
--rw-rw-rw-   0        0        0   313836 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/fonts/boxicons.ttf
--rw-rw-rw-   0        0        0   313912 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/fonts/boxicons.woff
--rw-rw-rw-   0        0        0   115388 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/fonts/boxicons.woff2
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.603148 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/php-email-form/
--rw-rw-rw-   0        0        0   232262 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/php-email-form/php-email-form.php
--rw-rw-rw-   0        0        0     2731 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/php-email-form/validate.js
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.605782 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/purecounter/
--rw-rw-rw-   0        0        0     4958 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/purecounter/purecounter.js
--rw-rw-rw-   0        0        0     5417 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/purecounter/purecounter_vanilla.js
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.620624 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/
--rw-rw-rw-   0        0        0   110438 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.css
--rw-rw-rw-   0        0        0   403228 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.eot
--rw-rw-rw-   0        0        0   110450 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.less
--rw-rw-rw-   0        0        0  1195522 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.svg
--rw-rw-rw-   0        0        0   897931 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.symbol.svg
--rw-rw-rw-   0        0        0   403056 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.ttf
--rw-rw-rw-   0        0        0   172876 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.woff
--rw-rw-rw-   0        0        0   125268 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.woff2
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.625186 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/swiper/
--rw-rw-rw-   0        0        0    16466 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/swiper/swiper-bundle.min.css
--rw-rw-rw-   0        0        0   143070 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/swiper/swiper-bundle.min.js
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.438371 django-mentor_ds_myenglish-1.0.0/mentor/templates/
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.648465 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/
--rw-rw-rw-   0        0        0      863 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_about.html
--rw-rw-rw-   0        0        0     4552 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_contact.html
--rw-rw-rw-   0        0        0      482 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_counts.html
--rw-rw-rw-   0        0        0     1735 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_courses.html
--rw-rw-rw-   0        0        0     1101 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_cta.html
--rw-rw-rw-   0        0        0     1084 2023-02-07 07:24:38.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_events.html
--rw-rw-rw-   0        0        0     2791 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_faq.html
--rw-rw-rw-   0        0        0     1016 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_features.html
--rw-rw-rw-   0        0        0      694 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_hero.html
--rw-rw-rw-   0        0        0     2344 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_intro.html
--rw-rw-rw-   0        0        0     1274 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_testimonials.html
--rw-rw-rw-   0        0        0     1322 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_trainers.html
--rw-rw-rw-   0        0        0     1755 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_why_us.html
--rw-rw-rw-   0        0        0      612 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/analytics.html
--rw-rw-rw-   0        0        0     1733 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/footer.html
--rw-rw-rw-   0        0        0     2040 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/header.html
--rw-rw-rw-   0        0        0     4224 2023-02-07 07:18:28.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/index.html
--rw-rw-rw-   0        0        0     1522 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/seo.html
-drwxrwxrwx   0        0        0        0 2023-02-07 07:28:31.653203 django-mentor_ds_myenglish-1.0.0/mentor/templatetags/
--rw-rw-rw-   0        0        0        0 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/templatetags/__init__.py
--rw-rw-rw-   0        0        0     3540 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/templatetags/mentor_myenglish_tags.py
--rw-rw-rw-   0        0        0      435 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/templatetags/utils.py
--rw-rw-rw-   0        0        0      271 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/mentor/urls.py
--rw-rw-rw-   0        0        0     4031 2023-02-07 07:18:28.000000 django-mentor_ds_myenglish-1.0.0/mentor/views.py
--rw-rw-rw-   0        0        0      112 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      758 2023-02-07 07:28:31.656431 django-mentor_ds_myenglish-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:46.077611 django-mentor_ds_myenglish-1.0.1/
+-rw-rw-rw-   0        0        0     1093 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      267 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2817 2023-05-09 01:36:46.078645 django-mentor_ds_myenglish-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2307 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.935129 django-mentor_ds_myenglish-1.0.1/django_mentor_ds_myenglish.egg-info/
+-rw-rw-rw-   0        0        0     2817 2023-05-09 01:36:45.000000 django-mentor_ds_myenglish-1.0.1/django_mentor_ds_myenglish.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6362 2023-05-09 01:36:45.000000 django-mentor_ds_myenglish-1.0.1/django_mentor_ds_myenglish.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 01:36:45.000000 django-mentor_ds_myenglish-1.0.1/django_mentor_ds_myenglish.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-05-09 01:36:45.000000 django-mentor_ds_myenglish-1.0.1/django_mentor_ds_myenglish.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-09 01:36:45.000000 django-mentor_ds_myenglish-1.0.1/django_mentor_ds_myenglish.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.941749 django-mentor_ds_myenglish-1.0.1/mentor/
+-rw-rw-rw-   0        0        0        0 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/__init__.py
+-rw-rw-rw-   0        0        0       66 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/admin.py
+-rw-rw-rw-   0        0        0      150 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/apps.py
+-rw-rw-rw-   0        0        0     1178 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/forms.py
+-rw-rw-rw-   0        0        0       60 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/models.py
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.902652 django-mentor_ds_myenglish-1.0.1/mentor/static/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.903677 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.943048 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/js/
+-rw-rw-rw-   0        0        0     4545 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/js/main.js
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.951979 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/
+-rw-rw-rw-   0        0        0     3301 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_footer.scss
+-rw-rw-rw-   0        0        0     2019 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_general.scss
+-rw-rw-rw-   0        0        0     1012 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_header.scss
+-rw-rw-rw-   0        0        0     1462 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_hero.scss
+-rw-rw-rw-   0        0        0     3743 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_nav.scss
+-rw-rw-rw-   0        0        0    17426 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_sections.scss
+-rw-rw-rw-   0        0        0      498 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_variables.scss
+-rw-rw-rw-   0        0        0      136 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/style.scss
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.913220 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.955312 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/animate.css/
+-rw-rw-rw-   0        0        0    70607 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/animate.css/animate.compat.css
+-rw-rw-rw-   0        0        0    95374 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/animate.css/animate.css
+-rw-rw-rw-   0        0        0    71750 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/animate.css/animate.min.css
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.957482 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/aos/
+-rw-rw-rw-   0        0        0    26053 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/aos/aos.css
+-rw-rw-rw-   0        0        0    14690 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/aos/aos.js
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.907054 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:46.005869 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/
+-rw-rw-rw-   0        0        0    71861 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0   210292 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0    53265 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0   131408 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-rw-   0        0        0    71935 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-rw-   0        0        0   210296 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-rw-   0        0        0    53340 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-rw-   0        0        0   131485 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-rw-   0        0        0     7965 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0   110811 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0     6490 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0    40345 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-rw-   0        0        0     7958 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-rw-   0        0        0   110824 2022-11-26 09:41:49.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-rw-   0        0        0     6562 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-rw-   0        0        0    48707 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-rw-   0        0        0    74135 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0   196370 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-rw-   0        0        0    56365 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-rw-   0        0        0   115601 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-rw-   0        0        0    74002 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-rw-   0        0        0   196313 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-rw-   0        0        0    56293 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-rw-   0        0        0   115436 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-rw-   0        0        0   237872 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0        0        0   606249 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   194699 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   521459 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0   237386 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-rw-rw-   0        0        0   606069 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-rw-   0        0        0   194803 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-rw-   0        0        0   765329 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:46.023177 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/
+-rw-rw-rw-   0        0        0   207083 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0   448881 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-rw-   0        0        0    79790 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   330849 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0   135367 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.js
+-rw-rw-rw-   0        0        0   306814 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-rw-   0        0        0    73539 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-rw-   0        0        0   220143 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-rw-   0        0        0   144701 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0        0        0   307954 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.js.map
+-rw-rw-rw-   0        0        0    60104 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0   215897 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.min.js.map
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.962175 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/
+-rw-rw-rw-   0        0        0    88585 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-rw-rw-   0        0        0    47187 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   211136 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/bootstrap-icons.scss
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.964433 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/fonts/
+-rw-rw-rw-   0        0        0   150592 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-rw-rw-   0        0        0   112440 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-rw-rw-   0        0        0   218010 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/index.html
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.907054 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:46.028200 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/css/
+-rw-rw-rw-   0        0        0     7522 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/css/animations.css
+-rw-rw-rw-   0        0        0    92272 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/css/boxicons.css
+-rw-rw-rw-   0        0        0    66571 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/css/boxicons.min.css
+-rw-rw-rw-   0        0        0      683 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/css/transformations.css
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:46.036716 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/fonts/
+-rw-rw-rw-   0        0        0   396413 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/fonts/boxicons.eot
+-rw-rw-rw-   0        0        0  1216389 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/fonts/boxicons.svg
+-rw-rw-rw-   0        0        0   313836 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/fonts/boxicons.ttf
+-rw-rw-rw-   0        0        0   313912 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/fonts/boxicons.woff
+-rw-rw-rw-   0        0        0   115388 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/fonts/boxicons.woff2
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:46.039223 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/php-email-form/
+-rw-rw-rw-   0        0        0   232262 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/php-email-form/php-email-form.php
+-rw-rw-rw-   0        0        0     2731 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/php-email-form/validate.js
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:46.041396 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/purecounter/
+-rw-rw-rw-   0        0        0     4958 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/purecounter/purecounter.js
+-rw-rw-rw-   0        0        0     5417 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/purecounter/purecounter_vanilla.js
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:46.053520 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/
+-rw-rw-rw-   0        0        0   110438 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.css
+-rw-rw-rw-   0        0        0   403228 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.eot
+-rw-rw-rw-   0        0        0   110450 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.less
+-rw-rw-rw-   0        0        0  1195522 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.svg
+-rw-rw-rw-   0        0        0   897931 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.symbol.svg
+-rw-rw-rw-   0        0        0   403056 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.ttf
+-rw-rw-rw-   0        0        0   172876 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.woff
+-rw-rw-rw-   0        0        0   125268 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.woff2
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:46.055668 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/swiper/
+-rw-rw-rw-   0        0        0    16466 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/swiper/swiper-bundle.min.css
+-rw-rw-rw-   0        0        0   143070 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/swiper/swiper-bundle.min.js
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:45.914253 django-mentor_ds_myenglish-1.0.1/mentor/templates/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:46.074504 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/
+-rw-rw-rw-   0        0        0      863 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_about.html
+-rw-rw-rw-   0        0        0     4552 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_contact.html
+-rw-rw-rw-   0        0        0      482 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_counts.html
+-rw-rw-rw-   0        0        0     1735 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_courses.html
+-rw-rw-rw-   0        0        0     1101 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_cta.html
+-rw-rw-rw-   0        0        0     1084 2023-02-07 07:24:38.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_events.html
+-rw-rw-rw-   0        0        0     2791 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_faq.html
+-rw-rw-rw-   0        0        0     1016 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_features.html
+-rw-rw-rw-   0        0        0      694 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_hero.html
+-rw-rw-rw-   0        0        0     2344 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_intro.html
+-rw-rw-rw-   0        0        0     1274 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_testimonials.html
+-rw-rw-rw-   0        0        0     1322 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_trainers.html
+-rw-rw-rw-   0        0        0     1755 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_why_us.html
+-rw-rw-rw-   0        0        0      612 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/analytics.html
+-rw-rw-rw-   0        0        0     1823 2023-05-09 01:36:27.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/footer.html
+-rw-rw-rw-   0        0        0     2040 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/header.html
+-rw-rw-rw-   0        0        0     4224 2023-02-07 07:18:28.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/index.html
+-rw-rw-rw-   0        0        0     1522 2023-02-07 07:24:04.000000 django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/seo.html
+drwxrwxrwx   0        0        0        0 2023-05-09 01:36:46.077611 django-mentor_ds_myenglish-1.0.1/mentor/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     3540 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/templatetags/mentor_myenglish_tags.py
+-rw-rw-rw-   0        0        0      435 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/templatetags/utils.py
+-rw-rw-rw-   0        0        0      271 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/mentor/urls.py
+-rw-rw-rw-   0        0        0     4031 2023-02-07 07:18:28.000000 django-mentor_ds_myenglish-1.0.1/mentor/views.py
+-rw-rw-rw-   0        0        0      112 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      758 2023-05-09 01:36:46.079678 django-mentor_ds_myenglish-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-11-26 09:41:50.000000 django-mentor_ds_myenglish-1.0.1/setup.py
```

### Comparing `django-mentor_ds_myenglish-1.0.0/LICENSE` & `django-mentor_ds_myenglish-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/PKG-INFO` & `django-mentor_ds_myenglish-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mentor_ds_myenglish
-Version: 1.0.0
+Version: 1.0.1
 Summary: mentor_pro porting for django
 Home-page: https://www.demiansoft.com
 Author: hyungjin kim
 Author-email: hj3415@gmail.com
 Project-URL: Bug Tracker, https://pypi.org/project/util-demian/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-mentor_ds_myenglish-1.0.0/README.md` & `django-mentor_ds_myenglish-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/django_mentor_ds_myenglish.egg-info/PKG-INFO` & `django-mentor_ds_myenglish-1.0.1/django_mentor_ds_myenglish.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mentor-ds-myenglish
-Version: 1.0.0
+Version: 1.0.1
 Summary: mentor_pro porting for django
 Home-page: https://www.demiansoft.com
 Author: hyungjin kim
 Author-email: hj3415@gmail.com
 Project-URL: Bug Tracker, https://pypi.org/project/util-demian/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-mentor_ds_myenglish-1.0.0/django_mentor_ds_myenglish.egg-info/SOURCES.txt` & `django-mentor_ds_myenglish-1.0.1/django_mentor_ds_myenglish.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/forms.py` & `django-mentor_ds_myenglish-1.0.1/mentor/forms.py`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/js/main.js` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/js/main.js`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_footer.scss` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_general.scss` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_header.scss` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_hero.scss` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_hero.scss`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_nav.scss` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/scss/_sections.scss` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/scss/_sections.scss`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/animate.css/animate.compat.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/animate.css/animate.compat.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/animate.css/animate.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/animate.css/animate.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/animate.css/animate.min.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/animate.css/animate.min.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/aos/aos.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/aos/aos.js` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.min.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.min.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.min.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.js` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.js` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.js.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.min.js` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.js` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.js.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.min.js` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap/js/bootstrap.min.js.map` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/bootstrap-icons.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/bootstrap-icons.json` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/bootstrap-icons.scss` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/bootstrap-icons/index.html` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/bootstrap-icons/index.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/css/animations.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/css/animations.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/css/boxicons.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/css/boxicons.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/css/boxicons.min.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/css/boxicons.min.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/css/transformations.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/css/transformations.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/fonts/boxicons.eot` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/fonts/boxicons.eot`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/fonts/boxicons.svg` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/fonts/boxicons.svg`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/fonts/boxicons.ttf` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/fonts/boxicons.ttf`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/fonts/boxicons.woff` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/fonts/boxicons.woff`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/boxicons/fonts/boxicons.woff2` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/boxicons/fonts/boxicons.woff2`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/php-email-form/php-email-form.php` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/php-email-form/validate.js` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/purecounter/purecounter.js` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/purecounter/purecounter.js`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/purecounter/purecounter_vanilla.js` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/purecounter/purecounter_vanilla.js`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.eot` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.eot`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.less` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.less`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.svg` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.svg`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.symbol.svg` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.symbol.svg`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.ttf` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.ttf`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.woff` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.woff`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/remixicon/remixicon.woff2` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/remixicon/remixicon.woff2`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/swiper/swiper-bundle.min.css` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/static/mentor/vendor/swiper/swiper-bundle.min.js` & `django-mentor_ds_myenglish-1.0.1/mentor/static/mentor/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_about.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_about.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_contact.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_contact.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_courses.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_courses.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_cta.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_cta.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_events.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_events.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_faq.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_faq.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_features.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_features.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_hero.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_hero.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_intro.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_intro.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_testimonials.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_testimonials.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_trainers.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_trainers.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/_why_us.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/_why_us.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/analytics.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/analytics.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/footer.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/footer.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% load static %}
 
 <footer id="footer">
   <div class="container d-md-flex py-4">
     <div class="me-md-auto text-center text-md-start">
       <div class="copyright">
-        &copy; Copyright <a href="https://demiansoft.com" target="_blank"><strong><span>Demiansoft</span></strong></a>. All Rights Reserved
+        &copy; Copyright <a href="https://demiansoft.com" target="_blank"><strong><span>Demiansoft</span></strong></a><a href="https://map.naver.com/v5/entry/place/13289684?c=15,0,0,0,dh" target="_blank">.</a> All Rights Reserved
       </div>
       <div class="credits">
         {{ basic_info.company_name }} | {{ basic_info.owner}} | {{ basic_info.addr }} | 사업자등록번호: {{ basic_info.business_reg_number }}
       </div>
     </div>
     <div class="social-links text-center text-md-right pt-3 pt-md-0">
       {% if social.twitter %}
```

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/header.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/header.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/index.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/index.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templates/mentor/seo.html` & `django-mentor_ds_myenglish-1.0.1/mentor/templates/mentor/seo.html`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/templatetags/mentor_myenglish_tags.py` & `django-mentor_ds_myenglish-1.0.1/mentor/templatetags/mentor_myenglish_tags.py`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/mentor/views.py` & `django-mentor_ds_myenglish-1.0.1/mentor/views.py`

 * *Files identical despite different names*

### Comparing `django-mentor_ds_myenglish-1.0.0/setup.cfg` & `django-mentor_ds_myenglish-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 6d65 6e74 6f72   = django-mentor
 00000020: 5f64 735f 6d79 656e 676c 6973 680d 0a76  _ds_myenglish..v
-00000030: 6572 7369 6f6e 203d 2031 2e30 2e30 0d0a  ersion = 1.0.0..
+00000030: 6572 7369 6f6e 203d 2031 2e30 2e31 0d0a  ersion = 1.0.1..
 00000040: 6175 7468 6f72 203d 2068 7975 6e67 6a69  author = hyungji
 00000050: 6e20 6b69 6d0d 0a61 7574 686f 725f 656d  n kim..author_em
 00000060: 6169 6c20 3d20 686a 3334 3135 4067 6d61  ail = hj3415@gma
 00000070: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000080: 696f 6e20 3d20 6d65 6e74 6f72 5f70 726f  ion = mentor_pro
 00000090: 2070 6f72 7469 6e67 2066 6f72 2064 6a61   porting for dja
 000000a0: 6e67 6f0d 0a6c 6f6e 675f 6465 7363 7269  ngo..long_descri
```

