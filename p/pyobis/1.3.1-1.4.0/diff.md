# Comparing `tmp/pyobis-1.3.1.tar.gz` & `tmp/pyobis-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobis-1.3.1.tar", last modified: Thu Mar 16 11:23:04 2023, max compression
+gzip compressed data, was "pyobis-1.4.0.tar", last modified: Tue May  9 07:19:40 2023, max compression
```

## Comparing `pyobis-1.3.1.tar` & `pyobis-1.4.0.tar`

### file list

```diff
@@ -1,70 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:23:04.466937 pyobis-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:23:04.450937 pyobis-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:23:04.454937 pyobis-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-16 11:22:36.000000 pyobis-1.3.1/.github/workflows/deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-16 11:22:36.000000 pyobis-1.3.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-16 11:22:36.000000 pyobis-1.3.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-16 11:22:36.000000 pyobis-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-16 11:22:36.000000 pyobis-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-16 11:22:36.000000 pyobis-1.3.1/CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-03-16 11:22:36.000000 pyobis-1.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-03-16 11:22:36.000000 pyobis-1.3.1/Changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-16 11:22:36.000000 pyobis-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-16 11:22:36.000000 pyobis-1.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-03-16 11:23:04.466937 pyobis-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-03-16 11:22:36.000000 pyobis-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:23:04.454937 pyobis-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-03-16 11:22:36.000000 pyobis-1.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-16 11:22:36.000000 pyobis-1.3.1/docs/changelog_link.rst
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-16 11:22:36.000000 pyobis-1.3.1/docs/checklist.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-03-16 11:22:36.000000 pyobis-1.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-16 11:22:36.000000 pyobis-1.3.1/docs/dataset.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-03-16 11:22:36.000000 pyobis-1.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-03-16 11:22:36.000000 pyobis-1.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-16 11:22:36.000000 pyobis-1.3.1/docs/nodes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-16 11:22:36.000000 pyobis-1.3.1/docs/occurrences.rst
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-16 11:22:36.000000 pyobis-1.3.1/docs/taxa.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:23:04.462937 pyobis-1.3.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   636046 2023-03-16 11:22:36.000000 pyobis-1.3.1/notebooks/MeasurementOrFact_Analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-16 11:22:36.000000 pyobis-1.3.1/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   504507 2023-03-16 11:22:36.000000 pyobis-1.3.1/notebooks/biodiversity_mapping.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   612201 2023-03-16 11:22:36.000000 pyobis-1.3.1/notebooks/contributions_quantification.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1295057 2023-03-16 11:22:36.000000 pyobis-1.3.1/notebooks/depth_time_series.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   543168 2023-03-16 11:22:36.000000 pyobis-1.3.1/notebooks/migration_patterns.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  2551587 2023-03-16 11:22:36.000000 pyobis-1.3.1/notebooks/occurrences_ocean_sunfish.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1849421 2023-03-16 11:22:36.000000 pyobis-1.3.1/notebooks/usage_guide.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:23:04.462937 pyobis-1.3.1/pyobis/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-16 11:23:04.000000 pyobis-1.3.1/pyobis/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:23:04.466937 pyobis-1.3.1/pyobis/checklist/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/checklist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/checklist/checklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/checklist/test_checklist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:23:04.466937 pyobis-1.3.1/pyobis/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/dataset/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:23:04.466937 pyobis-1.3.1/pyobis/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/nodes/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/nodes/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/obisutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:23:04.466937 pyobis-1.3.1/pyobis/occurrences/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/occurrences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22953 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/occurrences/occurrences.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/occurrences/test_occurrence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:23:04.466937 pyobis-1.3.1/pyobis/taxa/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/taxa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/taxa/taxa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyobis/taxa/test_taxa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:23:04.466937 pyobis-1.3.1/pyobis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-03-16 11:23:04.000000 pyobis-1.3.1/pyobis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-16 11:23:04.000000 pyobis-1.3.1/pyobis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 11:23:04.000000 pyobis-1.3.1/pyobis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-16 11:23:04.000000 pyobis-1.3.1/pyobis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 11:23:04.000000 pyobis-1.3.1/pyobis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-16 11:22:36.000000 pyobis-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-16 11:22:36.000000 pyobis-1.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-16 11:22:36.000000 pyobis-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-16 11:23:04.466937 pyobis-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-16 11:22:36.000000 pyobis-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.469058 pyobis-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.441057 pyobis-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.445057 pyobis-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-09 07:19:09.000000 pyobis-1.4.0/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-09 07:19:09.000000 pyobis-1.4.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-09 07:19:09.000000 pyobis-1.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-09 07:19:09.000000 pyobis-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-09 07:19:09.000000 pyobis-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-09 07:19:09.000000 pyobis-1.4.0/CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-09 07:19:09.000000 pyobis-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-09 07:19:09.000000 pyobis-1.4.0/Changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-09 07:19:09.000000 pyobis-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-09 07:19:09.000000 pyobis-1.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-09 07:19:40.473058 pyobis-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-09 07:19:09.000000 pyobis-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.445057 pyobis-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-09 07:19:09.000000 pyobis-1.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 07:19:09.000000 pyobis-1.4.0/docs/changelog_link.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-09 07:19:09.000000 pyobis-1.4.0/docs/checklist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-05-09 07:19:09.000000 pyobis-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-09 07:19:09.000000 pyobis-1.4.0/docs/dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-09 07:19:09.000000 pyobis-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-09 07:19:09.000000 pyobis-1.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 07:19:09.000000 pyobis-1.4.0/docs/nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-09 07:19:09.000000 pyobis-1.4.0/docs/occurrences.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-09 07:19:09.000000 pyobis-1.4.0/docs/taxa.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.453057 pyobis-1.4.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   636046 2023-05-09 07:19:09.000000 pyobis-1.4.0/notebooks/MeasurementOrFact_Analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-09 07:19:09.000000 pyobis-1.4.0/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   504507 2023-05-09 07:19:09.000000 pyobis-1.4.0/notebooks/biodiversity_mapping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   612201 2023-05-09 07:19:09.000000 pyobis-1.4.0/notebooks/contributions_quantification.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1295057 2023-05-09 07:19:09.000000 pyobis-1.4.0/notebooks/depth_time_series.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   543168 2023-05-09 07:19:09.000000 pyobis-1.4.0/notebooks/migration_patterns.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  2551587 2023-05-09 07:19:09.000000 pyobis-1.4.0/notebooks/occurrences_ocean_sunfish.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1849421 2023-05-09 07:19:09.000000 pyobis-1.4.0/notebooks/usage_guide.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.457057 pyobis-1.4.0/pyobis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 07:19:40.000000 pyobis-1.4.0/pyobis/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.457057 pyobis-1.4.0/pyobis/checklist/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/checklist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.457057 pyobis-1.4.0/pyobis/checklist/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/checklist/cassettes/test_checklist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/checklist/cassettes/test_checklist_newest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/checklist/cassettes/test_checklist_redlist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/checklist/checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/checklist/test_checklist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.457057 pyobis-1.4.0/pyobis/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.457057 pyobis-1.4.0/pyobis/dataset/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/dataset/cassettes/test_dataset_get_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/dataset/cassettes/test_dataset_get_url.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   257668 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/dataset/cassettes/test_dataset_search_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   257508 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/dataset/cassettes/test_dataset_search_url.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/dataset/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.461058 pyobis-1.4.0/pyobis/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.461058 pyobis-1.4.0/pyobis/nodes/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/nodes/cassettes/test_nodes_activities_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/nodes/cassettes/test_nodes_activities_url.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    92872 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/nodes/cassettes/test_nodes_search_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    94675 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/nodes/cassettes/test_nodes_search_url.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/nodes/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/nodes/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/obisutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.461058 pyobis-1.4.0/pyobis/occurrences/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/occurrences/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.469058 pyobis-1.4.0/pyobis/occurrences/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)   141345 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/occurrences/cassettes/test_occurrence_search_mof.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/occurrences/cassettes/test_occurrences_centroid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/occurrences/cassettes/test_occurrences_get.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   623116 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/occurrences/cassettes/test_occurrences_getpoints.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   593383 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/occurrences/cassettes/test_occurrences_grid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/occurrences/cassettes/test_occurrences_point.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)  4791387 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/occurrences/cassettes/test_occurrences_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/occurrences/cassettes/test_occurrences_search_61.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    79145 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/occurrences/cassettes/test_occurrences_tile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    25265 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/occurrences/occurrences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/occurrences/test_occurrence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.469058 pyobis-1.4.0/pyobis/taxa/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/taxa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.469058 pyobis-1.4.0/pyobis/taxa/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/taxa/cassettes/test_taxa_annotations_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/taxa/cassettes/test_taxa_annotations_url.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/taxa/cassettes/test_taxa_search_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/taxa/cassettes/test_taxa_search_url.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/taxa/cassettes/test_taxa_taxon_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/taxa/cassettes/test_taxa_taxon_url.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/taxa/taxa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyobis/taxa/test_taxa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:19:40.457057 pyobis-1.4.0/pyobis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-09 07:19:40.000000 pyobis-1.4.0/pyobis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-09 07:19:40.000000 pyobis-1.4.0/pyobis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:19:40.000000 pyobis-1.4.0/pyobis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 07:19:40.000000 pyobis-1.4.0/pyobis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 07:19:40.000000 pyobis-1.4.0/pyobis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-09 07:19:09.000000 pyobis-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-09 07:19:09.000000 pyobis-1.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 07:19:09.000000 pyobis-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-09 07:19:40.473058 pyobis-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-09 07:19:09.000000 pyobis-1.4.0/setup.py
```

### Comparing `pyobis-1.3.1/.github/workflows/deploy-docs.yml` & `pyobis-1.4.0/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/.github/workflows/pypi.yml` & `pyobis-1.4.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/.github/workflows/tests.yml` & `pyobis-1.4.0/.github/workflows/tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -11,23 +11,24 @@
         os: [windows-latest, ubuntu-latest, macos-latest]
       fail-fast: false
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Setup Micromamba
-      uses: mamba-org/provision-with-micromamba@v14
+      uses: mamba-org/provision-with-micromamba@v15
       with:
         environment-file: false
 
     - name: Install on Python ${{ matrix.python-version }}
       shell: bash -l {0}
       run: |
         micromamba create --name TEST python=${{ matrix.python-version }} --file requirements.txt --file requirements-dev.txt --channel conda-forge
         micromamba activate TEST
         python -m pip install -e . --no-deps --force-reinstall
 
     - name: Run Unit Tests
       shell: bash -l {0}
       run: |
         micromamba activate TEST
