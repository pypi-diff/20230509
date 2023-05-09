# Comparing `tmp/matfree-0.0.4.tar.gz` & `tmp/matfree-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matfree-0.0.4.tar", last modified: Thu May  4 12:44:31 2023, max compression
+gzip compressed data, was "matfree-0.0.5.tar", last modified: Tue May  9 10:18:46 2023, max compression
```

## Comparing `matfree-0.0.4.tar` & `matfree-0.0.5.tar`

### file list

```diff
@@ -1,80 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.929407 matfree-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.913407 matfree-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.917407 matfree-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-04 12:44:14.000000 matfree-0.0.4/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-04 12:44:14.000000 matfree-0.0.4/.github/workflows/doc-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-04 12:44:14.000000 matfree-0.0.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-04 12:44:14.000000 matfree-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-04 12:44:14.000000 matfree-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 12:44:14.000000 matfree-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-04 12:44:14.000000 matfree-0.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-04 12:44:31.929407 matfree-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-04 12:44:14.000000 matfree-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.917407 matfree-0.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.917407 matfree-0.0.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/api/decomp.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/api/hutch.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/api/montecarlo.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/api/slq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.917407 matfree-0.0.4/docs/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/benchmarks/control_variates.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/benchmarks/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/benchmarks/jacobian_squared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.917407 matfree-0.0.4/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/dev/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.917407 matfree-0.0.4/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-04 12:44:14.000000 matfree-0.0.4/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.921407 matfree-0.0.4/matfree/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-04 12:44:31.000000 matfree-0.0.4/matfree/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.925407 matfree-0.0.4/matfree/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/func.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/np.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/plt.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/prng.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/backend/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/benchmark_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/hutch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/slq.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-04 12:44:14.000000 matfree-0.0.4/matfree/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.921407 matfree-0.0.4/matfree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-04 12:44:31.000000 matfree-0.0.4/matfree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-04 12:44:31.000000 matfree-0.0.4/matfree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:44:31.000000 matfree-0.0.4/matfree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 12:44:31.000000 matfree-0.0.4/matfree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 12:44:31.000000 matfree-0.0.4/matfree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-04 12:44:14.000000 matfree-0.0.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-04 12:44:14.000000 matfree-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-04 12:44:31.929407 matfree-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 12:44:14.000000 matfree-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.925407 matfree-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.925407 matfree-0.0.4/tests/test_decomp/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_decomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_decomp/test_gkl_bidiagonal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_decomp/test_lanczos_tridiagonal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_decomp/test_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.925407 matfree-0.0.4/tests/test_hutch/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_hutch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_hutch/test_diagonal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_hutch/test_frobeniusnorm_squared.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_hutch/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_hutch/test_trace_and_diagonal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.925407 matfree-0.0.4/tests/test_montecarlo/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_montecarlo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_montecarlo/test_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_montecarlo/test_van_der_corput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:44:31.929407 matfree-0.0.4/tests/test_slq/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_slq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_slq/test_logdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-04 12:44:14.000000 matfree-0.0.4/tests/test_slq/test_logdet_autodiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.610597 matfree-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.610597 matfree-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-09 10:18:32.000000 matfree-0.0.5/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-09 10:18:32.000000 matfree-0.0.5/.github/workflows/doc-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-09 10:18:32.000000 matfree-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-09 10:18:32.000000 matfree-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-09 10:18:32.000000 matfree-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 10:18:32.000000 matfree-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-09 10:18:32.000000 matfree-0.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-09 10:18:46.618598 matfree-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-09 10:18:32.000000 matfree-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.610597 matfree-0.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.614597 matfree-0.0.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/api/decomp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/api/hutch.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/api/montecarlo.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/api/slq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.614597 matfree-0.0.5/docs/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/benchmarks/control_variates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/benchmarks/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/benchmarks/jacobian_squared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.614597 matfree-0.0.5/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/dev/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.614597 matfree-0.0.5/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-09 10:18:32.000000 matfree-0.0.5/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.614597 matfree-0.0.5/matfree/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-09 10:18:46.000000 matfree-0.0.5/matfree/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/matfree/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/np.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/plt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/prng.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/backend/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/benchmark_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/hutch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/slq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-09 10:18:32.000000 matfree-0.0.5/matfree/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.614597 matfree-0.0.5/matfree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-09 10:18:46.000000 matfree-0.0.5/matfree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-09 10:18:46.000000 matfree-0.0.5/matfree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:18:46.000000 matfree-0.0.5/matfree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-09 10:18:46.000000 matfree-0.0.5/matfree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 10:18:46.000000 matfree-0.0.5/matfree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-09 10:18:32.000000 matfree-0.0.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-09 10:18:32.000000 matfree-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-09 10:18:46.622598 matfree-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 10:18:32.000000 matfree-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/tests/test_decomp/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_decomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_decomp/test_gkl_full_reortho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_decomp/test_lanczos_full_reortho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_decomp/test_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/tests/test_hutch/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_hutch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_hutch/test_diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_hutch/test_frobeniusnorm_squared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_hutch/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_hutch/test_trace_and_diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_hutch/test_trace_with_variance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/tests/test_montecarlo/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_montecarlo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_montecarlo/test_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_montecarlo/test_multiestimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_montecarlo/test_van_der_corput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:18:46.618598 matfree-0.0.5/tests/test_slq/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_slq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_slq/test_logdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-09 10:18:32.000000 matfree-0.0.5/tests/test_slq/test_logdet_autodiff.py
```

### Comparing `matfree-0.0.4/.github/workflows/ci.yaml` & `matfree-0.0.5/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/.github/workflows/doc-publish.yml` & `matfree-0.0.5/.github/workflows/doc-publish.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/.github/workflows/release.yml` & `matfree-0.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/.gitignore` & `matfree-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/.pre-commit-config.yaml` & `matfree-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/LICENSE` & `matfree-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/PKG-INFO` & `matfree-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matfree
-Version: 0.0.4
+Version: 0.0.5
 Summary: Matrix-free numerical linear algebra including trace-estimation.
 Author: Nicholas Krämer
 Author-email: pekra@dtu.dk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cpu
