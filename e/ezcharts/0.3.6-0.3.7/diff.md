# Comparing `tmp/ezcharts-0.3.6.tar.gz` & `tmp/ezcharts-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcharts-0.3.6.tar", last modified: Fri Mar 31 11:41:23 2023, max compression
+gzip compressed data, was "ezcharts-0.3.7.tar", last modified: Tue May  9 15:08:59 2023, max compression
```

## Comparing `ezcharts-0.3.6.tar` & `ezcharts-0.3.7.tar`

### file list

```diff
@@ -1,193 +1,199 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.479740 ezcharts-0.3.6/
--rw-rw-rw-   0 root         (0) root         (0)    15820 2023-03-30 09:48:38.000000 ezcharts-0.3.6/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-03-30 09:48:38.000000 ezcharts-0.3.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5779 2023-03-31 11:41:23.479740 ezcharts-0.3.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5524 2023-03-30 09:48:38.000000 ezcharts-0.3.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.295724 ezcharts-0.3.6/ezcharts/
--rw-rw-rw-   0 root         (0) root         (0)     1736 2023-03-31 11:37:09.000000 ezcharts-0.3.6/ezcharts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.299724 ezcharts-0.3.6/ezcharts/components/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/components/ezchart.py
--rw-rw-rw-   0 root         (0) root         (0)     6322 2023-03-31 11:37:09.000000 ezcharts-0.3.6/ezcharts/components/fastcat.py
--rw-rw-rw-   0 root         (0) root         (0)     1858 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/components/nextclade.py
--rw-rw-rw-   0 root         (0) root         (0)     1634 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/components/params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.299724 ezcharts-0.3.6/ezcharts/components/reports/
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/components/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/components/reports/comp.py
--rw-rw-rw-   0 root         (0) root         (0)     7291 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/components/reports/labs.py
--rw-rw-rw-   0 root         (0) root         (0)     2422 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/components/theme.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/components/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.291724 ezcharts-0.3.6/ezcharts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.299724 ezcharts-0.3.6/ezcharts/data/images/
--rw-rw-rw-   0 root         (0) root         (0)     1978 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/images/LAB_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)    33283 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/images/OND_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)    32771 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/images/ONT_logo.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.291724 ezcharts-0.3.6/ezcharts/data/reference/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.303725 ezcharts-0.3.6/ezcharts/data/reference/hg19/
--rw-rw-rw-   0 root         (0) root         (0)     6297 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/reference/hg19/cytoBand.txt.gz
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.303725 ezcharts-0.3.6/ezcharts/data/reference/hg38/
--rw-rw-rw-   0 root         (0) root         (0)    11449 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/reference/hg38/cytoBand.txt.gz
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.303725 ezcharts-0.3.6/ezcharts/data/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1636 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/scripts/epi2melabs.js
--rw-rw-rw-   0 root         (0) root         (0)     1236 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/scripts/nextclade.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.303725 ezcharts-0.3.6/ezcharts/data/styles/
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/styles/epi2melabs.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.303725 ezcharts-0.3.6/ezcharts/data/test/
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/test/fastcat.stats.gz
--rw-rw-rw-   0 root         (0) root         (0)    28549 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/test/hg38_cnv.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)     2420 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/test/hg38_some_bands.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)    16943 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/test/nextclade.json
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/test/params.json
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/test/plot-spec.json
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/test/versions.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.303725 ezcharts-0.3.6/ezcharts/data/themes/
--rw-rw-rw-   0 root         (0) root         (0)     5771 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/themes/epi2melabs.json
--rw-rw-rw-   0 root         (0) root         (0)     5536 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/themes/walden.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.303725 ezcharts-0.3.6/ezcharts/data/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.291724 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.307725 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/js/
--rw-rw-rw-   0 root         (0) root         (0)    80599 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.315726 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/
--rw-rw-rw-   0 root         (0) root         (0)     5066 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
--rw-rw-rw-   0 root         (0) root         (0)     2055 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
--rw-rw-rw-   0 root         (0) root         (0)     1751 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
--rw-rw-rw-   0 root         (0) root         (0)     3195 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     6685 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss
--rw-rw-rw-   0 root         (0) root         (0)     6941 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss
--rw-rw-rw-   0 root         (0) root         (0)     5751 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss
--rw-rw-rw-   0 root         (0) root         (0)     1948 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss
--rw-rw-rw-   0 root         (0) root         (0)     1201 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss
--rw-rw-rw-   0 root         (0) root         (0)     8093 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)    10554 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_helpers.scss
--rw-rw-rw-   0 root         (0) root         (0)     1158 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss
--rw-rw-rw-   0 root         (0) root         (0)     6775 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     4043 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss
--rw-rw-rw-   0 root         (0) root         (0)     7762 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss
--rw-rw-rw-   0 root         (0) root         (0)     4665 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss
--rw-rw-rw-   0 root         (0) root         (0)     9104 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss
--rw-rw-rw-   0 root         (0) root         (0)     4725 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss
--rw-rw-rw-   0 root         (0) root         (0)     3944 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss
--rw-rw-rw-   0 root         (0) root         (0)     6907 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss
--rw-rw-rw-   0 root         (0) root         (0)    12404 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss
--rw-rw-rw-   0 root         (0) root         (0)     7371 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss
--rw-rw-rw-   0 root         (0) root         (0)     4413 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss
--rw-rw-rw-   0 root         (0) root         (0)     2490 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss
--rw-rw-rw-   0 root         (0) root         (0)     3939 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_transitions.scss
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss
--rw-rw-rw-   0 root         (0) root         (0)    17886 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)     3840 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss
--rw-rw-rw-   0 root         (0) root         (0)    73610 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)     1253 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-reboot.scss
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.315726 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss
--rw-rw-rw-   0 root         (0) root         (0)     4833 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss
--rw-rw-rw-   0 root         (0) root         (0)     5868 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss
--rw-rw-rw-   0 root         (0) root         (0)     2796 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss
--rw-rw-rw-   0 root         (0) root         (0)     2603 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-text.scss
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     1142 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss
--rw-rw-rw-   0 root         (0) root         (0)      478 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_validation.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.319726 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_clearfix.scss
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_color-bg.scss
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_colored-links.scss
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss
--rw-rw-rw-   0 root         (0) root         (0)      399 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_ratio.scss
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stacks.scss
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stretched-link.scss
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_text-truncation.scss
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_visually-hidden.scss
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_vr.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.323727 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_backdrop.scss
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_banner.scss
--rw-rw-rw-   0 root         (0) root         (0)     2031 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_box-shadow.scss
--rw-rw-rw-   0 root         (0) root         (0)     4580 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss
--rw-rw-rw-   0 root         (0) root         (0)     3220 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_clearfix.scss
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-mode.scss
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-scheme.scss
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_container.scss
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss
--rw-rw-rw-   0 root         (0) root         (0)     4164 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)     1956 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss
--rw-rw-rw-   0 root         (0) root         (0)     4726 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_image.scss
--rw-rw-rw-   0 root         (0) root         (0)      582 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_lists.scss
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_pagination.scss
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_reset-text.scss
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_resize.scss
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_text-truncate.scss
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss
--rw-rw-rw-   0 root         (0) root         (0)     3380 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.323727 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/
--rw-rw-rw-   0 root         (0) root         (0)     1737 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.323727 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/
--rw-rw-rw-   0 root         (0) root         (0)    10029 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss
--rw-rw-rw-   0 root         (0) root         (0)  1017477 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/echarts.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.323727 ezcharts-0.3.6/ezcharts/data/vendor/simple-datatables/
--rw-rw-rw-   0 root         (0) root         (0)     3104 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/simple-datatables/simple-datatables.css
--rw-rw-rw-   0 root         (0) root         (0)    38201 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/data/vendor/simple-datatables/simple-datatables.js
--rw-rw-rw-   0 root         (0) root         (0)     8533 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/demo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.327727 ezcharts-0.3.6/ezcharts/layout/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.327727 ezcharts-0.3.6/ezcharts/layout/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/snippets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2840 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/snippets/banner.py
--rw-rw-rw-   0 root         (0) root         (0)     2106 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/snippets/cards.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/snippets/document.py
--rw-rw-rw-   0 root         (0) root         (0)     2126 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/snippets/grid.py
--rw-rw-rw-   0 root         (0) root         (0)     2529 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/snippets/offcanvas.py
--rw-rw-rw-   0 root         (0) root         (0)     2758 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/snippets/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/snippets/section.py
--rw-rw-rw-   0 root         (0) root         (0)     1550 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/snippets/stats.py
--rw-rw-rw-   0 root         (0) root         (0)     7587 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/snippets/table.py
--rw-rw-rw-   0 root         (0) root         (0)     5636 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/snippets/tabs.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/layout/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.479740 ezcharts-0.3.6/ezcharts/plots/
--rw-rw-rw-   0 root         (0) root         (0)     8937 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/plots/_base.py
--rw-rw-rw-   0 root         (0) root         (0) 13970130 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/plots/_model.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/plots/axisgrid.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/plots/categorical.py
--rw-rw-rw-   0 root         (0) root         (0)     5065 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/plots/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)    12727 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/plots/ideogram.py
--rw-rw-rw-   0 root         (0) root         (0)     2903 2023-03-31 11:37:10.000000 ezcharts-0.3.6/ezcharts/plots/matrix.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/plots/regression.py
--rw-rw-rw-   0 root         (0) root         (0)     5424 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/plots/relational.py
--rw-rw-rw-   0 root         (0) root         (0)     6139 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/plots/util.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-03-30 09:48:38.000000 ezcharts-0.3.6/ezcharts/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 11:41:23.299724 ezcharts-0.3.6/ezcharts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5779 2023-03-31 11:41:23.000000 ezcharts-0.3.6/ezcharts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7906 2023-03-31 11:41:23.000000 ezcharts-0.3.6/ezcharts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 11:41:23.000000 ezcharts-0.3.6/ezcharts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-03-31 11:41:23.000000 ezcharts-0.3.6/ezcharts.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 11:40:25.000000 ezcharts-0.3.6/ezcharts.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       77 2023-03-31 11:41:23.000000 ezcharts-0.3.6/ezcharts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-31 11:41:23.000000 ezcharts-0.3.6/ezcharts.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-03-30 09:48:38.000000 ezcharts-0.3.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 11:41:23.479740 ezcharts-0.3.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2187 2023-03-30 09:48:38.000000 ezcharts-0.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:59.098583 ezcharts-0.3.7/
+-rw-rw-rw-   0 root         (0) root         (0)    15820 2023-05-09 15:05:25.000000 ezcharts-0.3.7/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-09 15:05:25.000000 ezcharts-0.3.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5779 2023-05-09 15:08:59.098583 ezcharts-0.3.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5524 2023-05-09 15:05:25.000000 ezcharts-0.3.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.098496 ezcharts-0.3.7/ezcharts/
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.118498 ezcharts-0.3.7/ezcharts/components/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/components/ezchart.py
+-rw-rw-rw-   0 root         (0) root         (0)     6322 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/components/fastcat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/components/nextclade.py
+-rw-rw-rw-   0 root         (0) root         (0)     1634 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/components/params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.126499 ezcharts-0.3.7/ezcharts/components/reports/
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/components/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/components/reports/comp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7291 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/components/reports/labs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7345 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/components/reports/ond.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/components/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/components/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.078495 ezcharts-0.3.7/ezcharts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.138500 ezcharts-0.3.7/ezcharts/data/images/
+-rw-rw-rw-   0 root         (0) root         (0)     1978 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/images/LAB_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/images/OND_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    33283 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/images/OND_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)    32771 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/images/ONT_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)   894078 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/images/dots.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.074494 ezcharts-0.3.7/ezcharts/data/reference/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.198505 ezcharts-0.3.7/ezcharts/data/reference/hg19/
+-rw-rw-rw-   0 root         (0) root         (0)     6297 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/reference/hg19/cytoBand.txt.gz
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.198505 ezcharts-0.3.7/ezcharts/data/reference/hg38/
+-rw-rw-rw-   0 root         (0) root         (0)    11449 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/reference/hg38/cytoBand.txt.gz
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.202505 ezcharts-0.3.7/ezcharts/data/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/scripts/epi2melabs.js
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/scripts/nextclade.html
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/scripts/ond.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.202505 ezcharts-0.3.7/ezcharts/data/styles/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/styles/epi2melabs.scss
+-rw-rw-rw-   0 root         (0) root         (0)   898896 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/styles/ond.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.390522 ezcharts-0.3.7/ezcharts/data/test/
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/test/fastcat.stats.gz
+-rw-rw-rw-   0 root         (0) root         (0)    28549 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/test/hg38_cnv.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2420 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/test/hg38_some_bands.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)    16943 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/test/nextclade.json
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/test/params.json
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/test/plot-spec.json
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/test/versions.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.394522 ezcharts-0.3.7/ezcharts/data/themes/
+-rw-rw-rw-   0 root         (0) root         (0)     5771 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/themes/epi2melabs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5764 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/themes/ond.json
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/themes/walden.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.394522 ezcharts-0.3.7/ezcharts/data/vendor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.078495 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.518533 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/js/
+-rw-rw-rw-   0 root         (0) root         (0)    80599 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.642544 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2055 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1751 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3195 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6685 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6941 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss
+-rw-rw-rw-   0 root         (0) root         (0)     5751 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1948 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss
+-rw-rw-rw-   0 root         (0) root         (0)     8093 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)    10554 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_helpers.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6775 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4043 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3944 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6907 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss
+-rw-rw-rw-   0 root         (0) root         (0)    12404 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss
+-rw-rw-rw-   0 root         (0) root         (0)     7371 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_transitions.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss
+-rw-rw-rw-   0 root         (0) root         (0)    17886 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss
+-rw-rw-rw-   0 root         (0) root         (0)    73610 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-reboot.scss
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.646544 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4833 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss
+-rw-rw-rw-   0 root         (0) root         (0)     5868 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2603 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-text.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss
+-rw-rw-rw-   0 root         (0) root         (0)      478 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_validation.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.654545 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_clearfix.scss
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_color-bg.scss
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_colored-links.scss
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss
+-rw-rw-rw-   0 root         (0) root         (0)      399 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_ratio.scss
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stacks.scss
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stretched-link.scss
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_text-truncation.scss
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_visually-hidden.scss
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_vr.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.694548 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_backdrop.scss
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_banner.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_box-shadow.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4580 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_clearfix.scss
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-mode.scss
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-scheme.scss
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_container.scss
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4164 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4726 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_image.scss
+-rw-rw-rw-   0 root         (0) root         (0)      582 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_lists.scss
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_pagination.scss
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_reset-text.scss
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_resize.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_text-truncate.scss
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3380 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.694548 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.694548 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/
+-rw-rw-rw-   0 root         (0) root         (0)    10029 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss
+-rw-rw-rw-   0 root         (0) root         (0)  1017477 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/echarts.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.694548 ezcharts-0.3.7/ezcharts/data/vendor/simple-datatables/
+-rw-rw-rw-   0 root         (0) root         (0)     3104 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/simple-datatables/simple-datatables.css
+-rw-rw-rw-   0 root         (0) root         (0)    38201 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/data/vendor/simple-datatables/simple-datatables.js
+-rw-rw-rw-   0 root         (0) root         (0)     8533 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/demo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.702549 ezcharts-0.3.7/ezcharts/layout/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.726551 ezcharts-0.3.7/ezcharts/layout/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/snippets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2880 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/snippets/banner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2119 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/snippets/cards.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/snippets/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     2126 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/snippets/grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2605 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/snippets/offcanvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2758 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/snippets/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/snippets/section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1550 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/snippets/stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     7587 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/snippets/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     5636 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/snippets/tabs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2893 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/layout/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:59.094583 ezcharts-0.3.7/ezcharts/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     8969 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/plots/_base.py
+-rw-rw-rw-   0 root         (0) root         (0) 13970130 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/plots/_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/plots/axisgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2945 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/plots/categorical.py
+-rw-rw-rw-   0 root         (0) root         (0)     5065 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/plots/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)    12727 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/plots/ideogram.py
+-rw-rw-rw-   0 root         (0) root         (0)     2903 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/plots/matrix.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/plots/regression.py
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/plots/relational.py
+-rw-rw-rw-   0 root         (0) root         (0)     6139 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/plots/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-05-09 15:05:25.000000 ezcharts-0.3.7/ezcharts/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 15:08:58.114498 ezcharts-0.3.7/ezcharts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5779 2023-05-09 15:08:58.000000 ezcharts-0.3.7/ezcharts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8094 2023-05-09 15:08:58.000000 ezcharts-0.3.7/ezcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 15:08:58.000000 ezcharts-0.3.7/ezcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-09 15:08:58.000000 ezcharts-0.3.7/ezcharts.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 15:07:51.000000 ezcharts-0.3.7/ezcharts.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-09 15:08:58.000000 ezcharts-0.3.7/ezcharts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-09 15:08:58.000000 ezcharts-0.3.7/ezcharts.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-05-09 15:05:25.000000 ezcharts-0.3.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 15:08:59.098583 ezcharts-0.3.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2023-05-09 15:05:25.000000 ezcharts-0.3.7/setup.py
```

### Comparing `ezcharts-0.3.6/LICENSE.md` & `ezcharts-0.3.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/PKG-INFO` & `ezcharts-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcharts
-Version: 0.3.6
+Version: 0.3.7
 Summary: eCharts plotting API.
 Home-page: https://github.com/epi2me-labs/ezcharts
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `ezcharts-0.3.6/README.md` & `ezcharts-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/__init__.py` & `ezcharts-0.3.7/ezcharts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Simple eCharts API."""
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 
 import argparse
 import importlib
 import logging
 
 from ezcharts import util
 from ezcharts.plots.axisgrid import *  # noqa: F401,F403
```