-        python -m pytest -rxs --cov=pyobis ./pyobis
+        # use --vcr-record=all when recording new cassettes. We never record on CIs though
+        python -m pytest -rxs --cov=pyobis ./pyobis --vcr-record=none
```

### Comparing `pyobis-1.3.1/.pre-commit-config.yaml` & `pyobis-1.4.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -18,28 +18,28 @@
   rev: 6.0.0
   hooks:
     - id: flake8
       exclude: ^(docs/source/conf.py|pyobis/obisissues.py)
       args: [--max-line-length=105]
 
 - repo: https://github.com/pycqa/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
     - id: isort
       additional_dependencies: [toml]
       args: ["--profile", "black", "--filter-files"]
 
 - repo: https://github.com/psf/black
-  rev: 22.10.0
+  rev: 23.3.0
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v0.991
+  rev: v1.2.0
   hooks:
   - id: mypy
     exclude: docs/source/conf.py
     entry: bash -c 'exec env CONDA_PREFIX="$(python -c "import sys; print(sys.executable)")"'
     args: ["--ignore-missing-imports", "--python-executable=CONDA_PREFIX"]
 
 - repo: https://github.com/keewis/blackdoc
@@ -62,22 +62,22 @@
 #           (?x)^(
 #               .*\.yaml
 #           )$
 #       args:
 #         - --quiet-level=2
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.0
+  rev: v3.3.2
   hooks:
     - id: pyupgrade
       args:
         - --py36-plus
 
 - repo: https://github.com/asottile/add-trailing-comma
