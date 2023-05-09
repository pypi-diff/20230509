# Comparing `tmp/livvkit-3.0.1.tar.gz` & `tmp/livvkit-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/livvkit-3.0.1.tar", last modified: Mon Dec  6 15:48:07 2021, max compression
+gzip compressed data, was "livvkit-3.1.0.tar", last modified: Tue May  9 20:34:22 2023, max compression
```

## Comparing `livvkit-3.0.1.tar` & `livvkit-3.1.0.tar`

### file list

```diff
@@ -1,130 +1,139 @@
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/
--rw-rw----   0 mek      (81536) mek      (81536)     1494 2021-11-22 16:46:42.000000 livvkit-3.0.1/LICENSE
--rw-rw----   0 mek      (81536) mek      (81536)      270 2021-11-22 16:46:42.000000 livvkit-3.0.1/LIVVkit.yml
--rw-rw----   0 mek      (81536) mek      (81536)      191 2021-11-22 16:46:42.000000 livvkit-3.0.1/MANIFEST.in
--rw-rw----   0 mek      (81536) mek      (81536)     6811 2021-12-06 15:48:07.000000 livvkit-3.0.1/PKG-INFO
--rw-rw----   0 mek      (81536) mek      (81536)     5995 2021-11-22 16:46:42.000000 livvkit-3.0.1/README.md
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/
--rw-rw----   0 mek      (81536) mek      (81536)     2614 2021-12-06 15:46:35.000000 livvkit-3.0.1/livvkit/__init__.py
--rwxrwx---   0 mek      (81536) mek      (81536)     6123 2021-12-06 15:46:09.000000 livvkit-3.0.1/livvkit/__main__.py
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/bundles/
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/bundles/CISM_glissade/
--rw-rw----   0 mek      (81536) mek      (81536)       15 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/bundles/CISM_glissade/__init__.py
--rw-rw----   0 mek      (81536) mek      (81536)     4112 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/bundles/CISM_glissade/numerics.json
--rw-rw----   0 mek      (81536) mek      (81536)     8980 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/bundles/CISM_glissade/numerics.py
--rw-rw----   0 mek      (81536) mek      (81536)      853 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/bundles/CISM_glissade/performance.json
--rw-rw----   0 mek      (81536) mek      (81536)     5517 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/bundles/CISM_glissade/verification.json
--rw-rw----   0 mek      (81536) mek      (81536)     4463 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/bundles/CISM_glissade/verification.py
--rw-rw----   0 mek      (81536) mek      (81536)       15 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/bundles/__init__.py
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/components/
--rw-rw----   0 mek      (81536) mek      (81536)       15 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/components/__init__.py
--rw-rw----   0 mek      (81536) mek      (81536)     4621 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/components/numerics.py
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/components/numerics_tests/
--rw-rw----   0 mek      (81536) mek      (81536)       15 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/components/numerics_tests/__init__.py
--rw-rw----   0 mek      (81536) mek      (81536)      953 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/components/numerics_tests/ismip.json
--rw-rw----   0 mek      (81536) mek      (81536)     7639 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/components/numerics_tests/ismip.py
--rw-rw----   0 mek      (81536) mek      (81536)    18513 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/components/performance.py
--rw-rw----   0 mek      (81536) mek      (81536)     5844 2021-12-06 15:46:35.000000 livvkit-3.0.1/livvkit/components/validation.py
--rw-rw----   0 mek      (81536) mek      (81536)    12266 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/components/verification.py
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/data/
--rw-rw----   0 mek      (81536) mek      (81536)      500 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/Evans2019.bib
--rw-rw----   0 mek      (81536) mek      (81536)      592 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/Kennedy2017.bib
--rw-rw----   0 mek      (81536) mek      (81536)       15 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/__init__.py
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/data/numerics/
--rw-rw----   0 mek      (81536) mek      (81536)       15 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/__init__.py
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/
--rw-rw----   0 mek      (81536) mek      (81536)    22195 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpA_Fig5_005.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22195 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpA_Fig5_010.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22195 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpA_Fig5_020.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22195 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpA_Fig5_040.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22195 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpA_Fig5_080.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22195 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpA_Fig5_160.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22111 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpC_Fig8_005.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22111 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpC_Fig8_010.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22111 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpC_Fig8_020.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22111 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpC_Fig8_040.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22111 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpC_Fig8_080.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22111 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpC_Fig8_160.txt
--rw-rw----   0 mek      (81536) mek      (81536)    23196 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpF_Fig12_000.txt
--rw-rw----   0 mek      (81536) mek      (81536)    23274 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpF_Fig12_001.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22804 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpF_Fig13_000.txt
--rw-rw----   0 mek      (81536) mek      (81536)    22867 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpF_Fig13_001.txt
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/elements/
--rw-rw----   0 mek      (81536) mek      (81536)     1581 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/__init__.py
--rw-rw----   0 mek      (81536) mek      (81536)    31288 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/elements.py
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/elements/templates/
--rw-rw----   0 mek      (81536) mek      (81536)      659 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/bit4bit.html
--rw-rw----   0 mek      (81536) mek      (81536)      619 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/bit4bit.tex
--rw-rw----   0 mek      (81536) mek      (81536)      322 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/diff.html
--rw-rw----   0 mek      (81536) mek      (81536)       98 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/diff.tex
--rw-rw----   0 mek      (81536) mek      (81536)      198 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/document.tex
--rw-rw----   0 mek      (81536) mek      (81536)       92 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/err.html
--rw-rw----   0 mek      (81536) mek      (81536)       94 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/err.tex
--rw-rw----   0 mek      (81536) mek      (81536)      156 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/gallery.html
--rw-rw----   0 mek      (81536) mek      (81536)       97 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/gallery.tex
--rw-rw----   0 mek      (81536) mek      (81536)      512 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/image.html
--rw-rw----   0 mek      (81536) mek      (81536)      243 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/image.tex
--rw-rw----   0 mek      (81536) mek      (81536)      257 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/page.html
--rw-rw----   0 mek      (81536) mek      (81536)      123 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/page.tex
--rw-rw----   0 mek      (81536) mek      (81536)       35 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/raw.html
--rw-rw----   0 mek      (81536) mek      (81536)       58 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/raw.tex
--rw-rw----   0 mek      (81536) mek      (81536)      126 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/section.html
--rw-rw----   0 mek      (81536) mek      (81536)       97 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/section.tex
--rw-rw----   0 mek      (81536) mek      (81536)      638 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/table.html
--rw-rw----   0 mek      (81536) mek      (81536)      661 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/table.tex
--rw-rw----   0 mek      (81536) mek      (81536)      528 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/table_transposed.html
--rw-rw----   0 mek      (81536) mek      (81536)      535 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/table_transposed.tex
--rw-rw----   0 mek      (81536) mek      (81536)      334 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/tabs.html
--rw-rw----   0 mek      (81536) mek      (81536)      160 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/elements/templates/tabs.tex
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/resources/
--rw-rw----   0 mek      (81536) mek      (81536)       25 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/.gitignore
--rw-rw----   0 mek      (81536) mek      (81536)       15 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/__init__.py
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/resources/css/
--rw-rw----   0 mek      (81536) mek      (81536)      850 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/css/acknowledgments.css
--rw-rw----   0 mek      (81536) mek      (81536)      792 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/css/captionjs.min.css
--rw-rw----   0 mek      (81536) mek      (81536)    29503 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/css/jquery-ui.min.css
--rw-rw----   0 mek      (81536) mek      (81536)     2831 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/css/lightbox.min.css
--rw-rw----   0 mek      (81536) mek      (81536)     3350 2021-12-06 15:46:21.000000 livvkit-3.0.1/livvkit/resources/css/livv.css
--rw-rw----   0 mek      (81536) mek      (81536)     6137 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/css/normalize.css
--rw-rw----   0 mek      (81536) mek      (81536)   337355 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/favicon.ico
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/resources/imgs/
--rw-rw----   0 mek      (81536) mek      (81536)  5268054 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/imgs/DOE-logo.png
--rw-rw----   0 mek      (81536) mek      (81536)    12540 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/imgs/LANL-logo.png
--rw-rw----   0 mek      (81536) mek      (81536)    73756 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/imgs/ORNL-logo.png
--rw-rw----   0 mek      (81536) mek      (81536)     2663 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/imgs/b4b.png
--rw-rw----   0 mek      (81536) mek      (81536)  1531845 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/imgs/background.jpg
--rw-rw----   0 mek      (81536) mek      (81536)      280 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/imgs/close.png
--rw-rw----   0 mek      (81536) mek      (81536)    21895 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/imgs/icon.svg
--rw-rw----   0 mek      (81536) mek      (81536)     8476 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/imgs/loading.gif
--rw-rw----   0 mek      (81536) mek      (81536)     1855 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/imgs/na.png
--rw-rw----   0 mek      (81536) mek      (81536)     1350 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/imgs/next.png
--rw-rw----   0 mek      (81536) mek      (81536)     1360 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/imgs/prev.png
--rw-rw----   0 mek      (81536) mek      (81536)     2784 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/index.html
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/resources/js/
--rw-rw----   0 mek      (81536) mek      (81536)     3788 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/js/common.js
--rw-rw----   0 mek      (81536) mek      (81536)   240427 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/js/jquery-ui.min.js
--rw-rw----   0 mek      (81536) mek      (81536)     2308 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/js/jquery.caption.min.js
--rw-rw----   0 mek      (81536) mek      (81536)    85589 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/js/jquery.min.js
--rw-rw----   0 mek      (81536) mek      (81536)     9372 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/js/lightbox.min.js
--rw-rw----   0 mek      (81536) mek      (81536)     9771 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/js/lightbox.min.map
--rw-rw----   0 mek      (81536) mek      (81536)     2835 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/numerics.html
--rw-rw----   0 mek      (81536) mek      (81536)     2883 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/performance.html
--rw-rw----   0 mek      (81536) mek      (81536)     2833 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/validation.html
--rw-rw----   0 mek      (81536) mek      (81536)     2845 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/resources/verification.html
--rw-rw----   0 mek      (81536) mek      (81536)     4827 2021-12-06 15:46:35.000000 livvkit-3.0.1/livvkit/scheduler.py
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit/util/
--rw-rw----   0 mek      (81536) mek      (81536)     2728 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/util/LIVVDict.py
--rw-rw----   0 mek      (81536) mek      (81536)       15 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/util/__init__.py
--rw-rw----   0 mek      (81536) mek      (81536)     5971 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/util/bib.py
--rw-rw----   0 mek      (81536) mek      (81536)    50608 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/util/colormaps.py
--rw-rw----   0 mek      (81536) mek      (81536)     8508 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/util/functions.py
--rw-rw----   0 mek      (81536) mek      (81536)     8677 2021-11-22 16:46:42.000000 livvkit-3.0.1/livvkit/util/options.py
-drwxrwx---   0 mek      (81536) mek      (81536)        0 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit.egg-info/
--rw-rw----   0 mek      (81536) mek      (81536)     6811 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit.egg-info/PKG-INFO
--rw-rw----   0 mek      (81536) mek      (81536)     3980 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit.egg-info/SOURCES.txt
--rw-rw----   0 mek      (81536) mek      (81536)        1 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit.egg-info/dependency_links.txt
--rw-rw----   0 mek      (81536) mek      (81536)       48 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit.egg-info/entry_points.txt
--rw-rw----   0 mek      (81536) mek      (81536)      160 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit.egg-info/requires.txt
--rw-rw----   0 mek      (81536) mek      (81536)        8 2021-12-06 15:48:07.000000 livvkit-3.0.1/livvkit.egg-info/top_level.txt
--rw-rw----   0 mek      (81536) mek      (81536)       38 2021-12-06 15:48:07.000000 livvkit-3.0.1/setup.cfg
--rw-rw----   0 mek      (81536) mek      (81536)     4103 2021-11-22 16:46:42.000000 livvkit-3.0.1/setup.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.084772 livvkit-3.1.0/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     1494 2022-12-09 19:32:32.000000 livvkit-3.1.0/LICENSE
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      375 2023-05-09 20:25:03.000000 livvkit-3.1.0/LIVVkit.yml
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      191 2022-12-09 19:32:32.000000 livvkit-3.1.0/MANIFEST.in
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     6791 2023-05-09 20:34:22.084256 livvkit-3.1.0/PKG-INFO
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     5995 2022-12-09 19:32:32.000000 livvkit-3.1.0/README.md
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:21.999475 livvkit-3.1.0/livvkit/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     2614 2023-05-09 20:25:03.000000 livvkit-3.1.0/livvkit/__init__.py
+-rwxr-xr-x   0 mkelleher (40354) ncar      (1000)     6123 2023-01-06 22:20:52.000000 livvkit-3.1.0/livvkit/__main__.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.001862 livvkit-3.1.0/livvkit/bundles/
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.003975 livvkit-3.1.0/livvkit/bundles/CISM_glissade/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       15 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/bundles/CISM_glissade/__init__.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     4112 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/bundles/CISM_glissade/numerics.json
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     8980 2022-12-16 14:29:52.000000 livvkit-3.1.0/livvkit/bundles/CISM_glissade/numerics.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      853 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/bundles/CISM_glissade/performance.json
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     5517 2022-12-15 20:43:54.000000 livvkit-3.1.0/livvkit/bundles/CISM_glissade/verification.json
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     4519 2023-05-09 20:25:03.000000 livvkit-3.1.0/livvkit/bundles/CISM_glissade/verification.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.005018 livvkit-3.1.0/livvkit/bundles/CISM_new/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     4112 2022-12-14 17:00:22.000000 livvkit-3.1.0/livvkit/bundles/CISM_new/numerics.json
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      853 2022-12-14 17:00:22.000000 livvkit-3.1.0/livvkit/bundles/CISM_new/performance.json
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     5517 2022-12-14 17:00:22.000000 livvkit-3.1.0/livvkit/bundles/CISM_new/verification.json
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       15 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/bundles/__init__.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.006810 livvkit-3.1.0/livvkit/components/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       15 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/components/__init__.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     4621 2023-01-04 16:02:05.000000 livvkit-3.1.0/livvkit/components/numerics.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.007834 livvkit-3.1.0/livvkit/components/numerics_tests/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       15 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/components/numerics_tests/__init__.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      953 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/components/numerics_tests/ismip.json
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     7639 2023-05-09 20:13:32.000000 livvkit-3.1.0/livvkit/components/numerics_tests/ismip.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    18512 2023-05-09 20:25:03.000000 livvkit-3.1.0/livvkit/components/performance.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     5844 2022-12-14 16:58:57.000000 livvkit-3.1.0/livvkit/components/validation.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    13400 2023-05-09 20:25:03.000000 livvkit-3.1.0/livvkit/components/verification.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.008833 livvkit-3.1.0/livvkit/data/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      500 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/Evans2019.bib
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      592 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/Kennedy2017.bib
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       15 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/__init__.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.009160 livvkit-3.1.0/livvkit/data/numerics/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       15 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/__init__.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.016636 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22195 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpA_Fig5_005.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22195 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpA_Fig5_010.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22195 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpA_Fig5_020.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22195 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpA_Fig5_040.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22195 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpA_Fig5_080.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22195 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpA_Fig5_160.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22111 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpC_Fig8_005.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22111 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpC_Fig8_010.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22111 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpC_Fig8_020.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22111 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpC_Fig8_040.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22111 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpC_Fig8_080.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22111 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpC_Fig8_160.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    23196 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpF_Fig12_000.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    23274 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpF_Fig12_001.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22804 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpF_Fig13_000.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    22867 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpF_Fig13_001.txt
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.017438 livvkit-3.1.0/livvkit/elements/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     1581 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/__init__.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    31288 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/elements.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.026114 livvkit-3.1.0/livvkit/elements/templates/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      659 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/bit4bit.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      619 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/bit4bit.tex
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      322 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/diff.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       98 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/diff.tex
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      198 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/document.tex
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       92 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/err.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       94 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/err.tex
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      156 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/gallery.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       97 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/gallery.tex
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      512 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/image.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      243 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/image.tex
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      257 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/page.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      123 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/page.tex
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       35 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/raw.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       58 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/raw.tex
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      126 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/section.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       97 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/section.tex
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      638 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/table.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      661 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/table.tex
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      528 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/table_transposed.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      535 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/table_transposed.tex
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      334 2022-12-09 19:32:32.000000 livvkit-3.1.0/livvkit/elements/templates/tabs.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      160 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/elements/templates/tabs.tex
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.030585 livvkit-3.1.0/livvkit/resources/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       25 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/.gitignore
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       15 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/__init__.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.032826 livvkit-3.1.0/livvkit/resources/css/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      850 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/css/acknowledgments.css
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      792 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/css/captionjs.min.css
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    29503 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/css/jquery-ui.min.css
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     2831 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/css/lightbox.min.css
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     3606 2023-05-09 20:25:03.000000 livvkit-3.1.0/livvkit/resources/css/livv.css
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     6137 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/css/normalize.css
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)   337355 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/favicon.ico
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.069643 livvkit-3.1.0/livvkit/resources/imgs/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)  5268054 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/imgs/DOE-logo.png
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    12540 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/imgs/LANL-logo.png
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    73756 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/imgs/ORNL-logo.png
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     2663 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/imgs/b4b.png
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)  1531845 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/imgs/background.jpg
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      280 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/imgs/close.png
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    21895 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/imgs/icon.svg
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     8476 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/imgs/loading.gif
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     1855 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/imgs/na.png
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     1350 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/imgs/next.png
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     1360 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/imgs/prev.png
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     2784 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/index.html
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.077703 livvkit-3.1.0/livvkit/resources/js/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     3788 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/js/common.js
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)   240427 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/js/jquery-ui.min.js
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     2308 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/js/jquery.caption.min.js
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    85589 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/js/jquery.min.js
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     9372 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/js/lightbox.min.js
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     9771 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/js/lightbox.min.map
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     2835 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/numerics.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     2883 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/performance.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     2833 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/validation.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     2845 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/resources/verification.html
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     4827 2022-12-14 16:58:57.000000 livvkit-3.1.0/livvkit/scheduler.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.081823 livvkit-3.1.0/livvkit/util/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     2728 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/util/LIVVDict.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       15 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/util/__init__.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     5971 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/util/bib.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    50608 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/util/colormaps.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     8508 2022-12-09 19:32:33.000000 livvkit-3.1.0/livvkit/util/functions.py
+-rwxr-xr-x   0 mkelleher (40354) ncar      (1000)     5843 2022-12-15 19:55:23.000000 livvkit-3.1.0/livvkit/util/move_tests.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     9414 2023-05-09 20:25:03.000000 livvkit-3.1.0/livvkit/util/options.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.001516 livvkit-3.1.0/livvkit.egg-info/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     6791 2023-05-09 20:34:21.999944 livvkit-3.1.0/livvkit.egg-info/PKG-INFO
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     4206 2023-05-09 20:34:21.000000 livvkit-3.1.0/livvkit.egg-info/SOURCES.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)        1 2023-05-09 20:34:21.000000 livvkit-3.1.0/livvkit.egg-info/dependency_links.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       47 2023-05-09 20:34:21.000000 livvkit-3.1.0/livvkit.egg-info/entry_points.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)      160 2023-05-09 20:34:21.000000 livvkit-3.1.0/livvkit.egg-info/requires.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)        8 2023-05-09 20:34:21.000000 livvkit-3.1.0/livvkit.egg-info/top_level.txt
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)       38 2023-05-09 20:34:22.084896 livvkit-3.1.0/setup.cfg
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     4103 2022-12-09 19:32:33.000000 livvkit-3.1.0/setup.py
+drwxr-xr-x   0 mkelleher (40354) ncar      (1000)        0 2023-05-09 20:34:22.083460 livvkit-3.1.0/tests/
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)    42083 2023-05-08 19:09:27.000000 livvkit-3.1.0/tests/test_elements.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     4463 2022-12-09 19:32:33.000000 livvkit-3.1.0/tests/test_util_bib.py
+-rw-r--r--   0 mkelleher (40354) ncar      (1000)     5079 2022-12-09 19:32:33.000000 livvkit-3.1.0/tests/test_util_functions.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `livvkit-3.0.1/LICENSE` & `livvkit-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/PKG-INFO` & `livvkit-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: livvkit
-Version: 3.0.1
+Version: 3.1.0
 Summary: The land ice verification and validation toolkit
 Home-page: https://github.com/LIVVkit/LIVVkit
 Author: Joseph H. Kennedy et al.
 Author-email: kennedyjh@ornl.gov
 License: BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -200,9 +199,7 @@
 
 **Katherine J. Evans** 
 * github: @kevans32
 * email: <a href="mailto:evanskj@ornl.gov">evanskj [at] ornl.gov</a>
 
 If you're emailing us, we recommend CC-ing all of us. 
 
-
-
```