```

### Comparing `matfree-0.0.4/README.md` & `matfree-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/docs/benchmarks/control_variates.py` & `matfree-0.0.5/docs/benchmarks/control_variates.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/docs/benchmarks/jacobian_squared.py` & `matfree-0.0.5/docs/benchmarks/jacobian_squared.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     errors, stds, times = [], [], []
     for n in outer_loop:
         fun_bind = func.partial(fun, int(n))
         err, tim = evaluate(fun_bind, inner_loop)
 
         errors.append(np.mean(err))
         stds.append(np.std(err))
-        times.append(np.amin(tim))
+        times.append(np.array_min(tim))
 
     return np.asarray(errors), np.asarray(stds), np.asarray(times)
 
 
 def evaluate(fun, keys):
     """Evaluate all metrics of a function."""
     errors, times = zip(*[fun(key) for key in keys])
```

### Comparing `matfree-0.0.4/docs/index.md` & `matfree-0.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/matfree/backend/control_flow.py` & `matfree-0.0.5/matfree/backend/control_flow.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     return jax.lax.fori_loop(lower, upper, body_fun, init_val)
 
 
 def while_loop(cond_fun, body_fun, init_val):
     return jax.lax.while_loop(cond_fun, body_fun, init_val)
 
 
-def map(fun, /, xs):  # noqa: A001
+def array_map(fun, /, xs):
     return jax.lax.map(fun, xs)
```

### Comparing `matfree-0.0.4/matfree/backend/func.py` & `matfree-0.0.5/matfree/backend/func.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/matfree/backend/linalg.py` & `matfree-0.0.5/matfree/backend/linalg.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/matfree/backend/np.py` & `matfree-0.0.5/matfree/backend/np.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 # But deviate in a few points:
 # * The functions here do not have all the arguments specified in the API
 #   (we only wrap the arguments we need)
 # * Our current version of diag/diagonal is slightly different
 # * We do not use methods on Array types, e.g. shape(), dtype(). Instead
 #   these are functions. (Not all backends might always follow this method interface.)
 # * We do not implement any constants (e.g. NaN, Pi). Instead, these are methods.
-
+# * We call max/min/amax/amin array_max and elementwise_max.
+#   This is more verbose than what the array API suggests.
 
 import jax.numpy as jnp
 
 # Creation functions:
 
 
 def arange(start, /, stop=None, step=1):
@@ -95,20 +96,23 @@
     return jnp.std(x, axis)
 
 
 def sum(x, /, axis=None):  # noqa: A001
     return jnp.sum(x, axis)
 
 
-# todo: change amax and maximum to array_max, elementwise_max
-def amin(x, /):
+def array_min(x, /):
     return jnp.amin(x)
 
 