-  rev: v2.3.0
+  rev: v2.4.0
   hooks:
     - id: add-trailing-comma
 
 # - repo: https://github.com/pycqa/pydocstyle
 #   rev: 6.1.1
 #   hooks:
 #     - id: pydocstyle
```

### Comparing `pyobis-1.3.1/CONDUCT.md` & `pyobis-1.4.0/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/CONTRIBUTING.md` & `pyobis-1.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/Changelog.rst` & `pyobis-1.4.0/Changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+1.4.0 (2023-04-11)
+-----------------------
+- MAJOR:
+    - none
+- MINOR:
+    - enables request size and time estimation in `occurrences.search()` method. #127
+- PATCH:
+    - fixes "missing 'id' error" in non-paginated queries. #127
+
 1.3.1 (2023-03-03)
 -----------------------
 - MAJOR:
     - none
 - MINOR:
     - none
 - PATCH:
```

### Comparing `pyobis-1.3.1/LICENSE` & `pyobis-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/PKG-INFO` & `pyobis-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobis
-Version: 1.3.1
+Version: 1.4.0
 Summary: Python client for OBIS
 Home-page: https://github.com/iobis/pyobis
 Author: pyOBIS Community
 Author-email: pyobis-mailing-list@googlegroups.com
 License: MIT
 Project-URL: Documentation, https://iobis.github.io/pyobis
 Project-URL: Bug Tracker, https://github.com/iobis/pyobis
