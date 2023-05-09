# Comparing `tmp/vis_cpu-1.0.1.tar.gz` & `tmp/vis_cpu-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vis_cpu-1.0.1.tar", last modified: Tue Aug 16 19:20:09 2022, max compression
+gzip compressed data, was "vis_cpu-1.1.0.tar", last modified: Tue May  9 17:29:06 2023, max compression
```

## Comparing `vis_cpu-1.0.1.tar` & `vis_cpu-1.1.0.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.338262 vis_cpu-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)      644 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.318262 vis_cpu-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.322262 vis_cpu-1.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)      462 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (116)      632 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (116)      299 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.github/ISSUE_TEMPLATE/question.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.322262 vis_cpu-1.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)      827 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.github/PULL_REQUEST_TEMPLATE/feature.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.322262 vis_cpu-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2038 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1808 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.github/workflows/run_notebooks.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     2142 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.github/workflows/test_suite.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     2400 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.github/workflows/test_suite_gpu.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      599 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      289 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1219 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      392 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)      125 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4477 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1076 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2105 2022-08-16 19:20:09.338262 vis_cpu-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.326262 vis_cpu-1.0.1/ci/
--rw-r--r--   0 runner    (1001) docker     (116)      430 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/ci/notebook-env.yml
--rw-r--r--   0 runner    (1001) docker     (116)      428 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/ci/test-env.yml
--rw-r--r--   0 runner    (1001) docker     (116)       42 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.326262 vis_cpu-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     5592 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.326262 vis_cpu-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)       18 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      468 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       41 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (116)       43 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (116)     9130 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      136 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1343 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       67 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.326262 vis_cpu-1.0.1/docs/templates/
--rw-r--r--   0 runner    (1001) docker     (116)      611 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/templates/custom-class.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1229 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/templates/custom-module.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.326262 vis_cpu-1.0.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (116)   152252 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/tutorials/vis_cpu_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)      180 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (116)     7806 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/docs/understanding_the_algorithm.rst
--rw-r--r--   0 runner    (1001) docker     (116)      146 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1776 2022-08-16 19:20:09.338262 vis_cpu-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       63 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.318262 vis_cpu-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.330262 vis_cpu-1.0.1/src/vis_cpu/
--rw-r--r--   0 runner    (1001) docker     (116)      699 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/src/vis_cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       57 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/src/vis_cpu/_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     7392 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/src/vis_cpu/_uvbeam_to_raw.py
--rw-r--r--   0 runner    (1001) docker     (116)    10814 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/src/vis_cpu/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    11641 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/src/vis_cpu/conversions.py
--rw-r--r--   0 runner    (1001) docker     (116)    12031 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/src/vis_cpu/cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.330262 vis_cpu-1.0.1/src/vis_cpu/data/
--rw-r--r--   0 runner    (1001) docker     (116)  2635200 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/src/vis_cpu/data/NF_HERA_Dipole_small.fits
--rw-r--r--   0 runner    (1001) docker     (116)    21027 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/src/vis_cpu/gpu.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.334262 vis_cpu-1.0.1/src/vis_cpu/gpu_src/
--rw-r--r--   0 runner    (1001) docker     (116)     5326 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/src/vis_cpu/gpu_src/beam_interpolation.cu
--rw-r--r--   0 runner    (1001) docker     (116)     4128 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/src/vis_cpu/gpu_src/measurement_equation.cu
--rw-r--r--   0 runner    (1001) docker     (116)     4419 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/src/vis_cpu/plot.py
--rw-r--r--   0 runner    (1001) docker     (116)     4960 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/src/vis_cpu/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.330262 vis_cpu-1.0.1/src/vis_cpu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2105 2022-08-16 19:20:09.000000 vis_cpu-1.0.1/src/vis_cpu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1629 2022-08-16 19:20:09.000000 vis_cpu-1.0.1/src/vis_cpu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-16 19:20:09.000000 vis_cpu-1.0.1/src/vis_cpu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       44 2022-08-16 19:20:09.000000 vis_cpu-1.0.1/src/vis_cpu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-16 19:20:08.000000 vis_cpu-1.0.1/src/vis_cpu.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      272 2022-08-16 19:20:09.000000 vis_cpu-1.0.1/src/vis_cpu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2022-08-16 19:20:09.000000 vis_cpu-1.0.1/src/vis_cpu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-16 19:20:09.338262 vis_cpu-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     5293 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      578 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     6181 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/tests/test_beam_interp_gpu.py
--rw-r--r--   0 runner    (1001) docker     (116)    14690 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/tests/test_beams.py
--rw-r--r--   0 runner    (1001) docker     (116)     3771 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/tests/test_compare_pyuvsim.py
--rw-r--r--   0 runner    (1001) docker     (116)     7915 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2317 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/tests/test_cpu_vs_gpu.py
--rw-r--r--   0 runner    (1001) docker     (116)     1748 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (116)     1338 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/tests/test_vis_cpu.py
--rw-r--r--   0 runner    (1001) docker     (116)     5122 2022-08-16 19:19:51.000000 vis_cpu-1.0.1/tests/test_vis_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.244417 vis_cpu-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.232417 vis_cpu-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.236417 vis_cpu-1.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/.github/ISSUE_TEMPLATE/question.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.236417 vis_cpu-1.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/.github/PULL_REQUEST_TEMPLATE/feature.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.236417 vis_cpu-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/.github/workflows/run_notebooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/.github/workflows/test_suite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-09 17:29:06.244417 vis_cpu-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.236417 vis_cpu-1.1.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/ci/notebook-env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/ci/test-env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.240417 vis_cpu-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.240417 vis_cpu-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.240417 vis_cpu-1.1.0/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/templates/custom-class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/templates/custom-module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.240417 vis_cpu-1.1.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   152252 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/tutorials/vis_cpu_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/docs/understanding_the_algorithm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   425984 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/gpu-analysis.nvprof
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-09 17:29:06.244417 vis_cpu-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.232417 vis_cpu-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.240417 vis_cpu-1.1.0/src/vis_cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/src/vis_cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/src/vis_cpu/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/src/vis_cpu/_uvbeam_to_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/src/vis_cpu/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/src/vis_cpu/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/src/vis_cpu/cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.240417 vis_cpu-1.1.0/src/vis_cpu/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2635200 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/src/vis_cpu/data/NF_HERA_Dipole_small.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/src/vis_cpu/gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.244417 vis_cpu-1.1.0/src/vis_cpu/gpu_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/src/vis_cpu/gpu_src/beam_interpolation.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/src/vis_cpu/gpu_src/measurement_equation.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/src/vis_cpu/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/src/vis_cpu/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.240417 vis_cpu-1.1.0/src/vis_cpu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-09 17:29:06.000000 vis_cpu-1.1.0/src/vis_cpu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-09 17:29:06.000000 vis_cpu-1.1.0/src/vis_cpu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:29:06.000000 vis_cpu-1.1.0/src/vis_cpu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 17:29:06.000000 vis_cpu-1.1.0/src/vis_cpu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:29:05.000000 vis_cpu-1.1.0/src/vis_cpu.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-09 17:29:06.000000 vis_cpu-1.1.0/src/vis_cpu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 17:29:06.000000 vis_cpu-1.1.0/src/vis_cpu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:29:06.244417 vis_cpu-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/tests/test_beam_interp_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/tests/test_beams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/tests/test_compare_pyuvsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/tests/test_cpu_vs_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/tests/test_gpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/tests/test_vis_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-05-09 17:28:52.000000 vis_cpu-1.1.0/tests/test_vis_gpu.py
```

### Comparing `vis_cpu-1.0.1/.coveragerc` & `vis_cpu-1.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `vis_cpu-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/.github/PULL_REQUEST_TEMPLATE/feature.md` & `vis_cpu-1.1.0/.github/PULL_REQUEST_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/.github/workflows/publish-to-pypi.yaml` & `vis_cpu-1.1.0/.github/workflows/publish-to-pypi.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: Deploy to PyPI
 
 on: push
 
 jobs:
   build-n-publish:
     name: Deploy
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@master
       # https://github.com/ansible/pylibssh/blob/1e7b17f/.github/workflows/build-test-n-publish.yml#L146-L151
       - name: Get history and tags for SCM versioning to work
         run: |
           git fetch --prune --unshallow
           git fetch --depth=1 origin +refs/tags/*:refs/tags/*
@@ -19,15 +19,14 @@
         uses: actions/setup-python@v1
         with:
           python-version: 3.9
       - name: Install pep517
         run: |
           python -m pip install build
           python -m pip install setuptools_scm setuptools>42
-          python setup.py --version
       - name: Create setuptools_scm env variable
         if: startsWith(github.ref, 'refs/tags/') != true
         shell: bash
         run: |
           wget https://gist.github.com/plaplant/0902f09e59166bac742bbd554f3cd2f9/raw/make_dev_version.sh -O ../make_dev_version.sh
           version=$(bash ../make_dev_version.sh)
           echo "SETUPTOOLS_SCM_PRETEND_VERSION=$version" >> $GITHUB_ENV
```