-def maximum(x1, x2):  # todo: call this max()
+def array_max(x, /, axis=None):
+    return jnp.amax(x, axis=axis)
+
+
+def elementwise_max(x1, x2, /):
     return jnp.maximum(x1, x2)
 
 
 def nanmean(x, /, axis=None):
     return jnp.nanmean(x, axis)
```

### Comparing `matfree-0.0.4/matfree/backend/prng.py` & `matfree-0.0.5/matfree/backend/prng.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/matfree/benchmark_util.py` & `matfree-0.0.5/matfree/benchmark_util.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/matfree/decomp.py` & `matfree-0.0.5/matfree/decomp.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from matfree.backend import containers, control_flow, func, linalg, np
 from matfree.backend.typing import Any, Array, Callable, Tuple
 
 
 def svd(v0: Array, depth: int, Av: Callable, vA: Callable, matrix_shape: Tuple[int]):
     """Approximate singular value decomposition.
 
+    Uses GKL with full reorthogonalisation to bi-diagonalise the target matrix
+    and computes the full SVD of the (small) bidiagonal matrix.
+
     Parameters
     ----------
     v0:
         Initial vector for Golub-Kahan-Lanczos bidiagonalisation.
     depth:
         Depth of the Krylov space constructed by Golub-Kahan-Lanczos bidiagonalisation.
         Choosing `depth = min(nrows, ncols) - 1` would yield behaviour similar to
@@ -19,15 +22,15 @@
         Matrix-vector product function.
     vA:
         Vector-matrix product function.
     matrix_shape:
         Shape of the matrix involved in matrix-vector and vector-matrix products.
     """
     # Factorise the matrix
-    alg = golub_kahan_lanczos_bidiagonal(depth, matrix_shape=matrix_shape)
+    alg = gkl_full_reortho(depth, matrix_shape=matrix_shape)
     u, (d, e), vt, _ = decompose_fori_loop(0, depth + 1, v0, Av, vA, alg=alg)
 
     # Compute SVD of factorisation
     B = _bidiagonal_dense(d, e)
     U, S, Vt = linalg.svd(B, full_matrices=False)
 
     # Combine orthogonal transformations
@@ -75,56 +78,54 @@
     def body_fun(_, s):
         return alg.step(s, *matvec_funs)
 
     result = control_flow.fori_loop(lower, upper, body_fun=body_fun, init_val=init_val)
     return alg.extract(result)
 
 
-def lanczos_tridiagonal(depth, /) -> DecompAlg:
-    """**Lanczos** algorithm with pre-allocation and re-orthogonalisation.
+def lanczos_full_reortho(depth, /) -> DecompAlg:
+    """**Lanczos** algorithm with pre-allocation & full reorthogonalisation.
 
     Decompose a matrix into a product of orthogonal-**tridiagonal**-orthogonal matrices.
     Use this algorithm for approximate **eigenvalue** decompositions.
 
     Lanczos' algorithm assumes a symmetric matrix.
     """
     # this algorithm is massively unstable.
     # but despite this instability, quadrature might be stable?
     # https://www.sciencedirect.com/science/article/abs/pii/S0920563200918164
     return DecompAlg(
-        init=func.partial(_lanczos_tridiagonal_init, depth),
-        step=_lanczos_tridiagonal_apply,
-        extract=_lanczos_tridiagonal_extract,
+        init=func.partial(_lanczos_full_reortho_init, depth),
+        step=_lanczos_full_reortho_apply,
+        extract=_lanczos_full_reortho_extract,
     )
 
 
 class _LanczosState(containers.NamedTuple):
     i: int
     basis: Any
     tridiag: Any
     q: Any
 
 
-def _lanczos_tridiagonal_init(depth: int, init_vec: Array) -> _LanczosState:
+def _lanczos_full_reortho_init(depth: int, init_vec: Array) -> _LanczosState:
     (ncols,) = np.shape(init_vec)
     if depth >= ncols or depth < 1:
         raise ValueError
 
     diag = np.zeros((depth + 1,))
     offdiag = np.zeros((depth,))
     basis = np.zeros((depth + 1, ncols))
 
     return _LanczosState(0, basis, (diag, offdiag), init_vec)
 
 
-def _lanczos_tridiagonal_apply(state: _LanczosState, Av: Callable) -> _LanczosState:
+def _lanczos_full_reortho_apply(state: _LanczosState, Av: Callable) -> _LanczosState:
     i, basis, (diag, offdiag), vec = state
 
-    # This one is a hack:
-    #
     # Re-orthogonalise against ALL basis elements before storing.
     # Note: we re-orthogonalise against ALL columns of Q, not just
     # the ones we have already computed. This increases the complexity
     # of the whole iteration from n(n+1)/2 to n^2, but has the advantage
     # that the whole computation has static bounds (thus we can JIT it all).
     # Since 'Q' is padded with zeros, the numerical values are identical
     # between both modes of computing.
@@ -142,73 +143,73 @@
     vec, (coeff, _) = _gram_schmidt_orthogonalise_set(vec, basis_vectors_previous)
     diag = diag.at[i].set(coeff)
     offdiag = offdiag.at[i - 1].set(length)
 
     return _LanczosState(i + 1, basis, (diag, offdiag), vec)
 
 
-def _lanczos_tridiagonal_extract(state: _LanczosState, /):
+def _lanczos_full_reortho_extract(state: _LanczosState, /):
     _, basis, (diag, offdiag), _ = state
     return basis, (diag, offdiag)
 
 
-def golub_kahan_lanczos_bidiagonal(depth, /, matrix_shape) -> DecompAlg:
-    """**Golub-Kahan-Lanczos** algorithm with pre-allocation and re-orthogonalisation.
+def gkl_full_reortho(depth, /, matrix_shape) -> DecompAlg:
+    """**Golub-Kahan-Lanczos** algorithm with pre-allocation & full reorthogonalisation.
 
     Decompose a matrix into a product of orthogonal-**bidiagonal**-orthogonal matrices.
     Use this algorithm for approximate **singular value** decompositions.
     """
     return DecompAlg(
-        init=func.partial(_gkl_bidiagonal_init, depth, matrix_shape),
-        step=_gkl_bidiagonal_apply,
-        extract=_gkl_bidiagonal_extract,
+        init=func.partial(_gkl_full_reortho_init, depth, matrix_shape),
+        step=_gkl_full_reortho_apply,
+        extract=_gkl_full_reortho_extract,
     )
 
 
 class _GKLState(containers.NamedTuple):
     i: int
     Us: Any
     Vs: Any
     alphas: Any
     betas: Any
     beta: Any
     vk: Any
 
 
