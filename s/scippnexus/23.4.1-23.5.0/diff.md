# Comparing `tmp/scippnexus-23.4.1.tar.gz` & `tmp/scippnexus-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scippnexus-23.4.1.tar", last modified: Tue Apr 25 05:46:29 2023, max compression
+gzip compressed data, was "scippnexus-23.5.0.tar", last modified: Tue May  9 04:46:44 2023, max compression
```

## Comparing `scippnexus-23.4.1.tar` & `scippnexus-23.5.0.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.400649 scippnexus-23.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-25 05:46:13.000000 scippnexus-23.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-04-25 05:46:13.000000 scippnexus-23.4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1989 2023-04-25 05:46:13.000000 scippnexus-23.4.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-04-25 05:46:13.000000 scippnexus-23.4.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-25 05:46:13.000000 scippnexus-23.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-04-25 05:46:13.000000 scippnexus-23.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-25 05:46:13.000000 scippnexus-23.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-25 05:46:13.000000 scippnexus-23.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-25 05:46:29.400649 scippnexus-23.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-04-25 05:46:13.000000 scippnexus-23.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/conda/
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-04-25 05:46:13.000000 scippnexus-23.4.1/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    17823 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/_static/logo-2022.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/_templates/scipp-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/_templates/scipp-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/_templates/sections/header-article.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/about/
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6546 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/about/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8453 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/getting-started/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10348 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/getting-started/quick-start-guide.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (122)     9320 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/user-guide/application-definitions.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/user-guide/classes.rst
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/user-guide/functions.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11308 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/user-guide/nexus-classes.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4037 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/version.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-25 05:46:13.000000 scippnexus-23.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.392649 scippnexus-23.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      572 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.392649 scippnexus-23.4.1/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    70398 2023-04-25 05:46:13.000000 scippnexus-23.4.1/resources/logo-2022.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-25 05:46:29.400649 scippnexus-23.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.384649 scippnexus-23.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus/
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/_hdf5_nexus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus/data/
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      876 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus/definitions/
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/definitions/nxcansas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7424 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md
--rw-r--r--   0 runner    (1001) docker     (122)      941 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/file.py
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/leaf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nexus_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxcylindrical_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)    11291 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     9912 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxdetector.py
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxdisk_chopper.py
--rw-r--r--   0 runner    (1001) docker     (122)     5064 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxevent_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxfermi_chopper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2419 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxlog.py
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxmonitor.py
--rw-r--r--   0 runner    (1001) docker     (122)    24870 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxobject.py
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxoff_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxsample.py
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxsource.py
--rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxtransformations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus/v2/
--rw-r--r--   0 runner    (1001) docker     (122)      613 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.384649 scippnexus-23.4.1/src/scippnexus/v2/application_definitions/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus/v2/application_definitions/nxcansas/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/application_definitions/nxcansas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4970 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/attrs.py
--rw-r--r--   0 runner    (1001) docker     (122)    18014 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8974 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/field.py
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/file.py
--rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nexus_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3137 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nxcylindrical_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)    22638 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nxdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     6001 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nxevent_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nxoff_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nxsample.py
--rw-r--r--   0 runner    (1001) docker     (122)     8552 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nxtransformations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-25 05:46:29.000000 scippnexus-23.4.1/src/scippnexus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2805 2023-04-25 05:46:29.000000 scippnexus-23.4.1/src/scippnexus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 05:46:29.000000 scippnexus-23.4.1/src/scippnexus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-25 05:46:29.000000 scippnexus-23.4.1/src/scippnexus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-25 05:46:29.000000 scippnexus-23.4.1/src/scippnexus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.400649 scippnexus-23.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3863 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/application_definition_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/externalfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     3317 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/load_files_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    23629 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nexus_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxcylindrical_geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    26815 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxdata_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    27234 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxdetector_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxevent_data_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxmonitor_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxoff_geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxsample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    18218 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxtransformations_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.790512 scippnexus-23.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.778512 scippnexus-23.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-09 04:46:34.000000 scippnexus-23.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.778512 scippnexus-23.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-05-09 04:46:34.000000 scippnexus-23.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1989 2023-05-09 04:46:34.000000 scippnexus-23.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-05-09 04:46:34.000000 scippnexus-23.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-09 04:46:34.000000 scippnexus-23.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-09 04:46:34.000000 scippnexus-23.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-05-09 04:46:34.000000 scippnexus-23.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-09 04:46:34.000000 scippnexus-23.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-09 04:46:44.790512 scippnexus-23.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-05-09 04:46:34.000000 scippnexus-23.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.778512 scippnexus-23.5.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-05-09 04:46:34.000000 scippnexus-23.5.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    17823 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/_static/logo-2022.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/_templates/scipp-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/_templates/scipp-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/_templates/sections/header-article.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7029 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/about/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8453 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/getting-started/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10348 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/getting-started/quick-start-guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (122)     9320 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/user-guide/application-definitions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/user-guide/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/user-guide/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11308 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/user-guide/nexus-classes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     4037 2023-05-09 04:46:34.000000 scippnexus-23.5.0/docs/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-05-09 04:46:34.000000 scippnexus-23.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-09 04:46:34.000000 scippnexus-23.5.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.782512 scippnexus-23.5.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    70398 2023-05-09 04:46:34.000000 scippnexus-23.5.0/resources/logo-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-09 04:46:44.790512 scippnexus-23.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.778512 scippnexus-23.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.786512 scippnexus-23.5.0/src/scippnexus/
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/_hdf5_nexus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.786512 scippnexus-23.5.0/src/scippnexus/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      876 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.786512 scippnexus-23.5.0/src/scippnexus/definitions/
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/definitions/nxcansas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.786512 scippnexus-23.5.0/src/scippnexus/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7424 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md
+-rw-r--r--   0 runner    (1001) docker     (122)      941 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      911 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/leaf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nexus_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxcylindrical_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11291 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9912 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxdetector.py
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxdisk_chopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5064 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxevent_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxfermi_chopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2419 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxlog.py
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxmonitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24870 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxoff_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxsample.py
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxsource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/nxtransformations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.790512 scippnexus-23.5.0/src/scippnexus/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.778512 scippnexus-23.5.0/src/scippnexus/v2/application_definitions/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.790512 scippnexus-23.5.0/src/scippnexus/v2/application_definitions/nxcansas/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/application_definitions/nxcansas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4970 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18015 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8974 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/field.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nexus_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3137 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nxcylindrical_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26648 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nxdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6001 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nxevent_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nxoff_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nxsample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8552 2023-05-09 04:46:34.000000 scippnexus-23.5.0/src/scippnexus/v2/nxtransformations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.786512 scippnexus-23.5.0/src/scippnexus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-09 04:46:44.000000 scippnexus-23.5.0/src/scippnexus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-05-09 04:46:44.000000 scippnexus-23.5.0/src/scippnexus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 04:46:44.000000 scippnexus-23.5.0/src/scippnexus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-09 04:46:44.000000 scippnexus-23.5.0/src/scippnexus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-09 04:46:44.000000 scippnexus-23.5.0/src/scippnexus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 04:46:44.790512 scippnexus-23.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3863 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/application_definition_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/externalfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3317 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/load_files_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19370 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nexus_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxcylindrical_geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26815 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxdata_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30034 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxdetector_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxevent_data_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8869 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxlog_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxmonitor_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxoff_geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxsample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18218 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tests/nxtransformations_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-05-09 04:46:34.000000 scippnexus-23.5.0/tox.ini
```

### Comparing `scippnexus-23.4.1/.github/workflows/ci.yml` & `scippnexus-23.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/.github/workflows/docs.yml` & `scippnexus-23.5.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/.github/workflows/release.yml` & `scippnexus-23.5.0/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     needs: [build_wheels, build_conda]
     runs-on: ubuntu-20.04
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
       - uses: actions/download-artifact@v2
       - uses: actions/setup-python@v3