```

### Comparing `pyobis-1.3.1/README.md` & `pyobis-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/docs/Makefile` & `pyobis-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/docs/conf.py` & `pyobis-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/docs/index.rst` & `pyobis-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/docs/make.bat` & `pyobis-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/docs/occurrences.rst` & `pyobis-1.4.0/docs/occurrences.rst`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/docs/taxa.rst` & `pyobis-1.4.0/docs/taxa.rst`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/notebooks/MeasurementOrFact_Analysis.ipynb` & `pyobis-1.4.0/notebooks/MeasurementOrFact_Analysis.ipynb`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/notebooks/README.md` & `pyobis-1.4.0/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/notebooks/biodiversity_mapping.ipynb` & `pyobis-1.4.0/notebooks/biodiversity_mapping.ipynb`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/notebooks/contributions_quantification.ipynb` & `pyobis-1.4.0/notebooks/contributions_quantification.ipynb`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/notebooks/depth_time_series.ipynb` & `pyobis-1.4.0/notebooks/depth_time_series.ipynb`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/notebooks/migration_patterns.ipynb` & `pyobis-1.4.0/notebooks/migration_patterns.ipynb`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/notebooks/occurrences_ocean_sunfish.ipynb` & `pyobis-1.4.0/notebooks/occurrences_ocean_sunfish.ipynb`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/notebooks/usage_guide.ipynb` & `pyobis-1.4.0/notebooks/usage_guide.ipynb`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/pyobis/__init__.py` & `pyobis-1.4.0/pyobis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/pyobis/checklist/checklist.py` & `pyobis-1.4.0/pyobis/checklist/checklist.py`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/pyobis/checklist/test_checklist.py` & `pyobis-1.4.0/pyobis/checklist/test_checklist.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Tests for checklist module"""
+import pytest
 import requests
 
 from pyobis import checklist
 
 
+@pytest.mark.vcr()
 def test_checklist():
     """
     checklist.list - basic test for data, check type, size and other methods
     """
     query = checklist.list(scientificname="Mola mola")
     assert not query.data
     query.execute()
@@ -15,14 +17,15 @@
     assert 2 == len(query.data)
     assert dict == query.data["results"][0].__class__
     assert int == query.data["results"][0]["taxonID"].__class__
     assert "Mola mola" == query.data["results"][0]["species"]
     assert requests.get(query.api_url).status_code == 200
 
 
+@pytest.mark.vcr()
 def test_checklist_redlist():
     """
     checklist.redlist - basic test for data, check type, size and other methods
     """
     query = checklist.redlist(scientificname="Mola mola")
     assert not query.data
     query.execute()
@@ -30,14 +33,15 @@
     assert 2 == len(query.data)
     assert dict == query.data["results"][0].__class__
     assert int == query.data["results"][0]["taxonID"].__class__
     assert "Mola mola" == query.data["results"][0]["species"]
     assert requests.get(query.api_url).status_code == 200
 
 
+@pytest.mark.vcr()
 def test_checklist_newest():
     """
     checklist.newest - basic test for data, check type, size and other methods
     """
     query = checklist.newest(scientificname="Mola mola")
     assert not query.data
     query.execute()
```

### Comparing `pyobis-1.3.1/pyobis/dataset/dataset.py` & `pyobis-1.4.0/pyobis/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/pyobis/nodes/nodes.py` & `pyobis-1.4.0/pyobis/nodes/nodes.py`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/pyobis/nodes/test_nodes.py` & `pyobis-1.4.0/pyobis/nodes/test_nodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Tests for nodes module"""
+import pytest
 import requests
 
 from pyobis import nodes
 
 
+@pytest.mark.vcr()
 def test_nodes_search_data():
     """
     nodes.search - test for data, check type, size and other methods
     """
     query = nodes.search(id="4bf79a01-65a9-4db6-b37b-18434f26ddfc")
     assert not query.data
     query.execute()
@@ -15,24 +17,26 @@
     assert 2 == len(query.data)
     assert dict == query.data["results"][0].__class__
     assert str == str(query.data["results"][0]["description"]).__class__
     assert str == query.data["results"][0]["id"].__class__
     assert query.to_pandas().__class__.__name__ == "DataFrame"
 
 
+@pytest.mark.vcr()
 def test_nodes_search_url():
     """
     nodes.activities - basic test for url, url are accessible and
     mapper_url correct for supported methods
     """
     query = nodes.search(id="4bf79a01-65a9-4db6-b37b-18434f26ddfc")
     assert requests.get(query.api_url).status_code == 200
     assert requests.get(query.mapper_url).status_code == 200
 
 
+@pytest.mark.vcr()
 def test_nodes_activities_data():
     """
     nodes.activities - basic test for data, check type, size and other methods
     """
     query = nodes.activities(id="4bf79a01-65a9-4db6-b37b-18434f26ddfc")
     assert not query.data
     query.execute()
@@ -40,14 +44,15 @@
     assert 2 == len(query.data)
     assert dict == query.data["results"][0].__class__
     assert str == str(query.data["results"][0]["description"]).__class__
     assert str == query.data["results"][0]["id"].__class__
     assert query.to_pandas().__class__.__name__ == "DataFrame"
 
 
+@pytest.mark.vcr()
 def test_nodes_activities_url():
     """
     nodes.activities - basic test for url, url are accessible and
     mapper_url correct for supported methods
     """
     query = nodes.activities(id="4bf79a01-65a9-4db6-b37b-18434f26ddfc")
     assert requests.get(query.api_url).status_code == 200