### Comparing `livvkit-3.0.1/README.md` & `livvkit-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/__init__.py` & `livvkit-3.1.0/livvkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 import getpass
 import platform
 import socket
 
 from livvkit import bundles
 from livvkit import resources
 
-__version_info__ = (3, 0, 1)
+__version_info__ = (3, 1, 0)
 __version__ = '.'.join(str(vi) for vi in __version_info__)
 
 cwd = os.getcwd()
 timestamp = time.strftime("%Y-%m-%d %H:%M:%S")
 user = getpass.getuser()
 machine = socket.gethostname()
 os_type = platform.system() + " " + platform.release()
```

### Comparing `livvkit-3.0.1/livvkit/__main__.py` & `livvkit-3.1.0/livvkit/__main__.py`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/bundles/CISM_glissade/numerics.json` & `livvkit-3.1.0/livvkit/bundles/CISM_glissade/numerics.json`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/bundles/CISM_glissade/numerics.py` & `livvkit-3.1.0/livvkit/bundles/CISM_glissade/numerics.py`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/bundles/CISM_glissade/performance.json` & `livvkit-3.1.0/livvkit/bundles/CISM_glissade/performance.json`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/bundles/CISM_glissade/verification.json` & `livvkit-3.1.0/livvkit/bundles/CISM_glissade/verification.json`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/bundles/CISM_glissade/verification.py` & `livvkit-3.1.0/livvkit/bundles/CISM_glissade/verification.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import numpy as np
 
 from configparser import ConfigParser
 
 from livvkit import elements
 
 
-def parse_log(file_path):
+def parse_log(file_path, title=None):
     """
     Parse a CISM output log and extract some information.
 
     Args:
         file_path: absolute path to the log file
 
     Return:
@@ -88,15 +88,17 @@
             iters_to_converge.append(int(iter_number))
     data = {
         "Dycore Type": [dycore_type],
         "Processor Count": [proc_count],
         "Converged Iterations": [len(converged_iters)],
         "Avg. Iterations to Converge": [np.mean(iters_to_converge)]
     }
-    return elements.Table("Output Log", data)
+    if title is None:
+        title = "Output Log"
+    return elements.Table(title, data)
 
 
 def parse_config(file_path):
     """
     Convert the CISM configuration file to a python dictionary
 
     Args:
```