-      - uses: pypa/gh-action-pypi-publish@v1.8.5
+      - uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
 
   upload_conda:
     name: Deploy Conda Forge
     needs: [build_wheels, build_conda]
```

### Comparing `scippnexus-23.4.1/.pre-commit-config.yaml` & `scippnexus-23.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/LICENSE` & `scippnexus-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/PKG-INFO` & `scippnexus-23.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scippnexus
-Version: 23.4.1
+Version: 23.5.0
 Summary: h5py-like utility for NeXus files based with seamless scipp integration
 Home-page: https://scipp.github.io/scippnexus
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/scippnexus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `scippnexus-23.4.1/README.md` & `scippnexus-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/conda/meta.yaml` & `scippnexus-23.5.0/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/_static/favicon.ico` & `scippnexus-23.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/_static/logo-2022.svg` & `scippnexus-23.5.0/docs/_static/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/_templates/scipp-class-template.rst` & `scippnexus-23.5.0/docs/_templates/scipp-class-template.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/_templates/scipp-module-template.rst` & `scippnexus-23.5.0/docs/_templates/scipp-module-template.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/_templates/sections/header-article.html` & `scippnexus-23.5.0/docs/_templates/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/about/about.rst` & `scippnexus-23.5.0/docs/about/about.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/about/release-notes.rst` & `scippnexus-23.5.0/docs/about/release-notes.rst`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,28 @@
    Contributors
    ~~~~~~~~~~~~
 
    Simon Heybrock :sup:`a`\ ,
    Neil Vaytet :sup:`a`\ ,
    and Jan-Lukas Wynen :sup:`a`
 