```

### Comparing `pyobis-1.3.1/pyobis/obisutils.py` & `pyobis-1.4.0/pyobis/obisutils.py`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/pyobis/occurrences/occurrences.py` & `pyobis-1.4.0/pyobis/occurrences/occurrences.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 /occurrences/ API endpoints as documented on https://api.obis.org/.
 """
 
 import json
 import sys
+import warnings
+from time import time
 from urllib.parse import urlencode
 
 import pandas as pd
 import requests
 
 from ..obisutils import (
     build_api_url,
@@ -20,15 +22,15 @@
 
 class OccResponse:
     """
     An OBIS Occurrence response class
     """
 
     def __init__(self, url, args, isSearch, hasMapper, isKML):
-        """ "
+        """
         Initialise the object parameters
         """
         self.data = None
         self.api_url = build_api_url(url, args)
         self.mapper_url = None
         if hasMapper:
             if not args["taxonid"] and args["scientificname"]:
@@ -44,46 +46,76 @@
 
         # private members
         self.__args = args
         self.__url = url
         self.__isSearch = isSearch
         self.__isKML = isKML
 
+        # fetch the total length of records
+        if not self.__isKML:
+            starting_time = time()
+            self.__out_head_record = obis_GET(
+                self.__url,
+                {**self.__args, **{"size": 1}},
+                "application/json; charset=utf-8",
+            )
+            ending_time = time()
+            if "total" in self.__out_head_record:
+                self.__total_records = (
+                    self.__out_head_record["total"]
+                    if "size" not in self.__args or not self.__args["size"]
+                    else self.__args["size"]
+                )
+                # a simple calculation gives us the total expected time
+                # nearly for all requests of size 1, the server takes up 99.5% of the time
+                # to respond, and it takes only 0.5% of the time for network download. So
+                # the total time can be estimated easily although this might not be accurate
+                # for larger than 100k records, because the network download takes
+                # even smaller fraction of the total round-trip time
+                print(
+                    f"{self.__total_records} to be fetched. Estimated time = ",
+                    (ending_time - starting_time) * 0.995,
+                    f" {(ending_time - starting_time) * 0.005 * self.__total_records:.0f} ",
+                    "seconds",
+                )
+
     def execute(self, **kwargs):
         """
         Execute or fetch the data based on the query
         """
         if not self.__isSearch and not self.__isKML:
             out = obis_GET(
                 self.__url, self.__args, "application/json; charset=utf-8", **kwargs
             )
+            self.data = out
 
         elif self.__isKML:
-            print("hello")
             out = requests.get(self.__url, params=self.__args, **kwargs)
             out.raise_for_status()
             out = out.content
+            self.data = out
 
         elif self.__isSearch:
             # setting default parameters from arguments list
             mof = self.__args["mof"]
             size = self.__args["size"]
 
-            self.__args["size"] = 1
-            out = obis_GET(
-                self.__url, self.__args, "application/json; charset=utf-8", **kwargs
-            )
             size = (
-                out["total"] if not size else size
+                self.__total_records if not size else size
             )  # if the user has set some size or else we fetch all the records
 
-            outdf = pd.DataFrame(columns=pd.DataFrame(out["results"]).columns)
+            outdf = pd.DataFrame(
+                columns=pd.DataFrame(self.__out_head_record["results"]).columns,
+            )
 
-            for i in range(5000, size + 1, 5000):
-                self.__args["size"] = 5000
+            for i in range(10000, size + 1, 10000):
+                # if there is no 'id' then there should be no pagination
+                if "id" not in outdf.columns:
+                    break
+                self.__args["size"] = 10000
                 print(
                     "{}[{}{}] {}/{}".format(
                         "Fetching: ",
                         "█" * int((i - 1) * 100 / size),
                         "." * (100 - int((i + 1) * 100 / size)),
                         i,
                         size,
@@ -101,15 +133,15 @@
                         pd.DataFrame(res["results"]).infer_objects(),
                     ],
                     ignore_index=True,
                 )
                 # make sure that we set the `after` parameter when fetching subsequent records
                 self.__args["after"] = outdf["id"].iloc[-1]
 
-            self.__args["size"] = size % 5000
+            self.__args["size"] = size % 10000
             # we have already fetched records as a set of 5000 records each time,
             # now we need to get remaining records from the total
             print(
                 "{}[{}{}] {}/{}".format("Fetching: ", "█" * 100, "." * 0, size, size),
                 end="\r",
                 file=sys.stdout,
                 flush=True,
@@ -119,31 +151,30 @@
             )
             outdf = pd.concat(
                 [outdf.infer_objects(), pd.DataFrame(res["results"]).infer_objects()],
                 ignore_index=True,
             )
             print(f"\nFetched {size} records.")
 
-            if mof and out["total"] > 0:
+            if mof and self.__total_records > 0:
                 mofNormalized = pd.json_normalize(
                     json.loads(outdf.to_json(orient="records")),
                     "mof",
                     ["id"],
                 )
                 merged = pd.merge(
                     outdf,
                     mofNormalized,
                     on="id",
                     how="inner",
                 )
                 self.data = merged
                 return self.data
             self.data = outdf
-            return self.data
-        self.data = out
+
         return self.data
 
     def to_pandas(self):
         """
         Convert the results into a pandas DataFrame
         """
         return pd.DataFrame(self.data["results"])
@@ -166,15 +197,21 @@
         q1.data # get the data
         q1.api_url # get the API url
 
     """
     url = obis_baseurl + "occurrence/" + str(id)
     args = {}
 
-    return OccResponse(url, {**args,**kwargs}, isSearch=False, hasMapper=False, isKML=False)
+    return OccResponse(
+        url,
+        {**args, **kwargs},
+        isSearch=False,
+        hasMapper=False,
+        isKML=False,
+    )
 
 
 def search(
     scientificname=None,
     taxonid=None,
     nodeid=None,
     datasetid=None,
@@ -214,15 +251,16 @@
     :param startdate: [Fixnum] Start date, formatted as YYYY-MM-DD
     :param enddate: [Boolean] End date, formatted as YYYY-MM-DD
     :param startdepth: [Fixnum] Start depth, in meters. Depth below sea level are treated
         as positive numbers.
     :param enddepth: [Boolean] End depth, in meters. Depth below sea level are treated
         as positive numbers.
     :param flags: Prev. qc [String] Quality control flags
-    :param fields: [String] Comma seperated list of field names
+    :param fields: [String] Comma seperated list of field names. Leave blank to include all.
+        For fetching records more than 10k, must specify 'id' explicitly too.
     :param size: [Fixnum] Number of results to return. Default: All records
     :param offset: [Fixnum] Start at record. Default: 0
     :param mof: [Boolean] Include MeasurementOrFact records, true/false.
         Default: 0
     :param hasextensions: [String] Extensions that need to be present
         (e.g. MeasurementOrFact, DNADerivedData).
     :return: A dictionary
@@ -265,14 +303,19 @@
         occurrences.search(
             scientificname="Abra", mof=True, hasextensions="MeasurementOrFact", size=100
             ).execute()
     """
     url = obis_baseurl + "occurrence"
     scientificname = handle_arrstr(scientificname)
     taxonid = handle_arrint(taxonid)
+    if fields and "id" not in fields:
+        warnings.warn(
+            "You have specified custom fields but 'id' is not included. \
+            Include 'id' explicitly in the fields or else only upto 10,000 records will be fetched.",
+        )
     args = {
         "taxonid": taxonid,
         "nodeid": nodeid,
         "datasetid": datasetid,
         "scientificname": scientificname,
         "startdate": startdate,
         "enddate": enddate,
@@ -283,15 +326,21 @@
         "fields": fields,
         "flags": flags,
         "offset": offset,
         "mof": mof,
         "size": size,
         "hasextensions": hasextensions,
     }
-    return OccResponse(url, {**args,**kwargs}, isSearch=True, hasMapper=True, isKML=False)
+    return OccResponse(
+        url,
+        {**args, **kwargs},
+        isSearch=True,
+        hasMapper=True,
+        isKML=False,
+    )
 
 
 def grid(
     precision,
     geojson=True,
     scientificname=None,
     taxonid=None,
@@ -362,17 +411,29 @@
         "wrims": wrims,
         "event": event,
         "flags": flags,
         "exclude": exclude,
     }
     if not geojson:
         url += "/kml"
-        return OccResponse(url, {**args,**kwargs}, isSearch=False, hasMapper=False, isKML=True)
-
-    return OccResponse(url, {**args,**kwargs}, isSearch=False, hasMapper=False, isKML=False)
+        return OccResponse(
+            url,
+            {**args, **kwargs},
+            isSearch=False,
+            hasMapper=False,
+            isKML=True,
+        )
+
+    return OccResponse(
+        url,
+        {**args, **kwargs},
+        isSearch=False,
+        hasMapper=False,
+        isKML=False,
+    )
 
 
 def getpoints(
     scientificname=None,
     taxonid=None,
     datasetid=None,
     nodeid=None,
@@ -441,15 +502,21 @@
         "hab": hab,
         "wrims": wrims,
         "event": event,
         "flags": flags,
         "exclude": exclude,
     }
 
-    return OccResponse(url, {**args, **kwargs}, isSearch=False, hasMapper=False, isKML=False)
+    return OccResponse(
+        url,
+        {**args, **kwargs},
+        isSearch=False,
+        hasMapper=False,
+        isKML=False,
+    )
 
 
 def point(
     x,
     y,
     z=None,
     scientificname=None,
@@ -524,15 +591,21 @@
         "hab": hab,
         "wrims": wrims,
         "event": event,
         "flags": flags,
         "exclude": exclude,
     }
 
-    return OccResponse(url, {**args,**kwargs}, isSearch=False, hasMapper=False, isKML=False)
+    return OccResponse(
+        url,
+        {**args, **kwargs},
+        isSearch=False,
+        hasMapper=False,
+        isKML=False,
+    )
 
 
 def tile(
     x,
     y,
     z,
     mvt=0,
@@ -608,17 +681,29 @@
         "wrims": wrims,
         "event": event,
         "flags": flags,
         "exclude": exclude,
     }
     if mvt:
         url += ".mvt"
-        return OccResponse(url, {**args,**kwargs}, isSearch=False, hasMapper=False, isKML=True)
-
-    return OccResponse(url, {**args,**kwargs}, isSearch=False, hasMapper=False, isKML=False)
+        return OccResponse(
+            url,
+            {**args, **kwargs},
+            isSearch=False,
+            hasMapper=False,
+            isKML=True,
+        )
+
+    return OccResponse(
+        url,
+        {**args, **kwargs},
+        isSearch=False,
+        hasMapper=False,
+        isKML=False,
+    )
 
 
 def centroid(
     scientificname=None,
     taxonid=None,
     datasetid=None,
     nodeid=None,
@@ -683,15 +768,21 @@
         "hab": hab,
         "wrims": wrims,
         "event": event,
         "flags": flags,
         "exclude": exclude,
     }
 
-    return OccResponse(url, {**args,**kwargs}, isSearch=False, hasMapper=False, isKML=False)
+    return OccResponse(
+        url,
+        {**args, **kwargs},
+        isSearch=False,
+        hasMapper=False,
+        isKML=False,
+    )
 
 
 def lookup_taxon(scientificname):
     """
     Lookup for taxon metadata with scientificname
 
     :param scientificname: [String] Scientific Name
```