### Comparing `vis_cpu-1.0.1/.github/workflows/run_notebooks.yaml` & `vis_cpu-1.1.0/.github/workflows/run_notebooks.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -11,54 +11,59 @@
     branches:
       - 'main'
 
 jobs:
   notebooks:
     name: Running Docs Notebooks
     runs-on: ubuntu-latest
-    defaults:
-     run:
-       # Adding -l {0} ensures conda can be found properly in each step
-       shell: bash -l {0}
+    # defaults:
+    #  run:
+    #    # Adding -l {0} ensures conda can be found properly in each step
+    #    shell: bash -l {0}
     steps:
       - uses: actions/checkout@main
         with:
           fetch-depth: 1
-
-      - name: Cache conda
-        uses: actions/cache@v2
-        env:
-          # Increase this value to reset cache if ci/test-env.yml has not changed
-          CACHE_NUMBER: 0
-        with:
-          path: ~/conda_pkgs_dir
-          key:
-            ${{ runner.os }}-conda-${{ env.CACHE_NUMBER }}-${{ matrix.python-version }}-${{ hashFiles('ci/test-env.yml', 'setup.cfg') }}
-
-      - name: Setup Miniconda
-        uses: conda-incubator/setup-miniconda@v2.1.1
+      - uses: mpi4py/setup-mpi@v1
+      - name: Setup Python
+        uses: actions/setup-python@v4
         with:
-          # auto-update-conda: true
-          miniconda-version: "latest"
-          python-version: '3.10'
-          environment-file: ci/notebook-env.yml
-          activate-environment: viscpu
-          channels: conda-forge,defaults
-          channel-priority: strict
-          use-only-tar-bz2: true
+          python-version: ${{ matrix.python-version }}
 
-      - name: Conda Info
-        run: |
-          conda info -a
-          conda list
+      # - name: Cache conda
+      #   uses: actions/cache@v2
+      #   env:
+      #     # Increase this value to reset cache if ci/test-env.yml has not changed
+      #     CACHE_NUMBER: 0
+      #   with:
+      #     path: ~/conda_pkgs_dir
+      #     key:
+      #       ${{ runner.os }}-conda-${{ env.CACHE_NUMBER }}-${{ matrix.python-version }}-${{ hashFiles('ci/test-env.yml', 'setup.cfg') }}
+
+      # - name: Setup Miniconda
+      #   uses: conda-incubator/setup-miniconda@v2.1.1
+      #   with:
+      #     # auto-update-conda: true
+      #     miniconda-version: "latest"
+      #     python-version: '3.10'
+      #     environment-file: ci/notebook-env.yml
+      #     activate-environment: viscpu
+      #     channels: conda-forge,defaults
+      #     channel-priority: strict
+      #     use-only-tar-bz2: true
+
+      # - name: Conda Info
+      #   run: |
+      #     conda info -a
+      #     conda list
 
       - name: Install
         run: |
           echo $(which pip)
-          pip install .[test]
+          pip install .[test] papermill jupyter ipykernel
 
       - name: Install ipykernel
         run: python -m ipykernel install --user --name viscpu --display-name "viscpu"
 
       - name: Run Notebooks
         run: |
           papermill -k viscpu docs/tutorials/vis_cpu_tutorial.ipynb tmp.ipynb
```

### Comparing `vis_cpu-1.0.1/.gitignore` & `vis_cpu-1.1.0/.gitignore`

 * *Files 20% similar despite different names*

```diff
@@ -49,7 +49,8 @@
 
 # Per-project virtualenvs
 .venv*/
 .vscode/
 full-stats-*.txt
 stats-*.pkl
 summary-stats-*.pkl