+v23.05.0
+--------
+
+Features
+~~~~~~~~
+
+* ``scippnexus.v2``: Support NXlog with "sublogs" such as connection_status and alarm `#138 <https://github.com/scipp/scippnexus/pull/138>`_.
+* ``scippnexus.v2``: Fall back to dim labels from HDF5 if NeXus does not define labels in NXdata and related classes `#139 <https://github.com/scipp/scippnexus/pull/139>`_.
+
+v23.04.1
+--------
+
+* ``scippnexus.v2``: Fix event selection of length 0 `#137 <https://github.com/scipp/scippnexus/pull/137>`_.
+
 v23.04.0
 --------
 
 Features
 ~~~~~~~~
 
 * Added the future API of ``scippnexus`` as ``scippnexus.v2``.
```

### Comparing `scippnexus-23.4.1/docs/conf.py` & `scippnexus-23.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/getting-started/installation.rst` & `scippnexus-23.5.0/docs/getting-started/installation.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/getting-started/quick-start-guide.ipynb` & `scippnexus-23.5.0/docs/getting-started/quick-start-guide.ipynb`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/index.rst` & `scippnexus-23.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/user-guide/application-definitions.ipynb` & `scippnexus-23.5.0/docs/user-guide/application-definitions.ipynb`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/user-guide/classes.rst` & `scippnexus-23.5.0/docs/user-guide/classes.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/user-guide/nexus-classes.ipynb` & `scippnexus-23.5.0/docs/user-guide/nexus-classes.ipynb`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/docs/version.py` & `scippnexus-23.5.0/docs/version.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/pyproject.toml` & `scippnexus-23.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/requirements/ci.txt` & `scippnexus-23.5.0/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/requirements/docs.txt` & `scippnexus-23.5.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/requirements/static.txt` & `scippnexus-23.5.0/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/resources/logo-2022.svg` & `scippnexus-23.5.0/resources/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/setup.cfg` & `scippnexus-23.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/__init__.py` & `scippnexus-23.5.0/src/scippnexus/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/_common.py` & `scippnexus-23.5.0/src/scippnexus/_common.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/_hdf5_nexus.py` & `scippnexus-23.5.0/src/scippnexus/_hdf5_nexus.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/data/__init__.py` & `scippnexus-23.5.0/src/scippnexus/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/definition.py` & `scippnexus-23.5.0/src/scippnexus/definition.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/definitions/nxcansas.py` & `scippnexus-23.5.0/src/scippnexus/definitions/nxcansas.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md` & `scippnexus-23.5.0/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/file.py` & `scippnexus-23.5.0/src/scippnexus/file.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/leaf.py` & `scippnexus-23.5.0/src/scippnexus/leaf.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/nexus_classes.py` & `scippnexus-23.5.0/src/scippnexus/nexus_classes.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/nxcylindrical_geometry.py` & `scippnexus-23.5.0/src/scippnexus/nxcylindrical_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/nxdata.py` & `scippnexus-23.5.0/src/scippnexus/nxdata.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/nxdetector.py` & `scippnexus-23.5.0/src/scippnexus/nxdetector.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/nxevent_data.py` & `scippnexus-23.5.0/src/scippnexus/nxevent_data.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/nxlog.py` & `scippnexus-23.5.0/src/scippnexus/nxlog.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/nxmonitor.py` & `scippnexus-23.5.0/src/scippnexus/nxmonitor.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/nxobject.py` & `scippnexus-23.5.0/src/scippnexus/nxobject.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/nxoff_geometry.py` & `scippnexus-23.5.0/src/scippnexus/nxoff_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/nxsample.py` & `scippnexus-23.5.0/src/scippnexus/nxsample.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/nxtransformations.py` & `scippnexus-23.5.0/src/scippnexus/nxtransformations.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/typing.py` & `scippnexus-23.5.0/src/scippnexus/typing.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/__init__.py` & `scippnexus-23.5.0/src/scippnexus/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py` & `scippnexus-23.5.0/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/attrs.py` & `scippnexus-23.5.0/src/scippnexus/v2/attrs.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/base.py` & `scippnexus-23.5.0/src/scippnexus/v2/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 
         items = {name: _make_child(obj) for name, obj in self._group.items()}
         # In the case of NXevent_data, the `cue_` fields are unusable, since
         # the definition is broken (the cue_index points into the
         # event_time_offset/event_id fields, instead of the
         # event_time_zero/event_index fields). In the case of NXlog they may
         # be some utility if we deal with extremely long time-series that
-        # could be leverage for label-based indexing in the future.
+        # could be leveraged for label-based indexing in the future.
         items = {k: v for k, v in items.items() if not k.startswith('cue_')}
         for suffix in ('_errors', '_error'):
             field_with_errors = [name for name in items if f'{name}{suffix}' in items]
             for name in field_with_errors:
                 values = items[name]
                 errors = items[f'{name}{suffix}']
                 if (isinstance(values, Field) and isinstance(errors, Field)
```

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/field.py` & `scippnexus-23.5.0/src/scippnexus/v2/field.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/file.py` & `scippnexus-23.5.0/src/scippnexus/v2/file.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/nexus_classes.py` & `scippnexus-23.5.0/src/scippnexus/v2/nexus_classes.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/nxcylindrical_geometry.py` & `scippnexus-23.5.0/src/scippnexus/v2/nxcylindrical_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/nxdata.py` & `scippnexus-23.5.0/src/scippnexus/v2/nxdata.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import uuid
 from functools import cached_property
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import scipp as sc
 
