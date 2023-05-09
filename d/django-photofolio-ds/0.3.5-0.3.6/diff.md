# Comparing `tmp/django-photofolio_ds-0.3.5.tar.gz` & `tmp/django-photofolio_ds-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-photofolio_ds-0.3.5.tar", last modified: Wed Dec  7 01:58:04 2022, max compression
+gzip compressed data, was "django-photofolio_ds-0.3.6.tar", last modified: Tue May  9 02:01:45 2023, max compression
```

## Comparing `django-photofolio_ds-0.3.5.tar` & `django-photofolio_ds-0.3.6.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.918491 django-photofolio_ds-0.3.5/
--rw-rw-rw-   0        0        0     1093 2022-12-02 00:59:34.000000 django-photofolio_ds-0.3.5/LICENSE
--rw-rw-rw-   0        0        0      279 2022-12-02 00:59:34.000000 django-photofolio_ds-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3002 2022-12-07 01:58:04.918491 django-photofolio_ds-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     2494 2022-12-02 00:59:34.000000 django-photofolio_ds-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.652249 django-photofolio_ds-0.3.5/django_photofolio_ds.egg-info/
--rw-rw-rw-   0        0        0     3002 2022-12-07 01:58:04.000000 django-photofolio_ds-0.3.5/django_photofolio_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8131 2022-12-07 01:58:04.000000 django-photofolio_ds-0.3.5/django_photofolio_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-07 01:58:04.000000 django-photofolio_ds-0.3.5/django_photofolio_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2022-12-07 01:58:04.000000 django-photofolio_ds-0.3.5/django_photofolio_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-12-07 01:58:04.000000 django-photofolio_ds-0.3.5/django_photofolio_ds.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.664260 django-photofolio_ds-0.3.5/photofolio/
--rw-rw-rw-   0        0        0        0 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/__init__.py
--rw-rw-rw-   0        0        0       66 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/admin.py
--rw-rw-rw-   0        0        0      158 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/apps.py
--rw-rw-rw-   0        0        0     1178 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/forms.py
--rw-rw-rw-   0        0        0       60 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/models.py
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.614215 django-photofolio_ds-0.3.5/photofolio/static/
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.618218 django-photofolio_ds-0.3.5/photofolio/static/photofolio/
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.665261 django-photofolio_ds-0.3.5/photofolio/static/photofolio/css/
--rw-rw-rw-   0        0        0    24674 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/css/main.css
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.670266 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/
--rw-rw-rw-   0        0        0     1738 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/apple-touch-icon.png
--rw-rw-rw-   0        0        0      491 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/favicon.png
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.709300 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/
--rw-rw-rw-   0        0        0   254691 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-1.jpg
--rw-rw-rw-   0        0        0   325115 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-10.jpg
--rw-rw-rw-   0        0        0   191991 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-11.jpg
--rw-rw-rw-   0        0        0   118728 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-12.jpg
--rw-rw-rw-   0        0        0   613771 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-13.jpg
--rw-rw-rw-   0        0        0   339998 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-14.jpg
--rw-rw-rw-   0        0        0   169145 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-15.jpg
--rw-rw-rw-   0        0        0   299838 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-16.jpg
--rw-rw-rw-   0        0        0   376843 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-2.jpg
--rw-rw-rw-   0        0        0   301323 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-3.jpg
--rw-rw-rw-   0        0        0   290800 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-4.jpg
--rw-rw-rw-   0        0        0   493094 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-5.jpg
--rw-rw-rw-   0        0        0   351024 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-6.jpg
--rw-rw-rw-   0        0        0   371929 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-7.jpg
--rw-rw-rw-   0        0        0   187657 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-8.jpg
--rw-rw-rw-   0        0        0   152783 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-9.jpg
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.718309 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/portfolio/
--rw-rw-rw-   0        0        0    67064 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/portfolio/app-1.jpg
--rw-rw-rw-   0        0        0    80146 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/portfolio/books-1.jpg
--rw-rw-rw-   0        0        0    25514 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/portfolio/branding-1.jpg
--rw-rw-rw-   0        0        0    62035 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/portfolio/product-1.jpg
--rw-rw-rw-   0        0        0   238663 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/profile-img.jpg
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.730320 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/testimonials/
--rw-rw-rw-   0        0        0    39727 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/testimonials/testimonials-1.jpg
--rw-rw-rw-   0        0        0    57584 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/testimonials/testimonials-2.jpg
--rw-rw-rw-   0        0        0    17247 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/testimonials/testimonials-3.jpg
--rw-rw-rw-   0        0        0    20220 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/testimonials/testimonials-4.jpg
--rw-rw-rw-   0        0        0    22595 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/testimonials/testimonials-5.jpg
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.732321 django-photofolio_ds-0.3.5/photofolio/static/photofolio/js/
--rw-rw-rw-   0        0        0     4241 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/js/main.js
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.746335 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/
--rw-rw-rw-   0        0        0      506 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/_footer.scss
--rw-rw-rw-   0        0        0     5193 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/_general.scss
--rw-rw-rw-   0        0        0     1102 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/_header.scss
--rw-rw-rw-   0        0        0     1354 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/_hero.scss
--rw-rw-rw-   0        0        0     4493 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/_nav.scss
--rw-rw-rw-   0        0        0      214 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/_sections.scss
--rw-rw-rw-   0        0        0      553 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/main.scss
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.761348 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/
--rw-rw-rw-   0        0        0      651 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_about.scss
--rw-rw-rw-   0        0        0     2718 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_contact.scss
--rw-rw-rw-   0        0        0     3656 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_gallery-single.scss
--rw-rw-rw-   0        0        0     1177 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_gallery.scss
--rw-rw-rw-   0        0        0      511 2022-12-02 00:59:36.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_pricing.scss
--rw-rw-rw-   0        0        0     1423 2022-12-07 01:55:09.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_services.scss
--rw-rw-rw-   0        0        0     1716 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_testimonials.scss
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.623223 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.764351 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/aos/
--rw-rw-rw-   0        0        0    26053 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/aos/aos.css
--rw-rw-rw-   0        0        0    14690 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/aos/aos.js
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.621222 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.840420 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/
--rw-rw-rw-   0        0        0    71861 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0   210292 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0    53265 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0   131408 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-rw-   0        0        0    71935 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-rw-   0        0        0   210296 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-rw-   0        0        0    53340 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-rw-   0        0        0   131485 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-rw-   0        0        0     7965 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0   110811 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0     6490 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0    40345 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-rw-   0        0        0     7958 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-rw-   0        0        0   110824 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-rw-   0        0        0     6562 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-rw-   0        0        0    48707 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-rw-   0        0        0    74135 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.css
--rw-rw-rw-   0        0        0   196370 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-rw-   0        0        0    56365 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-rw-   0        0        0   115601 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-rw-   0        0        0    74002 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-rw-   0        0        0   196313 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-rw-   0        0        0    56293 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-rw-   0        0        0   115436 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-rw-   0        0        0   237872 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.css
--rw-rw-rw-   0        0        0   606249 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   194699 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   521459 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0   237386 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.css
--rw-rw-rw-   0        0        0   606069 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-rw-   0        0        0   194803 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-rw-   0        0        0   765329 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.866443 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/
--rw-rw-rw-   0        0        0   207083 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0   448881 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-rw-   0        0        0    79790 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   330849 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0   135367 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.js
--rw-rw-rw-   0        0        0   306814 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-rw-rw-   0        0        0    73539 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-rw-rw-   0        0        0   220143 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-rw-   0        0        0   144701 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.js
--rw-rw-rw-   0        0        0   307954 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.js.map
--rw-rw-rw-   0        0        0    60104 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   215897 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.min.js.map
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.772358 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/
--rw-rw-rw-   0        0        0    88585 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/bootstrap-icons.css
--rw-rw-rw-   0        0        0    47187 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   211136 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/bootstrap-icons.scss
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.776362 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/fonts/
--rw-rw-rw-   0        0        0   150592 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-rw-rw-   0        0        0   112440 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-rw-rw-   0        0        0   218010 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/index.html
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.623223 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.874451 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/css/
--rw-rw-rw-   0        0        0    17372 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/css/glightbox.css
--rw-rw-rw-   0        0        0    13749 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/css/glightbox.min.css
--rw-rw-rw-   0        0        0    52561 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/css/plyr.css
--rw-rw-rw-   0        0        0    45081 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/css/plyr.min.css
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.878455 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/js/
--rw-rw-rw-   0        0        0   109391 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/js/glightbox.js
--rw-rw-rw-   0        0        0    55880 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/js/glightbox.min.js
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.881458 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/php-email-form/
--rw-rw-rw-   0        0        0   232262 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/php-email-form/php-email-form.php
--rw-rw-rw-   0        0        0     2731 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/php-email-form/validate.js
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.885462 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/swiper/
--rw-rw-rw-   0        0        0    16466 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/swiper/swiper-bundle.min.css
--rw-rw-rw-   0        0        0   143070 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/swiper/swiper-bundle.min.js
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.624224 django-photofolio_ds-0.3.5/photofolio/templates/
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.903478 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/
--rw-rw-rw-   0        0        0      833 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/_about.html
--rw-rw-rw-   0        0        0     3030 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/_contact.html
--rw-rw-rw-   0        0        0      777 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/_gallery.html
--rw-rw-rw-   0        0        0      509 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/_hero.html
--rw-rw-rw-   0        0        0      505 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/_pricing.html
--rw-rw-rw-   0        0        0      480 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/_services.html
--rw-rw-rw-   0        0        0     1176 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/_testimonials.html
--rw-rw-rw-   0        0        0      267 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/footer.html
--rw-rw-rw-   0        0        0     3110 2022-12-07 01:46:18.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/header.html
--rw-rw-rw-   0        0        0     2302 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/index.html
--rw-rw-rw-   0        0        0     1460 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/seo.html
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.913487 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/
--rw-rw-rw-   0        0        0     2799 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/about.html
--rw-rw-rw-   0        0        0     2660 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/contact.html
--rw-rw-rw-   0        0        0    10081 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/gallery-single.html
--rw-rw-rw-   0        0        0     2694 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/gallery.html
--rw-rw-rw-   0        0        0     5902 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/sample-inner-page.html
--rw-rw-rw-   0        0        0     3091 2022-12-07 01:55:09.000000 django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/services.html
-drwxrwxrwx   0        0        0        0 2022-12-07 01:58:04.916489 django-photofolio_ds-0.3.5/photofolio/templatetags/
--rw-rw-rw-   0        0        0        0 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/photofolio/templatetags/__init__.py
--rw-rw-rw-   0        0        0     3442 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/templatetags/sections.py
--rw-rw-rw-   0        0        0      632 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/urls.py
--rw-rw-rw-   0        0        0     4924 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/photofolio/views.py
--rw-rw-rw-   0        0        0      112 2022-12-02 00:59:38.000000 django-photofolio_ds-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0      756 2022-12-07 01:58:04.920493 django-photofolio_ds-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-12-02 00:59:37.000000 django-photofolio_ds-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:45.007316 django-photofolio_ds-0.3.6/
+-rw-rw-rw-   0        0        0     1093 2022-11-26 09:41:57.000000 django-photofolio_ds-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0      279 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3002 2023-05-09 02:01:45.007316 django-photofolio_ds-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2494 2022-11-26 09:41:57.000000 django-photofolio_ds-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.683890 django-photofolio_ds-0.3.6/django_photofolio_ds.egg-info/
+-rw-rw-rw-   0        0        0     3002 2023-05-09 02:01:44.000000 django-photofolio_ds-0.3.6/django_photofolio_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8131 2023-05-09 02:01:44.000000 django-photofolio_ds-0.3.6/django_photofolio_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 02:01:44.000000 django-photofolio_ds-0.3.6/django_photofolio_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-05-09 02:01:44.000000 django-photofolio_ds-0.3.6/django_photofolio_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-09 02:01:44.000000 django-photofolio_ds-0.3.6/django_photofolio_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.692270 django-photofolio_ds-0.3.6/photofolio/
+-rw-rw-rw-   0        0        0        0 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/__init__.py
+-rw-rw-rw-   0        0        0       66 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/admin.py
+-rw-rw-rw-   0        0        0      158 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/apps.py
+-rw-rw-rw-   0        0        0     1178 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/forms.py
+-rw-rw-rw-   0        0        0       60 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/models.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.655068 django-photofolio_ds-0.3.6/photofolio/static/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.659802 django-photofolio_ds-0.3.6/photofolio/static/photofolio/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.694465 django-photofolio_ds-0.3.6/photofolio/static/photofolio/css/
+-rw-rw-rw-   0        0        0    24674 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/css/main.css
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.715725 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/
+-rw-rw-rw-   0        0        0     1738 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      491 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/favicon.png
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.829214 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/
+-rw-rw-rw-   0        0        0   254691 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-1.jpg
+-rw-rw-rw-   0        0        0   325115 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-10.jpg
+-rw-rw-rw-   0        0        0   191991 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-11.jpg
+-rw-rw-rw-   0        0        0   118728 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-12.jpg
+-rw-rw-rw-   0        0        0   613771 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-13.jpg
+-rw-rw-rw-   0        0        0   339998 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-14.jpg
+-rw-rw-rw-   0        0        0   169145 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-15.jpg
+-rw-rw-rw-   0        0        0   299838 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-16.jpg
+-rw-rw-rw-   0        0        0   376843 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-2.jpg
+-rw-rw-rw-   0        0        0   301323 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-3.jpg
+-rw-rw-rw-   0        0        0   290800 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-4.jpg
+-rw-rw-rw-   0        0        0   493094 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-5.jpg
+-rw-rw-rw-   0        0        0   351024 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-6.jpg
+-rw-rw-rw-   0        0        0   371929 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-7.jpg
+-rw-rw-rw-   0        0        0   187657 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-8.jpg
+-rw-rw-rw-   0        0        0   152783 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-9.jpg
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.848353 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/portfolio/
+-rw-rw-rw-   0        0        0    67064 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/portfolio/app-1.jpg
+-rw-rw-rw-   0        0        0    80146 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/portfolio/books-1.jpg
+-rw-rw-rw-   0        0        0    25514 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/portfolio/branding-1.jpg
+-rw-rw-rw-   0        0        0    62035 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/portfolio/product-1.jpg
+-rw-rw-rw-   0        0        0   238663 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/profile-img.jpg
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.877143 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/testimonials/
+-rw-rw-rw-   0        0        0    39727 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/testimonials/testimonials-1.jpg
+-rw-rw-rw-   0        0        0    57584 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/testimonials/testimonials-2.jpg
+-rw-rw-rw-   0        0        0    17247 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/testimonials/testimonials-3.jpg
+-rw-rw-rw-   0        0        0    20220 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/testimonials/testimonials-4.jpg
+-rw-rw-rw-   0        0        0    22595 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/testimonials/testimonials-5.jpg
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.878158 django-photofolio_ds-0.3.6/photofolio/static/photofolio/js/
+-rw-rw-rw-   0        0        0     4241 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/js/main.js
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.886475 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/
+-rw-rw-rw-   0        0        0      506 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/_footer.scss
+-rw-rw-rw-   0        0        0     5193 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/_general.scss
+-rw-rw-rw-   0        0        0     1102 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/_header.scss
+-rw-rw-rw-   0        0        0     1354 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/_hero.scss
+-rw-rw-rw-   0        0        0     4493 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/_nav.scss
+-rw-rw-rw-   0        0        0      214 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/_sections.scss
+-rw-rw-rw-   0        0        0      553 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/main.scss
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.895427 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/
+-rw-rw-rw-   0        0        0      651 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_about.scss
+-rw-rw-rw-   0        0        0     2718 2022-11-26 09:41:59.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_contact.scss
+-rw-rw-rw-   0        0        0     3656 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_gallery-single.scss
+-rw-rw-rw-   0        0        0     1177 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_gallery.scss
+-rw-rw-rw-   0        0        0      511 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_pricing.scss
+-rw-rw-rw-   0        0        0     1423 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_services.scss
+-rw-rw-rw-   0        0        0     1716 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_testimonials.scss
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.664599 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.897695 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/aos/
+-rw-rw-rw-   0        0        0    26053 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/aos/aos.css
+-rw-rw-rw-   0        0        0    14690 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/aos/aos.js
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.662187 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.951356 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/
+-rw-rw-rw-   0        0        0    71861 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0   210292 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0    53265 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0   131408 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-rw-   0        0        0    71935 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-rw-   0        0        0   210296 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-rw-   0        0        0    53340 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-rw-   0        0        0   131485 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-rw-   0        0        0     7965 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0   110811 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0     6490 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0    40345 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-rw-   0        0        0     7958 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-rw-   0        0        0   110824 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-rw-   0        0        0     6562 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-rw-   0        0        0    48707 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-rw-   0        0        0    74135 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0   196370 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-rw-   0        0        0    56365 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-rw-   0        0        0   115601 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-rw-   0        0        0    74002 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-rw-   0        0        0   196313 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-rw-   0        0        0    56293 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-rw-   0        0        0   115436 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-rw-   0        0        0   237872 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0        0        0   606249 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   194699 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   521459 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0   237386 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-rw-rw-   0        0        0   606069 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-rw-   0        0        0   194803 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-rw-   0        0        0   765329 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.970801 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/
+-rw-rw-rw-   0        0        0   207083 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0   448881 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-rw-   0        0        0    79790 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   330849 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0   135367 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.js
+-rw-rw-rw-   0        0        0   306814 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-rw-   0        0        0    73539 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-rw-   0        0        0   220143 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-rw-   0        0        0   144701 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0        0        0   307954 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.js.map
+-rw-rw-rw-   0        0        0    60104 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0   215897 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.min.js.map
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.903076 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/
+-rw-rw-rw-   0        0        0    88585 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-rw-rw-   0        0        0    47187 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   211136 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/bootstrap-icons.scss
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.905701 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/fonts/
+-rw-rw-rw-   0        0        0   150592 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-rw-rw-   0        0        0   112440 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-rw-rw-   0        0        0   218010 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/index.html
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.663190 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.975921 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/css/
+-rw-rw-rw-   0        0        0    17372 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/css/glightbox.css
+-rw-rw-rw-   0        0        0    13749 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/css/glightbox.min.css
+-rw-rw-rw-   0        0        0    52561 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/css/plyr.css
+-rw-rw-rw-   0        0        0    45081 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/css/plyr.min.css
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.978432 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/js/
+-rw-rw-rw-   0        0        0   109391 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/js/glightbox.js
+-rw-rw-rw-   0        0        0    55880 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/js/glightbox.min.js
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.982020 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/php-email-form/
+-rw-rw-rw-   0        0        0   232262 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/php-email-form/php-email-form.php
+-rw-rw-rw-   0        0        0     2731 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/php-email-form/validate.js
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.984390 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/swiper/
+-rw-rw-rw-   0        0        0    16466 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/swiper/swiper-bundle.min.css
+-rw-rw-rw-   0        0        0   143070 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/swiper/swiper-bundle.min.js
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.665604 django-photofolio_ds-0.3.6/photofolio/templates/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:44.997055 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/
+-rw-rw-rw-   0        0        0      833 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/_about.html
+-rw-rw-rw-   0        0        0     3030 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/_contact.html
+-rw-rw-rw-   0        0        0      777 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/_gallery.html
+-rw-rw-rw-   0        0        0      509 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/_hero.html
+-rw-rw-rw-   0        0        0      505 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/_pricing.html
+-rw-rw-rw-   0        0        0      480 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/_services.html
+-rw-rw-rw-   0        0        0     1176 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/_testimonials.html
+-rw-rw-rw-   0        0        0      357 2023-05-09 02:01:28.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/footer.html
+-rw-rw-rw-   0        0        0     3110 2022-12-08 08:45:17.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/header.html
+-rw-rw-rw-   0        0        0     2302 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/index.html
+-rw-rw-rw-   0        0        0     1460 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/seo.html
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:45.003343 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/
+-rw-rw-rw-   0        0        0     2799 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/about.html
+-rw-rw-rw-   0        0        0     2660 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/contact.html
+-rw-rw-rw-   0        0        0    10081 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/gallery-single.html
+-rw-rw-rw-   0        0        0     2694 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/gallery.html
+-rw-rw-rw-   0        0        0     5902 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/sample-inner-page.html
+-rw-rw-rw-   0        0        0     3091 2022-12-08 08:45:17.000000 django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/services.html
+drwxrwxrwx   0        0        0        0 2023-05-09 02:01:45.006103 django-photofolio_ds-0.3.6/photofolio/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/photofolio/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     3442 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/templatetags/sections.py
+-rw-rw-rw-   0        0        0      632 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/urls.py
+-rw-rw-rw-   0        0        0     4924 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/photofolio/views.py
+-rw-rw-rw-   0        0        0      112 2022-11-26 09:42:01.000000 django-photofolio_ds-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0      756 2023-05-09 02:01:45.009631 django-photofolio_ds-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-11-26 09:42:00.000000 django-photofolio_ds-0.3.6/setup.py
```

### Comparing `django-photofolio_ds-0.3.5/LICENSE` & `django-photofolio_ds-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/PKG-INFO` & `django-photofolio_ds-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-photofolio_ds
-Version: 0.3.5
+Version: 0.3.6
 Summary: photofolio_pro porting for django
 Home-page: https://www.demiansoft.com
 Author: hyungjin kim
 Author-email: hj3415@gmail.com
 Project-URL: Bug Tracker, https://pypi.org/project/util-demian/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-photofolio_ds-0.3.5/README.md` & `django-photofolio_ds-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/django_photofolio_ds.egg-info/PKG-INFO` & `django-photofolio_ds-0.3.6/django_photofolio_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-photofolio-ds