+.hypothesis/*
```

### Comparing `vis_cpu-1.0.1/.pre-commit-config.yaml` & `vis_cpu-1.1.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 exclude: '^docs/conf.py|^src/vis_cpu/data/'
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.3.0
+  rev: v4.4.0
   hooks:
   - id: trailing-whitespace
   - id: check-added-large-files
   - id: check-ast
   - id: check-json
   - id: check-merge-conflict
   - id: check-xml
@@ -14,46 +14,46 @@
   - id: debug-statements
   - id: end-of-file-fixer
   - id: requirements-txt-fixer
   - id: mixed-line-ending
     args: ['--fix=no']
 
 - repo: https://github.com/PyCQA/flake8
-  rev: 4.0.1
+  rev: 6.0.0
   hooks:
   - id: flake8
     additional_dependencies:
       - flake8-docstrings
       - flake8-builtins
       - flake8-logging-format
       - flake8-rst-docstrings
       - flake8-rst
       - flake8-markdown
       - flake8-bugbear
       - flake8-comprehensions
       - flake8-print
 
 - repo: https://github.com/psf/black
-  rev: 22.6.0
+  rev: 23.3.0
   hooks:
   - id: black
 
 - repo: https://github.com/pre-commit/pygrep-hooks
-  rev: v1.9.0
+  rev: v1.10.0
   hooks:
     - id: rst-backticks
 
 - repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v2.37.1
+  rev: v3.4.0
   hooks:
   - id: pyupgrade
-    args: [--py38-plus]
+    args: [--py39-plus]
 
 - repo: https://github.com/asottile/setup-cfg-fmt
-  rev: v1.20.2
+  rev: v2.2.0
   hooks:
   - id: setup-cfg-fmt
```

### Comparing `vis_cpu-1.0.1/CHANGELOG.rst` & `vis_cpu-1.1.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =========
 Changelog
 =========
 
+Dev
+===
+
+Fixed
+-----
+
+- Better handling of errors when GPUs are present but currently unavailable for some
+  reason.
+
 Version 1.0.1
 =============
 
 Fixed
 -----
 
 - When getting the raw beam data for GPU, there was a check for whether the beam covers
```

### Comparing `vis_cpu-1.0.1/LICENSE.txt` & `vis_cpu-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/PKG-INFO` & `vis_cpu-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: vis_cpu
-Version: 1.0.1
+Version: 1.1.0
 Summary: Fast visibility simulator with interface to CPU and GPU
 Home-page: https://github.com/hera-team/vis_cpu
 Author: HERA-Team
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+Provides-Extra: all
+Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: gpu
 Provides-Extra: profile
 Provides-Extra: test
 License-File: LICENSE.txt
 
 =======
```

### Comparing `vis_cpu-1.0.1/README.rst` & `vis_cpu-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/docs/Makefile` & `vis_cpu-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/docs/conf.py` & `vis_cpu-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/docs/index.rst` & `vis_cpu-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/docs/templates/custom-class.rst` & `vis_cpu-1.1.0/docs/templates/custom-class.rst`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/docs/templates/custom-module.rst` & `vis_cpu-1.1.0/docs/templates/custom-module.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {{ fullname | escape | underline}}
 
 .. automodule:: {{ fullname }}
    :exclude-members: profile
+
    {% block attributes %}
    {% if attributes %}
    .. rubric:: {{ _('Module Attributes') }}
 
    .. autosummary::
       :toctree:
    {% for item in attributes %}
```

### Comparing `vis_cpu-1.0.1/docs/tutorials/vis_cpu_tutorial.ipynb` & `vis_cpu-1.1.0/docs/tutorials/vis_cpu_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/docs/understanding_the_algorithm.rst` & `vis_cpu-1.1.0/docs/understanding_the_algorithm.rst`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/setup.cfg` & `vis_cpu-1.1.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -9,23 +9,26 @@
 license = MIT
 license_file = LICENSE.txt
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
+	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 install_requires = 
 	astropy
 	numpy
+	psutil
 	pyuvdata>=2.2.8
 	scipy
-	typing-extensions;python_version<'3.8'
+python_requires = >=3.9
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
@@ -33,34 +36,40 @@
 	tests
 
 [options.entry_points]
 console_scripts = 
 	viscpu = vis_cpu.cli:main
 
 [options.extras_require]
+all = 
+	vis-cpu[gpu,profile,dev]
+dev = 
+	vis-cpu[docs,test]
 docs = 
+	furo
+	ipython
 	nbsphinx
 	numpydoc
 	sphinx
-	sphinx-rtd-theme
 gpu = 
 	jinja2
 	pycuda
 	scikit-cuda
 profile = 
 	click
 	line-profiler
-	pyuvsim
+	pyuvsim>=1.2.5
 test = 
+	hypothesis
 	ipython
 	matplotlib
 	pyradiosky
 	pytest
 	pytest-cov
-	pyuvsim[sim]
+	pyuvsim[sim]>=1.2.5
 
 [test]
 extras = True
 
 [tool:pytest]
 addopts = 
 	--cov vis_cpu --cov-report term-missing
@@ -93,17 +102,19 @@
 	W503
 	F403
 	F401
 	E231
 	C901
 	D401
 	B007
+	G004
 per-file-ignores = 
 	src/vis_cpu/cli.py: T201,T001
 	tests/*.py: T201,T001,E402
+	setup.py: D100
 max-line-length = 88
 max-complexity = 25
 rst-roles = 
 	class
 	func
 	mod
 	data
```

### Comparing `vis_cpu-1.0.1/src/vis_cpu/__init__.py` & `vis_cpu-1.1.0/src/vis_cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/src/vis_cpu/_uvbeam_to_raw.py` & `vis_cpu-1.1.0/src/vis_cpu/_uvbeam_to_raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,38 +123,42 @@
     )
 
     if not covers_sky_weak:
         raise ValueError(
             "The beam data does not cover the full sky. Cannot use in vis_cpu."
         )
 
+    if not uvbeam.future_array_shapes:
+        uvbeam.use_future_array_shapes()
+
     # Simplest Case: everything is already in the regular format we need.
     if (
         naz == len(az)
         and np.isclose(dza, delta_za)
         and is_regular_grid
         and covers_sky_strong
     ):
         # Returned data has shape (Nax, Nfeeds, Nza, Naz)
-        return uvbeam.data_array[:, 0, :, 0], delta_az, dza
+        return uvbeam.data_array[:, :, 0], delta_az, dza
     elif (
         naz == len(az)
         and np.isclose(dza, delta_za)
         and is_regular_grid
         and covers_sky_almost_strong
     ):
-        data = uvbeam.data_array[:, 0, :, 0]
+        data = uvbeam.data_array[:, :, 0]
         data = np.concatenate((data, data[..., [0]]), axis=-1)
         return data, delta_az, dza
     else:
         warnings.warn(
             "The raw beam data is either irregular, or does not have the spacing you "
             "desire. This means we need to interpolate to a grid, from which a second "
             "round of interpolation will be performed in the visibility calculation."
-            "You might be able to avoid this by not specifying a desired naz and dza."
+            "You might be able to avoid this by not specifying a desired naz and dza.",
+            stacklevel=1,
         )
 
         # We have to treat az and za differently. For az, we need to start at 0 and end at 2pi exactly.
         # This is because it wraps, and our interpolation function needs to be regular
         # over the wrap itself. On the other hand, za just needs to extend at least to
         # the horizon, and we can't know for certain with the input beam goes to the
         # antipode or the horizon before we run the function. Therefore, providing nza
@@ -165,15 +169,15 @@
         out = uvbeam.interp(
             new_az, new_za, az_za_grid=True, check_azza_domain=False, **interp_kwargs
         )[0]
         out = out.reshape(out.shape[:-1] + (len(new_za), naz))
 
         # Returned data has shape (Nax, Nfeeds, Nza, Naz)
         if uvbeam.beam_type == "efield":
-            return out[:, 0, :, 0], new_az[1] - new_az[0], dza
+            return out[:, :, 0], new_az[1] - new_az[0], dza
         else:
             # For a power beam, we just want to the I part of the XX pol.
             # Also, need the sqrt of the beam (to make it quasi X)
-            out = out[0, 0, 0, 0]
+            out = out[0, 0, 0]
 
             # But we need to return it with the nax and nfeed dimensions (both have size 1)
             return out[np.newaxis, np.newaxis], new_az[1] - new_az[0], dza
```

### Comparing `vis_cpu-1.0.1/src/vis_cpu/cli.py` & `vis_cpu-1.1.0/src/vis_cpu/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,24 +31,24 @@
 
 
 # These specify which line(s) in the code correspond to which algorithmic step.
 VIS_CPU_STEPS = {
     "eq2top": ("np.dot(eq2top",),
     "beam_interp": ("_evaluate_beam_cpu(",),
     "get_tau": ("np.dot(antpos",),
-    "get_antenna_vis": ("v = get_antenna_vis(",),
+    "get_antenna_vis": ("v = _get_antenna_vis(",),
     "get_baseline_vis": ("vis[t] =",),
 }
 
 VIS_GPU_STEPS = {
     "eq2top": ("# compute crdtop",),
     "beam_interp": ("do_beam_interpolation(",),
     "get_tau": ("# compute tau",),
     "get_antenna_vis": ("meas_eq(",),
-    "get_baseline_vis": ("vis_inner_product(",),
+    "get_baseline_vis": ("cublas_complex_mm(",),
 }
 
 profiler = LineProfiler()
 
 main = click.Group()
 
 
@@ -187,26 +187,27 @@
         line_stats, total_time, VIS_GPU_STEPS if gpu else VIS_CPU_STEPS
     )
 
     print()
     print("------------- Summary of timings -------------")
     for thing, (hits, time, time_per_hit, percent, nlines) in thing_stats.items():
         print(
-            f"{thing:>19}: {hits:>4} hits, {time:.2f} seconds, {time_per_hit:.2f} sec/hit, {percent:3.2f}%, {nlines} lines"
+            f"{thing:>19}: {hits:>4} hits, {time:.3e} seconds, {time_per_hit:.3e} sec/hit, {percent:3.2f}%, {nlines} lines"
         )
     print("----------------------------------------------")
 
     with open(f"{outdir}/summary-stats-{str_id}.pkl", "wb") as fl:
         pickle.dump(thing_stats, fl)
 
 
 def get_line_based_stats(lstats) -> tuple[dict, float]:
     """Convert the line-number based stats into line-based stats."""
+    time_unit = lstats.unit
     (fn, lineno, name), timings = sorted(lstats.timings.items())[0]
-    d, total_time = get_stats_and_lines(fn, lineno, timings)
+    d, total_time = get_stats_and_lines(fn, lineno, timings, time_unit)
     return d, total_time
 
 
 def get_summary_stats(line_data, total_time, ids):
     """Convert a line-by-line set of stats into a summary of major components."""
     # specify contents of lines where important things happen
     thing_stats = {"total": (1, total_time, total_time / 1, 100, len(line_data))}
@@ -225,30 +226,30 @@
                     break
             elif len(lines) == 1 and init_line:
                 break
 
         if not assoc_lines:
             raise RuntimeError(
                 f"Could not find any lines for {thing} satisfying '{lines}'. "
-                f"Possible lines: {' | '.join(list(line_data.keys()))}"
+                "Possible lines:\n" + "\n".join(list(line_data.keys()))
             )
 
         # save (hits, time, time/hits, percent, nlines)
         thing_stats[thing] = (
             line_data[assoc_lines[0]][0],
             sum(line_data[ln][1] for ln in assoc_lines),
             sum(line_data[ln][2] for ln in assoc_lines),
             sum(line_data[ln][3] for ln in assoc_lines),
             len(assoc_lines),
         )
 
     return thing_stats
 
 
-def get_stats_and_lines(filename, start_lineno, timings):
+def get_stats_and_lines(filename, start_lineno, timings, time_unit):
     """Match up timing stats with line content of the code."""
     d = {}
     total_time = 0.0
     linenos = []
     for lineno, nhits, time in timings:
         total_time += time
         linenos.append(lineno)
@@ -263,21 +264,21 @@
 
     for lineno, nhits, time in timings:
         percent = 100 * time / total_time
         idx = all_linenos.index(lineno)
 
         d[sublines[idx].rstrip("\n").rstrip("\r")] = (
             nhits,
-            time / 1e6,
-            float(time) / nhits / 1e6,
+            time * time_unit,
+            float(time) / nhits * time_unit,
             percent,
             lineno,
         )
 
-    return d, total_time / 1e6
+    return d, total_time * time_unit
 
 
 def get_standard_sim_params(
     use_analytic_beam: bool, nfreq, ntime, nants, nsource, nbeams
 ):
     """Create some standard random simulation parameters for use in profiling.
```

### Comparing `vis_cpu-1.0.1/src/vis_cpu/conversions.py` & `vis_cpu-1.1.0/src/vis_cpu/conversions.py`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/src/vis_cpu/cpu.py` & `vis_cpu-1.1.0/src/vis_cpu/cpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 """CPU-based implementation of the visibility simulator."""
 from __future__ import annotations
 
+import datetime
+import gc
+import linecache
 import logging
 import numpy as np
-import warnings
+import psutil
+import time
+import tracemalloc as tm
 from astropy.constants import c
+from collections.abc import Sequence
+
+# from pympler import tracker
 from pyuvdata import UVBeam
-from re import I
-from scipy.interpolate import RectBivariateSpline
-from typing import Callable, Optional, Sequence
+from typing import Callable
 
 from . import conversions
+from ._utils import human_readable_size
 
 # This enables us to put in profile decorators that will be no-ops if no profiling
 # library is being used.
 try:
     profile
 except NameError:
     from ._utils import no_op as profile
@@ -135,28 +142,30 @@
                 "reuse_spline": True,
                 "check_azza_domain": False,
                 "spline_opts": spline_opts,
             }
             if isinstance(bm, UVBeam)
             else {}
         )
+        if isinstance(bm, UVBeam) and not bm.future_array_shapes:
+            bm.use_future_array_shapes()
 
         interp_beam = bm.interp(
             az_array=az,
             za_array=za,
             freq_array=np.atleast_1d(freq),
             **kw,
         )[0]
 
         if polarized:
-            interp_beam = interp_beam[:, 0, :, 0, :]
+            interp_beam = interp_beam[:, :, 0, :]
         else:
             # Here we have already asserted that the beam is a power beam and
             # has only one polarization, so we just evaluate that one.
-            interp_beam = np.sqrt(interp_beam[0, 0, 0, 0, :])
+            interp_beam = np.sqrt(interp_beam[0, 0, 0, :])
 
         A_s[:, :, i] = interp_beam
 
         # Check for invalid beam values
         if check:
             sm = np.sum(A_s)
             if np.isinf(sm) or np.isnan(sm):
@@ -196,14 +205,15 @@
     crd_eq: np.ndarray,
     I_sky: np.ndarray,
     beam_list: Sequence[UVBeam | Callable] | None,
     precision: int = 1,
     polarized: bool = False,
     beam_idx: np.ndarray | None = None,
     beam_spline_opts: dict | None = None,
+    max_progress_reports: int = 100,
 ):
     """
     Calculate visibility from an input intensity map and beam model.
 
     Parameters
     ----------
     antpos : array_like
@@ -245,22 +255,32 @@
         Whether to simulate a full polarized response in terms of nn, ne, en,
         ee visibilities. See Eq. 6 of Kohn+ (arXiv:1802.04151) for notation.
         Default: False.
     beam_idx
         Optional length-NANT array specifying a beam index for each antenna.
         By default, either a single beam is assumed to apply to all antennas or
         each antenna gets its own beam.
+    beam_spline_opts : dict, optional
+        Dictionary of options to pass to the beam interpolation function.
+    max_progress_reports : int, optional
+        Maximum number of progress reports to print to the screen (if logging level
+        allows). Default is 100.
 
     Returns
     -------
     vis : array_like
         Simulated visibilities. If `polarized = True`, the output will have
         shape (NTIMES, NFEED, NFEED, NANTS, NANTS), otherwise it will have
         shape (NTIMES, NANTS, NANTS).
     """
+    if not tm.is_tracing() and logger.isEnabledFor(logging.INFO):
+        tm.start()
+
+    highest_peak = _memtrace(0)
+
     nax, nfeed, nant, ntimes = _validate_inputs(
         precision, polarized, antpos, eq2tops, crd_eq, I_sky
     )
 
     if precision == 1:
         real_dtype = np.float32
         complex_dtype = np.complex64
@@ -277,30 +297,41 @@
     # polarization channels
     Isqrt = np.sqrt(0.5 * I_sky).astype(real_dtype)
     antpos = antpos.astype(real_dtype)
 
     ang_freq = real_dtype(2.0 * np.pi * freq)
 
     # Zero arrays: beam pattern, visibilities, delays, complex voltages
-    vis = np.zeros((ntimes, nfeed * nant, nfeed * nant), dtype=complex_dtype)
+    vis = np.full((ntimes, nfeed * nant, nfeed * nant), 0.0, dtype=complex_dtype)
+    logger.info(f"Visibility Array takes {vis.nbytes/1024**2:.1f} MB")
+
     crd_eq = crd_eq.astype(real_dtype)
 
+    # Have up to 100 reports as it iterates through time.
+    report_chunk = ntimes // max_progress_reports + 1
+    pr = psutil.Process()
+    tstart = time.time()
+    mlast = pr.memory_info().rss
+    plast = tstart
+
+    highest_peak = _memtrace(highest_peak)
+
     # Loop over time samples
     for t, eq2top in enumerate(eq2tops.astype(real_dtype)):
         # Dot product converts ECI cosines (i.e. from RA and Dec) into ENU
         # (topocentric) cosines, with (tx, ty, tz) = (e, n, u) components
         # relative to the center of the array
         tx, ty, tz = crd_top = np.dot(eq2top, crd_eq)
         above_horizon = tz > 0
         tx = tx[above_horizon]
         ty = ty[above_horizon]
         nsrcs_up = len(tx)
         isqrt = Isqrt[above_horizon]
 
-        A_s = np.zeros((nax, nfeed, nbeam, nsrcs_up), dtype=complex_dtype)
+        A_s = np.full((nax, nfeed, nbeam, nsrcs_up), 0.0, dtype=complex_dtype)
 
         _evaluate_beam_cpu(
             A_s,
             beam_list,
             tx,
             ty,
             polarized,
@@ -321,14 +352,18 @@
         )
         _log_array("vant", v)
 
         # Compute visibilities using product of complex voltages (upper triangle).
         vis[t] = v.conj().dot(v.T)
         _log_array("vis", vis[t])
 
+        if not (t % report_chunk or t == ntimes - 1):
+            plast, mlast = _log_progress(tstart, plast, t + 1, ntimes, pr, mlast)
+            highest_peak = _memtrace(highest_peak)
+
     vis.shape = (ntimes, nfeed, nant, nfeed, nant)
 
     # Return visibilities with or without multiple polarization channels
     return vis.transpose((0, 1, 3, 2, 4)) if polarized else vis[:, 0, :, 0, :]
 
 
 def _get_antenna_vis(
@@ -344,13 +379,51 @@
     # v has shape (Nants, Nsources) and is sqrt(I)*exp(1j tau*nu)
     # Here we expand A_s to all ants (from its beams), then broadcast to v, so we
     # end up with shape (Nax, Nfeed, Nants, Nsources)
     v = A_s[:, beam_idx] * v[np.newaxis, :, np.newaxis, :]  # ^ but Nbeam -> Nant
     return v.reshape((nfeed * nant, nax * nsrcs_up))  # reform into matrix
 
 
+def _memtrace(highest_peak) -> int:
+    if logger.isEnabledFor(logging.INFO):
+        cm, pm = tm.get_traced_memory()
+        logger.info(f"Starting Memory usage  : {cm/1024**3:.3f} GB")
+        logger.info(f"Starting Peak Mem usage: {pm/1024**3:.3f} GB")
+        logger.info(f"Traemalloc Peak Memory (tot)(GB): {highest_peak / 1024**3:.2f}")
+        tm.reset_peak()
+        return max(pm, highest_peak)
+
+
 def _log_array(name, x):
     """Debug logging of the value of an array."""
-    if logger.getEffectiveLevel() <= logging.DEBUG:  # pragma: no cover
+    if logger.isEnabledFor(logging.DEBUG):  # pragma: no cover
         logger.debug(
             f"CPU: {name}: {x.flatten() if x.size < 40 else x.flatten()[:40]} {x.shape}"
         )
+
+
+def _log_progress(start_time, prev_time, iters, niters, pr, last_mem):
+    """Logging of progress."""
+    if not logger.isEnabledFor(logging.INFO):
+        return prev_time, last_mem
+
+    t = time.time()
+    lapsed = datetime.timedelta(seconds=(t - prev_time))
+    total = datetime.timedelta(seconds=(t - start_time))
+    per_iter = total / iters
+    expected = per_iter * niters
+
+    rss = pr.memory_info().rss
+    mem = human_readable_size(rss)
+    memdiff = human_readable_size(rss - last_mem, indicate_sign=True)
+
+    logger.info(
+        f"""
+        Progress Info   [{iters}/{niters} times ({100 * iters / niters:.1f}%)]
+            -> Update Time:   {lapsed}
+            -> Total Time:    {total} [{per_iter} per integration]
+            -> Expected Time: {expected} [{expected - total} remaining]
+            -> Memory Usage:  {mem}  [{memdiff}]
+        """
+    )
+
+    return t, rss
```

### Comparing `vis_cpu-1.0.1/src/vis_cpu/data/NF_HERA_Dipole_small.fits` & `vis_cpu-1.1.0/src/vis_cpu/data/NF_HERA_Dipole_small.fits`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/src/vis_cpu/gpu.py` & `vis_cpu-1.1.0/src/vis_cpu/gpu.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 """GPU implementation of the simulator."""
 from __future__ import annotations
 
 import logging
 import numpy as np
+import psutil
+import time
 import warnings
 from astropy.constants import c as speed_of_light
+from collections.abc import Sequence
 from pathlib import Path
 from pyuvdata import UVBeam
-from typing import Callable, Optional, Sequence
+from typing import Callable, Optional
 
 from . import conversions
+from ._utils import ceildiv
 from ._uvbeam_to_raw import uvbeam_to_azza_grid
-from .cpu import _evaluate_beam_cpu, _validate_inputs, _wrangle_beams, vis_cpu
+from .cpu import (
+    _evaluate_beam_cpu,
+    _log_progress,
+    _validate_inputs,
+    _wrangle_beams,
+    vis_cpu,
+)
 
 logger = logging.getLogger(__name__)
 
 # This enables us to put in profile decorators that will be no-ops if no profiling
 # library is being used.
 try:
     profile
@@ -39,14 +49,21 @@
         cublasSgemm,
         cublasZgemm,
     )
 
     HAVE_CUDA = True
 
 except ImportError:
+    # if not installed, don't warn
+    HAVE_CUDA = False
+    Template = no_op
+except Exception as e:  # pragma: no cover
+    # if installed but having initialization issues
+    # warn, but default back to non-gpu functionality
+    warnings.warn(str(e), stacklevel=2)
     HAVE_CUDA = False
     Template = no_op
 
 
 ONE_OVER_C = 1.0 / speed_of_light.value
 
 templates = Path(__file__).parent / "gpu_src"
@@ -101,21 +118,23 @@
     precision: int = 1,
     beam_spline_opts: dict | None = None,
 ) -> np.ndarray:
     """GPU implementation of the visibility simulator."""
     if not HAVE_CUDA:
         raise ImportError("You need to install the [gpu] extra to use this function!")
 
+    pr = psutil.Process()
     nax, nfeed, nant, ntimes = _validate_inputs(
         precision, polarized, antpos, eq2tops, crd_eq, I_sky
     )
 
     if beam_spline_opts:
         warnings.warn(
-            "You have passed beam_spline_opts, but these are not used in GPU."
+            "You have passed beam_spline_opts, but these are not used in GPU.",
+            stacklevel=1,
         )
 
     nsrc = len(I_sky)
 
     if precision == 1:
         real_dtype, complex_dtype = np.float32, np.complex64
         cublas_real_mm = cublasSgemm
@@ -132,53 +151,51 @@
 
     # ensure data types
     antpos = antpos.astype(real_dtype)
     eq2tops = eq2tops.astype(real_dtype)
     crd_eq = crd_eq.astype(real_dtype)
     Isqrt = np.sqrt(0.5 * I_sky).astype(real_dtype)
 
-    chunk = max(
-        min(nsrc, min_chunks),
-        2 ** int(np.ceil(np.log2(float(nant * nsrc) / max_memory / 2))),
-    )
-    npixc = nsrc // chunk
-
     beam_list, nbeam, beam_idx = _wrangle_beams(
         beam_idx=beam_idx,
         beam_list=beam_list,
         polarized=polarized,
         nant=nant,
         freq=freq,
     )
 
-    # Ways to block up threads for sending to GPU calculations. "Meas" is for the
-    # measurement equation function, and "prod" is for the inner-product calculation.
-    meas_block = (
-        max(1, nthreads // (nant * nax * nfeed)),
-        min(nthreads, nant * nax),
-        min(nthreads, nfeed),
+    total_beam_pix = sum(
+        beam.data_array.shape[-2] * beam.data_array.shape[-1]
+        for beam in beam_list
+        if hasattr(beam, "data_array")
     )
 
-    logger.info(
-        f"Using {np.prod(meas_block)} threads in total for measurement equation."
+    nchunks = min(
+        max(
+            min_chunks,
+            _get_required_chunks(
+                nax, nfeed, nant, nsrc, nbeam, total_beam_pix, precision
+            ),
+        ),
+        nsrc,
     )
-    logger.info(f"Using a shared-memory buffer of size {5*meas_block[0]}.")
+
+    npixc = nsrc // nchunks
 
     use_uvbeam = isinstance(beam_list[0], UVBeam)
     if use_uvbeam and not all(isinstance(b, UVBeam) for b in beam_list):
         raise ValueError(
             "vis_gpu only support beam_lists with either all UVBeam or all AnalyticBeam objects."
         )
 
     cuda_params = {
         "NANT": nant,
         "NAX": nax,
         "NFEED": nfeed,
         "NBEAM": nbeam,
-        "BLOCK_PX": meas_block[0],
         "DTYPE": DTYPE,
         "CDTYPE": CDTYPE,
         "f": "f" if precision == 1 else "",
     }
 
     if use_uvbeam:
         # We need to make sure that each beam "raw" data is on the same grid.
@@ -261,212 +278,209 @@
     # sent from CPU each time
     eq2top_gpu = gpuarray.empty(shape=(3, 3), dtype=real_dtype)
     # will be set on GPU
     crdtop_gpu = gpuarray.empty(shape=(3, npixc), dtype=real_dtype)
     # will be set on GPU
     vis_gpus = [
         gpuarray.empty(shape=(nfeed * nant, nfeed * nant), dtype=complex_dtype)
-        for _ in range(chunk)
+        for _ in range(nchunks)
     ]
 
     # output CPU buffers for downloading answers
     vis_cpus = [
-        np.empty(shape=(nfeed * nant, nfeed * nant), dtype=complex_dtype)
-        for _ in range(chunk)
+        np.zeros(shape=(nfeed * nant, nfeed * nant), dtype=complex_dtype)
+        for _ in range(nchunks)
     ]
-    streams = [driver.Stream() for _ in range(chunk)]
+    streams = [driver.Stream() for _ in range(nchunks)]
     event_order = [
         "start",
         "upload",
         "eq2top",
         "tau",
         "meas_eq",
         "vis",
         "end",
     ]
 
     if use_uvbeam:
         event_order.insert(4, "interpolation")
 
-    vis = np.empty((ntimes, nfeed * nant, nfeed * nant), dtype=complex_dtype)
+    vis = np.full((ntimes, nfeed * nant, nfeed * nant), 0.0, dtype=complex_dtype)
 
-    logger.info("Running With %s chunks: ", chunk)
+    logger.info(f"Running With {nchunks} chunks")
+
+    report_chunk = ntimes // 100 + 1
+    pr = psutil.Process()
+    tstart = time.time()
+    mlast = pr.memory_info().rss
+    plast = tstart
 
     for t in range(ntimes):
         eq2top_gpu.set(eq2tops[t])  # defines sky orientation for this time step
-        events = [{e: driver.Event() for e in event_order} for _ in range(chunk)]
-
-        for c in range(chunk + 2):
-            cc = c - 1
-            ccc = c - 2
-            if 0 <= ccc < chunk:
-                stream = streams[ccc]
-                vis_gpus[ccc].get(ary=vis_cpus[ccc], stream=stream)
-                events[ccc]["end"].record(stream)
-            if 0 <= cc < chunk:
-                stream = streams[cc]
-                cublasSetStream(h, stream.handle)
-
-                # cublas arrays are in Fortran order, so P=M*N is actually
-                # peformed as P.T = N.T * M.T
-                cublas_real_mm(  # compute crdtop = dot(eq2top,crd_eq)
-                    h,
-                    "n",
-                    "n",
-                    npixc,
-                    3,
-                    3,
-                    1.0,
-                    crd_eq_gpu.gpudata,
-                    npixc,
-                    eq2top_gpu.gpudata,
-                    3,
-                    0.0,
-                    crdtop_gpu.gpudata,
-                    npixc,
-                )
-                events[cc]["eq2top"].record(stream)
-
-                tx, ty, tz = crdtop_gpu.get_async(stream=stream)
-                above_horizon = tz > 0
-                tx = tx[above_horizon]
-                ty = ty[above_horizon]
-                nsrcs_up = len(tx)
-                crdtop_lim_gpu = gpuarray.to_gpu_async(
-                    crdtop_gpu.get_async(stream=stream)[:, above_horizon].copy(),
-                    stream=stream,
-                )
-
-                if nsrcs_up < 1:
-                    continue
+        events = [{e: driver.Event() for e in event_order} for _ in range(nchunks)]
 
-                tau_gpu = gpuarray.empty(shape=(nant, nsrcs_up), dtype=real_dtype)
-
-                cublas_real_mm(  # compute tau = dot(antpos,crdtop) / speed_of_light
-                    h,
-                    "n",
-                    "n",
-                    nsrcs_up,
-                    nant,
-                    3,
-                    ONE_OVER_C,
-                    crdtop_lim_gpu.gpudata,
-                    nsrcs_up,
-                    antpos_gpu.gpudata,
-                    3,
-                    0.0,
-                    tau_gpu.gpudata,
-                    nsrcs_up,
-                )
-                events[cc]["tau"].record(stream)
+        for c, (stream, event) in enumerate(zip(streams, events)):
+            event["start"].record(stream)
+            crd_eq_gpu.set_async(crd_eq[:, c * npixc : (c + 1) * npixc], stream=stream)
+            Isqrt_gpu.set_async(Isqrt[c * npixc : (c + 1) * npixc], stream=stream)
+            event["upload"].record(stream)
+
+            cublasSetStream(h, stream.handle)
+
+            # cublas arrays are in Fortran order, so P=M*N is actually
+            # peformed as P.T = N.T * M.T
+            cublas_real_mm(  # compute crdtop = dot(eq2top,crd_eq)
+                h,
+                "n",
+                "n",
+                npixc,
+                3,
+                3,
+                1.0,
+                crd_eq_gpu.gpudata,
+                npixc,
+                eq2top_gpu.gpudata,
+                3,
+                0.0,
+                crdtop_gpu.gpudata,
+                npixc,
+            )
+            event["eq2top"].record(stream)
 
-                # Need to do this in polar coordinates, NOT (l,m), at least for
-                # polarized beams. This is because at zenith, the Efield components are
-                # discontinuous (in power they are continuous). When interpolating the
-                # E-field components, you need to treat the zenith point differently
-                # depending on which "side" of zenith you're on. This is doable in polar
-                # coordinates, but not in Cartesian coordinates.
-                A_gpu = do_beam_interpolation(
-                    freq,
-                    beam_list,
-                    polarized,
-                    nthreads,
-                    nax,
-                    nfeed,
-                    complex_dtype,
-                    nbeam,
-                    use_uvbeam,
-                    daz,
-                    dza,
-                    beam_interp,
-                    beam_data_gpu,
-                    events,
-                    cc,
-                    stream,
-                    tx,
-                    ty,
-                    nsrcs_up,
-                )
+            tx, ty, tz = crdtop_gpu.get_async(stream=stream)
+            above_horizon = tz > 0
+            tx = tx[above_horizon]
+            ty = ty[above_horizon]
+            nsrcs_up = len(tx)
+
+            if nsrcs_up < 1:
+                continue
+
+            crdtop_lim_gpu = gpuarray.to_gpu_async(
+                crdtop_gpu.get_async(stream=stream)[:, above_horizon].copy(),
+                stream=stream,
+            )
 
-                v_gpu = gpuarray.empty(
-                    shape=(nfeed * nant, nax * nsrcs_up), dtype=complex_dtype
-                )
-                Isqrt_lim_gpu = gpuarray.to_gpu_async(
-                    Isqrt_gpu.get()[above_horizon].copy(), stream=stream
-                )
+            tau_gpu = gpuarray.empty(shape=(nant, nsrcs_up), dtype=real_dtype)
 
-                # blocks of threads are mapped to (pixels,ants,freqs)
+            cublas_real_mm(  # compute tau = dot(antpos,crdtop) / speed_of_light
+                h,
+                "n",
+                "n",
+                nsrcs_up,
+                nant,
+                3,
+                ONE_OVER_C,
+                crdtop_lim_gpu.gpudata,
+                nsrcs_up,
+                antpos_gpu.gpudata,
+                3,
+                0.0,
+                tau_gpu.gpudata,
+                nsrcs_up,
+            )
+            event["tau"].record(stream)
 
-                grid = (
-                    int(np.ceil(nsrcs_up / float(meas_block[0]))),
-                    int(np.ceil(nax * nant / float(meas_block[1]))),
-                    int(np.ceil(nfeed / float(meas_block[2]))),
-                )
+            # Need to do this in polar coordinates, NOT (l,m), at least for
+            # polarized beams. This is because at zenith, the Efield components are
+            # discontinuous (in power they are continuous). When interpolating the
+            # E-field components, you need to treat the zenith point differently
+            # depending on which "side" of zenith you're on. This is doable in polar
+            # coordinates, but not in Cartesian coordinates.
+            A_gpu = do_beam_interpolation(
+                freq,
+                beam_list,
+                polarized,
+                nthreads,
+                nax,
+                nfeed,
+                complex_dtype,
+                nbeam,
+                use_uvbeam,
+                daz,
+                dza,
+                beam_interp,
+                beam_data_gpu,
+                event,
+                stream,
+                tx,
+                ty,
+                nsrcs_up,
+            )
 
-                logger.info(f"Measurement Eq. Grid Size: {grid}")
+            v_gpu = gpuarray.empty(
+                shape=(nfeed * nant, nax * nsrcs_up), dtype=complex_dtype
+            )
+            Isqrt_lim_gpu = gpuarray.to_gpu_async(
+                Isqrt_gpu.get()[above_horizon].copy(), stream=stream
+            )
 
-                _logdebug(A_gpu, "Beam")
+            _logdebug(A_gpu, "Beam")
 
-                # compute v = A * sqrtI * exp(1j*tau*freq)
-                meas_eq(
-                    A_gpu,
-                    Isqrt_lim_gpu,
-                    tau_gpu,
-                    ang_freq,
-                    np.uint(nsrcs_up),
-                    beam_idx,
-                    v_gpu,
-                    grid=grid,
-                    block=meas_block,
-                    stream=stream,
+            # compute v = A * sqrtI * exp(1j*tau*freq)
+            # Ways to block up threads for sending to GPU calculations. "Meas" is for the
+            # measurement equation function, and "prod" is for the inner-product calculation.
+            block, grid = _get_3d_block_grid(nthreads, nsrcs_up, nant * nax, nfeed)
+
+            if t == 0:
+                logger.info(
+                    f"Using {block} = {np.prod(block)} threads in total, in a grid of {grid}, "
+                    "for measurement equation."
                 )
-                events[cc]["meas_eq"].record(stream)
 
-                _logdebug(v_gpu, "vant")
-
-                # compute vis = dot(v, v.T)
-                # We want to take an outer product over feeds/antennas, contract over
-                # E-field components, and integrate over the sky.
-                # Remember cublas is in fortran order...
-                # v_gpu is (nfeed * nant, nax * nsrcs_up)
-                cublas_complex_mm(
-                    h,
-                    "c",  # conjugate transpose for first (remember fortran order)
-                    "n",  # no transpose for second.
-                    nfeed * nant,
-                    nfeed * nant,
-                    nax * nsrcs_up,
-                    1.0,
-                    v_gpu.gpudata,
-                    nax * nsrcs_up,
-                    v_gpu.gpudata,
-                    nax * nsrcs_up,
-                    0.0,
-                    vis_gpus[cc].gpudata,
-                    nfeed * nant,
-                )
+            meas_eq(
+                A_gpu,
+                Isqrt_lim_gpu,
+                tau_gpu,
+                ang_freq,
+                np.uint(nsrcs_up),
+                beam_idx,
+                v_gpu,
+                grid=grid,
+                block=block,
+                stream=stream,
+            )
+            event["meas_eq"].record(stream)
 
-                _logdebug(vis_gpus[cc], "Vis")
+            _logdebug(v_gpu, "vant")
 
-                events[cc]["vis"].record(stream)
+            # compute vis = dot(v, v.T)
+            # We want to take an outer product over feeds/antennas, contract over
+            # E-field components, and integrate over the sky.
+            # Remember cublas is in fortran order...
+            # v_gpu is (nfeed * nant, nax * nsrcs_up)
+            cublas_complex_mm(
+                h,
+                "c",  # conjugate transpose for first (remember fortran order)
+                "n",  # no transpose for second.
+                nfeed * nant,
+                nfeed * nant,
+                nax * nsrcs_up,
+                1.0,
+                v_gpu.gpudata,
+                nax * nsrcs_up,
+                v_gpu.gpudata,
+                nax * nsrcs_up,
+                0.0,
+                vis_gpus[c].gpudata,
+                nfeed * nant,
+            )
 
-            if c < chunk:
-                # This is the first thing that happens in the loop over chunks.
+            _logdebug(vis_gpus[c], "Vis")
 
-                stream = streams[c]
-                events[c]["start"].record(stream)
-                crd_eq_gpu.set_async(
-                    crd_eq[:, c * npixc : (c + 1) * npixc], stream=stream
-                )
-                Isqrt_gpu.set_async(Isqrt[c * npixc : (c + 1) * npixc], stream=stream)
-                events[c]["upload"].record(stream)
+            event["vis"].record(stream)
 
-        events[chunk - 1]["end"].synchronize()
+            vis_gpus[c].get(ary=vis_cpus[c], stream=stream)
+            event["end"].record(stream)
+        events[nchunks - 1]["end"].synchronize()
         vis[t] = sum(vis_cpus)
 
+        if not (t % report_chunk or t == ntimes - 1):
+            plast, mlast = _log_progress(tstart, plast, t + 1, ntimes, pr, mlast)
+
     # teardown GPU configuration
     cublasDestroy(h)
     vis = vis.conj().reshape((ntimes, nfeed, nant, nfeed, nant))
     return vis.transpose((0, 1, 3, 2, 4)) if polarized else vis[:, 0, :, 0, :]
 
 
 def do_beam_interpolation(
@@ -479,16 +493,15 @@
     complex_dtype,
     nbeam,
     use_uvbeam,
     daz,
     dza,
     beam_interp,
     beam_data_gpu,
-    events,
-    cc,
+    event,
     stream,
     tx,
     ty,
     nsrcs_up,
 ):
     """Perform the beam interpolation, choosing between CPU and GPU as necessary."""
     if use_uvbeam:  # perform interpolation on GPU
@@ -501,15 +514,15 @@
             az,
             za,
             gpu_func=beam_interp,
             nthreads=nthreads,
             stream=stream,
             return_on_cpu=False,
         )
-        events[cc]["interpolation"].record(stream)
+        event["interpolation"].record(stream)
     else:
         A_gpu = gpuarray.empty(shape=(nax, nfeed, nbeam, nsrcs_up), dtype=complex_dtype)
         A_s = np.zeros((nax, nfeed, nbeam, nsrcs_up), dtype=complex_dtype)
 
         _evaluate_beam_cpu(
             A_s,
             beam_list,
@@ -604,24 +617,15 @@
                 "NAX": nax,
                 "NFEED": nfeed,
             }
         )
         beam_interp_module = compiler.SourceModule(beam_interp_code)
         gpu_func = beam_interp_module.get_function("InterpolateBeamAltAz")
 
-    block = (
-        max(1, nthreads // nbeam // (nax * nfeed)),
-        min(nthreads, nbeam),
-        nax * nfeed,
-    )
-    grid = (
-        int(np.ceil(nsrc / float(block[0]))),
-        int(np.ceil(nbeam / float(block[1]))),
-        int(np.ceil(nax * nfeed / float(block[2]))),
-    )
+    block, grid = _get_3d_block_grid(nthreads, nsrc, nbeam, nax * nfeed)
 
     az_gpu = gpuarray.to_gpu_async(az, stream=stream)
     za_gpu = gpuarray.to_gpu_async(za, stream=stream)
     nsrc_uint = np.uint(nsrc)
 
     def fnc(beam_in, beam_out):
         gpu_func(
@@ -651,8 +655,62 @@
 
     if return_on_cpu:
         return beam_at_src.get_async(stream=stream)
     else:
         return beam_at_src
 
 
+def _get_3d_block_grid(nthreads: int, a: int, b: int, c: int):
+    """Create a block/grid layout for 3D where axis speed is a > b > c.
+
+    This puts a,b,c into the 1st 2nd and 3rd axes, and optimizes for the "a" axis
+    moving the fastest.
+    """
+    if nthreads < 1:
+        raise ValueError("nthreads must be at least 1")
+    if a < 1 or b < 1 or c < 1:
+        raise ValueError("a, b, and c must all be at least 1")
+
+    bla = min(nthreads, a)
+    blb = max(1, min(nthreads // bla, b))
+    blc = max(1, min(nthreads // (bla * blb), c))
+    block = (bla, blb, blc)
+
+    grid = (
+        ceildiv(a, block[0]),
+        ceildiv(b, block[1]),
+        ceildiv(c, block[2]),
+    )
+
+    return block, grid
+
+
 vis_gpu.__doc__ += vis_cpu.__doc__
+
+
+def _get_required_chunks(nax, nfeed, nant, nsrc, nbeam, nbeampix, precision):
+    freemem = driver.mem_get_info()[0]  # in bytes
+    size = 4 * precision
+
+    gpusize = [freemem]
+    ch = 0
+    while sum(gpusize) >= freemem and ch < 100:
+        ch += 1
+        gpusize = [
+            nant * 3 * size,
+            nsrc // ch * size,  # antpos
+            nbeampix * nfeed * nax * size * 2,  # Isqrt
+            3 * nsrc // ch * size,  # complex beam data
+            3 * nsrc // ch * size,  # crd_eq_gpu
+            nfeed * nant * nax * nant * ch * size * 2,  # crdtop
+            nax * nfeed * nbeam * nsrc // ch // 2 * size * 2,  # vis_gpus
+            nant * nsrc // ch // 2 * size * 2,  # interpolated beam  # ant-vis
+        ]
+        logger.debug(
+            f"nchunks={ch}. Array Sizes (bytes)={gpusize}. Total={sum(gpusize)}"
+        )
+
+    logger.info(
+        f"Total free mem on GPU: {freemem/(1024**3):.2f} GB. Requires {ch} chunks "
+        f"(estimate {sum(gpusize) / 1024**3:.2f} GB)"
+    )
+    return ch
```

### Comparing `vis_cpu-1.0.1/src/vis_cpu/gpu_src/beam_interpolation.cu` & `vis_cpu-1.1.0/src/vis_cpu/gpu_src/beam_interpolation.cu`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/src/vis_cpu/gpu_src/measurement_equation.cu` & `vis_cpu-1.1.0/src/vis_cpu/gpu_src/measurement_equation.cu`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,14 @@
 // NFEED    : # of feeds in the beam
 // -------------------------------------------------------------------------------------
 
 #include <cuComplex.h>
 #include <pycuda-helpers.hpp>
 #include <stdio.h>
 
-// Shared memory for storing per-antenna results to be reused among all ants
-// for "BLOCK_PX" pixels, avoiding a rush on global memory.
-__shared__ {{ DTYPE }} sh_buf[{{ BLOCK_PX }}*5];
-
 // Compute A*I*exp(ij*tau*freq) for all antennas, storing output in v
 __global__ void MeasEq(
     {{ CDTYPE }} *A,
     {{ DTYPE }} *sqrtI,
     {{ DTYPE }} *tau,
     double freq,
     uint nsrc,
@@ -33,37 +29,31 @@
     {{ CDTYPE }} *v
 ){
     const uint nbeam = {{ NBEAM }};
     const uint nax  = {{ NAX }};
     const uint nfeed= {{ NFEED }};
     const uint nant = {{ NANT }};
 
-    const uint tx = threadIdx.x; // First dim is src
-    const uint ty = threadIdx.y; // Second dim is ant
-
     const uint src  =  blockIdx.x * blockDim.x + threadIdx.x;  // first thread dim is src on sky
     const uint antax = blockIdx.y * blockDim.y + threadIdx.y;  // second thread dim is nax*nant
     const uint feed  = blockIdx.z * blockDim.z + threadIdx.z;  // third thread dim is nfeed
 
     uint ant = antax / nax;
     uint ax = antax % nax;
     uint beam = beam_idx[ant];
 
     {{ CDTYPE }} amp;
     {{ DTYPE }} phs;
     if (ant >= nant || ax >= nax || feed >= nfeed || src >= nsrc) return;
-    if (ty == 0)
-        sh_buf[tx] = sqrtI[src];
-    __syncthreads(); // make sure all memory is loaded before computing
 
     // Create both real/imag parts of the "amplitude"
     uint tau_indx = ant*nsrc + src;
     uint Aindx = ax*(nfeed*nbeam*nsrc) + feed*nbeam*nsrc + beam*nsrc + src;
-    amp.x = A[Aindx].x * sh_buf[tx];
-    amp.y = A[Aindx].y * sh_buf[tx];
+    amp.x = A[Aindx].x * sqrtI[src];
+    amp.y = A[Aindx].y * sqrtI[src];
 
     phs = tau[tau_indx] * freq;
 
     uint vidx = feed*(nant*nax*nsrc) + ant*nax*nsrc + ax*nsrc + src;
     v[vidx] = cuCmul{{ f }}(amp, make_{{ CDTYPE }}(cos(phs), sin(phs)));
 
     __syncthreads(); // make sure everyone used mem before kicking out
```

### Comparing `vis_cpu-1.0.1/src/vis_cpu/plot.py` & `vis_cpu-1.1.0/src/vis_cpu/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     # Get source az, za (note the azimuth convention used by UVBeam)
     tx, ty, tz = np.dot(eq2top, crd_eq)
     az, za = conversions.enu_to_az_za(enu_e=tx, enu_n=ty, orientation="uvbeam")
 
     # Get beam values
     interp_beam = beam.interp(az, za, np.atleast_1d(ref_freq))[0]
-    A_s = interp_beam[0, 0, 1, 0]  # (2, 1, 2, 1, Nptsrc)
+    A_s = interp_beam[0, 1, 0]  # (2, 2, 1, Nptsrc)
 
     # Horizon cut
     A_s = np.where(tz > 0, A_s, np.nan)
 
     return az, za, A_s
```

### Comparing `vis_cpu-1.0.1/src/vis_cpu/wrapper.py` & `vis_cpu-1.1.0/src/vis_cpu/wrapper.py`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/src/vis_cpu.egg-info/PKG-INFO` & `vis_cpu-1.1.0/src/vis_cpu.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: vis-cpu
-Version: 1.0.1
+Version: 1.1.0
 Summary: Fast visibility simulator with interface to CPU and GPU
 Home-page: https://github.com/hera-team/vis_cpu
 Author: HERA-Team
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+Provides-Extra: all
+Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: gpu
 Provides-Extra: profile
 Provides-Extra: test
 License-File: LICENSE.txt
 
 =======
```

### Comparing `vis_cpu-1.0.1/src/vis_cpu.egg-info/SOURCES.txt` & `vis_cpu-1.1.0/src/vis_cpu.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 .pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 LICENSE.txt
 README.rst
 codecov.yml
+gpu-analysis.nvprof
 pyproject.toml
 setup.cfg
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/question.md
 .github/PULL_REQUEST_TEMPLATE/feature.md
 .github/workflows/publish-to-pypi.yaml
 .github/workflows/run_notebooks.yaml
 .github/workflows/test_suite.yaml
-.github/workflows/test_suite_gpu.yaml
 ci/notebook-env.yml
 ci/test-env.yml
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
@@ -57,10 +57,12 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_beam_interp_gpu.py
 tests/test_beams.py
 tests/test_compare_pyuvsim.py
 tests/test_conversions.py
 tests/test_cpu_vs_gpu.py
+tests/test_gpu_utils.py
 tests/test_plot.py
+tests/test_utils.py
 tests/test_vis_cpu.py
 tests/test_vis_gpu.py
```

### Comparing `vis_cpu-1.0.1/tests/__init__.py` & `vis_cpu-1.1.0/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tests."""
 import numpy as np
+from astropy import units as un
 from astropy.coordinates import EarthLocation, Latitude, Longitude
 from astropy.time import Time
 from astropy.units import Quantity
 from pathlib import Path
 from pyradiosky import SkyModel
 from pyuvdata import UVBeam
 from pyuvsim import AnalyticBeam, simsetup
@@ -135,15 +136,15 @@
     # Set up sky model
     sky_model = SkyModel(
         name=[str(i) for i in range(len(ra_dec))],
         ra=Longitude(ra_dec[:, 0], "rad"),
         dec=Latitude(ra_dec[:, 1], "rad"),
         spectral_type="spectral_index",
         spectral_index=sources[:, 3],
-        stokes=stokes,
+        stokes=stokes * un.Jy,
         reference_frequency=Quantity(reference_frequency, "Hz"),
     )
 
     # Calculate stokes at all the frequencies.
     sky_model.at_frequencies(Quantity(freqs, "Hz"), inplace=True)
 
     return (
```

### Comparing `vis_cpu-1.0.1/tests/conftest.py` & `vis_cpu-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/tests/test_beam_interp_gpu.py` & `vis_cpu-1.1.0/tests/test_beam_interp_gpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,18 +174,18 @@
         iax,
         axx,
     ) in enumerate(new_beam_gpu):
         for ifd, feed in enumerate(axx):
             for ibeam, bm in enumerate(feed):
                 print(iax, ifd, ibeam)
                 np.testing.assert_allclose(
-                    new_beam_uvb[iax, 0, ifd, 0].real, bm.real, rtol=1e-6
+                    new_beam_uvb[iax, ifd, 0].real, bm.real, rtol=1e-6
                 )
                 np.testing.assert_allclose(
-                    new_beam_uvb[iax, 0, ifd, 0].imag, bm.imag, rtol=1e-6
+                    new_beam_uvb[iax, ifd, 0].imag, bm.imag, rtol=1e-6
                 )
 
 
 def test_wrong_beamtype():
     """Tests that a meaningful error is raised for a dumb beamtype."""
     # Create a small and simple beam with Nax=1, Nfeed=1
     za = np.linspace(0, 1, 5)
```

### Comparing `vis_cpu-1.0.1/tests/test_beams.py` & `vis_cpu-1.1.0/tests/test_beams.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,27 +156,27 @@
 @pytest.fixture(scope="module")
 def freq() -> np.ndarray:
     """Frequencies for tests."""
     return np.linspace(100.0e6, 120.0e6, NFREQ)  # Hz
 
 
 @pytest.fixture(scope="function")
-def beam_list_unpol() -> List[EllipticalBeam]:
+def beam_list_unpol() -> list[EllipticalBeam]:
     """Get Gaussian beam and transform into an elliptical version."""
     base_beam = AnalyticBeam("gaussian", diameter=14.0)
     beam_analytic = EllipticalBeam(base_beam, xstretch=2.2, ystretch=1.0, rotation=40.0)
     beam_analytic = conversions.prepare_beam(
         beam_analytic, polarized=False, use_feed="x"
     )
 
     return [beam_analytic, beam_analytic]
 
 
 @pytest.fixture(scope="function")
-def beam_list_pol() -> List[EllipticalBeam]:
+def beam_list_pol() -> list[EllipticalBeam]:
     """Get Gaussian beam and transform into an elliptical version with polarization."""
     base_beam = AnalyticBeam("gaussian", diameter=14.0)
     beam_analytic = EllipticalBeam(base_beam, xstretch=2.2, ystretch=1.0, rotation=40.0)
     beam_analytic = conversions.prepare_beam(
         beam_analytic, polarized=True, use_feed="x"
     )
 
@@ -414,16 +414,18 @@
 
 
 def test_covers_sky_almost_strong(uvbeam):
     """Test that beam covers sky almost completely."""
     beam1 = uvbeam.copy()
     beam2 = uvbeam.copy()
 
+    # Restrict to a certain frequency
     beam1.data_array = beam1.data_array[:, :, :, [0]]
     beam2.data_array = beam2.data_array[:, :, :, [0]]
+
     beam1.Nfreqs = 1
     beam2.Nfreqs = 1
 
     beam1.axis1_array = np.linspace(0, 2 * np.pi, beam1.axis1_array.size)
     beam2.axis1_array = np.linspace(0, 2 * np.pi, beam2.axis1_array.size)
 
     beam1.data_array[..., -1] = beam1.data_array[..., 0]
```

### Comparing `vis_cpu-1.0.1/tests/test_compare_pyuvsim.py` & `vis_cpu-1.1.0/tests/test_compare_pyuvsim.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 
     # If it passes this test, but fails the following tests, then its probably an
     # ordering issue.
     for i in range(nants):
         for j in range(i, nants):
             for if1, feed1 in enumerate(("X", "Y") if polarized else ("X",)):
                 for if2, feed2 in enumerate(("X", "Y") if polarized else ("X",)):
-
                     d_uvsim = uvd_uvsim.get_data(
                         (i, j, feed1 + feed2)
                     ).T  # pyuvsim visibility
                     d_viscpu = (
                         vis_vc[:, :, if1, if2, i, j]
                         if polarized
                         else vis_vc[:, :, i, j]
```

### Comparing `vis_cpu-1.0.1/tests/test_conversions.py` & `vis_cpu-1.1.0/tests/test_conversions.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
     dec = hera_lat * np.ones(ra.size)  # Dec = HERA latitude
 
     # Get Cartesian coords for these sources in our ECI system
     crd_eq = conversions.point_source_crd_eq(ra, dec)
 
     # Loop over LSTs
     for i, lst in enumerate(lsts):
-
         # Rotation matrices from ECI <-> ENU
         mat_eci_to_enu = conversions.eci_to_enu_matrix(lst, lat=hera_lat)
         mat_enu_to_eci = conversions.enu_to_eci_matrix(lst, lat=hera_lat)
 
         # Test that transforms are one anothers' inverse
         assert np.allclose(np.dot(mat_eci_to_enu, mat_enu_to_eci), np.eye(3))
         assert np.allclose(np.dot(mat_enu_to_eci, mat_eci_to_enu), np.eye(3))
```

### Comparing `vis_cpu-1.0.1/tests/test_cpu_vs_gpu.py` & `vis_cpu-1.1.0/tests/test_cpu_vs_gpu.py`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/tests/test_plot.py` & `vis_cpu-1.1.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `vis_cpu-1.0.1/tests/test_vis_cpu.py` & `vis_cpu-1.1.0/tests/test_vis_cpu.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,9 +45,10 @@
         dec,
         freq,
         lsts,
         beams=[beam, beam],
         polarized=polarized,
         precision=1,
         latitude=-30.7215 * np.pi / 180.0,
+        max_progress_reports=2,
     )
     assert np.all(~np.isnan(vis))  # check that there are no NaN values
```

### Comparing `vis_cpu-1.0.1/tests/test_vis_gpu.py` & `vis_cpu-1.1.0/tests/test_vis_gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 pytest.importorskip("pycuda")
 
 import numpy as np
 from pyuvsim.analyticbeam import AnalyticBeam
 
 from vis_cpu import simulate_vis
+from vis_cpu.gpu import _get_3d_block_grid
 
 from . import get_standard_sim_params
 
 
 def test_gpu_with_spline_opts():
     """Compare vis_cpu and pyuvsim simulated visibilities."""
     (
```