### Comparing `livvkit-3.0.1/livvkit/components/numerics.py` & `livvkit-3.1.0/livvkit/components/numerics.py`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/components/numerics_tests/ismip.json` & `livvkit-3.1.0/livvkit/components/numerics_tests/ismip.json`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/components/numerics_tests/ismip.py` & `livvkit-3.1.0/livvkit/components/numerics_tests/ismip.py`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/components/performance.py` & `livvkit-3.1.0/livvkit/components/performance.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
         timing_data[subcase] = dict()
         for mcase in model_cases[subcase]:
             config["case"] = "-".join([subcase, mcase])
             bpath = (os.path.join(bench_dir, subcase, mcase.replace("-", os.path.sep))
                      if mcase in bench_subcases else None)
             mpath = os.path.join(model_dir, subcase, mcase.replace("-", os.path.sep))
             timing_data[subcase][mcase] = _analyze_case(mpath, bpath, config)
-
     # Create scaling and timing breakdown plots
     weak_data = weak_scaling(timing_data, config['scaling_var'],
                              config['weak_scaling_points'])
     strong_data = strong_scaling(timing_data, config['scaling_var'],
                                  config['strong_scaling_points'])
 
     timing_plots = [
```

### Comparing `livvkit-3.0.1/livvkit/components/validation.py` & `livvkit-3.1.0/livvkit/components/validation.py`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/components/verification.py` & `livvkit-3.1.0/livvkit/components/verification.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,15 +53,22 @@
     summary = LIVVDict()
     model_cases = functions.collect_cases(model_dir)
     bench_cases = functions.collect_cases(bench_dir)
 
     for subcase in sorted(model_cases):
         bench_subcases = bench_cases[subcase] if subcase in bench_cases else []
         case_sections = []
-        for mcase in sorted(model_cases[subcase], key=functions.sort_processor_counts):
+        try:
+            _mcases = sorted(model_cases[subcase], key=functions.sort_processor_counts)
+        except ValueError:
+            _mcases = sorted(model_cases[subcase])
+
+        for mcase in _mcases:
+            if "setup_mesh" in mcase:
+                continue
             bpath = (os.path.join(bench_dir, subcase, mcase.replace("-", os.path.sep))
                      if mcase in bench_subcases else "")
             mpath = os.path.join(model_dir, subcase, mcase.replace("-", os.path.sep))
             case_result = _analyze_case(mpath, bpath, config)
             case_sections.append(elements.Section(mcase, case_result))
             summary[subcase] = _summarize_result(case_result, summary[subcase])
         tabs[subcase] = case_sections
@@ -83,20 +90,25 @@
     """ Runs all of the verification checks on a particular case """
     bundle = livvkit.verification_model_module
     test_out = functions.find_file(test_dir, "*"+config["output_ext"])
     ref_out = functions.find_file(ref_dir, "*"+config["output_ext"])
     test_config = functions.find_file(test_dir, "*"+config["config_ext"])
     ref_config = functions.find_file(ref_dir, "*"+config["config_ext"])
     model_log = functions.find_file(test_dir, "*"+config["logfile_ext"])
-    el = [
-            bit_for_bit(test_out, ref_out, config),
-            elements.FileDiff("Configuration Comparison",
-                              ref_config, test_config),
-            bundle.parse_log(model_log)
-         ]
+    ref_log = functions.find_file(ref_dir, "*"+config["logfile_ext"])
+    try:
+        el = [
+                bit_for_bit(test_out, ref_out, config, bundle),
+                elements.FileDiff("Configuration Comparison",
+                                ref_config, test_config),
+            bundle.parse_log(ref_log, title="Benchmark Output Log"),
+            bundle.parse_log(model_log, title="Model Output Log"),
+        ]
+    except (FileNotFoundError, IndexError):
+        el = []
     return el
 
 
 def _print_summary(case, summary):
     """ Show some statistics from the run """
     for dof, data in summary.items():
         b4b = data["Bit for Bit"]
@@ -165,40 +177,42 @@
 def populate_metadata(case, config):
     """ Provide some top level information for the summary """
     return {"Type": "Summary",
             "Title": "Verification",
             "Headers": ["Bit for Bit", "Configurations", "Std. Out Files"]}
 
 
-def bit_for_bit(model_path, bench_path, config):
+def bit_for_bit(model_path, bench_path, config, bundle=None):
     """
     Checks whether the given files have bit for bit solution matches
     on the given variable list.
 
     Args:
         model_path: absolute path to the model dataset
         bench_path: absolute path to the benchmark dataset
         config: the configuration of the set of analyses
 
     Returns:
         A dictionary created by the elements object corresponding to
         the results of the bit for bit testing
     """
     fname = model_path.split(os.path.sep)[-1]
+    title = "_".join(model_path.split(os.path.sep)[-5:])[:-3]
     # Error handling
     if not (os.path.isfile(bench_path) and os.path.isfile(model_path)):
         return elements.Error("Bit for Bit",
                               "File named " + fname + " has no suitable match!")
     try:
         model_data = Dataset(model_path)
         bench_data = Dataset(bench_path)
     except (FileNotFoundError, PermissionError):
         return elements.Error("Bit for Bit",
                               "File named " + fname + " could not be read!")
-    if not (len(model_data.dimensions['time']) > 0 and len(bench_data.dimensions['time']) > 0):
+    _timevar = config.get("time_var", "time")
+    if not (len(model_data.dimensions[_timevar]) > 0 and len(bench_data.dimensions[_timevar]) > 0):
         return elements.Error("Bit for Bit",
                               "File named " + fname + " could not be read!")
 
     # Begin bit for bit analysis
     plot_elements = []
     table_data = {'Variable': [], 'Max Error': [], 'Index of Max Error': [], 'RMS Error': []}
     for var in config["bit_for_bit_vars"]:
@@ -206,20 +220,27 @@
             table_data['Variable'].append(var)
 
             m_vardata = model_data.variables[var][:]
             b_vardata = bench_data.variables[var][:]
             diff_data = m_vardata - b_vardata
 
             if diff_data.any():
+                if hasattr(bundle, "plot_bit_for_bit"):
+                    # Try to use the bundle's plotting routine first, mainly for MALI
+                    _plot = bundle.plot_bit_for_bit
+                else:
+                    # Default back to the local plotting routine
+                    _plot = plot_bit_for_bit
+
                 table_data["Max Error"].append(np.amax(np.absolute(diff_data)))
                 table_data["Index of Max Error"].append(str(
                         np.unravel_index(np.absolute(diff_data).argmax(), diff_data.shape)))
                 table_data["RMS Error"].append(np.sqrt(np.sum(np.square(diff_data).flatten()) /
                                                diff_data.size))
-                plot_elements.append(plot_bit_for_bit(fname, var, m_vardata, b_vardata, diff_data))
+                plot_elements.append(_plot(title, var, model_data, bench_data, diff_data))
             else:
                 table_data["Max Error"].append(0)
                 table_data["Index of Max Error"].append("N/A")
                 table_data["RMS Error"].append(0)
                 plot_elements.append(elements.B4BImage('', '{} is bit-for-bit'.format(var),
                                                        page_path=os.path.join(livvkit.output_dir, "verification")))
         else:
@@ -235,14 +256,20 @@
 
 def plot_bit_for_bit(case, var_name, model_data, bench_data, diff_data):
     """ Create a bit for bit plot """
     plot_title = ""
     plot_name = case + "_" + var_name + ".png"
     plot_path = os.path.join(os.path.join(livvkit.output_dir, "verification", "imgs"))
     functions.mkdir_p(plot_path)
+
+    # The new MALI bundle needs the full dataset to plot, so that gets passed now
+    # here we only need the variable data since no coords are plotted
+    model_data = model_data.variables[var_name]
+    bench_data = bench_data.variables[var_name]
+
     m_ndim = np.ndim(model_data)
     b_ndim = np.ndim(bench_data)
     if m_ndim != b_ndim:
         return "Dataset dimensions didn't match!"
     if m_ndim == 3:
         model_data = model_data[-1]
         bench_data = bench_data[-1]
```

### Comparing `livvkit-3.0.1/livvkit/data/Kennedy2017.bib` & `livvkit-3.1.0/livvkit/data/Kennedy2017.bib`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpA_Fig5_005.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpA_Fig5_005.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpA_Fig5_010.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpA_Fig5_010.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpA_Fig5_020.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpA_Fig5_020.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpA_Fig5_040.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpA_Fig5_040.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpA_Fig5_080.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpA_Fig5_080.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpA_Fig5_160.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpA_Fig5_160.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpC_Fig8_005.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpC_Fig8_005.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpC_Fig8_010.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpC_Fig8_010.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpC_Fig8_020.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpC_Fig8_020.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpC_Fig8_040.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpC_Fig8_040.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpC_Fig8_080.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpC_Fig8_080.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpC_Fig8_160.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpC_Fig8_160.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpF_Fig12_000.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpF_Fig12_000.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpF_Fig12_001.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpF_Fig12_001.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpF_Fig13_000.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpF_Fig13_000.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/data/numerics/ismip-hom/ExpF_Fig13_001.txt` & `livvkit-3.1.0/livvkit/data/numerics/ismip-hom/ExpF_Fig13_001.txt`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/elements/__init__.py` & `livvkit-3.1.0/livvkit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/elements/elements.py` & `livvkit-3.1.0/livvkit/elements/elements.py`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/elements/templates/bit4bit.html` & `livvkit-3.1.0/livvkit/elements/templates/bit4bit.html`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/elements/templates/bit4bit.tex` & `livvkit-3.1.0/livvkit/elements/templates/bit4bit.tex`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/elements/templates/image.html` & `livvkit-3.1.0/livvkit/elements/templates/image.html`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/elements/templates/table.html` & `livvkit-3.1.0/livvkit/elements/templates/table.html`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/elements/templates/table.tex` & `livvkit-3.1.0/livvkit/elements/templates/table.tex`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/elements/templates/table_transposed.html` & `livvkit-3.1.0/livvkit/elements/templates/table_transposed.html`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/elements/templates/table_transposed.tex` & `livvkit-3.1.0/livvkit/elements/templates/table_transposed.tex`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/css/acknowledgments.css` & `livvkit-3.1.0/livvkit/resources/css/acknowledgments.css`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/css/captionjs.min.css` & `livvkit-3.1.0/livvkit/resources/css/captionjs.min.css`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/css/jquery-ui.min.css` & `livvkit-3.1.0/livvkit/resources/css/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/css/lightbox.min.css` & `livvkit-3.1.0/livvkit/resources/css/lightbox.min.css`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/css/livv.css` & `livvkit-3.1.0/livvkit/resources/css/livv.css`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,28 @@
 }
 
 a {
     text-decoration: none;
     color: #007acc;
 }
 