### Comparing `ezcharts-0.3.6/ezcharts/components/ezchart.py` & `ezcharts-0.3.7/ezcharts/components/ezchart.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/components/fastcat.py` & `ezcharts-0.3.7/ezcharts/components/fastcat.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/components/nextclade.py` & `ezcharts-0.3.7/ezcharts/components/nextclade.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/components/params.py` & `ezcharts-0.3.7/ezcharts/components/params.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/components/reports/__init__.py` & `ezcharts-0.3.7/ezcharts/components/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/components/reports/comp.py` & `ezcharts-0.3.7/ezcharts/components/reports/comp.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/components/reports/labs.py` & `ezcharts-0.3.7/ezcharts/components/reports/labs.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/components/theme.py` & `ezcharts-0.3.7/ezcharts/components/theme.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,39 +37,45 @@
     loader=load_json)
 
 
 LAB_head_resources = [LAB_CSS, *base_head_resources, LAB_CHART_THEME]
 LAB_body_resources = [LAB_JS, *base_body_resources]
 
 
-class ONDLogo(img):
+class ONDLogo(div):
     """OND logo element."""
 
     def __init__(self) -> None:
         """Create an img with the data URI logo."""
         super().__init__(
-            inline(ImageResource('OND_logo.txt').data_file),
-            tagname='img',
-            style="height: 35px;",
+            inline(ImageResource('OND_logo.svg').data_file),
+            tagname='div',
+            style="width: 35px; height: 35px;",
             className="d-flex",
             alt="OND Logo")
 
 
 # TODO: Create
 OND_CSS = StyleResource(
-    path='epi2melabs.scss',
+    path='ond.scss',
     tag=style,
     loader=transpile)
 
 OND_JS = ScriptResource(
-    path='epi2melabs.js',
+    path='ond.js',
     tag=script,
     loader=inline)
 
