# Comparing `tmp/junifer-0.0.3.dev48.tar.gz` & `tmp/junifer-0.0.3.dev53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junifer-0.0.3.dev48.tar", last modified: Fri May  5 10:47:36 2023, max compression
+gzip compressed data, was "junifer-0.0.3.dev53.tar", last modified: Tue May  9 10:34:32 2023, max compression
```

## Comparing `junifer-0.0.3.dev48.tar` & `junifer-0.0.3.dev53.tar`

### file list

```diff
@@ -1,367 +1,367 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.117498 junifer-0.0.3.dev48/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.081499 junifer-0.0.3.dev48/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.081499 junifer-0.0.3.dev48/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/ISSUE_TEMPLATE/dataset-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/ISSUE_TEMPLATE/documention-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/ISSUE_TEMPLATE/marker-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.081499 junifer-0.0.3.dev48/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34353 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-05-05 10:47:36.117498 junifer-0.0.3.dev48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/conda-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.081499 junifer-0.0.3.dev48/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.073499 junifer-0.0.3.dev48/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.081499 junifer-0.0.3.dev48/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.081499 junifer-0.0.3.dev48/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.081499 junifer-0.0.3.dev48/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.085499 junifer-0.0.3.dev48/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/configs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/datagrabbers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/datareaders.rst
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/markers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/nilearn.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/builtin.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.085499 junifer-0.0.3.dev48/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.085499 junifer-0.0.3.dev48/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/changes/newsfragments/220.doc
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/changes/newsfragments/222.change
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/changes/newsfragments/222.enh
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.085499 junifer-0.0.3.dev48/docs/extending/
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/extending/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16558 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/extending/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/extending/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/extending/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/extending/marker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/extending/masks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/extending/parcellations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/help.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.085499 junifer-0.0.3.dev48/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    62148 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/images/junifer_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.085499 junifer-0.0.3.dev48/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/sphinxext/gh_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/starting.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.085499 junifer-0.0.3.dev48/docs/understanding/
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/understanding/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/understanding/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/understanding/datareader.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/understanding/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/understanding/marker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/understanding/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/understanding/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/understanding/storage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.085499 junifer-0.0.3.dev48/docs/using/
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/using/codeless.rst
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/using/masks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/using/queueing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/using/running.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.089499 junifer-0.0.3.dev48/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/examples/norun_hcpfc_pearson.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/examples/norun_ukbvm_gmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/examples/run_compute_parcel_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/examples/run_datagrabber_bids_datalad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/examples/run_ets_rss_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/examples/run_junifer_julearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/examples/run_run_gmd_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.089499 junifer-0.0.3.dev48/examples/yamls/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/examples/yamls/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/examples/yamls/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/examples/yamls/ukb_gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.089499 junifer-0.0.3.dev48/junifer/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-05 10:47:35.000000 junifer-0.0.3.dev48/junifer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.089499 junifer-0.0.3.dev48/junifer/api/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    22536 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.089499 junifer-0.0.3.dev48/junifer/api/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.089499 junifer-0.0.3.dev48/junifer/api/res/afni/
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/res/afni/3dAFNItoNIFTI
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/res/afni/3dRSFC
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/res/afni/3dReHo
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/res/afni/afni
--rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/res/afni/run_afni_docker.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/res/run_conda.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.089499 junifer-0.0.3.dev48/junifer/api/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.089499 junifer-0.0.3.dev48/junifer/api/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/tests/data/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/tests/data/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/tests/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23970 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.089499 junifer-0.0.3.dev48/junifer/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.089499 junifer-0.0.3.dev48/junifer/configs/juseless/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/juseless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.093499 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/ixi_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.093499 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/ucla.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/ukb_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.093499 junifer-0.0.3.dev48/junifer/configs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/configs/tests/test_juseless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.093499 junifer-0.0.3.dev48/junifer/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.073499 junifer-0.0.3.dev48/junifer/data/VOIs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.097499 junifer-0.0.3.dev48/junifer/data/VOIs/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/CogAC_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/CogAR_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/Empathy_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/Motor_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/MultiTask_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/Rew_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/ToM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/VigAtt_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/WM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/eMDN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/eSAD_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/VOIs/meta/extDMN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.073499 junifer-0.0.3.dev48/junifer/data/masks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.097499 junifer-0.0.3.dev48/junifer/data/masks/vickery-patil/
--rw-r--r--   0 runner    (1001) docker     (123)    88270 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    27401 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/parcellations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.101499 junifer-0.0.3.dev48/junifer/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/tests/test_parcellations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.101499 junifer-0.0.3.dev48/junifer/datagrabber/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.101499 junifer-0.0.3.dev48/junifer/datagrabber/aomic/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/aomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/aomic/id1000.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/aomic/piop1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/aomic/piop2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.105499 junifer-0.0.3.dev48/junifer/datagrabber/aomic/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/aomic/tests/test_id1000.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/aomic/tests/test_piop1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/aomic/tests/test_piop2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/hcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/pattern_datalad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.105499 junifer-0.0.3.dev48/junifer/datagrabber/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/tests/test_datagrabber_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/tests/test_datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/tests/test_hcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/tests/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/tests/test_pattern_datalad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datagrabber/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.105499 junifer-0.0.3.dev48/junifer/datareader/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datareader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datareader/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.105499 junifer-0.0.3.dev48/junifer/datareader/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/datareader/tests/test_default_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.105499 junifer-0.0.3.dev48/junifer/external/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.077499 junifer-0.0.3.dev48/junifer/external/h5io/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.105499 junifer-0.0.3.dev48/junifer/external/h5io/h5io/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/external/h5io/h5io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28748 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/external/h5io/h5io/_h5io.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/external/h5io/h5io/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/external/h5io/h5io/chunked_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/external/h5io/h5io/chunked_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.105499 junifer-0.0.3.dev48/junifer/external/nilearn/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/external/nilearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/external/nilearn/junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.105499 junifer-0.0.3.dev48/junifer/external/nilearn/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.105499 junifer-0.0.3.dev48/junifer/markers/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/ets_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.105499 junifer-0.0.3.dev48/junifer/markers/falff/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/falff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/falff/falff_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/falff/falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/falff/falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/falff/falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.109499 junifer-0.0.3.dev48/junifer/markers/falff/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/falff/tests/test_falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/falff/tests/test_falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/falff/tests/test_falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.109499 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.109499 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/parcel_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.109499 junifer-0.0.3.dev48/junifer/markers/reho/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/reho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/reho/reho_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/reho/reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/reho/reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/reho/reho_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.109499 junifer-0.0.3.dev48/junifer/markers/reho/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/reho/tests/test_reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/reho/tests/test_reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/reho/tests/test_reho_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/sphere_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.109499 junifer-0.0.3.dev48/junifer/markers/temporal_snr/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/temporal_snr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/temporal_snr/temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/temporal_snr/temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/temporal_snr/temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.109499 junifer-0.0.3.dev48/junifer/markers/temporal_snr/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.113499 junifer-0.0.3.dev48/junifer/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/tests/test_ets_rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/tests/test_marker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/tests/test_markers_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/tests/test_parcel_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/tests/test_sphere_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/markers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.113499 junifer-0.0.3.dev48/junifer/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/pipeline/pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/pipeline/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.113499 junifer-0.0.3.dev48/junifer/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/pipeline/tests/test_pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/pipeline/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/pipeline/tests/test_update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/pipeline/update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.113499 junifer-0.0.3.dev48/junifer/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/preprocess/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.113499 junifer-0.0.3.dev48/junifer/preprocess/confounds/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/preprocess/confounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21846 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/preprocess/confounds/fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.113499 junifer-0.0.3.dev48/junifer/preprocess/confounds/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21614 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.113499 junifer-0.0.3.dev48/junifer/preprocess/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/preprocess/tests/test_preprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.113499 junifer-0.0.3.dev48/junifer/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/storage/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/storage/pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20231 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/storage/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.113499 junifer-0.0.3.dev48/junifer/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/storage/tests/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/storage/tests/test_pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    27919 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/storage/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/storage/tests/test_storage_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/storage/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.113499 junifer-0.0.3.dev48/junifer/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.113499 junifer-0.0.3.dev48/junifer/testing/data/
--rw-r--r--   0 runner    (1001) docker     (123)   406849 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/testing/datagrabbers.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/testing/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.117498 junifer-0.0.3.dev48/junifer/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/testing/tests/test_spmauditory_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/testing/tests/test_testing_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.117498 junifer-0.0.3.dev48/junifer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.117498 junifer-0.0.3.dev48/junifer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.117498 junifer-0.0.3.dev48/junifer/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/utils/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/junifer/utils/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.089499 junifer-0.0.3.dev48/junifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-05-05 10:47:36.000000 junifer-0.0.3.dev48/junifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-05 10:47:36.000000 junifer-0.0.3.dev48/junifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:47:36.000000 junifer-0.0.3.dev48/junifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 10:47:36.000000 junifer-0.0.3.dev48/junifer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-05 10:47:36.000000 junifer-0.0.3.dev48/junifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 10:47:36.000000 junifer-0.0.3.dev48/junifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:47:36.117498 junifer-0.0.3.dev48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:47:36.117498 junifer-0.0.3.dev48/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/tools/create_aomic1000_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/tools/create_aomicpiop1_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/tools/create_aomicpiop2_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/tools/create_bids_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/tools/create_bids_example_dataset_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/tools/create_hcp1200_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-05 10:47:26.000000 junifer-0.0.3.dev48/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.491652 junifer-0.0.3.dev53/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.459652 junifer-0.0.3.dev53/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.459652 junifer-0.0.3.dev53/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/ISSUE_TEMPLATE/dataset-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/ISSUE_TEMPLATE/documention-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/ISSUE_TEMPLATE/marker-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.459652 junifer-0.0.3.dev53/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34353 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-09 10:34:32.491652 junifer-0.0.3.dev53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.459652 junifer-0.0.3.dev53/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.451652 junifer-0.0.3.dev53/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.459652 junifer-0.0.3.dev53/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.459652 junifer-0.0.3.dev53/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.459652 junifer-0.0.3.dev53/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.463652 junifer-0.0.3.dev53/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/datagrabbers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/datareaders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/nilearn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/builtin.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.463652 junifer-0.0.3.dev53/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.463652 junifer-0.0.3.dev53/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/changes/newsfragments/220.doc
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/changes/newsfragments/222.change
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/changes/newsfragments/222.enh
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.463652 junifer-0.0.3.dev53/docs/extending/
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/extending/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16558 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/extending/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/extending/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/extending/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/extending/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/extending/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/extending/parcellations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/help.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.463652 junifer-0.0.3.dev53/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    62148 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/images/junifer_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.463652 junifer-0.0.3.dev53/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/sphinxext/gh_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/starting.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.467652 junifer-0.0.3.dev53/docs/understanding/
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/understanding/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/understanding/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/understanding/datareader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/understanding/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/understanding/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/understanding/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/understanding/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/understanding/storage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.467652 junifer-0.0.3.dev53/docs/using/
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/using/codeless.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/using/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/using/queueing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/using/running.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.467652 junifer-0.0.3.dev53/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/examples/norun_hcpfc_pearson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/examples/norun_ukbvm_gmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/examples/run_compute_parcel_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/examples/run_datagrabber_bids_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/examples/run_ets_rss_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/examples/run_junifer_julearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/examples/run_run_gmd_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.467652 junifer-0.0.3.dev53/examples/yamls/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/examples/yamls/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/examples/yamls/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/examples/yamls/ukb_gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.467652 junifer-0.0.3.dev53/junifer/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-09 10:34:32.000000 junifer-0.0.3.dev53/junifer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.471652 junifer-0.0.3.dev53/junifer/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22536 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.471652 junifer-0.0.3.dev53/junifer/api/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.471652 junifer-0.0.3.dev53/junifer/api/res/afni/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/res/afni/3dAFNItoNIFTI
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/res/afni/3dRSFC
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/res/afni/3dReHo
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/res/afni/afni
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/res/afni/run_afni_docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/res/run_conda.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.471652 junifer-0.0.3.dev53/junifer/api/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.471652 junifer-0.0.3.dev53/junifer/api/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/tests/data/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/tests/data/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/tests/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23970 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.471652 junifer-0.0.3.dev53/junifer/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.471652 junifer-0.0.3.dev53/junifer/configs/juseless/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/juseless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.471652 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/ixi_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.471652 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/ucla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/ukb_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.471652 junifer-0.0.3.dev53/junifer/configs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/configs/tests/test_juseless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.471652 junifer-0.0.3.dev53/junifer/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.455652 junifer-0.0.3.dev53/junifer/data/VOIs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.475652 junifer-0.0.3.dev53/junifer/data/VOIs/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/CogAC_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/CogAR_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/Empathy_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/Motor_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/MultiTask_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/Rew_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/ToM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/VigAtt_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/WM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/eMDN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/eSAD_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/VOIs/meta/extDMN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.455652 junifer-0.0.3.dev53/junifer/data/masks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.475652 junifer-0.0.3.dev53/junifer/data/masks/vickery-patil/
+-rw-r--r--   0 runner    (1001) docker     (123)    88270 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27401 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/parcellations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.475652 junifer-0.0.3.dev53/junifer/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/tests/test_parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.475652 junifer-0.0.3.dev53/junifer/datagrabber/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.479652 junifer-0.0.3.dev53/junifer/datagrabber/aomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/aomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/aomic/id1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/aomic/piop1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/aomic/piop2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.479652 junifer-0.0.3.dev53/junifer/datagrabber/aomic/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/aomic/tests/test_id1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/aomic/tests/test_piop1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/aomic/tests/test_piop2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/hcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/pattern_datalad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.479652 junifer-0.0.3.dev53/junifer/datagrabber/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/tests/test_datagrabber_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/tests/test_datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/tests/test_hcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/tests/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/tests/test_pattern_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datagrabber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.479652 junifer-0.0.3.dev53/junifer/datareader/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datareader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datareader/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.479652 junifer-0.0.3.dev53/junifer/datareader/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/datareader/tests/test_default_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.479652 junifer-0.0.3.dev53/junifer/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.455652 junifer-0.0.3.dev53/junifer/external/h5io/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.479652 junifer-0.0.3.dev53/junifer/external/h5io/h5io/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-09 10:34:23.000000 junifer-0.0.3.dev53/junifer/external/h5io/h5io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28748 2023-05-09 10:34:23.000000 junifer-0.0.3.dev53/junifer/external/h5io/h5io/_h5io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 10:34:23.000000 junifer-0.0.3.dev53/junifer/external/h5io/h5io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-09 10:34:23.000000 junifer-0.0.3.dev53/junifer/external/h5io/h5io/chunked_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-09 10:34:23.000000 junifer-0.0.3.dev53/junifer/external/h5io/h5io/chunked_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.479652 junifer-0.0.3.dev53/junifer/external/nilearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/external/nilearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/external/nilearn/junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.479652 junifer-0.0.3.dev53/junifer/external/nilearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.483652 junifer-0.0.3.dev53/junifer/markers/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/ets_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.483652 junifer-0.0.3.dev53/junifer/markers/falff/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/falff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/falff/falff_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/falff/falff_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/falff/falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/falff/falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.483652 junifer-0.0.3.dev53/junifer/markers/falff/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/falff/tests/test_falff_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/falff/tests/test_falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/falff/tests/test_falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.483652 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.483652 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/parcel_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.483652 junifer-0.0.3.dev53/junifer/markers/reho/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/reho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/reho/reho_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/reho/reho_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/reho/reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/reho/reho_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.483652 junifer-0.0.3.dev53/junifer/markers/reho/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/reho/tests/test_reho_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/reho/tests/test_reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/reho/tests/test_reho_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/sphere_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.487652 junifer-0.0.3.dev53/junifer/markers/temporal_snr/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/temporal_snr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/temporal_snr/temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/temporal_snr/temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/temporal_snr/temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.487652 junifer-0.0.3.dev53/junifer/markers/temporal_snr/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.487652 junifer-0.0.3.dev53/junifer/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/tests/test_ets_rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/tests/test_marker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/tests/test_markers_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/tests/test_parcel_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/tests/test_sphere_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/markers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.487652 junifer-0.0.3.dev53/junifer/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/pipeline/pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/pipeline/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.487652 junifer-0.0.3.dev53/junifer/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/pipeline/tests/test_pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/pipeline/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/pipeline/tests/test_update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/pipeline/update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.487652 junifer-0.0.3.dev53/junifer/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/preprocess/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.487652 junifer-0.0.3.dev53/junifer/preprocess/confounds/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/preprocess/confounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21846 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/preprocess/confounds/fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.487652 junifer-0.0.3.dev53/junifer/preprocess/confounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21614 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.487652 junifer-0.0.3.dev53/junifer/preprocess/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/preprocess/tests/test_preprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.487652 junifer-0.0.3.dev53/junifer/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/storage/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/storage/pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20231 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/storage/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.491652 junifer-0.0.3.dev53/junifer/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/storage/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/storage/tests/test_pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27919 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/storage/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/storage/tests/test_storage_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/storage/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.491652 junifer-0.0.3.dev53/junifer/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.491652 junifer-0.0.3.dev53/junifer/testing/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   406849 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/testing/datagrabbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/testing/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.491652 junifer-0.0.3.dev53/junifer/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/testing/tests/test_spmauditory_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/testing/tests/test_testing_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.491652 junifer-0.0.3.dev53/junifer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.491652 junifer-0.0.3.dev53/junifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.491652 junifer-0.0.3.dev53/junifer/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/utils/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/junifer/utils/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.467652 junifer-0.0.3.dev53/junifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-09 10:34:32.000000 junifer-0.0.3.dev53/junifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-09 10:34:32.000000 junifer-0.0.3.dev53/junifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:34:32.000000 junifer-0.0.3.dev53/junifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 10:34:32.000000 junifer-0.0.3.dev53/junifer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-09 10:34:32.000000 junifer-0.0.3.dev53/junifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 10:34:32.000000 junifer-0.0.3.dev53/junifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:34:32.495652 junifer-0.0.3.dev53/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:34:32.491652 junifer-0.0.3.dev53/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/tools/create_aomic1000_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/tools/create_aomicpiop1_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/tools/create_aomicpiop2_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/tools/create_bids_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/tools/create_bids_example_dataset_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/tools/create_hcp1200_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-09 10:34:22.000000 junifer-0.0.3.dev53/tox.ini
```

### Comparing `junifer-0.0.3.dev48/.github/ISSUE_TEMPLATE/bug-report.yml` & `junifer-0.0.3.dev53/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/.github/ISSUE_TEMPLATE/dataset-request.yml` & `junifer-0.0.3.dev53/.github/ISSUE_TEMPLATE/dataset-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/.github/ISSUE_TEMPLATE/documention-request.yml` & `junifer-0.0.3.dev53/.github/ISSUE_TEMPLATE/documention-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/.github/ISSUE_TEMPLATE/feature-request.yml` & `junifer-0.0.3.dev53/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/.github/ISSUE_TEMPLATE/marker-request.yml` & `junifer-0.0.3.dev53/.github/ISSUE_TEMPLATE/marker-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/.github/workflows/ci-docs.yml` & `junifer-0.0.3.dev53/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/.github/workflows/ci.yml` & `junifer-0.0.3.dev53/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/.github/workflows/docs-preview.yml` & `junifer-0.0.3.dev53/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/.github/workflows/docs.yml` & `junifer-0.0.3.dev53/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/.github/workflows/lint.yml` & `junifer-0.0.3.dev53/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/.github/workflows/pypi.yml` & `junifer-0.0.3.dev53/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/.gitignore` & `junifer-0.0.3.dev53/.gitignore`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/LICENSE.md` & `junifer-0.0.3.dev53/LICENSE.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/PKG-INFO` & `junifer-0.0.3.dev53/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.3.dev48
+Version: 0.0.3.dev53
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/junifer
 Project-URL: documentation, https://juaml.github.io/junifer
 Project-URL: repository, https://github.com/juaml/junifer
@@ -32,14 +32,15 @@
 ![Junifer logo](docs/images/junifer_logo.png "junifer logo")
 
 # junifer - JUelich NeuroImaging FEature extractoR
 
 ![PyPI](https://img.shields.io/pypi/v/junifer?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/junifer?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/junifer?style=flat-square)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/junifer/badges/version.svg)](https://anaconda.org/conda-forge/junifer)
 ![GitHub](https://img.shields.io/github/license/juaml/junifer?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/junifer?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 
 ## About
 
 junifer is a data handling and feature extraction library targeted towards neuroimaging data specifically functional MRI data.
@@ -61,23 +62,28 @@
   * `markers`: Markers module.
   * `pipeline`: Pipeline module.
   * `preprocess`: Preprocessing module.
   * `storage`: Storage module.
   * `testing`: Testing components module.
   * `utils`: Utilities module (e.g. logging)
 
-
 ## Installation
 
 Use `pip` to install from PyPI like so:
 
 ```
 pip install junifer
 ```
 
+You can also install via `conda`, like so:
+
+```
+conda install -c conda-forge junifer
+```
+
 ## Citation
 
 If you use junifer in a scientific publication, we would appreciate if you cite our work. Currently, we do not have a publication, so feel free to use the project [URL](https://juaml.github.io/junifer).
 
 ## Funding
 
 We thank the [Helmholtz Imaging Platform](https://helmholtz-imaging.de/) and
```

