# Comparing `tmp/numba-stats-1.1.1.tar.gz` & `tmp/numba-stats-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba-stats-1.1.1.tar", last modified: Thu Apr 13 13:50:30 2023, max compression
+gzip compressed data, was "numba-stats-1.2.0.tar", last modified: Tue May  9 11:25:45 2023, max compression
```

## Comparing `numba-stats-1.1.1.tar` & `numba-stats-1.2.0.tar`

### file list

```diff
@@ -1,63 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.748338 numba-stats-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.724336 numba-stats-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.728336 numba-stats-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 13:50:01.000000 numba-stats-1.1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-13 13:50:01.000000 numba-stats-1.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-13 13:50:01.000000 numba-stats-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-13 13:50:01.000000 numba-stats-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 13:50:01.000000 numba-stats-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 13:50:01.000000 numba-stats-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-13 13:50:30.748338 numba-stats-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-13 13:50:01.000000 numba-stats-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.732336 numba-stats-1.1.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:01.000000 numba-stats-1.1.1/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-13 13:50:01.000000 numba-stats-1.1.1/benchmarks/test_stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-04-13 13:50:01.000000 numba-stats-1.1.1/coverage.sh
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-13 13:50:01.000000 numba-stats-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-13 13:50:30.748338 numba-stats-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 13:50:01.000000 numba-stats-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.724336 numba-stats-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.740337 numba-stats-1.1.1/src/numba_stats/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/_special.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 13:50:18.000000 numba-stats-1.1.1/src/numba_stats/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/bernstein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/cpoisson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/crystalball.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/crystalball_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/expon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/lognorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/poisson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/qgaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/t.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/truncexpon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/truncnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/tsallis.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/voigt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.740337 numba-stats-1.1.1/src/numba_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-13 13:50:30.000000 numba-stats-1.1.1/src/numba_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-13 13:50:30.000000 numba-stats-1.1.1/src/numba_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:50:30.000000 numba-stats-1.1.1/src/numba_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 13:50:30.000000 numba-stats-1.1.1/src/numba_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 13:50:30.000000 numba-stats-1.1.1/src/numba_stats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.748338 numba-stats-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_bernstein.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_cpoisson.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_crystalball.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_crystalball_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_expon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_lognorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_poisson.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_qgaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_t.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_truncexpon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_truncnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_tsallis.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.130054 numba-stats-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.114054 numba-stats-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.118054 numba-stats-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 11:25:14.000000 numba-stats-1.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-09 11:25:14.000000 numba-stats-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-09 11:25:14.000000 numba-stats-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-09 11:25:14.000000 numba-stats-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 11:25:14.000000 numba-stats-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-09 11:25:14.000000 numba-stats-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-09 11:25:45.130054 numba-stats-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-09 11:25:14.000000 numba-stats-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.118054 numba-stats-1.2.0/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-09 11:25:14.000000 numba-stats-1.2.0/bench/plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-09 11:25:14.000000 numba-stats-1.2.0/bench/test_stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-05-09 11:25:14.000000 numba-stats-1.2.0/coverage.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.114054 numba-stats-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.122054 numba-stats-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    70602 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/bernstein.density.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58277 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/expon.cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    57880 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/expon.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58675 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/expon.ppf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58022 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/norm.cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58418 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/norm.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58822 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/norm.ppf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59429 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/t.cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61026 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/t.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    57399 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/t.ppf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58746 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncexpon.cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59714 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncexpon.pdf.plus.norm.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58950 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncexpon.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58745 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncexpon.ppf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    62491 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncnorm.cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59095 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncnorm.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61300 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncnorm.ppf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/uniform.cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58392 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/uniform.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58792 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/uniform.ppf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    60274 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/voigt.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-09 11:25:14.000000 numba-stats-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-09 11:25:45.130054 numba-stats-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-09 11:25:14.000000 numba-stats-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.114054 numba-stats-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.126054 numba-stats-1.2.0/src/numba_stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/_special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 11:25:30.000000 numba-stats-1.2.0/src/numba_stats/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/bernstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/cpoisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/cruijff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/crystalball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/crystalball_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/expon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/lognorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/qgaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/truncexpon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/truncnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/tsallis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.126054 numba-stats-1.2.0/src/numba_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-09 11:25:44.000000 numba-stats-1.2.0/src/numba_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-09 11:25:44.000000 numba-stats-1.2.0/src/numba_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:25:44.000000 numba-stats-1.2.0/src/numba_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-09 11:25:44.000000 numba-stats-1.2.0/src/numba_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 11:25:44.000000 numba-stats-1.2.0/src/numba_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.130054 numba-stats-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_bernstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_cpoisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_cruijff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_crystalball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_crystalball_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_expon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_lognorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_qgaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_truncexpon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_truncnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_tsallis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_voigt.py
```

### Comparing `numba-stats-1.1.1/.github/workflows/release.yml` & `numba-stats-1.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/.pre-commit-config.yaml` & `numba-stats-1.2.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   - id: check-yaml
   - id: debug-statements
   - id: end-of-file-fixer
   - id: mixed-line-ending
   - id: sort-simple-yaml
   - id: file-contents-sorter
   - id: trailing-whitespace