-OND_head_resources = [OND_CSS, *base_head_resources]
+
+OND_CHART_THEME = ThemeResource(
+    path='ond.json',
+    tag=EZChartTheme,
+    loader=load_json)
+
+OND_head_resources = [OND_CSS, *base_head_resources, OND_CHART_THEME]
 OND_body_resources = [OND_JS, *base_body_resources]
 
 
 class ONTLogo(img):
     """ONT logo element."""
 
     def __init__(self) -> None:
```

### Comparing `ezcharts-0.3.6/ezcharts/components/versions.py` & `ezcharts-0.3.7/ezcharts/components/versions.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/images/LAB_logo.svg` & `ezcharts-0.3.7/ezcharts/data/images/LAB_logo.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/images/OND_logo.txt` & `ezcharts-0.3.7/ezcharts/data/images/OND_logo.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/images/ONT_logo.txt` & `ezcharts-0.3.7/ezcharts/data/images/ONT_logo.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/reference/hg19/cytoBand.txt.gz` & `ezcharts-0.3.7/ezcharts/data/reference/hg19/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/reference/hg38/cytoBand.txt.gz` & `ezcharts-0.3.7/ezcharts/data/reference/hg38/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/scripts/epi2melabs.js` & `ezcharts-0.3.7/ezcharts/data/scripts/epi2melabs.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/test/fastcat.stats.gz` & `ezcharts-0.3.7/ezcharts/data/test/fastcat.stats.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/test/hg38_cnv.bed.gz` & `ezcharts-0.3.7/ezcharts/data/test/hg38_cnv.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/test/hg38_some_bands.bed.gz` & `ezcharts-0.3.7/ezcharts/data/test/hg38_some_bands.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/test/nextclade.json` & `ezcharts-0.3.7/ezcharts/data/test/nextclade.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/test/params.json` & `ezcharts-0.3.7/ezcharts/data/test/params.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/test/plot-spec.json` & `ezcharts-0.3.7/ezcharts/data/test/plot-spec.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/themes/epi2melabs.json` & `ezcharts-0.3.7/ezcharts/data/themes/epi2melabs.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/themes/walden.json` & `ezcharts-0.3.7/ezcharts/data/themes/walden.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss` & `ezcharts-0.3.7/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/echarts.min.js` & `ezcharts-0.3.7/ezcharts/data/vendor/echarts.min.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/simple-datatables/simple-datatables.css` & `ezcharts-0.3.7/ezcharts/data/vendor/simple-datatables/simple-datatables.css`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/data/vendor/simple-datatables/simple-datatables.js` & `ezcharts-0.3.7/ezcharts/data/vendor/simple-datatables/simple-datatables.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/demo.py` & `ezcharts-0.3.7/ezcharts/demo.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/layout/base.py` & `ezcharts-0.3.7/ezcharts/layout/base.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/layout/resource.py` & `ezcharts-0.3.7/ezcharts/layout/resource.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/layout/snippets/__init__.py` & `ezcharts-0.3.7/ezcharts/layout/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/layout/snippets/banner.py` & `ezcharts-0.3.7/ezcharts/layout/snippets/banner.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,16 +42,17 @@
             className=f"{classes.container} {bg}",
             style=styles.container)
 
 
 class IBannerClasses(IClasses):
     """Section html classes."""
 
-    container: str = cls("px-4", "bg-dark")
-    inner: str = cls("container", "px-0", "py-5", "border-top", "text-white")
+    container: str = cls("px-4", "bg-dark", "labs-banner")
+    inner: str = cls(
+        "container", "px-0", "py-3", "border-top", "text-white", "report-title")
 
 
 class IBannerStyles(IStyles):
     """Section inline css styles."""
 
     container: str = css(
         "margin-bottom: -25px",
```