-def _gkl_bidiagonal_init(depth: int, matrix_shape, init_vec: Array) -> _GKLState:
+def _gkl_full_reortho_init(depth: int, matrix_shape, init_vec: Array) -> _GKLState:
     nrows, ncols = matrix_shape
     alphas = np.zeros((depth + 1,))
     betas = np.zeros((depth + 1,))
     Us = np.zeros((depth + 1, nrows))
     Vs = np.zeros((depth + 1, ncols))
     v0, _ = _normalise(init_vec)
     return _GKLState(0, Us, Vs, alphas, betas, 0.0, v0)
 
 
-def _gkl_bidiagonal_apply(state: _GKLState, Av: Callable, vA: Callable) -> _GKLState:
+def _gkl_full_reortho_apply(state: _GKLState, Av: Callable, vA: Callable) -> _GKLState:
     i, Us, Vs, alphas, betas, beta, vk = state
     Vs = Vs.at[i].set(vk)
     betas = betas.at[i].set(beta)
 
     uk = Av(vk) - beta * Us[i - 1]
     uk, alpha = _normalise(uk)
-    uk, _ = _gram_schmidt_orthogonalise_set(uk, Us)  # hack
-    uk, _ = _normalise(uk)  # hack
+    uk, _ = _gram_schmidt_orthogonalise_set(uk, Us)  # full reorthogonalisation
+    uk, _ = _normalise(uk)
     Us = Us.at[i].set(uk)
     alphas = alphas.at[i].set(alpha)
 
     vk = vA(uk) - alpha * vk
     vk, beta = _normalise(vk)
-    vk, _ = _gram_schmidt_orthogonalise_set(vk, Vs)  # hack
-    vk, _ = _normalise(vk)  # hack
+    vk, _ = _gram_schmidt_orthogonalise_set(vk, Vs)  # full reorthogonalisation
+    vk, _ = _normalise(vk)
 
     return _GKLState(i + 1, Us, Vs, alphas, betas, beta, vk)
 
 
-def _gkl_bidiagonal_extract(state: _GKLState, /):
+def _gkl_full_reortho_extract(state: _GKLState, /):
     _, uk_all, vk_all, alphas, betas, beta, vk = state
     return uk_all.T, (alphas, betas[1:]), vk_all, (beta, vk)
 
 
 def _normalise(vec):
     length = linalg.vector_norm(vec)
     return vec / length, length