-Version: 0.3.5
+Version: 0.3.6
 Summary: photofolio_pro porting for django
 Home-page: https://www.demiansoft.com
 Author: hyungjin kim
 Author-email: hj3415@gmail.com
 Project-URL: Bug Tracker, https://pypi.org/project/util-demian/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-photofolio_ds-0.3.5/django_photofolio_ds.egg-info/SOURCES.txt` & `django-photofolio_ds-0.3.6/django_photofolio_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/forms.py` & `django-photofolio_ds-0.3.6/photofolio/forms.py`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/css/main.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/css/main.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/apple-touch-icon.png` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-1.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-1.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-10.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-10.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-11.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-11.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-12.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-12.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-13.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-13.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-14.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-14.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-15.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-15.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-16.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-16.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-2.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-2.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-3.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-3.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-4.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-4.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-5.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-5.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-6.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-6.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-7.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-7.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-8.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-8.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/gallery/gallery-9.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/gallery/gallery-9.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/portfolio/app-1.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/portfolio/app-1.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/portfolio/books-1.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/portfolio/books-1.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/portfolio/branding-1.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/portfolio/branding-1.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/portfolio/product-1.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/portfolio/product-1.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/profile-img.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/profile-img.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/testimonials/testimonials-1.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/testimonials/testimonials-1.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/testimonials/testimonials-2.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/testimonials/testimonials-2.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/testimonials/testimonials-3.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/testimonials/testimonials-3.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/testimonials/testimonials-4.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/testimonials/testimonials-4.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/img/testimonials/testimonials-5.jpg` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/img/testimonials/testimonials-5.jpg`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/js/main.js` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/js/main.js`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/_general.scss` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/_header.scss` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/_hero.scss` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/_hero.scss`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/_nav.scss` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/main.scss` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/main.scss`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_about.scss` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_about.scss`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_contact.scss` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_contact.scss`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_gallery-single.scss` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_gallery-single.scss`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_gallery.scss` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_gallery.scss`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_services.scss` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_services.scss`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/scss/sections/_testimonials.scss` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/scss/sections/_testimonials.scss`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/aos/aos.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/aos/aos.js` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.min.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.min.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.min.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.js` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.js` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.js.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.min.js` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.js` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.js.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.min.js` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.min.js.map` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/bootstrap-icons.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/bootstrap-icons.json` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/bootstrap-icons.scss` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/bootstrap-icons/index.html` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/bootstrap-icons/index.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/css/glightbox.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/css/glightbox.min.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/css/plyr.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/css/plyr.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/css/plyr.min.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/css/plyr.min.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/js/glightbox.js` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/glightbox/js/glightbox.min.js` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/php-email-form/php-email-form.php` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/php-email-form/validate.js` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/swiper/swiper-bundle.min.css` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/static/photofolio/vendor/swiper/swiper-bundle.min.js` & `django-photofolio_ds-0.3.6/photofolio/static/photofolio/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/_about.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/_about.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/_contact.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/_contact.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/_gallery.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/_gallery.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/_testimonials.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/_testimonials.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/header.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/header.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/index.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/index.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/seo.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/seo.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/about.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/about.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/contact.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/contact.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/gallery-single.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/gallery-single.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/gallery.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/gallery.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/sample-inner-page.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/sample-inner-page.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templates/photofolio/sub/services.html` & `django-photofolio_ds-0.3.6/photofolio/templates/photofolio/sub/services.html`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/templatetags/sections.py` & `django-photofolio_ds-0.3.6/photofolio/templatetags/sections.py`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/urls.py` & `django-photofolio_ds-0.3.6/photofolio/urls.py`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/photofolio/views.py` & `django-photofolio_ds-0.3.6/photofolio/views.py`

 * *Files identical despite different names*

### Comparing `django-photofolio_ds-0.3.5/setup.cfg` & `django-photofolio_ds-0.3.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 7068 6f74 6f66   = django-photof
 00000020: 6f6c 696f 5f64 730d 0a76 6572 7369 6f6e  olio_ds..version
-00000030: 203d 2030 2e33 2e35 0d0a 6175 7468 6f72   = 0.3.5..author
+00000030: 203d 2030 2e33 2e36 0d0a 6175 7468 6f72   = 0.3.6..author
 00000040: 203d 2068 7975 6e67 6a69 6e20 6b69 6d0d   = hyungjin kim.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 686a 3334 3135 4067 6d61 696c 2e63 6f6d  hj3415@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 7068 6f74 6f66 6f6c 696f 5f70 726f 2070  photofolio_pro p
 00000090: 6f72 7469 6e67 2066 6f72 2064 6a61 6e67  orting for djang
 000000a0: 6f0d 0a6c 6f6e 675f 6465 7363 7269 7074  o..long_descript
```