-from .._common import convert_time_to_datetime64, to_child_select
+from .._common import _to_canonical_select, convert_time_to_datetime64, to_child_select
 from ..typing import H5Dataset, ScippIndex
 from .base import (
     Group,
     NexusStructureError,
     NXobject,
     asvariable,
     base_definitions_dict,
@@ -213,28 +213,32 @@
 
         indices_suffix = '_indices'
         indices_attrs = {
             key[:-len(indices_suffix)]: attr
             for key, attr in attrs.items() if key.endswith(indices_suffix)
         }
 
-        dims = np.array(group_dims)
+        dims = np.array(self._axes)
         self._dims_from_indices = {
             key: tuple(dims[np.array(indices).flatten()])
             for key, indices in indices_attrs.items()
         }
 
     def _get_dims(self, name, field):
         # Newly written files should always contain indices attributes, but the
         # standard recommends that readers should also make "best effort" guess
         # since legacy files do not set this attribute.
         if name == self._signal_name:
             return self._group_dims
         # Latest way of defining dims
         if (dims := self._dims_from_indices.get(name)) is not None:
+            if '.' in dims:
+                hdf5_dims = self._dims_from_hdf5(field)
+                return tuple(dim if dim != '.' else hdf5_dim
+                             for dim, hdf5_dim in zip(dims, hdf5_dims))
             return dims
         # Older way of defining dims via axis attribute
         if (axis := self._axis_index.get(name)) is not None:
             return (self._group_dims[axis - 1], )
         if name in self._aux_signals:
             return _guess_dims(self._group_dims, self._signal.dataset.shape,
                                field.dataset)
@@ -248,14 +252,27 @@
                 return self._group_dims
             return (name, )
         if self._signal is not None and self._group_dims is not None:
             signal_shape = self._signal.dataset.shape if isinstance(
                 self._signal, Field) else (self._signal.shape if isinstance(
                     self._signal, EventField) else None)
             return _guess_dims(self._group_dims, signal_shape, field.dataset)
+        # While not mandated or recommended by the standard, we can try to find HDF5
+        # dim labels as a fallback option for defining dimension labels. Ideally we
+        # would like to do so in NXobject._init_field, but this causes significant
+        # overhead for small files with many datasets. Defined here, this will only
+        # take effect for NXdata, NXdetector, NXlog, and NXmonitor.
+        return self._dims_from_hdf5(field)
+
+    def _dims_from_hdf5(self, field):
+        hdf5_dims = [dim.label for dim in getattr(field.dataset, 'dims', [])]
+        if any(dim != '' for dim in hdf5_dims):
+            while hdf5_dims and hdf5_dims[-1] == '':
+                hdf5_dims.pop()
+            return [f'dim_{i}' if dim == '' else dim for i, dim in enumerate(hdf5_dims)]
 
     @cached_property
     def sizes(self) -> Dict[str, int]:
         if not self._valid:
             return super().sizes
         sizes = dict(self._signal.sizes)
         for name in self._aux_signals:
@@ -338,28 +355,92 @@
 
 
 def _squeeze_trailing(dims: Tuple[str, ...], shape: Tuple[int, ...]) -> Tuple[int, ...]:
     return shape[:len(dims)] + tuple(size for size in shape[len(dims):] if size != 1)
 
 
 class NXlog(NXdata):
+    """
+    NXlog, a time-series that can be loaded as a DataArray.
+
+    In some cases the NXlog may contain additional time series, such as a connection
+    status or alarm. These cannot be handled in a standard way, since the result cannot
+    be represented as a single DataArray. Furthermore, they prevent positional
+    time-indexing, since the time coord of each time-series is different. We can
+    support label-based indexing for this in the future. If additional time-series
+    are contained within the NXlog then loading will return a DataGroup of the
+    individual time-series (DataArrays).
+    """
 
     def __init__(self, attrs: Dict[str, Any], children: Dict[str, Union[Field, Group]]):
+        children = dict(children)
+        self._sublogs = []
+        self._sublog_children = {}
+        for name in children:
+            if name.endswith('_time'):
+                self._sublogs.append(name[:-5])
+        # Extract all fields that belong to sublogs, since they will interfere with the
+        # setup logic in the base class (NXdata).
+        for name in self._sublogs:
+            for k in list(children):
+                if k.startswith(name):
+                    field = children.pop(k)
+                    self._init_field(field)
+                    field.sizes = {
+                        'time' if i == 0 else f'dim_{i}': size
+                        for i, size in enumerate(field.dataset.shape)
+                    }
+                    self._sublog_children[k] = field
+
         super().__init__(attrs=attrs,
                          children=children,
                          fallback_dims=('time', ),
                          fallback_signal_name='value')
 
+    def read_children(self, sel: ScippIndex) -> sc.DataGroup:
+        # Sublogs have distinct time axes (with a different length). Must disable
+        # positional indexing.
+        if self._sublogs and ('time' in _to_canonical_select(list(self.sizes), sel)):
+            raise sc.DimensionError(
+                "Cannot positionally select time since there are multiple "
+                "time fields. Label-based selection is not supported yet.")
+        dg = super().read_children(sel)
+        for name, field in self._sublog_children.items():
+            dg[name] = field[sel]
+        return dg
+
+    def _time_to_datetime(self, mapping):
+        if (time := mapping.get('time')) is not None:
+            if time.dtype != sc.DType.datetime64 and _is_time(time):
+                mapping['time'] = convert_time_to_datetime64(
+                    time, start=sc.epoch(unit=time.unit))
+
+    def _assemble_sublog(self,
+                         dg: sc.DataGroup,
+                         name: str,
+                         value_name: Optional[str] = None) -> sc.DataArray:
+        value_name = name if value_name is None else f'{name}_{value_name}'
+        da = sc.DataArray(dg.pop(value_name), coords={'time': dg.pop(f'{name}_time')})
+        for k in list(dg):
+            if k.startswith(name):
+                da.coords[k[len(name) + 1:]] = dg.pop(k)
+        self._time_to_datetime(da.coords)
+        return da
+
     def assemble(self,
                  dg: sc.DataGroup) -> Union[sc.DataGroup, sc.DataArray, sc.Dataset]:
-        if (time := dg.get('time')) is not None:
-            if time.dtype != sc.DType.datetime64 and _is_time(time):
-                dg['time'] = convert_time_to_datetime64(time,
-                                                        start=sc.epoch(unit=time.unit))
-        return super().assemble(dg)
+        self._time_to_datetime(dg)
+        dg = sc.DataGroup(dg)
+        sublogs = sc.DataGroup()
+        for name in self._sublogs:
+            # Somewhat arbitrary definition of which fields is the "value"
+            value_name = 'severity' if name == 'alarm' else None
+            sublogs[name] = self._assemble_sublog(dg, name, value_name=value_name)
+        out = super().assemble(dg)
+        return out if not sublogs else sc.DataGroup(value=out, **sublogs)
 
 
 def _find_embedded_nxevent_data(
         children: Dict[str, Union[Field, Group]]) -> Optional[Group]:
     if all(name in children for name in NXevent_data.mandatory_fields):
         parent = children['event_index'].parent._group
         event_group = Group(parent,
```

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/nxevent_data.py` & `scippnexus-23.5.0/src/scippnexus/v2/nxevent_data.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/nxoff_geometry.py` & `scippnexus-23.5.0/src/scippnexus/v2/nxoff_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/nxsample.py` & `scippnexus-23.5.0/src/scippnexus/v2/nxsample.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus/v2/nxtransformations.py` & `scippnexus-23.5.0/src/scippnexus/v2/nxtransformations.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/src/scippnexus.egg-info/PKG-INFO` & `scippnexus-23.5.0/src/scippnexus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scippnexus
-Version: 23.4.1
+Version: 23.5.0
 Summary: h5py-like utility for NeXus files based with seamless scipp integration
 Home-page: https://scipp.github.io/scippnexus
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/scippnexus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `scippnexus-23.4.1/src/scippnexus.egg-info/SOURCES.txt` & `scippnexus-23.5.0/src/scippnexus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -89,11 +89,12 @@
 tests/externalfile.py
 tests/load_files_test.py
 tests/nexus_test.py
 tests/nxcylindrical_geometry_test.py
 tests/nxdata_test.py
 tests/nxdetector_test.py
 tests/nxevent_data_test.py
+tests/nxlog_test.py
 tests/nxmonitor_test.py
 tests/nxoff_geometry_test.py
 tests/nxsample_test.py
 tests/nxtransformations_test.py
```

### Comparing `scippnexus-23.4.1/tests/application_definition_test.py` & `scippnexus-23.5.0/tests/application_definition_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/tests/conftest.py` & `scippnexus-23.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/tests/externalfile.py` & `scippnexus-23.5.0/tests/externalfile.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/tests/load_files_test.py` & `scippnexus-23.5.0/tests/load_files_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/tests/nexus_test.py` & `scippnexus-23.5.0/tests/nexus_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -95,120 +95,14 @@
     attr = np.chararray((), itemsize=5)
     attr[()] = b'NXlog'
     log.attrs['NX_class'] = attr
     group = snx.Group(log, definitions=snx.base_definitions())
     assert group.nx_class == NXlog
 
 
-def test_nxobject_log(h5root):
-    da = sc.DataArray(sc.array(dims=['time'], values=[1.1, 2.2, 3.3]),
-                      coords={
-                          'time':
-                          sc.epoch(unit='ns') +
-                          sc.array(dims=['time'], unit='s', values=[4.4, 5.5, 6.6]).to(
-                              unit='ns', dtype='int64')
-                      })
-    log = snx.create_class(h5root, 'log', NXlog)
-    snx.create_field(log, 'value', da.data)
-    snx.create_field(log, 'time', da.coords['time'] - sc.epoch(unit='ns'))
-    log = snx.Group(log, definitions=snx.base_definitions())
-    assert sc.identical(log[...], da)
-
-
-def test_nxlog_with_missing_value_triggers_fallback(nxroot):
-    time = sc.epoch(unit='ns') + sc.array(
-        dims=['time'], unit='s', values=[4.4, 5.5, 6.6]).to(unit='ns', dtype='int64')
-    log = nxroot['entry'].create_class('log', NXlog)
-    log['time'] = time - sc.epoch(unit='ns')
-    loaded = log[()]
-    # Fallback to DataGroup, but we still have partial info from NXlog: dim is time
-    assert_identical(loaded, sc.DataGroup(time=time))
-
-
-def test_nxlog_length_1(h5root):
-    nxroot = snx.Group(h5root, definitions=snx.base_definitions())
-    da = sc.DataArray(
-        sc.array(dims=['time'], values=[1.1]),
-        coords={
-            'time':
-            sc.epoch(unit='ns') +
-            sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
-        })
-    log = nxroot.create_class('log', NXlog)
-    log['value'] = da.data
-    log['time'] = da.coords['time'] - sc.epoch(unit='ns')
-    assert sc.identical(log[...], da)
-
-
-def test_nxlog_length_1_two_dims_no_time_defaults_inner_dim_name(nxroot):
-    var = sc.array(dims=['time', 'ignored'], values=[[1.1]])
-    log = nxroot['entry'].create_class('log', NXlog)
-    log['value'] = var
-    assert_identical(log[...], sc.DataArray(var.rename(ignored='dim_1')))
-
-
-def test_nxlog_length_1_two_dims_with_time_defaults_inner_dim_name(nxroot):
-    da = sc.DataArray(
-        sc.array(dims=['time', 'ignored'], values=[[1.1]]),
-        coords={
-            'time':
-            sc.epoch(unit='ns') +
-            sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
-        })
-    log = nxroot['entry'].create_class('log', NXlog)
-    log['value'] = da.data
-    log['time'] = da.coords['time'] - sc.epoch(unit='ns')
-    assert sc.identical(log[...], da.rename(ignored='dim_1'))
-
-
-def test_nxlog_axes_replaces_time_dim(nxroot):
-    da = sc.DataArray(
-        sc.array(dims=['time', 'ignored'], values=[[1.1]]),
-        coords={
-            'time':
-            sc.epoch(unit='ns') +
-            sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
-        })
-    log = nxroot['entry'].create_class('log', NXlog)
-    log._group.attrs['axes'] = ['yy', 'xx']
-    log['value'] = da.data
-    log['time'] = da.coords['time'] - sc.epoch(unit='ns')
-    expected = sc.DataArray(sc.array(dims=['yy', 'xx'], values=[[1.1]]),
-                            coords={'time': da.coords['time'].squeeze()})
-    assert sc.identical(log[...], expected)
-
-
-def test_nxlog_three_dims_with_time_of_length_1(nxroot):
-    da = sc.DataArray(
-        sc.array(dims=['time', 'a', 'b'], values=np.arange(9.).reshape(1, 3, 3)),
-        coords={
-            'time':
-            sc.epoch(unit='ns') +
-            sc.array(dims=['time'], unit='s', values=[4.4]).to(unit='ns', dtype='int64')
-        })
-    log = nxroot['entry'].create_class('log', NXlog)
-    log['value'] = da.data
-    log['time'] = da.coords['time'] - sc.epoch(unit='ns')
-    loaded = log[...]
-    assert_identical(
-        loaded.data,
-        sc.array(dims=['time', 'dim_1', 'dim_2'], values=np.arange(9.).reshape(1, 3,
-                                                                               3)))
-
-
-def test_nxlog_with_shape_0(nxroot):
-    da = sc.DataArray(sc.ones(dims=['time', 'ignored'], shape=(0, 1)),
-                      coords={'time': sc.ones(dims=['time'], shape=(0, ), unit='s')})
-    log = nxroot['entry'].create_class('log', NXlog)
-    log['value'] = da.data
-    log['time'] = da.coords['time']
-    da.coords['time'] = sc.datetimes(dims=['time'], values=[], unit='ns')
-    assert_identical(log[...], da.rename(ignored='dim_1'))
-
-
 def test_nxobject_event_data(nxroot):
     event_data = nxroot['entry'].create_class('events_0', NXevent_data)
     assert event_data.nx_class == NXevent_data
 
 
 def test_nxobject_getting_item_that_does_not_exists_raises_KeyError(nxroot):
     with pytest.raises(KeyError):
```

### Comparing `scippnexus-23.4.1/tests/nxcylindrical_geometry_test.py` & `scippnexus-23.5.0/tests/nxcylindrical_geometry_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/tests/nxdata_test.py` & `scippnexus-23.5.0/tests/nxdata_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/tests/nxdetector_test.py` & `scippnexus-23.5.0/tests/nxdetector_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -565,7 +565,81 @@
                 'face1_center':
                 sc.vectors(dims=['cylinder'], values=[[3, 0, 0]], unit='m'),
                 'face1_edge':
                 sc.vectors(dims=['cylinder'], values=[[0, 1, 0]], unit='m'),
                 'face2_center':
                 sc.vectors(dims=['cylinder'], values=[[0, 0, 0]], unit='m'),
             }))
