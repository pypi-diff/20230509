# Comparing `tmp/django-medilab_ds_mylifedc-0.8.3.tar.gz` & `tmp/django-medilab_ds_mylifedc-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-medilab_ds_mylifedc-0.8.3.tar", last modified: Wed Feb  8 04:31:03 2023, max compression
+gzip compressed data, was "django-medilab_ds_mylifedc-0.8.4.tar", last modified: Tue May  9 01:33:44 2023, max compression
```

## Comparing `django-medilab_ds_mylifedc-0.8.3.tar` & `django-medilab_ds_mylifedc-0.8.4.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.922965 django-medilab_ds_mylifedc-0.8.3/
--rw-rw-rw-   0        0        0     1093 2022-11-26 09:41:40.000000 django-medilab_ds_mylifedc-0.8.3/LICENSE
--rw-rw-rw-   0        0        0      297 2022-11-26 09:41:40.000000 django-medilab_ds_mylifedc-0.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3142 2023-02-08 04:31:03.923966 django-medilab_ds_mylifedc-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     2631 2022-11-26 09:41:40.000000 django-medilab_ds_mylifedc-0.8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:02.995173 django-medilab_ds_mylifedc-0.8.3/django_medilab_ds_mylifedc.egg-info/
--rw-rw-rw-   0        0        0     3142 2023-02-08 04:31:02.000000 django-medilab_ds_mylifedc-0.8.3/django_medilab_ds_mylifedc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10340 2023-02-08 04:31:02.000000 django-medilab_ds_mylifedc-0.8.3/django_medilab_ds_mylifedc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-08 04:31:02.000000 django-medilab_ds_mylifedc-0.8.3/django_medilab_ds_mylifedc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-02-08 04:31:02.000000 django-medilab_ds_mylifedc-0.8.3/django_medilab_ds_mylifedc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-02-08 04:31:02.000000 django-medilab_ds_mylifedc-0.8.3/django_medilab_ds_mylifedc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.021103 django-medilab_ds_mylifedc-0.8.3/medilab/
--rw-rw-rw-   0        0        0        0 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/__init__.py
--rw-rw-rw-   0        0        0      515 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/admin.py
--rw-rw-rw-   0        0        0      152 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/apps.py
--rw-rw-rw-   0        0        0     1178 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/forms.py
--rw-rw-rw-   0        0        0     1223 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/models.py
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:02.959230 django-medilab_ds_mylifedc-0.8.3/medilab/static/
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:02.962800 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.027106 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/css/
--rw-rw-rw-   0        0        0    31201 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/css/style.css
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.075740 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/
--rw-rw-rw-   0        0        0    61970 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/about.jpg
--rw-rw-rw-   0        0        0     1738 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/apple-touch-icon.png
--rw-rw-rw-   0        0        0    64859 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/departments-1.jpg
--rw-rw-rw-   0        0        0    48057 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/departments-2.jpg
--rw-rw-rw-   0        0        0    58282 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/departments-3.jpg
--rw-rw-rw-   0        0        0    56173 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/departments-4.jpg
--rw-rw-rw-   0        0        0    26888 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/departments-5.jpg
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.097745 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/doctors/
--rw-rw-rw-   0        0        0    28289 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/doctors/doctors-1.jpg
--rw-rw-rw-   0        0        0    24589 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/doctors/doctors-2.jpg
--rw-rw-rw-   0        0        0    26594 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/doctors/doctors-3.jpg
--rw-rw-rw-   0        0        0    30658 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/doctors/doctors-4.jpg
--rw-rw-rw-   0        0        0      491 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/favicon.png
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.140719 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/
--rw-rw-rw-   0        0        0    87051 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-1.jpg
--rw-rw-rw-   0        0        0    52988 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-2.jpg
--rw-rw-rw-   0        0        0    67200 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-3.jpg
--rw-rw-rw-   0        0        0   115379 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-4.jpg
--rw-rw-rw-   0        0        0    58795 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-5.jpg
--rw-rw-rw-   0        0        0    59213 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-6.jpg
--rw-rw-rw-   0        0        0    97603 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-7.jpg
--rw-rw-rw-   0        0        0   113565 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-8.jpg
--rw-rw-rw-   0        0        0   153715 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/hero-bg.jpg
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.167196 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/testimonials/
--rw-rw-rw-   0        0        0    39727 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/testimonials/testimonials-1.jpg
--rw-rw-rw-   0        0        0    57584 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/testimonials/testimonials-2.jpg
--rw-rw-rw-   0        0        0    17247 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/testimonials/testimonials-3.jpg
--rw-rw-rw-   0        0        0    20220 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/testimonials/testimonials-4.jpg
--rw-rw-rw-   0        0        0    22595 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/testimonials/testimonials-5.jpg
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.172808 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/js/
--rw-rw-rw-   0        0        0     5273 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/js/main.js
--rw-rw-rw-   0        0        0     1797 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/js/portfolio.js
--rw-rw-rw-   0        0        0      353 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/js/portfolio_slider.js
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.184381 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/
--rw-rw-rw-   0        0        0     3160 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_footer.scss
--rw-rw-rw-   0        0        0     1769 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_general.scss
--rw-rw-rw-   0        0        0     1981 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_header.scss
--rw-rw-rw-   0        0        0     1424 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_hero.scss
--rw-rw-rw-   0        0        0     3911 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_nav.scss
--rw-rw-rw-   0        0        0    20204 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_sections.scss
--rw-rw-rw-   0        0        0      499 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_variables.scss
--rw-rw-rw-   0        0        0      136 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/style.scss
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:02.975037 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.201626 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/animate.css/
--rw-rw-rw-   0        0        0    70607 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/animate.css/animate.compat.css
--rw-rw-rw-   0        0        0    95374 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/animate.css/animate.css
--rw-rw-rw-   0        0        0    71750 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/animate.css/animate.min.css
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.225125 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/aos/
--rw-rw-rw-   0        0        0    26053 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/aos/aos.css
--rw-rw-rw-   0        0        0    14690 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/aos/aos.js
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:02.965209 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.412162 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/
--rw-rw-rw-   0        0        0    71861 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0   210292 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0    53265 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0   131408 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-rw-   0        0        0    71935 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-rw-   0        0        0   210296 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-rw-   0        0        0    53340 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-rw-   0        0        0   131485 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-rw-   0        0        0     7965 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0   110811 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0     6490 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0    40345 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-rw-   0        0        0     7958 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-rw-   0        0        0   110824 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-rw-   0        0        0     6562 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-rw-   0        0        0    48707 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-rw-   0        0        0    74135 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.css
--rw-rw-rw-   0        0        0   196370 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-rw-   0        0        0    56365 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-rw-   0        0        0   115601 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-rw-   0        0        0    74002 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-rw-   0        0        0   196313 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-rw-   0        0        0    56293 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-rw-   0        0        0   115436 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-rw-   0        0        0   237872 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.css
--rw-rw-rw-   0        0        0   606249 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   194699 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   521459 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0   237386 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.css
--rw-rw-rw-   0        0        0   606069 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-rw-   0        0        0   194803 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-rw-   0        0        0   765329 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.535613 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/
--rw-rw-rw-   0        0        0   207083 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0   448881 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-rw-   0        0        0    79790 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   330849 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0   135367 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.js
--rw-rw-rw-   0        0        0   306814 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-rw-rw-   0        0        0    73539 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-rw-rw-   0        0        0   220143 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-rw-   0        0        0   144701 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.js
--rw-rw-rw-   0        0        0   307954 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.js.map
--rw-rw-rw-   0        0        0    60104 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   215897 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.min.js.map
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.248256 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/
--rw-rw-rw-   0        0        0    88585 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/bootstrap-icons.css
--rw-rw-rw-   0        0        0    47187 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   211136 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/bootstrap-icons.scss
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.259525 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/fonts/
--rw-rw-rw-   0        0        0   150592 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-rw-rw-   0        0        0   112440 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-rw-rw-   0        0        0   218010 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/index.html
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:02.966309 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.555259 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/css/
--rw-rw-rw-   0        0        0     7522 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/css/animations.css
--rw-rw-rw-   0        0        0    92272 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/css/boxicons.css
--rw-rw-rw-   0        0        0    66571 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/css/boxicons.min.css
--rw-rw-rw-   0        0        0      683 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/css/transformations.css
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.600244 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/fonts/
--rw-rw-rw-   0        0        0   396413 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/fonts/boxicons.eot
--rw-rw-rw-   0        0        0  1216389 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/fonts/boxicons.svg
--rw-rw-rw-   0        0        0   313836 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/fonts/boxicons.ttf
--rw-rw-rw-   0        0        0   313912 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/fonts/boxicons.woff
--rw-rw-rw-   0        0        0   115388 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/fonts/boxicons.woff2
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:02.967440 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.684298 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/
--rw-rw-rw-   0        0        0   137917 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/all.css
--rw-rw-rw-   0        0        0   100782 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/all.min.css
--rw-rw-rw-   0        0        0    22257 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/brands.css
--rw-rw-rw-   0        0        0    17821 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/brands.min.css
--rw-rw-rw-   0        0        0   112809 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/fontawesome.css
--rw-rw-rw-   0        0        0    80388 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/fontawesome.min.css
--rw-rw-rw-   0        0        0      619 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/regular.css
--rw-rw-rw-   0        0        0      566 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/regular.min.css
--rw-rw-rw-   0        0        0      611 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/solid.css
--rw-rw-rw-   0        0        0      558 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/solid.min.css
--rw-rw-rw-   0        0        0    21336 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/svg-with-js.css
--rw-rw-rw-   0        0        0    16699 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/svg-with-js.min.css
--rw-rw-rw-   0        0        0     1845 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/v4-font-face.css
--rw-rw-rw-   0        0        0     1750 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/v4-font-face.min.css
--rw-rw-rw-   0        0        0    40712 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/v4-shims.css
--rw-rw-rw-   0        0        0    26235 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/v4-shims.min.css
--rw-rw-rw-   0        0        0      871 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/v5-font-face.css
--rw-rw-rw-   0        0        0      794 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/v5-font-face.min.css
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.732580 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/
--rw-rw-rw-   0        0        0   181852 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0        0        0   105536 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0        0        0    60520 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0        0        0    23940 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0        0        0   388460 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0        0        0   154228 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
--rw-rw-rw-   0        0        0    10556 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf
--rw-rw-rw-   0        0        0     4960 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:02.972668 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.752373 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/css/
--rw-rw-rw-   0        0        0    17372 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/css/glightbox.css
--rw-rw-rw-   0        0        0    13749 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/css/glightbox.min.css
--rw-rw-rw-   0        0        0    52561 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/css/plyr.css
--rw-rw-rw-   0        0        0    45081 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/css/plyr.min.css
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.774637 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/js/
--rw-rw-rw-   0        0        0   109391 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/js/glightbox.js
--rw-rw-rw-   0        0        0    55880 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/js/glightbox.min.js
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.792138 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/isotope-layout/
--rw-rw-rw-   0        0        0    91398 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/isotope-layout/isotope.pkgd.js
--rw-rw-rw-   0        0        0    35445 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/isotope-layout/isotope.pkgd.min.js
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.795142 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/php-email-form/
--rw-rw-rw-   0        0        0   232262 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/php-email-form/php-email-form.php
--rw-rw-rw-   0        0        0     2731 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/php-email-form/validate.js
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.799551 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/purecounter/
--rw-rw-rw-   0        0        0     4958 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/purecounter/purecounter.js
--rw-rw-rw-   0        0        0     5417 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/purecounter/purecounter_vanilla.js
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.870416 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/
--rw-rw-rw-   0        0        0   110438 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.css
--rw-rw-rw-   0        0        0   403228 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.eot
--rw-rw-rw-   0        0        0   110450 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.less
--rw-rw-rw-   0        0        0  1195522 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.svg
--rw-rw-rw-   0        0        0   897931 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.symbol.svg
--rw-rw-rw-   0        0        0   403056 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.ttf
--rw-rw-rw-   0        0        0   172876 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.woff
--rw-rw-rw-   0        0        0   125268 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.woff2
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.873924 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/swiper/
--rw-rw-rw-   0        0        0    16466 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/swiper/swiper-bundle.min.css
--rw-rw-rw-   0        0        0   143070 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/swiper/swiper-bundle.min.js
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:02.976158 django-medilab_ds_mylifedc-0.8.3/medilab/templates/
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.912013 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/
--rw-rw-rw-   0        0        0     1315 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_about.html
--rw-rw-rw-   0        0        0     1622 2023-02-03 01:08:45.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_appointment.html
--rw-rw-rw-   0        0        0     4727 2023-02-03 00:30:07.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_contact.html
--rw-rw-rw-   0        0        0      714 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_counts.html
--rw-rw-rw-   0        0        0     1431 2023-02-06 01:59:52.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_cta.html
--rw-rw-rw-   0        0        0     1886 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_departments.html
--rw-rw-rw-   0        0        0     1753 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_doctors.html
--rw-rw-rw-   0        0        0     1486 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_faq.html
--rw-rw-rw-   0        0        0      721 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_gallery.html
--rw-rw-rw-   0        0        0      647 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_hero.html
--rw-rw-rw-   0        0        0     5584 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_portfolio-details.html
--rw-rw-rw-   0        0        0     4795 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_portfolio.html
--rw-rw-rw-   0        0        0     1532 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_services.html
--rw-rw-rw-   0        0        0     1115 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_testimonials.html
--rw-rw-rw-   0        0        0     2306 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_why_us.html
--rw-rw-rw-   0        0        0     1183 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/analytics.html
--rw-rw-rw-   0        0        0     1703 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/footer.html
--rw-rw-rw-   0        0        0     2847 2023-02-03 00:50:21.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/header.html
--rw-rw-rw-   0        0        0     4885 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/index.html
--rw-rw-rw-   0        0        0     1460 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/seo.html
-drwxrwxrwx   0        0        0        0 2023-02-08 04:31:03.921966 django-medilab_ds_mylifedc-0.8.3/medilab/templatetags/
--rw-rw-rw-   0        0        0        0 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templatetags/__init__.py
--rw-rw-rw-   0        0        0     4991 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templatetags/sections.py
--rw-rw-rw-   0        0        0      435 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/templatetags/utils.py
--rw-rw-rw-   0        0        0      276 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/medilab/urls.py
--rw-rw-rw-   0        0        0     4003 2023-01-02 04:26:44.000000 django-medilab_ds_mylifedc-0.8.3/medilab/views.py
--rw-rw-rw-   0        0        0      112 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/pyproject.toml
--rw-rw-rw-   0        0        0      759 2023-02-08 04:31:03.925005 django-medilab_ds_mylifedc-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.717182 django-medilab_ds_mylifedc-0.8.4/
+-rw-rw-rw-   0        0        0     1093 2022-11-26 09:41:40.000000 django-medilab_ds_mylifedc-0.8.4/LICENSE
+-rw-rw-rw-   0        0        0      297 2022-11-26 09:41:40.000000 django-medilab_ds_mylifedc-0.8.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3142 2023-05-09 01:33:44.718185 django-medilab_ds_mylifedc-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2631 2022-11-26 09:41:40.000000 django-medilab_ds_mylifedc-0.8.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.388292 django-medilab_ds_mylifedc-0.8.4/django_medilab_ds_mylifedc.egg-info/
+-rw-rw-rw-   0        0        0     3142 2023-05-09 01:33:44.000000 django-medilab_ds_mylifedc-0.8.4/django_medilab_ds_mylifedc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10340 2023-05-09 01:33:44.000000 django-medilab_ds_mylifedc-0.8.4/django_medilab_ds_mylifedc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 01:33:44.000000 django-medilab_ds_mylifedc-0.8.4/django_medilab_ds_mylifedc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-05-09 01:33:44.000000 django-medilab_ds_mylifedc-0.8.4/django_medilab_ds_mylifedc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-09 01:33:44.000000 django-medilab_ds_mylifedc-0.8.4/django_medilab_ds_mylifedc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.394856 django-medilab_ds_mylifedc-0.8.4/medilab/
+-rw-rw-rw-   0        0        0        0 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/__init__.py
+-rw-rw-rw-   0        0        0      515 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/admin.py
+-rw-rw-rw-   0        0        0      152 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/apps.py
+-rw-rw-rw-   0        0        0     1178 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/forms.py
+-rw-rw-rw-   0        0        0     1223 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/models.py
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.354412 django-medilab_ds_mylifedc-0.8.4/medilab/static/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.356622 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.396291 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/css/
+-rw-rw-rw-   0        0        0    31201 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/css/style.css
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.446618 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/
+-rw-rw-rw-   0        0        0    61970 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/about.jpg
+-rw-rw-rw-   0        0        0     1738 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/apple-touch-icon.png
+-rw-rw-rw-   0        0        0    64859 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/departments-1.jpg
+-rw-rw-rw-   0        0        0    48057 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/departments-2.jpg
+-rw-rw-rw-   0        0        0    58282 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/departments-3.jpg
+-rw-rw-rw-   0        0        0    56173 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/departments-4.jpg
+-rw-rw-rw-   0        0        0    26888 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/departments-5.jpg
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.467664 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/doctors/
+-rw-rw-rw-   0        0        0    28289 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/doctors/doctors-1.jpg
+-rw-rw-rw-   0        0        0    24589 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/doctors/doctors-2.jpg
+-rw-rw-rw-   0        0        0    26594 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/doctors/doctors-3.jpg
+-rw-rw-rw-   0        0        0    30658 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/doctors/doctors-4.jpg
+-rw-rw-rw-   0        0        0      491 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/favicon.png
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.508523 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/
+-rw-rw-rw-   0        0        0    87051 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-1.jpg
+-rw-rw-rw-   0        0        0    52988 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-2.jpg
+-rw-rw-rw-   0        0        0    67200 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-3.jpg
+-rw-rw-rw-   0        0        0   115379 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-4.jpg
+-rw-rw-rw-   0        0        0    58795 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-5.jpg
+-rw-rw-rw-   0        0        0    59213 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-6.jpg
+-rw-rw-rw-   0        0        0    97603 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-7.jpg
+-rw-rw-rw-   0        0        0   113565 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-8.jpg
+-rw-rw-rw-   0        0        0   153715 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/hero-bg.jpg
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.533898 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/testimonials/
+-rw-rw-rw-   0        0        0    39727 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/testimonials/testimonials-1.jpg
+-rw-rw-rw-   0        0        0    57584 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/testimonials/testimonials-2.jpg
+-rw-rw-rw-   0        0        0    17247 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/testimonials/testimonials-3.jpg
+-rw-rw-rw-   0        0        0    20220 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/testimonials/testimonials-4.jpg
+-rw-rw-rw-   0        0        0    22595 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/testimonials/testimonials-5.jpg
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.536910 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/js/
+-rw-rw-rw-   0        0        0     5273 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/js/main.js
+-rw-rw-rw-   0        0        0     1797 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/js/portfolio.js
+-rw-rw-rw-   0        0        0      353 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/js/portfolio_slider.js
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.544818 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/
+-rw-rw-rw-   0        0        0     3160 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_footer.scss
+-rw-rw-rw-   0        0        0     1769 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_general.scss
+-rw-rw-rw-   0        0        0     1981 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_header.scss
+-rw-rw-rw-   0        0        0     1424 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_hero.scss
+-rw-rw-rw-   0        0        0     3911 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_nav.scss
+-rw-rw-rw-   0        0        0    20204 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_sections.scss
+-rw-rw-rw-   0        0        0      499 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_variables.scss
+-rw-rw-rw-   0        0        0      136 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/style.scss
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.363445 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.549164 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/animate.css/
+-rw-rw-rw-   0        0        0    70607 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/animate.css/animate.compat.css
+-rw-rw-rw-   0        0        0    95374 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/animate.css/animate.css
+-rw-rw-rw-   0        0        0    71750 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/animate.css/animate.min.css
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.551338 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/aos/
+-rw-rw-rw-   0        0        0    26053 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/aos/aos.css
+-rw-rw-rw-   0        0        0    14690 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/aos/aos.js
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.358841 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.601886 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/
+-rw-rw-rw-   0        0        0    71861 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0   210292 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0    53265 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0   131408 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-rw-   0        0        0    71935 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-rw-   0        0        0   210296 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-rw-   0        0        0    53340 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-rw-   0        0        0   131485 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-rw-   0        0        0     7965 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0   110811 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0     6490 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0    40345 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-rw-   0        0        0     7958 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-rw-   0        0        0   110824 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-rw-   0        0        0     6562 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-rw-   0        0        0    48707 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-rw-   0        0        0    74135 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0   196370 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-rw-   0        0        0    56365 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-rw-   0        0        0   115601 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-rw-   0        0        0    74002 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-rw-   0        0        0   196313 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-rw-   0        0        0    56293 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-rw-   0        0        0   115436 2022-11-26 09:41:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-rw-   0        0        0   237872 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0        0        0   606249 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   194699 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   521459 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0   237386 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-rw-rw-   0        0        0   606069 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-rw-   0        0        0   194803 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-rw-   0        0        0   765329 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.619823 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/
+-rw-rw-rw-   0        0        0   207083 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0   448881 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-rw-   0        0        0    79790 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   330849 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0   135367 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.js
+-rw-rw-rw-   0        0        0   306814 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-rw-   0        0        0    73539 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-rw-   0        0        0   220143 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-rw-   0        0        0   144701 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0        0        0   307954 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.js.map
+-rw-rw-rw-   0        0        0    60104 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0   215897 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.min.js.map
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.556149 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/
+-rw-rw-rw-   0        0        0    88585 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-rw-rw-   0        0        0    47187 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   211136 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/bootstrap-icons.scss
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.558721 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/fonts/
+-rw-rw-rw-   0        0        0   150592 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-rw-rw-   0        0        0   112440 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-rw-rw-   0        0        0   218010 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/index.html
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.359876 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.623310 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/css/
+-rw-rw-rw-   0        0        0     7522 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/css/animations.css
+-rw-rw-rw-   0        0        0    92272 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/css/boxicons.css
+-rw-rw-rw-   0        0        0    66571 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/css/boxicons.min.css
+-rw-rw-rw-   0        0        0      683 2022-11-26 09:41:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/css/transformations.css
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.632134 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/fonts/
+-rw-rw-rw-   0        0        0   396413 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/fonts/boxicons.eot
+-rw-rw-rw-   0        0        0  1216389 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/fonts/boxicons.svg
+-rw-rw-rw-   0        0        0   313836 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/fonts/boxicons.ttf
+-rw-rw-rw-   0        0        0   313912 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/fonts/boxicons.woff
+-rw-rw-rw-   0        0        0   115388 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/fonts/boxicons.woff2
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.361058 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.652272 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/
+-rw-rw-rw-   0        0        0   137917 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/all.css
+-rw-rw-rw-   0        0        0   100782 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/all.min.css
+-rw-rw-rw-   0        0        0    22257 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/brands.css
+-rw-rw-rw-   0        0        0    17821 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/brands.min.css
+-rw-rw-rw-   0        0        0   112809 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/fontawesome.css
+-rw-rw-rw-   0        0        0    80388 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/fontawesome.min.css
+-rw-rw-rw-   0        0        0      619 2022-11-26 09:41:46.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/regular.css
+-rw-rw-rw-   0        0        0      566 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/regular.min.css
+-rw-rw-rw-   0        0        0      611 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/solid.css
+-rw-rw-rw-   0        0        0      558 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/solid.min.css
+-rw-rw-rw-   0        0        0    21336 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/svg-with-js.css
+-rw-rw-rw-   0        0        0    16699 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/svg-with-js.min.css
+-rw-rw-rw-   0        0        0     1845 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/v4-font-face.css
+-rw-rw-rw-   0        0        0     1750 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/v4-font-face.min.css
+-rw-rw-rw-   0        0        0    40712 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/v4-shims.css
+-rw-rw-rw-   0        0        0    26235 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/v4-shims.min.css
+-rw-rw-rw-   0        0        0      871 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/v5-font-face.css
+-rw-rw-rw-   0        0        0      794 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/v5-font-face.min.css
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.662980 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/
+-rw-rw-rw-   0        0        0   181852 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0        0        0   105536 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0        0        0    60520 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0        0        0    23940 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0        0        0   388460 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0        0        0   154228 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
+-rw-rw-rw-   0        0        0    10556 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf
+-rw-rw-rw-   0        0        0     4960 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.362402 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.666982 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/css/
+-rw-rw-rw-   0        0        0    17372 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/css/glightbox.css
+-rw-rw-rw-   0        0        0    13749 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/css/glightbox.min.css
+-rw-rw-rw-   0        0        0    52561 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/css/plyr.css
+-rw-rw-rw-   0        0        0    45081 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/css/plyr.min.css
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.668982 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/js/
+-rw-rw-rw-   0        0        0   109391 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/js/glightbox.js
+-rw-rw-rw-   0        0        0    55880 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/js/glightbox.min.js
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.671498 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/isotope-layout/
+-rw-rw-rw-   0        0        0    91398 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/isotope-layout/isotope.pkgd.js
+-rw-rw-rw-   0        0        0    35445 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/isotope-layout/isotope.pkgd.min.js
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.674004 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/php-email-form/
+-rw-rw-rw-   0        0        0   232262 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/php-email-form/php-email-form.php
+-rw-rw-rw-   0        0        0     2731 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/php-email-form/validate.js
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.676003 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/purecounter/
+-rw-rw-rw-   0        0        0     4958 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/purecounter/purecounter.js
+-rw-rw-rw-   0        0        0     5417 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/purecounter/purecounter_vanilla.js
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.689282 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/
+-rw-rw-rw-   0        0        0   110438 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.css
+-rw-rw-rw-   0        0        0   403228 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.eot
+-rw-rw-rw-   0        0        0   110450 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.less
+-rw-rw-rw-   0        0        0  1195522 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.svg
+-rw-rw-rw-   0        0        0   897931 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.symbol.svg
+-rw-rw-rw-   0        0        0   403056 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.ttf
+-rw-rw-rw-   0        0        0   172876 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.woff
+-rw-rw-rw-   0        0        0   125268 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.woff2
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.692282 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/swiper/
+-rw-rw-rw-   0        0        0    16466 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/swiper/swiper-bundle.min.css
+-rw-rw-rw-   0        0        0   143070 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/swiper/swiper-bundle.min.js
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.364535 django-medilab_ds_mylifedc-0.8.4/medilab/templates/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.713182 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/
+-rw-rw-rw-   0        0        0     1315 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_about.html
+-rw-rw-rw-   0        0        0     1622 2023-02-03 01:08:45.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_appointment.html
+-rw-rw-rw-   0        0        0     4727 2023-02-03 00:30:07.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_contact.html
+-rw-rw-rw-   0        0        0      714 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_counts.html
+-rw-rw-rw-   0        0        0     1431 2023-02-06 01:59:52.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_cta.html
+-rw-rw-rw-   0        0        0     1886 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_departments.html
+-rw-rw-rw-   0        0        0     1753 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_doctors.html
+-rw-rw-rw-   0        0        0     1486 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_faq.html
+-rw-rw-rw-   0        0        0      721 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_gallery.html
+-rw-rw-rw-   0        0        0      647 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_hero.html
+-rw-rw-rw-   0        0        0     5584 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_portfolio-details.html
+-rw-rw-rw-   0        0        0     4795 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_portfolio.html
+-rw-rw-rw-   0        0        0     1532 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_services.html
+-rw-rw-rw-   0        0        0     1115 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_testimonials.html
+-rw-rw-rw-   0        0        0     2306 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_why_us.html
+-rw-rw-rw-   0        0        0     1183 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/analytics.html
+-rw-rw-rw-   0        0        0     1793 2023-05-09 01:33:24.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/footer.html
+-rw-rw-rw-   0        0        0     2847 2023-02-03 00:50:21.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/header.html
+-rw-rw-rw-   0        0        0     4885 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/index.html
+-rw-rw-rw-   0        0        0     1460 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/seo.html
+drwxrwxrwx   0        0        0        0 2023-05-09 01:33:44.716184 django-medilab_ds_mylifedc-0.8.4/medilab/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     4991 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templatetags/sections.py
+-rw-rw-rw-   0        0        0      435 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/templatetags/utils.py
+-rw-rw-rw-   0        0        0      276 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/medilab/urls.py
+-rw-rw-rw-   0        0        0     4003 2023-01-02 04:26:44.000000 django-medilab_ds_mylifedc-0.8.4/medilab/views.py
+-rw-rw-rw-   0        0        0      112 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/pyproject.toml
+-rw-rw-rw-   0        0        0      759 2023-05-09 01:33:44.719184 django-medilab_ds_mylifedc-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-11-26 09:41:47.000000 django-medilab_ds_mylifedc-0.8.4/setup.py
```

### Comparing `django-medilab_ds_mylifedc-0.8.3/LICENSE` & `django-medilab_ds_mylifedc-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/PKG-INFO` & `django-medilab_ds_mylifedc-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-medilab_ds_mylifedc
-Version: 0.8.3
+Version: 0.8.4
 Summary: medilab_pro porting for django
 Home-page: https://www.demiansoft.com
 Author: hyungjin kim
 Author-email: hj3415@gmail.com
 Project-URL: Bug Tracker, https://pypi.org/project/util-demian/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-medilab_ds_mylifedc-0.8.3/README.md` & `django-medilab_ds_mylifedc-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/django_medilab_ds_mylifedc.egg-info/PKG-INFO` & `django-medilab_ds_mylifedc-0.8.4/django_medilab_ds_mylifedc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-medilab-ds-mylifedc