```

### Comparing `matfree-0.0.4/matfree/hutch.py` & `matfree-0.0.5/matfree/hutch.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,41 @@
 
     def quadform(vec):
         return linalg.vecdot(vec, Av(vec))
 
     return montecarlo.estimate(quadform, **kwargs)
 
 
+def trace_with_variance(Av: Callable, /, **kwargs) -> Array:
+    """Estimate the trace of a matrix and the variance of the estimator.
+
+    Parameters
+    ----------
+    Av:
+        Matrix-vector product function.
+    **kwargs:
+        Keyword-arguments to be passed to
+        [montecarlo.estimate()][matfree.montecarlo.estimate].
+    """
+
+    def quadform(vec):
+        return linalg.vecdot(vec, Av(vec))
+
+    def mean_squared_fun(x, axis):
+        return np.mean(x**2, axis=axis)
+
+    mean, second_moment = montecarlo.multiestimate(
+        quadform,
+        statistics_batch=[np.mean, mean_squared_fun],
+        statistics_combine=[np.mean, np.mean],
+        **kwargs,
+    )
+    return mean, second_moment - mean**2
+
+
 def frobeniusnorm_squared(Av: Callable, /, **kwargs) -> Array:
     r"""Estimate the squared Frobenius norm of a matrix stochastically.
 
     The Frobenius norm of a matrix $A$ is defined as
 
     $$
     \|A\|_F^2 = \text{trace}(A^\top A)
```

### Comparing `matfree-0.0.4/matfree/slq.py` & `matfree-0.0.5/matfree/slq.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     return montecarlo.estimate(quadratic_form, **kwargs)
 
 
 def quadratic_form_slq_symmetric(matfun, Av, order, /):
     """Approximate quadratic form for stochastic Lanczos quadrature."""
 
     def quadform(v0, /):
-        algorithm = decomp.lanczos_tridiagonal(order)
+        algorithm = decomp.lanczos_full_reortho(order)
         _, tridiag = decomp.decompose_fori_loop(0, order + 1, v0, Av, alg=algorithm)
         (diag, off_diag) = tridiag
 
         # todo: once jax supports eigh_tridiagonal(eigvals_only=False),
         #  use it here. Until then: an eigen-decomposition of size (order + 1)
         #  does not hurt too much...
         diag = linalg.diagonal_matrix(diag)
```

### Comparing `matfree-0.0.4/matfree/test_util.py` & `matfree-0.0.5/matfree/test_util.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/matfree.egg-info/PKG-INFO` & `matfree-0.0.5/matfree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matfree
-Version: 0.0.4
+Version: 0.0.5
 Summary: Matrix-free numerical linear algebra including trace-estimation.
 Author: Nicholas Krämer
 Author-email: pekra@dtu.dk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cpu
```

### Comparing `matfree-0.0.4/matfree.egg-info/SOURCES.txt` & `matfree-0.0.5/matfree.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -43,21 +43,23 @@
 matfree/backend/prng.py
 matfree/backend/progressbar.py
 matfree/backend/testing.py
 matfree/backend/time.py
 matfree/backend/typing.py
 tests/__init__.py
 tests/test_decomp/__init__.py
-tests/test_decomp/test_gkl_bidiagonal.py
-tests/test_decomp/test_lanczos_tridiagonal.py
+tests/test_decomp/test_gkl_full_reortho.py
+tests/test_decomp/test_lanczos_full_reortho.py
 tests/test_decomp/test_svd.py
 tests/test_hutch/__init__.py
 tests/test_hutch/test_diagonal.py
 tests/test_hutch/test_frobeniusnorm_squared.py
 tests/test_hutch/test_trace.py
 tests/test_hutch/test_trace_and_diagonal.py
+tests/test_hutch/test_trace_with_variance.py
 tests/test_montecarlo/__init__.py
 tests/test_montecarlo/test_estimate.py
+tests/test_montecarlo/test_multiestimate.py
 tests/test_montecarlo/test_van_der_corput.py
 tests/test_slq/__init__.py
 tests/test_slq/test_logdet.py
 tests/test_slq/test_logdet_autodiff.py
```

### Comparing `matfree-0.0.4/mkdocs.yml` & `matfree-0.0.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/pyproject.toml` & `matfree-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/setup.cfg` & `matfree-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/tests/test_decomp/test_gkl_bidiagonal.py` & `matfree-0.0.5/tests/test_decomp/test_gkl_full_reortho.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,20 @@
     return test_util.asymmetric_matrix_from_singular_values(d, nrows=nrows, ncols=ncols)
 
 
 @testing.parametrize("nrows", [50])
 @testing.parametrize("ncols", [49])
 @testing.parametrize("num_significant_singular_vals", [4])
 @testing.parametrize("order", [6])  # ~1.5 * num_significant_eigvals
-def test_golub_kahan_lanczos_bidiagonal(A, order):
+def test_gkl_full_reortho(A, order):
     """Test that Lanczos tridiagonalisation yields an orthogonal-tridiagonal decomp."""
     nrows, ncols = np.shape(A)
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(ncols,))
-    alg = decomp.golub_kahan_lanczos_bidiagonal(order, matrix_shape=np.shape(A))
+    alg = decomp.gkl_full_reortho(order, matrix_shape=np.shape(A))
 
     def Av(v):
         return A @ v
 
     def vA(v):
         return v @ A
```

### Comparing `matfree-0.0.4/tests/test_decomp/test_lanczos_tridiagonal.py` & `matfree-0.0.5/tests/test_decomp/test_lanczos_full_reortho.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 @testing.parametrize("num_significant_eigvals", [4])
 def test_error_for_too_high_order(A):
     """Assert graceful failure if the depth matches or exceeds the number of columns."""
     n, _ = np.shape(A)
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
     with testing.raises(ValueError):
-        alg = decomp.lanczos_tridiagonal(n + 10)
+        alg = decomp.lanczos_full_reortho(n + 10)
         _ = decomp.decompose_fori_loop(0, n + 10, v0, lambda v: A @ v, alg=alg)
     with testing.raises(ValueError):
-        alg = decomp.lanczos_tridiagonal(n)
+        alg = decomp.lanczos_full_reortho(n)
         _ = decomp.decompose_fori_loop(0, n + 1, v0, lambda v: A @ v, alg=alg)
 
 
 @testing.parametrize("n", [6])
 @testing.parametrize("num_significant_eigvals", [6])
 def test_max_order(A):
     """If m == n, the matrix should be equal to the full tridiagonal."""
     n, _ = np.shape(A)
     order = n - 1
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
-    alg = decomp.lanczos_tridiagonal(order)
+    alg = decomp.lanczos_full_reortho(order)
     Q, (d_m, e_m) = decomp.decompose_fori_loop(
         0, order + 1, v0, lambda v: A @ v, alg=alg
     )
 
     # Lanczos is not stable.
     tols_decomp = {"atol": 1e-5, "rtol": 1e-5}
 
@@ -76,15 +76,15 @@
 @testing.parametrize("num_significant_eigvals", [4])
 @testing.parametrize("order", [6])  # ~1.5 * num_significant_eigvals
 def test_identity(A, order):
     """Test that Lanczos tridiagonalisation yields an orthogonal-tridiagonal decomp."""
     n, _ = np.shape(A)
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
-    alg = decomp.lanczos_tridiagonal(order)
+    alg = decomp.lanczos_full_reortho(order)
     Q, tridiag = decomp.decompose_fori_loop(0, order + 1, v0, lambda v: A @ v, alg=alg)
     (d_m, e_m) = tridiag
 
     # Lanczos is not stable.
     tols_decomp = {"atol": 1e-5, "rtol": 1e-5}
 
     assert np.shape(Q) == (order + 1, n)
```

### Comparing `matfree-0.0.4/tests/test_decomp/test_svd.py` & `matfree-0.0.5/tests/test_decomp/test_svd.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/tests/test_hutch/test_diagonal.py` & `matfree-0.0.5/tests/test_hutch/test_diagonal.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/tests/test_hutch/test_frobeniusnorm_squared.py` & `matfree-0.0.5/tests/test_hutch/test_frobeniusnorm_squared.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/tests/test_hutch/test_trace.py` & `matfree-0.0.5/tests/test_hutch/test_trace.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/tests/test_hutch/test_trace_and_diagonal.py` & `matfree-0.0.5/tests/test_hutch/test_trace_and_diagonal.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/tests/test_montecarlo/test_estimate.py` & `matfree-0.0.5/tests/test_montecarlo/test_estimate.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/tests/test_montecarlo/test_van_der_corput.py` & `matfree-0.0.5/tests/test_montecarlo/test_van_der_corput.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/tests/test_slq/test_logdet.py` & `matfree-0.0.5/tests/test_slq/test_logdet.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.4/tests/test_slq/test_logdet_autodiff.py` & `matfree-0.0.5/tests/test_slq/test_logdet_autodiff.py`

 * *Files identical despite different names*