### Comparing `ezcharts-0.3.6/ezcharts/layout/snippets/cards.py` & `ezcharts-0.3.7/ezcharts/layout/snippets/cards.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     classes: Optional[str] = None
 
 
 class ICardClasses(IClasses):
     """Cards html classes."""
 
     container: str = cls("container", "px-0")
-    card: str = cls("card", "px-0", "mb-4")
+    card: str = cls("card", "px-0", "mb-4", "shadow-sm")
     card_body: str = cls("card-body")
     card_heading: str = cls("card-header")
     card_text: str = cls("card-text")
     card_footer: str = cls("card-footer small")
 
 
 class Cards(Snippet):
```

### Comparing `ezcharts-0.3.6/ezcharts/layout/snippets/document.py` & `ezcharts-0.3.7/ezcharts/layout/snippets/document.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/layout/snippets/grid.py` & `ezcharts-0.3.7/ezcharts/layout/snippets/grid.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/layout/snippets/offcanvas.py` & `ezcharts-0.3.7/ezcharts/layout/snippets/offcanvas.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class IOffCanvasClasses(IClasses):
     """Cards html classes."""
 
     container: str = cls("container", "px-0")
     offcanvas: str = cls("offcanvas", "offcanvas-bottom", "h-auto")
-    offcanvas_button: str = cls("btn")
+    offcanvas_button: str = cls("")
     offcanvas_header: str = cls("offcanvas-header")
     offcanvas_title: str = cls("offcanvas-title")
     offcanvas_body: str = cls("offcanvas-body")
 
 
 class OffCanvas(Snippet):
     """A styled section tag."""