-Version: 0.8.3
+Version: 0.8.4
 Summary: medilab_pro porting for django
 Home-page: https://www.demiansoft.com
 Author: hyungjin kim
 Author-email: hj3415@gmail.com
 Project-URL: Bug Tracker, https://pypi.org/project/util-demian/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-medilab_ds_mylifedc-0.8.3/django_medilab_ds_mylifedc.egg-info/SOURCES.txt` & `django-medilab_ds_mylifedc-0.8.4/django_medilab_ds_mylifedc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/admin.py` & `django-medilab_ds_mylifedc-0.8.4/medilab/admin.py`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/forms.py` & `django-medilab_ds_mylifedc-0.8.4/medilab/forms.py`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/models.py` & `django-medilab_ds_mylifedc-0.8.4/medilab/models.py`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/css/style.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/css/style.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/about.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/about.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/apple-touch-icon.png` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/departments-1.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/departments-1.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/departments-2.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/departments-2.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/departments-3.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/departments-3.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/departments-4.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/departments-4.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/departments-5.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/departments-5.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/doctors/doctors-1.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/doctors/doctors-1.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/doctors/doctors-2.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/doctors/doctors-2.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/doctors/doctors-3.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/doctors/doctors-3.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/doctors/doctors-4.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/doctors/doctors-4.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-1.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-1.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-2.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-2.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-3.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-3.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-4.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-4.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-5.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-5.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-6.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-6.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-7.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-7.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/gallery/gallery-8.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/gallery/gallery-8.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/hero-bg.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/hero-bg.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/testimonials/testimonials-1.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/testimonials/testimonials-1.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/testimonials/testimonials-2.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/testimonials/testimonials-2.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/testimonials/testimonials-3.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/testimonials/testimonials-3.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/testimonials/testimonials-4.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/testimonials/testimonials-4.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/img/testimonials/testimonials-5.jpg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/img/testimonials/testimonials-5.jpg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/js/main.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/js/main.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/js/portfolio.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/js/portfolio.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_footer.scss` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_general.scss` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_header.scss` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_hero.scss` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_hero.scss`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_nav.scss` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/scss/_sections.scss` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/scss/_sections.scss`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/animate.css/animate.compat.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/animate.css/animate.compat.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/animate.css/animate.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/animate.css/animate.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/animate.css/animate.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/animate.css/animate.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/aos/aos.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/aos/aos.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.min.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.js.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.min.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.js.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.min.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap/js/bootstrap.min.js.map` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/bootstrap-icons.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/bootstrap-icons.json` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/bootstrap-icons.scss` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/bootstrap-icons/index.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/bootstrap-icons/index.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/css/animations.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/css/animations.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/css/boxicons.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/css/boxicons.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/css/boxicons.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/css/boxicons.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/css/transformations.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/css/transformations.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/fonts/boxicons.eot` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/fonts/boxicons.eot`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/fonts/boxicons.svg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/fonts/boxicons.svg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/fonts/boxicons.ttf` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/fonts/boxicons.ttf`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/fonts/boxicons.woff` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/fonts/boxicons.woff`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/boxicons/fonts/boxicons.woff2` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/boxicons/fonts/boxicons.woff2`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/all.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/all.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/all.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/brands.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/brands.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/brands.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/brands.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/fontawesome.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/fontawesome.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/regular.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/regular.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/regular.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/regular.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/solid.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/solid.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/solid.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/svg-with-js.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/svg-with-js.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/v4-font-face.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/v4-font-face.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/v4-font-face.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/v4-font-face.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/v4-shims.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/v4-shims.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/v5-font-face.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/v5-font-face.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/css/v5-font-face.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/css/v5-font-face.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-brands-400.ttf` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-brands-400.woff2` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-regular-400.ttf` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-regular-400.woff2` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-solid-900.ttf` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-solid-900.woff2` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/css/glightbox.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/css/glightbox.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/css/plyr.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/css/plyr.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/css/plyr.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/css/plyr.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/js/glightbox.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/glightbox/js/glightbox.min.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/isotope-layout/isotope.pkgd.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/isotope-layout/isotope.pkgd.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/isotope-layout/isotope.pkgd.min.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/isotope-layout/isotope.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/php-email-form/php-email-form.php` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/php-email-form/validate.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/purecounter/purecounter.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/purecounter/purecounter.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/purecounter/purecounter_vanilla.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/purecounter/purecounter_vanilla.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.eot` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.eot`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.less` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.less`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.svg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.svg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.symbol.svg` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.symbol.svg`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.ttf` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.ttf`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.woff` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.woff`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/remixicon/remixicon.woff2` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/remixicon/remixicon.woff2`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/swiper/swiper-bundle.min.css` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/static/medilab/vendor/swiper/swiper-bundle.min.js` & `django-medilab_ds_mylifedc-0.8.4/medilab/static/medilab/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_about.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_about.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_appointment.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_appointment.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_contact.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_contact.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_counts.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_counts.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_cta.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_cta.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_departments.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_departments.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_doctors.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_doctors.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_faq.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_faq.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_gallery.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_gallery.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_hero.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_hero.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_portfolio-details.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_portfolio-details.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_portfolio.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_portfolio.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_services.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_services.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_testimonials.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_testimonials.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/_why_us.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/_why_us.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/analytics.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/analytics.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/footer.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/footer.html`

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

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/header.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/header.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/index.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/index.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templates/medilab/seo.html` & `django-medilab_ds_mylifedc-0.8.4/medilab/templates/medilab/seo.html`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/templatetags/sections.py` & `django-medilab_ds_mylifedc-0.8.4/medilab/templatetags/sections.py`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/medilab/views.py` & `django-medilab_ds_mylifedc-0.8.4/medilab/views.py`

 * *Files identical despite different names*

### Comparing `django-medilab_ds_mylifedc-0.8.3/setup.cfg` & `django-medilab_ds_mylifedc-0.8.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 6d65 6469 6c61   = django-medila
 00000020: 625f 6473 5f6d 796c 6966 6564 630d 0a76  b_ds_mylifedc..v
-00000030: 6572 7369 6f6e 203d 2030 2e38 2e33 0d0a  ersion = 0.8.3..
+00000030: 6572 7369 6f6e 203d 2030 2e38 2e34 0d0a  ersion = 0.8.4..
 00000040: 6175 7468 6f72 203d 2068 7975 6e67 6a69  author = hyungji
 00000050: 6e20 6b69 6d0d 0a61 7574 686f 725f 656d  n kim..author_em
 00000060: 6169 6c20 3d20 686a 3334 3135 4067 6d61  ail = hj3415@gma
 00000070: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000080: 696f 6e20 3d20 6d65 6469 6c61 625f 7072  ion = medilab_pr
 00000090: 6f20 706f 7274 696e 6720 666f 7220 646a  o porting for dj
 000000a0: 616e 676f 0d0a 6c6f 6e67 5f64 6573 6372  ango..long_descr
```