### Comparing `pyobis-1.3.1/pyobis/occurrences/test_occurrence.py` & `pyobis-1.4.0/pyobis/occurrences/test_occurrence.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Tests for occurrences module methods"""
+import pytest
 import requests
 
 from pyobis import occurrences
 
 
+@pytest.mark.vcr()
 def test_occurrences_search():
     """
     occurrences.search - basic test for data, check type, size and other methods
     """
     size = 10100
     query = occurrences.search(scientificname="Mola mola", size=size)
     assert not query.data  # the data is none after query building but before executing
     query.execute()
     assert size == len(query.data)
     assert "Mola mola" == query.data.scientificName[0]
 
 
+@pytest.mark.vcr()
 def test_occurrence_search_mof():
     """
     occurrences.search - basic test for data with MoF extension, check type, size and other methods
     """
     query = occurrences.search(
         scientificname="Abra alba",
         mof=True,
@@ -29,14 +32,15 @@
     assert not query.data
     query.execute()
     assert "Abra alba" == query.data.scientificName[0]
     assert requests.get(query.api_url).status_code == 200
     assert requests.get(query.mapper_url).status_code == 200
 
 
+@pytest.mark.vcr()
 def test_occurrences_search_61():
     """
     Search returns same object-type regardless of mof=True or mof=False.
     Tests for https://github.com/iobis/pyobis/issues/61.
     """
     TEST_QUERY = dict(
         scientificname="Mola mola",
@@ -44,28 +48,30 @@
     )
     q1 = occurrences.search(mof=True, **TEST_QUERY).execute()
     q2 = occurrences.search(mof=False, **TEST_QUERY).execute()
 
     assert type(q1) == type(q2)
 
 
+@pytest.mark.vcr()
 def test_occurrences_get():
     """
     occurrences.get - basic test for data, check type, size and other methods
     """
-    query = occurrences.get(id=occurrences.search(size=1).execute()['id'].values[0])
+    query = occurrences.get(id=occurrences.search(size=1).execute()["id"].values[0])
     assert not query.data
     query.execute()
     assert "dict" == query.data.__class__.__name__
     assert 2 == len(query.data)
     assert list == list(query.data.keys()).__class__
     assert requests.get(query.api_url).status_code == 200
     assert query.to_pandas().__class__.__name__ == "DataFrame"
 
 
+@pytest.mark.vcr()
 def test_occurrences_grid():
     """
     occurrences.grid - basic test for data, check type, size and other methods
     """
     query = occurrences.grid(5, geojson=True, scientificname="Abra alba")
     assert not query.data
     query.execute()
@@ -73,42 +79,45 @@
     assert 2 == len(query.data)
     assert list == list(query.data.keys()).__class__
     query = occurrences.grid(5, geojson=False, scientificname="Mola mola")
     assert requests.get(query.api_url).status_code == 200
     assert not query.mapper_url
 
 
+@pytest.mark.vcr()
 def test_occurrences_getpoints():
     """
     occurrences.getpoints - basic test for data, check type, size and other methods
     """
     query = occurrences.getpoints(scientificname=["Mola mola", "Abra alba"])
     assert not query.data
     query.execute()
     assert "dict" == query.data.__class__.__name__
     assert 2 == len(query.data)
     assert list == list(query.data.keys()).__class__
     assert requests.get(query.api_url).status_code == 200
     assert not query.mapper_url
 
 
+@pytest.mark.vcr()
 def test_occurrences_point():
     """
     occurrences.point - basic test for data, check type, size and other methods
     """
     query = occurrences.point(x=1.77, y=54.22, scientificname="Mola mola")
     assert not query.data
     query.execute()
     assert "dict" == query.data.__class__.__name__
     assert 2 == len(query.data)
     assert list == list(query.data.keys()).__class__
     assert requests.get(query.api_url).status_code == 200
     assert not query.mapper_url
 
 
+@pytest.mark.vcr()
 def test_occurrences_tile():
     """
     occurrences.tile - basic test for data, check type, size and other methods
     """
     query = occurrences.tile(x=1.77, y=52.26, z=0.5, mvt=0, scientificname="Mola mola")
     assert not query.data
     query.execute()
@@ -120,14 +129,15 @@
     assert requests.get(query.api_url).status_code == 200
     query = occurrences.tile(x=1.77, y=52.26, z=0.5, mvt=0, scientificname="Mola mola")
     query.execute()
     assert requests.get(query.api_url).status_code == 200
     assert not query.mapper_url
 
 
+@pytest.mark.vcr()
 def test_occurrences_centroid():
     """
     occurrences.centroid - basic test for data, check type, size and other methods
     """
     query = occurrences.centroid(scientificname="Mola mola")
     assert not query.data
     query.execute()
```

### Comparing `pyobis-1.3.1/pyobis/taxa/taxa.py` & `pyobis-1.4.0/pyobis/taxa/taxa.py`

 * *Files identical despite different names*

### Comparing `pyobis-1.3.1/pyobis/taxa/test_taxa.py` & `pyobis-1.4.0/pyobis/taxa/test_taxa.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,79 @@
 """Tests for taxa module - search methods"""
+import pytest
 import requests
 
 from pyobis import taxa
 
 
+@pytest.mark.vcr()
 def test_taxa_search_data():
     """
     taxa.search - basic test for data, check type, size and other methods
     """
     query = taxa.search(scientificname="Mola mola")
     assert not query.data  # the data is none after query building but before executing
     query.execute()
     assert "dict" == query.data.__class__.__name__
     assert list == list(query.data.keys()).__class__
     assert 2 == len(query.data)
 
 
+@pytest.mark.vcr()
 def test_taxa_search_url():
     """
     taxa.search - basic test for url, url are accessible and
     mapper_url is None for unsupported methods
     """
     query = taxa.search(scientificname="Mola mola")
     assert requests.get(query.api_url).status_code == 200
     assert not query.mapper_url
 
 
+@pytest.mark.vcr()
 def test_taxa_taxon_data():
     """
     taxa.taxon - basic test for data, check type, size and other methods
     """
     query = taxa.taxon(545439)
     assert not query.data
     query.execute()
     assert dict == query.data.__class__
     assert 2 == len(query.data)
     assert list == list(query.data.keys()).__class__
     assert 545439 == query.data["results"][0]["taxonID"]
     assert query.to_pandas().__class__.__name__ == "DataFrame"
 
 
+@pytest.mark.vcr()
 def test_taxa_taxon_url():
     """
     taxa.taxon - basic test for url, url are accessible and
     mapper_url is None for unsupported methods
     """
     query = taxa.taxon(545439)
     assert requests.get(query.api_url).status_code == 200
     assert not query.mapper_url
 
 
+@pytest.mark.vcr()
 def test_taxa_annotations_data():
     """
     taxa.annotations - basic test for data, check type, size and other methods
     """
     query = taxa.annotations(scientificname="Abra")
     assert not query.data
     query.execute()
     assert dict == query.data.__class__
     assert 2 == len(query.data)
     assert list == list(query.data.keys()).__class__
     assert query.to_pandas().__class__.__name__ == "DataFrame"
 
 
+@pytest.mark.vcr()
 def test_taxa_annotations_url():
     """
     taxa.annotations - basic test for url, url are accessible and
     mapper_url is None for unsupported methods
     """
     query = taxa.annotations(scientificname="Abra")
     assert requests.get(query.api_url).status_code == 200
```

### Comparing `pyobis-1.3.1/pyobis.egg-info/PKG-INFO` & `pyobis-1.4.0/pyobis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobis
-Version: 1.3.1
+Version: 1.4.0
 Summary: Python client for OBIS
 Home-page: https://github.com/iobis/pyobis
 Author: pyOBIS Community
 Author-email: pyobis-mailing-list@googlegroups.com
 License: MIT
 Project-URL: Documentation, https://iobis.github.io/pyobis
 Project-URL: Bug Tracker, https://github.com/iobis/pyobis
```

### Comparing `pyobis-1.3.1/setup.cfg` & `pyobis-1.4.0/setup.cfg`

 * *Files identical despite different names*