+.section h2{
+    background-color: #66c2ff;
+    color: white;
+    margin-top: 0;
+    padding: 0.5em;
+    text-align: center;
+}
+.section {
+    padding-top: 0;
+    border-left: 2px solid #66c2ff;
+    border-right: 2px solid #66c2ff;
+    margin-top: .5em;
+}
+
 /******************************************************************************
   Header/Footer Styling
 ******************************************************************************/
 #header {
     min-width: 800px;
 	background-color: #222222;
     border-bottom: 1px solid #222222;
```

### Comparing `livvkit-3.0.1/livvkit/resources/css/normalize.css` & `livvkit-3.1.0/livvkit/resources/css/normalize.css`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/favicon.ico` & `livvkit-3.1.0/livvkit/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/imgs/DOE-logo.png` & `livvkit-3.1.0/livvkit/resources/imgs/DOE-logo.png`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/imgs/LANL-logo.png` & `livvkit-3.1.0/livvkit/resources/imgs/LANL-logo.png`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/imgs/ORNL-logo.png` & `livvkit-3.1.0/livvkit/resources/imgs/ORNL-logo.png`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/imgs/b4b.png` & `livvkit-3.1.0/livvkit/resources/imgs/b4b.png`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/imgs/background.jpg` & `livvkit-3.1.0/livvkit/resources/imgs/background.jpg`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/imgs/icon.svg` & `livvkit-3.1.0/livvkit/resources/imgs/icon.svg`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/imgs/loading.gif` & `livvkit-3.1.0/livvkit/resources/imgs/loading.gif`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/imgs/na.png` & `livvkit-3.1.0/livvkit/resources/imgs/na.png`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/imgs/next.png` & `livvkit-3.1.0/livvkit/resources/imgs/next.png`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/imgs/prev.png` & `livvkit-3.1.0/livvkit/resources/imgs/prev.png`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/index.html` & `livvkit-3.1.0/livvkit/resources/index.html`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/js/common.js` & `livvkit-3.1.0/livvkit/resources/js/common.js`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/js/jquery-ui.min.js` & `livvkit-3.1.0/livvkit/resources/js/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/js/jquery.caption.min.js` & `livvkit-3.1.0/livvkit/resources/js/jquery.caption.min.js`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/js/jquery.min.js` & `livvkit-3.1.0/livvkit/resources/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/js/lightbox.min.js` & `livvkit-3.1.0/livvkit/resources/js/lightbox.min.js`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/js/lightbox.min.map` & `livvkit-3.1.0/livvkit/resources/js/lightbox.min.map`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/numerics.html` & `livvkit-3.1.0/livvkit/resources/numerics.html`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/performance.html` & `livvkit-3.1.0/livvkit/resources/performance.html`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/validation.html` & `livvkit-3.1.0/livvkit/resources/validation.html`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/resources/verification.html` & `livvkit-3.1.0/livvkit/resources/verification.html`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/scheduler.py` & `livvkit-3.1.0/livvkit/scheduler.py`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/util/LIVVDict.py` & `livvkit-3.1.0/livvkit/util/LIVVDict.py`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/util/bib.py` & `livvkit-3.1.0/livvkit/util/bib.py`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/util/colormaps.py` & `livvkit-3.1.0/livvkit/util/colormaps.py`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/util/functions.py` & `livvkit-3.1.0/livvkit/util/functions.py`

 * *Files identical despite different names*

### Comparing `livvkit-3.0.1/livvkit/util/options.py` & `livvkit-3.1.0/livvkit/util/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,14 +157,25 @@
             print("    the path:")
             print("\n"+livvkit.bench_dir+"\n\n")
             sys.exit(1)
 
         livvkit.model_bundle = os.path.basename(livvkit.model_dir)
         livvkit.bench_bundle = os.path.basename(livvkit.bench_dir)
 