### Comparing `junifer-0.0.3.dev48/README.md` & `junifer-0.0.3.dev53/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ![Junifer logo](docs/images/junifer_logo.png "junifer logo")
 
 # junifer - JUelich NeuroImaging FEature extractoR
 
 ![PyPI](https://img.shields.io/pypi/v/junifer?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/junifer?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/junifer?style=flat-square)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/junifer/badges/version.svg)](https://anaconda.org/conda-forge/junifer)
 ![GitHub](https://img.shields.io/github/license/juaml/junifer?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/junifer?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 
 ## About
 
 junifer is a data handling and feature extraction library targeted towards neuroimaging data specifically functional MRI data.
@@ -30,23 +31,28 @@
   * `markers`: Markers module.
   * `pipeline`: Pipeline module.
   * `preprocess`: Preprocessing module.
   * `storage`: Storage module.
   * `testing`: Testing components module.
   * `utils`: Utilities module (e.g. logging)
 
-
 ## Installation
 
 Use `pip` to install from PyPI like so:
 
 ```
 pip install junifer
 ```
 
+You can also install via `conda`, like so:
+
+```
+conda install -c conda-forge junifer
+```
+
 ## Citation
 
 If you use junifer in a scientific publication, we would appreciate if you cite our work. Currently, we do not have a publication, so feel free to use the project [URL](https://juaml.github.io/junifer).
 
 ## Funding
 
 We thank the [Helmholtz Imaging Platform](https://helmholtz-imaging.de/) and
```

### Comparing `junifer-0.0.3.dev48/codecov.yml` & `junifer-0.0.3.dev53/codecov.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/conda-env.yml` & `junifer-0.0.3.dev53/conda-env.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/Makefile` & `junifer-0.0.3.dev53/docs/Makefile`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/_static/css/custom.css` & `junifer-0.0.3.dev53/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/_templates/versions.html` & `junifer-0.0.3.dev53/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/builtin.rst` & `junifer-0.0.3.dev53/docs/builtin.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/changes/contributors.inc` & `junifer-0.0.3.dev53/docs/changes/contributors.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/conf.py` & `junifer-0.0.3.dev53/docs/conf.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/contribution.rst` & `junifer-0.0.3.dev53/docs/contribution.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/extending/coordinates.rst` & `junifer-0.0.3.dev53/docs/extending/coordinates.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/extending/datagrabber.rst` & `junifer-0.0.3.dev53/docs/extending/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/extending/extension.rst` & `junifer-0.0.3.dev53/docs/extending/extension.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/extending/index.rst` & `junifer-0.0.3.dev53/docs/extending/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/extending/marker.rst` & `junifer-0.0.3.dev53/docs/extending/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/extending/masks.rst` & `junifer-0.0.3.dev53/docs/extending/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/extending/parcellations.rst` & `junifer-0.0.3.dev53/docs/extending/parcellations.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/faq.rst` & `junifer-0.0.3.dev53/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/help.rst` & `junifer-0.0.3.dev53/docs/help.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/images/junifer_logo.png` & `junifer-0.0.3.dev53/docs/images/junifer_logo.png`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/index.rst` & `junifer-0.0.3.dev53/docs/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/installation.rst` & `junifer-0.0.3.dev53/docs/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,27 @@
 
 Use ``pip`` to install julearn from `PyPI <https://pypi.org>`_, like so:
 
 .. code-block:: bash
 
     pip install junifer
 
+You can also install via ``conda``, like so:
+
+.. code-block:: bash
+
+    conda install -c conda-forge junifer
+
+.. attention::
+
+   Installation on macOS and Windows might fail via ``conda`` due to ``datalad``.
+   In that case, please refer to
+   `Datalad installation instructions
+   <http://handbook.datalad.org/en/latest/intro/installation.html>`_ for solutions.
+   In case the problem persists, please install it via ``pip`` as mentioned earlier.
 
 .. _install_development_git:
 
 Local Git repository
 ~~~~~~~~~~~~~~~~~~~~
 
 Follow the `detailed contribution guidelines <contribution.rst>`_.
```

### Comparing `junifer-0.0.3.dev48/docs/links.inc` & `junifer-0.0.3.dev53/docs/links.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/maintaining.rst` & `junifer-0.0.3.dev53/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/sphinxext/gh_substitutions.py` & `junifer-0.0.3.dev53/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/starting.rst` & `junifer-0.0.3.dev53/docs/starting.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/understanding/data.rst` & `junifer-0.0.3.dev53/docs/understanding/data.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/understanding/datagrabber.rst` & `junifer-0.0.3.dev53/docs/understanding/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/understanding/datareader.rst` & `junifer-0.0.3.dev53/docs/understanding/datareader.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/understanding/index.rst` & `junifer-0.0.3.dev53/docs/understanding/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/understanding/marker.rst` & `junifer-0.0.3.dev53/docs/understanding/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/understanding/pipeline.rst` & `junifer-0.0.3.dev53/docs/understanding/pipeline.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/understanding/preprocess.rst` & `junifer-0.0.3.dev53/docs/understanding/preprocess.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/understanding/storage.rst` & `junifer-0.0.3.dev53/docs/understanding/storage.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/using/codeless.rst` & `junifer-0.0.3.dev53/docs/using/codeless.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/using/index.rst` & `junifer-0.0.3.dev53/docs/using/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/using/masks.rst` & `junifer-0.0.3.dev53/docs/using/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/using/queueing.rst` & `junifer-0.0.3.dev53/docs/using/queueing.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/using/running.rst` & `junifer-0.0.3.dev53/docs/using/running.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/docs/whats_new.rst` & `junifer-0.0.3.dev53/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/examples/norun_hcpfc_pearson.py` & `junifer-0.0.3.dev53/examples/norun_hcpfc_pearson.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/examples/norun_ukbvm_gmd.py` & `junifer-0.0.3.dev53/examples/norun_ukbvm_gmd.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/examples/run_compute_parcel_mean.py` & `junifer-0.0.3.dev53/examples/run_compute_parcel_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/examples/run_datagrabber_bids_datalad.py` & `junifer-0.0.3.dev53/examples/run_datagrabber_bids_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/examples/run_ets_rss_marker.py` & `junifer-0.0.3.dev53/examples/run_ets_rss_marker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/examples/run_junifer_julearn.py` & `junifer-0.0.3.dev53/examples/run_junifer_julearn.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/examples/run_run_gmd_mean.py` & `junifer-0.0.3.dev53/examples/run_run_gmd_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/examples/yamls/gmd_mean.yaml` & `junifer-0.0.3.dev53/examples/yamls/gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/examples/yamls/ukb_gmd_mean.yaml` & `junifer-0.0.3.dev53/examples/yamls/ukb_gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/api/cli.py` & `junifer-0.0.3.dev53/junifer/api/cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/api/decorators.py` & `junifer-0.0.3.dev53/junifer/api/decorators.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/api/functions.py` & `junifer-0.0.3.dev53/junifer/api/functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/api/parser.py` & `junifer-0.0.3.dev53/junifer/api/parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/api/res/afni/run_afni_docker.sh` & `junifer-0.0.3.dev53/junifer/api/res/afni/run_afni_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/api/tests/test_api_utils.py` & `junifer-0.0.3.dev53/junifer/api/tests/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/api/tests/test_cli.py` & `junifer-0.0.3.dev53/junifer/api/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/api/tests/test_functions.py` & `junifer-0.0.3.dev53/junifer/api/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/api/tests/test_parser.py` & `junifer-0.0.3.dev53/junifer/api/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/api/utils.py` & `junifer-0.0.3.dev53/junifer/api/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py` & `junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/camcan_vbm.py` & `junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/ixi_vbm.py` & `junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py` & `junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py` & `junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py` & `junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/tests/test_ucla.py` & `junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/tests/test_ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py` & `junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/ucla.py` & `junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/configs/juseless/datagrabbers/ukb_vbm.py` & `junifer-0.0.3.dev53/junifer/configs/juseless/datagrabbers/ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/configs/tests/test_juseless.py` & `junifer-0.0.3.dev53/junifer/configs/tests/test_juseless.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt` & `junifer-0.0.3.dev53/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt` & `junifer-0.0.3.dev53/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/VOIs/meta/Rew_VOIs.txt` & `junifer-0.0.3.dev53/junifer/data/VOIs/meta/Rew_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/VOIs/meta/WM_VOIs.txt` & `junifer-0.0.3.dev53/junifer/data/VOIs/meta/WM_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/coordinates.py` & `junifer-0.0.3.dev53/junifer/data/coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz` & `junifer-0.0.3.dev53/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz` & `junifer-0.0.3.dev53/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz` & `junifer-0.0.3.dev53/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/masks.py` & `junifer-0.0.3.dev53/junifer/data/masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/parcellations.py` & `junifer-0.0.3.dev53/junifer/data/parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/tests/test_coordinates.py` & `junifer-0.0.3.dev53/junifer/data/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/tests/test_data_utils.py` & `junifer-0.0.3.dev53/junifer/data/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/tests/test_masks.py` & `junifer-0.0.3.dev53/junifer/data/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/tests/test_parcellations.py` & `junifer-0.0.3.dev53/junifer/data/tests/test_parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/data/utils.py` & `junifer-0.0.3.dev53/junifer/data/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/__init__.py` & `junifer-0.0.3.dev53/junifer/datagrabber/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/aomic/id1000.py` & `junifer-0.0.3.dev53/junifer/datagrabber/aomic/id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/aomic/piop1.py` & `junifer-0.0.3.dev53/junifer/datagrabber/aomic/piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/aomic/piop2.py` & `junifer-0.0.3.dev53/junifer/datagrabber/aomic/piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/aomic/tests/test_id1000.py` & `junifer-0.0.3.dev53/junifer/datagrabber/aomic/tests/test_id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/aomic/tests/test_piop1.py` & `junifer-0.0.3.dev53/junifer/datagrabber/aomic/tests/test_piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/aomic/tests/test_piop2.py` & `junifer-0.0.3.dev53/junifer/datagrabber/aomic/tests/test_piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/base.py` & `junifer-0.0.3.dev53/junifer/datagrabber/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/datalad_base.py` & `junifer-0.0.3.dev53/junifer/datagrabber/datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/hcp.py` & `junifer-0.0.3.dev53/junifer/datagrabber/hcp.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/multiple.py` & `junifer-0.0.3.dev53/junifer/datagrabber/multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/pattern.py` & `junifer-0.0.3.dev53/junifer/datagrabber/pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/pattern_datalad.py` & `junifer-0.0.3.dev53/junifer/datagrabber/pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/tests/test_base.py` & `junifer-0.0.3.dev53/junifer/datagrabber/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/tests/test_datagrabber_utils.py` & `junifer-0.0.3.dev53/junifer/datagrabber/tests/test_datagrabber_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/tests/test_datalad_base.py` & `junifer-0.0.3.dev53/junifer/datagrabber/tests/test_datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/tests/test_hcp.py` & `junifer-0.0.3.dev53/junifer/datagrabber/tests/test_hcp.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/tests/test_multiple.py` & `junifer-0.0.3.dev53/junifer/datagrabber/tests/test_multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/tests/test_pattern.py` & `junifer-0.0.3.dev53/junifer/datagrabber/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/tests/test_pattern_datalad.py` & `junifer-0.0.3.dev53/junifer/datagrabber/tests/test_pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datagrabber/utils.py` & `junifer-0.0.3.dev53/junifer/datagrabber/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datareader/default.py` & `junifer-0.0.3.dev53/junifer/datareader/default.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/datareader/tests/test_default_reader.py` & `junifer-0.0.3.dev53/junifer/datareader/tests/test_default_reader.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/external/h5io/h5io/_h5io.py` & `junifer-0.0.3.dev53/junifer/external/h5io/h5io/_h5io.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/external/h5io/h5io/chunked_array.py` & `junifer-0.0.3.dev53/junifer/external/h5io/h5io/chunked_array.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/external/h5io/h5io/chunked_list.py` & `junifer-0.0.3.dev53/junifer/external/h5io/h5io/chunked_list.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/external/nilearn/junifer_nifti_spheres_masker.py` & `junifer-0.0.3.dev53/junifer/external/nilearn/junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py` & `junifer-0.0.3.dev53/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/__init__.py` & `junifer-0.0.3.dev53/junifer/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/base.py` & `junifer-0.0.3.dev53/junifer/markers/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/collection.py` & `junifer-0.0.3.dev53/junifer/markers/collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/ets_rss.py` & `junifer-0.0.3.dev53/junifer/markers/ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/falff/falff_base.py` & `junifer-0.0.3.dev53/junifer/markers/falff/falff_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/falff/falff_estimator.py` & `junifer-0.0.3.dev53/junifer/markers/falff/falff_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/falff/falff_parcels.py` & `junifer-0.0.3.dev53/junifer/markers/falff/falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/falff/falff_spheres.py` & `junifer-0.0.3.dev53/junifer/markers/falff/falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/falff/tests/test_falff_estimator.py` & `junifer-0.0.3.dev53/junifer/markers/falff/tests/test_falff_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/falff/tests/test_falff_parcels.py` & `junifer-0.0.3.dev53/junifer/markers/falff/tests/test_falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/falff/tests/test_falff_spheres.py` & `junifer-0.0.3.dev53/junifer/markers/falff/tests/test_falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py` & `junifer-0.0.3.dev53/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py` & `junifer-0.0.3.dev53/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py` & `junifer-0.0.3.dev53/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/functional_connectivity/functional_connectivity_base.py` & `junifer-0.0.3.dev53/junifer/markers/functional_connectivity/functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/functional_connectivity/functional_connectivity_parcels.py` & `junifer-0.0.3.dev53/junifer/markers/functional_connectivity/functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/functional_connectivity/functional_connectivity_spheres.py` & `junifer-0.0.3.dev53/junifer/markers/functional_connectivity/functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py` & `junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py` & `junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py` & `junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py` & `junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py` & `junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py` & `junifer-0.0.3.dev53/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/parcel_aggregation.py` & `junifer-0.0.3.dev53/junifer/markers/parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/reho/reho_base.py` & `junifer-0.0.3.dev53/junifer/markers/reho/reho_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/reho/reho_estimator.py` & `junifer-0.0.3.dev53/junifer/markers/reho/reho_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/reho/reho_parcels.py` & `junifer-0.0.3.dev53/junifer/markers/reho/reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/reho/reho_spheres.py` & `junifer-0.0.3.dev53/junifer/markers/reho/reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/reho/tests/test_reho_estimator.py` & `junifer-0.0.3.dev53/junifer/markers/reho/tests/test_reho_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/reho/tests/test_reho_parcels.py` & `junifer-0.0.3.dev53/junifer/markers/reho/tests/test_reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/reho/tests/test_reho_spheres.py` & `junifer-0.0.3.dev53/junifer/markers/reho/tests/test_reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/sphere_aggregation.py` & `junifer-0.0.3.dev53/junifer/markers/sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/temporal_snr/temporal_snr_base.py` & `junifer-0.0.3.dev53/junifer/markers/temporal_snr/temporal_snr_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/temporal_snr/temporal_snr_parcels.py` & `junifer-0.0.3.dev53/junifer/markers/temporal_snr/temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/temporal_snr/temporal_snr_spheres.py` & `junifer-0.0.3.dev53/junifer/markers/temporal_snr/temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py` & `junifer-0.0.3.dev53/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py` & `junifer-0.0.3.dev53/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/tests/test_collection.py` & `junifer-0.0.3.dev53/junifer/markers/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/tests/test_ets_rss.py` & `junifer-0.0.3.dev53/junifer/markers/tests/test_ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/tests/test_marker_utils.py` & `junifer-0.0.3.dev53/junifer/markers/tests/test_marker_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/tests/test_markers_base.py` & `junifer-0.0.3.dev53/junifer/markers/tests/test_markers_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/tests/test_parcel_aggregation.py` & `junifer-0.0.3.dev53/junifer/markers/tests/test_parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/tests/test_sphere_aggregation.py` & `junifer-0.0.3.dev53/junifer/markers/tests/test_sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/markers/utils.py` & `junifer-0.0.3.dev53/junifer/markers/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/pipeline/pipeline_step_mixin.py` & `junifer-0.0.3.dev53/junifer/pipeline/pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/pipeline/registry.py` & `junifer-0.0.3.dev53/junifer/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/pipeline/tests/test_pipeline_step_mixin.py` & `junifer-0.0.3.dev53/junifer/pipeline/tests/test_pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/pipeline/tests/test_registry.py` & `junifer-0.0.3.dev53/junifer/pipeline/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/pipeline/tests/test_update_meta_mixin.py` & `junifer-0.0.3.dev53/junifer/pipeline/tests/test_update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/pipeline/update_meta_mixin.py` & `junifer-0.0.3.dev53/junifer/pipeline/update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/pipeline/utils.py` & `junifer-0.0.3.dev53/junifer/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/preprocess/base.py` & `junifer-0.0.3.dev53/junifer/preprocess/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/preprocess/confounds/fmriprep_confound_remover.py` & `junifer-0.0.3.dev53/junifer/preprocess/confounds/fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py` & `junifer-0.0.3.dev53/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/preprocess/tests/test_preprocess_base.py` & `junifer-0.0.3.dev53/junifer/preprocess/tests/test_preprocess_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/stats.py` & `junifer-0.0.3.dev53/junifer/stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/storage/base.py` & `junifer-0.0.3.dev53/junifer/storage/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/storage/hdf5.py` & `junifer-0.0.3.dev53/junifer/storage/hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/storage/pandas_base.py` & `junifer-0.0.3.dev53/junifer/storage/pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/storage/sqlite.py` & `junifer-0.0.3.dev53/junifer/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/storage/tests/test_hdf5.py` & `junifer-0.0.3.dev53/junifer/storage/tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/storage/tests/test_pandas_base.py` & `junifer-0.0.3.dev53/junifer/storage/tests/test_pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/storage/tests/test_sqlite.py` & `junifer-0.0.3.dev53/junifer/storage/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/storage/tests/test_storage_base.py` & `junifer-0.0.3.dev53/junifer/storage/tests/test_storage_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/storage/tests/test_utils.py` & `junifer-0.0.3.dev53/junifer/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/storage/utils.py` & `junifer-0.0.3.dev53/junifer/storage/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv` & `junifer-0.0.3.dev53/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/testing/datagrabbers.py` & `junifer-0.0.3.dev53/junifer/testing/datagrabbers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/testing/registry.py` & `junifer-0.0.3.dev53/junifer/testing/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py` & `junifer-0.0.3.dev53/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/testing/tests/test_partlycloudytesting_datagrabber.py` & `junifer-0.0.3.dev53/junifer/testing/tests/test_partlycloudytesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/testing/tests/test_spmauditory_datagrabber.py` & `junifer-0.0.3.dev53/junifer/testing/tests/test_spmauditory_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/testing/tests/test_testing_registry.py` & `junifer-0.0.3.dev53/junifer/testing/tests/test_testing_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/testing/utils.py` & `junifer-0.0.3.dev53/junifer/testing/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/tests/test_stats.py` & `junifer-0.0.3.dev53/junifer/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/utils/logging.py` & `junifer-0.0.3.dev53/junifer/utils/logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/utils/tests/test_fs.py` & `junifer-0.0.3.dev53/junifer/utils/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer/utils/tests/test_logging.py` & `junifer-0.0.3.dev53/junifer/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/junifer.egg-info/PKG-INFO` & `junifer-0.0.3.dev53/junifer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.3.dev48
+Version: 0.0.3.dev53
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/junifer
 Project-URL: documentation, https://juaml.github.io/junifer
 Project-URL: repository, https://github.com/juaml/junifer
@@ -32,14 +32,15 @@
 ![Junifer logo](docs/images/junifer_logo.png "junifer logo")
 
 # junifer - JUelich NeuroImaging FEature extractoR
 
 ![PyPI](https://img.shields.io/pypi/v/junifer?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/junifer?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/junifer?style=flat-square)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/junifer/badges/version.svg)](https://anaconda.org/conda-forge/junifer)
 ![GitHub](https://img.shields.io/github/license/juaml/junifer?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/junifer?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 
 ## About
 
 junifer is a data handling and feature extraction library targeted towards neuroimaging data specifically functional MRI data.
@@ -61,23 +62,28 @@
   * `markers`: Markers module.
   * `pipeline`: Pipeline module.
   * `preprocess`: Preprocessing module.
   * `storage`: Storage module.
   * `testing`: Testing components module.
   * `utils`: Utilities module (e.g. logging)
 
-
 ## Installation
 
 Use `pip` to install from PyPI like so:
 
 ```
 pip install junifer
 ```
 
+You can also install via `conda`, like so:
+
+```
+conda install -c conda-forge junifer
+```
+
 ## Citation
 
 If you use junifer in a scientific publication, we would appreciate if you cite our work. Currently, we do not have a publication, so feel free to use the project [URL](https://juaml.github.io/junifer).
 
 ## Funding
 
 We thank the [Helmholtz Imaging Platform](https://helmholtz-imaging.de/) and
```

### Comparing `junifer-0.0.3.dev48/junifer.egg-info/SOURCES.txt` & `junifer-0.0.3.dev53/junifer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/pyproject.toml` & `junifer-0.0.3.dev53/pyproject.toml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/tools/create_aomic1000_example_dataset.py` & `junifer-0.0.3.dev53/tools/create_aomic1000_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/tools/create_aomicpiop1_example_dataset.py` & `junifer-0.0.3.dev53/tools/create_aomicpiop1_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/tools/create_aomicpiop2_example_dataset.py` & `junifer-0.0.3.dev53/tools/create_aomicpiop2_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/tools/create_bids_example_dataset.py` & `junifer-0.0.3.dev53/tools/create_bids_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/tools/create_bids_example_dataset_sessions.py` & `junifer-0.0.3.dev53/tools/create_bids_example_dataset_sessions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/tools/create_hcp1200_example_dataset.py` & `junifer-0.0.3.dev53/tools/create_hcp1200_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev48/tox.ini` & `junifer-0.0.3.dev53/tox.ini`

 * *Files identical despite different names*