@@ -47,15 +47,15 @@
     def add_offcanvas(
         self,
         title: str,
         label: str,
         new_uid: str,
         body: Optional[str] = None,
         offcanvas_cls: Optional[str] = None,
-        offcanvas_btn_cls: Optional[str] = "btn-primary",
+        offcanvas_btn_cls: Optional[str] = "btn-info",
         head_tag: Type[html_tag] = h5
     ) -> None:
         """Add cards to the grid."""
         button(
                 label,
                 type="button",
                 data_bs_toggle="offcanvas",
@@ -70,15 +70,18 @@
             id=new_uid,
             tabindex=-1,
             aria_labelledby="offcanvasBottomLabel",
             className=cls(
                 self.classes.offcanvas,
                 offcanvas_cls if offcanvas_cls is not None else '')):
 
-            with div(className=cls(self.classes.offcanvas_header)):
+            with div(className=cls(
+                    self.classes.offcanvas_header,
+                    'container',
+                    'px-0')):
                 head_tag(title, className=self.classes.offcanvas_title)
                 button(
                     type="button",
                     cls="btn-close",
                     data_bs_dismiss="offcanvas",
                     aria_label="Close")
```

### Comparing `ezcharts-0.3.6/ezcharts/layout/snippets/progress.py` & `ezcharts-0.3.7/ezcharts/layout/snippets/progress.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/layout/snippets/section.py` & `ezcharts-0.3.7/ezcharts/layout/snippets/section.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/layout/snippets/stats.py` & `ezcharts-0.3.7/ezcharts/layout/snippets/stats.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/layout/snippets/table.py` & `ezcharts-0.3.7/ezcharts/layout/snippets/table.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/layout/snippets/tabs.py` & `ezcharts-0.3.7/ezcharts/layout/snippets/tabs.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/plots/__init__.py` & `ezcharts-0.3.7/ezcharts/plots/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Plotting functionality via echarts."""
 
 import argparse
 
-import numpy as np
 import pandas as pd
 from pkg_resources import resource_filename
 import sigfig
 
 from ezcharts import util as ezutil
 from ezcharts.components.ezchart import EZChart
 from ezcharts.components.reports.comp import ComponentReport
@@ -20,15 +19,15 @@
 
 _logger = ezutil.get_named_logger("Plotter")
 
 
 class AxisLabelFormatter(JSCode):
     """Formatter for echarts axis labels."""
 
-    def __init__(self, sci_notation=(0.0001, 10000)):
+    def __init__(self, sci_notation=(0.001, 10000)):
         """Init.
 
         :param: sci_notation:
             True: use scientific notation for the axis.
             False: use raw values for the axis.
             tuple: Upper and lower limits for determining use of scientific notation.
         """
@@ -60,20 +59,20 @@
             use_sci = False
         else:
             if self.sci_notation is True:
                 use_sci = True
             elif self.sci_notation is False:
                 use_sci = False
             else:
-                # If any values fall outside the limits, covert all to sci_notation.
-                # Do not include zeros as they are always plotted as '0'.
+                # If the value with the largest magnitude (in other words, the largest
+                # positive or negative value or value furthest from zero) falls outside
+                # the limits, convert all to sci_notation.
                 sci_limits = self.sci_notation
-                v = np.array(values)
-                v = v[v != 0]
-                if ((v < sci_limits[0]) | (v > sci_limits[1])).any():
+                v = max(abs(min(values)), max(values))
+                if v < sci_limits[0] or v > sci_limits[1]:
                     use_sci = True
                 else:
                     use_sci = False
         super().__init__(self.jscode.replace('@use_sci', f"'{str(use_sci).lower()}'"))
         return use_sci
```

### Comparing `ezcharts-0.3.6/ezcharts/plots/_base.py` & `ezcharts-0.3.7/ezcharts/plots/_base.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/plots/_model.py` & `ezcharts-0.3.7/ezcharts/plots/_model.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/plots/categorical.py` & `ezcharts-0.3.7/ezcharts/plots/categorical.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,20 @@
             columns=hue, values=y_name, index=x_name).reset_index(drop=False)
         plt.legend = dict(orient='horizontal', top=25)
 
     if order:
         mapper = {x: pos for (pos, x) in enumerate(order)}
         data = data.sort_values(x_name, key=lambda x: x.map(mapper))
 
-    plt.xAxis = dict(name=x_name, type='category')
+    plt.xAxis = dict(
+        name=x_name,
+        type='category',
+        axisLabel=dict(interval=0, rotate=30),
+        axisTick=dict(alignWithLabel=True))
+
     plt.yAxis = dict(name=y_name, type='value')
 
     plt.add_dataset({
         'id': 'raw',
         'dimensions': data.columns,
         'source': data.values})
```

### Comparing `ezcharts-0.3.6/ezcharts/plots/distribution.py` & `ezcharts-0.3.7/ezcharts/plots/distribution.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/plots/ideogram.py` & `ezcharts-0.3.7/ezcharts/plots/ideogram.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/plots/matrix.py` & `ezcharts-0.3.7/ezcharts/plots/matrix.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/plots/relational.py` & `ezcharts-0.3.7/ezcharts/plots/relational.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/plots/util.py` & `ezcharts-0.3.7/ezcharts/plots/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts/util.py` & `ezcharts-0.3.7/ezcharts/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.3.6/ezcharts.egg-info/PKG-INFO` & `ezcharts-0.3.7/ezcharts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcharts
-Version: 0.3.6
+Version: 0.3.7
 Summary: eCharts plotting API.
 Home-page: https://github.com/epi2me-labs/ezcharts
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `ezcharts-0.3.6/ezcharts.egg-info/SOURCES.txt` & `ezcharts-0.3.7/ezcharts.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,32 +19,38 @@
 ezcharts/components/nextclade.py
 ezcharts/components/params.py
 ezcharts/components/theme.py
 ezcharts/components/versions.py
 ezcharts/components/reports/__init__.py
 ezcharts/components/reports/comp.py
 ezcharts/components/reports/labs.py
+ezcharts/components/reports/ond.py
 ezcharts/data/images/LAB_logo.svg
+ezcharts/data/images/OND_logo.svg
 ezcharts/data/images/OND_logo.txt
 ezcharts/data/images/ONT_logo.txt
+ezcharts/data/images/dots.svg
 ezcharts/data/reference/hg19/cytoBand.txt.gz
 ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
 ezcharts/data/reference/hg38/cytoBand.txt.gz
 ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
 ezcharts/data/scripts/epi2melabs.js
 ezcharts/data/scripts/nextclade.html
+ezcharts/data/scripts/ond.js
 ezcharts/data/styles/epi2melabs.scss
+ezcharts/data/styles/ond.scss
 ezcharts/data/test/fastcat.stats.gz
 ezcharts/data/test/hg38_cnv.bed.gz
 ezcharts/data/test/hg38_some_bands.bed.gz
 ezcharts/data/test/nextclade.json
 ezcharts/data/test/params.json
 ezcharts/data/test/plot-spec.json
 ezcharts/data/test/versions.txt
 ezcharts/data/themes/epi2melabs.json
+ezcharts/data/themes/ond.json
 ezcharts/data/themes/walden.json
 ezcharts/data/vendor/echarts.min.js
 ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
 ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
 ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
 ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
 ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
```

### Comparing `ezcharts-0.3.6/setup.py` & `ezcharts-0.3.7/setup.py`

 * *Files identical despite different names*