+        # For MPAS/COMPASS/MALI, the basename isn't MALI it's the generic "landice"
+        # check if the bundle is in the available bundles, then see if an available bundle
+        # is somewhere in the path, and use that bundle
+        if livvkit.model_bundle not in available_bundles:
+            bundle_in_path = [_bundle in livvkit.model_dir for _bundle in available_bundles]
+            if any(bundle_in_path):
+                # This uses the first found bundle in the path (Left-to-right) in the unlikely
+                # but possible instance that multiple bundles are in the path
+                livvkit.model_bundle = available_bundles[bundle_in_path.index(True)]
+                livvkit.bench_bundle = livvkit.model_bundle
+
         if livvkit.model_bundle in available_bundles:
             livvkit.numerics_model_config = os.path.join(
                 livvkit.bundle_dir, livvkit.model_bundle, "numerics.json")
             livvkit.numerics_model_module = importlib.import_module(
                 ".".join(["livvkit.bundles", livvkit.model_bundle, "numerics"]))
 
             livvkit.verification_model_config = os.path.join(
```

### Comparing `livvkit-3.0.1/livvkit.egg-info/PKG-INFO` & `livvkit-3.1.0/livvkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: livvkit
-Version: 3.0.1
+Version: 3.1.0
 Summary: The land ice verification and validation toolkit
 Home-page: https://github.com/LIVVkit/LIVVkit
 Author: Joseph H. Kennedy et al.
 Author-email: kennedyjh@ornl.gov
 License: BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -200,9 +199,7 @@
 
 **Katherine J. Evans** 
 * github: @kevans32
 * email: <a href="mailto:evanskj@ornl.gov">evanskj [at] ornl.gov</a>
 
 If you're emailing us, we recommend CC-ing all of us. 
 
-
-
```

### Comparing `livvkit-3.0.1/livvkit.egg-info/SOURCES.txt` & `livvkit-3.1.0/livvkit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 livvkit/bundles/__init__.py
 livvkit/bundles/CISM_glissade/__init__.py
 livvkit/bundles/CISM_glissade/numerics.json
 livvkit/bundles/CISM_glissade/numerics.py
 livvkit/bundles/CISM_glissade/performance.json
 livvkit/bundles/CISM_glissade/verification.json
 livvkit/bundles/CISM_glissade/verification.py
+livvkit/bundles/CISM_new/numerics.json
+livvkit/bundles/CISM_new/performance.json
+livvkit/bundles/CISM_new/verification.json
 livvkit/components/__init__.py
 livvkit/components/numerics.py
 livvkit/components/performance.py
 livvkit/components/validation.py
 livvkit/components/verification.py
 livvkit/components/numerics_tests/__init__.py
 livvkit/components/numerics_tests/ismip.json
@@ -104,8 +107,12 @@
 livvkit/resources/js/lightbox.min.js
 livvkit/resources/js/lightbox.min.map
 livvkit/util/LIVVDict.py
 livvkit/util/__init__.py
 livvkit/util/bib.py
 livvkit/util/colormaps.py
 livvkit/util/functions.py
-livvkit/util/options.py
+livvkit/util/move_tests.py
+livvkit/util/options.py
+tests/test_elements.py
+tests/test_util_bib.py
+tests/test_util_functions.py
```

### Comparing `livvkit-3.0.1/setup.py` & `livvkit-3.1.0/setup.py`

 * *Files identical despite different names*