+
+
+def test_falls_back_to_hdf5_dim_labels(nxroot):
+    detector = nxroot.create_class('detector0', NXdetector)
+    xy = sc.array(dims=['x', 'y'], values=[[1, 2], [3, 4]])
+    z = sc.array(dims=['z'], values=[1, 2, 3])
+    dataset = detector.create_field('xy', xy)
+    dataset.dims[0].label = 'x'
+    dataset.dims[1].label = 'y'
+    dataset = detector.create_field('z', z)
+    dataset.dims[0].label = 'z'
+    assert detector.sizes == {'x': 2, 'y': 2, 'z': 3}
+    dg = detector[()]
+    assert_identical(dg['xy'], xy)
+    assert_identical(dg['z'], z)
+
+
+def test_falls_back_to_partial_hdf5_dim_labels(nxroot):
+    detector = nxroot.create_class('detector0', NXdetector)
+    xyz = sc.ones(dims=['x', 'dim_1', 'z'], shape=(2, 2, 3))
+    dataset = detector.create_field('xyz', xyz)
+    dataset.dims[0].label = 'x'
+    dataset.dims[2].label = 'z'
+    assert detector.sizes == xyz.sizes
+    dg = detector[()]
+    assert_identical(dg['xyz'], xyz)
+
+
+def test_squeezes_trailing_when_fall_back_to_partial_hdf5_dim_labels(nxroot):
+    detector = nxroot.create_class('detector0', NXdetector)
+    x = sc.ones(dims=['x', 'dim_1'], shape=(2, 1))
+    dataset = detector.create_field('x', x)
+    dataset.dims[0].label = 'x'
+    assert detector.sizes == {'x': 2}
+    dg = detector[()]
+    assert_identical(dg['x'], sc.squeeze(x))
+
+
+def test_falls_back_to_hdf5_dim_labels_given_unnamed_axes(h5root):
+    xy = sc.array(dims=['x', 'y'], values=[[1, 2], [3, 4]])
+    z = sc.array(dims=['z'], values=[1, 2, 3])
+    detector = snx.create_class(h5root, 'detector0', NXdetector)
+    dataset = snx.create_field(detector, 'xy', xy)
+    dataset.dims[0].label = 'x'
+    dataset.dims[1].label = 'y'
+    dataset = snx.create_field(detector, 'z', z)
+    dataset.dims[0].label = 'z'
+    detector.attrs['axes'] = ['.', '.', '.']
+    detector.attrs['xy_indices'] = [0, 1]
+    detector.attrs['z_indices'] = [2]
+    detector = make_group(detector)
+    assert detector.sizes == {'x': 2, 'y': 2, 'z': 3}
+    dg = detector[()]
+    assert_identical(dg['xy'], xy)
+    assert_identical(dg['z'], z)
+
+
+def test_falls_back_to_hdf5_dim_labels_given_partially_axes(h5root):
+    xy = sc.array(dims=['x', 'yy'], values=[[1, 2], [3, 4]])
+    z = sc.array(dims=['zz'], values=[1, 2, 3])
+    detector = snx.create_class(h5root, 'detector0', NXdetector)
+    dataset = snx.create_field(detector, 'xy', xy)
+    dataset.dims[0].label = 'x'
+    dataset.dims[1].label = 'y'
+    dataset = snx.create_field(detector, 'z', z)
+    dataset.dims[0].label = 'z'
+    detector.attrs['axes'] = ['.', 'yy', 'zz']
+    detector.attrs['xy_indices'] = [0, 1]
+    detector.attrs['z_indices'] = [2]
+    detector = make_group(detector)
+    assert detector.sizes == {'x': 2, 'yy': 2, 'zz': 3}
+    dg = detector[()]
+    assert_identical(dg['xy'], xy)
+    assert_identical(dg['z'], z)
```

### Comparing `scippnexus-23.4.1/tests/nxevent_data_test.py` & `scippnexus-23.5.0/tests/nxevent_data_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/tests/nxmonitor_test.py` & `scippnexus-23.5.0/tests/nxmonitor_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/tests/nxoff_geometry_test.py` & `scippnexus-23.5.0/tests/nxoff_geometry_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/tests/nxsample_test.py` & `scippnexus-23.5.0/tests/nxsample_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/tests/nxtransformations_test.py` & `scippnexus-23.5.0/tests/nxtransformations_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.1/tox.ini` & `scippnexus-23.5.0/tox.ini`

 * *Files identical despite different names*