-    exclude: ^doc/_static/.*.svg
+    exclude: .*\.svg
 
 # Python linter (Flake8)
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
   - id: flake8
```

### Comparing `numba-stats-1.1.1/LICENSE` & `numba-stats-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/setup.cfg` & `numba-stats-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/_special.py` & `numba-stats-1.2.0/src/numba_stats/_special.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/_util.py` & `numba-stats-1.2.0/src/numba_stats/_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         impl = f"_{fname}"
         if impl not in d:
             continue
         fn = d[impl]
         args = inspect.signature(fn).parameters
         args = ", ".join([f"{x}" for x in args])
         doc_title = {
+            "density": "Return density.",
             "logpdf": "Return log of probability density.",
             "logpmf": "Return log of probability mass.",
             "pmf": "Return probability mass.",
             "pdf": "Return probability density.",
             "cdf": "Return cumulative probability.",
             "ppf": "Return quantile for given probability.",
         }.get(fname, None)
```

### Comparing `numba-stats-1.1.1/src/numba_stats/bernstein.py` & `numba-stats-1.2.0/src/numba_stats/bernstein.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/cpoisson.py` & `numba-stats-1.2.0/src/numba_stats/cpoisson.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/crystalball.py` & `numba-stats-1.2.0/src/numba_stats/crystalball.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/crystalball_ex.py` & `numba-stats-1.2.0/src/numba_stats/crystalball_ex.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/expon.py` & `numba-stats-1.2.0/src/numba_stats/expon.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/lognorm.py` & `numba-stats-1.2.0/src/numba_stats/lognorm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/norm.py` & `numba-stats-1.2.0/src/numba_stats/norm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/poisson.py` & `numba-stats-1.2.0/src/numba_stats/poisson.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/qgaussian.py` & `numba-stats-1.2.0/src/numba_stats/qgaussian.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/t.py` & `numba-stats-1.2.0/src/numba_stats/t.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/truncexpon.py` & `numba-stats-1.2.0/src/numba_stats/truncexpon.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from . import expon as _expon
 
 _doc_par = """
 x: ArrayLike
     Random variate.
 xmin : float
     Lower edge of the distribution.
-xmin : float
+xmax : float
     Upper edge of the distribution.
 loc : float
     Location of the mode.
 scale : float
     Width parameter.
 """
 
@@ -63,18 +63,16 @@
         else:
             z[i] = 0
     return z
 
 
 @_jit(4)
 def _ppf(p, xmin, xmax, loc, scale):
-    T = type(xmin)
-    scale2 = T(1) / scale
-    zmin = (xmin - loc) * scale2
-    zmax = (xmax - loc) * scale2
+    zmin = (xmin - loc) / scale
+    zmax = (xmax - loc) / scale
     pmin = _expon._cdf1(zmin)
     pmax = _expon._cdf1(zmax)
     z = p * (pmax - pmin) + pmin
     for i in _prange(len(z)):
         z[i] = _expon._ppf1(z[i])
     return z * scale + loc
```

### Comparing `numba-stats-1.1.1/src/numba_stats/truncnorm.py` & `numba-stats-1.2.0/src/numba_stats/truncnorm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/tsallis.py` & `numba-stats-1.2.0/src/numba_stats/tsallis.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/uniform.py` & `numba-stats-1.2.0/src/numba_stats/uniform.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/src/numba_stats/voigt.py` & `numba-stats-1.2.0/src/numba_stats/voigt.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_bernstein.py` & `numba-stats-1.2.0/tests/test_bernstein.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_crystalball.py` & `numba-stats-1.2.0/tests/test_crystalball.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_crystalball_ex.py` & `numba-stats-1.2.0/tests/test_crystalball_ex.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_doc.py` & `numba-stats-1.2.0/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_expon.py` & `numba-stats-1.2.0/tests/test_expon.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_lognorm.py` & `numba-stats-1.2.0/tests/test_lognorm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_norm.py` & `numba-stats-1.2.0/tests/test_norm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_qgaussian.py` & `numba-stats-1.2.0/tests/test_qgaussian.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_t.py` & `numba-stats-1.2.0/tests/test_t.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_truncexpon.py` & `numba-stats-1.2.0/tests/test_truncexpon.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_truncnorm.py` & `numba-stats-1.2.0/tests/test_truncnorm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_tsallis.py` & `numba-stats-1.2.0/tests/test_tsallis.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.1/tests/test_uniform.py` & `numba-stats-1.2.0/tests/test_uniform.py`

 * *Files identical despite different names*

