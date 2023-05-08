# Comparing `tmp/nasa-scrub-2.6.4.tar.gz` & `tmp/nasa-scrub-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nasa-scrub-2.6.4.tar", last modified: Tue Feb 21 05:22:57 2023, max compression
+gzip compressed data, was "nasa-scrub-2.6.5.tar", last modified: Mon May  8 23:50:48 2023, max compression
```

## Comparing `nasa-scrub-2.6.4.tar` & `nasa-scrub-2.6.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:57.404134 nasa-scrub-2.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-02-21 05:22:57.404134 nasa-scrub-2.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:57.400134 nasa-scrub-2.6.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)    24778 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/configuration-inputs.md
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/filtering.md
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/output.md
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/release-checklist.md
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/reviewing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/troubleshooting.md
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/docs/utilities.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:57.400134 nasa-scrub-2.6.4/nasa_scrub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-02-21 05:22:57.000000 nasa-scrub-2.6.4/nasa_scrub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-02-21 05:22:57.000000 nasa-scrub-2.6.4/nasa_scrub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 05:22:57.000000 nasa-scrub-2.6.4/nasa_scrub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-21 05:22:57.000000 nasa-scrub-2.6.4/nasa_scrub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 05:22:57.000000 nasa-scrub-2.6.4/nasa_scrub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-21 05:22:57.000000 nasa-scrub-2.6.4/nasa_scrub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:57.400134 nasa-scrub-2.6.4/scrub/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/scrub_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/scrubme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:57.400134 nasa-scrub-2.6.4/scrub/targets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/targets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:57.400134 nasa-scrub-2.6.4/scrub/targets/collaborator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/targets/collaborator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21734 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/targets/collaborator/do_collaborator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:57.400134 nasa-scrub-2.6.4/scrub/targets/scrub_gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/targets/scrub_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/targets/scrub_gui/do_scrub_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:57.400134 nasa-scrub-2.6.4/scrub/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:57.404134 nasa-scrub-2.6.4/scrub/tools/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/parsers/csv_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/parsers/get_codesonar_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/parsers/get_coverity_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/parsers/get_gbuild_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/parsers/get_gcc_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/parsers/get_javac_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/parsers/get_pylint_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/parsers/get_sonarqube_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/parsers/translate_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:57.404134 nasa-scrub-2.6.4/scrub/tools/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/templates/codeql.template
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/templates/codesonar.template
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/templates/coverity.template
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/templates/gbuild.template
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/templates/gcc.template
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/templates/javac.template
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/templates/pylint.template
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/tools/templates/sonarqube.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:57.404134 nasa-scrub-2.6.4/scrub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/utils/diff_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/utils/do_clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:57.404134 nasa-scrub-2.6.4/scrub/utils/filtering/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/utils/filtering/FilteringDefaults
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/utils/filtering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/utils/filtering/create_file_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/utils/filtering/do_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/utils/filtering/filter_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/utils/scrub_defaults.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    18633 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/scrub/utils/scrub_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-02-21 05:22:57.404134 nasa-scrub-2.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-21 05:22:36.000000 nasa-scrub-2.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.471542 nasa-scrub-2.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-08 23:50:48.471542 nasa-scrub-2.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.459542 nasa-scrub-2.6.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24778 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/configuration-inputs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/filtering.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/output.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/release-checklist.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/reviewing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/troubleshooting.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/docs/utilities.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.459542 nasa-scrub-2.6.5/nasa_scrub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-08 23:50:48.000000 nasa-scrub-2.6.5/nasa_scrub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-08 23:50:48.000000 nasa-scrub-2.6.5/nasa_scrub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 23:50:48.000000 nasa-scrub-2.6.5/nasa_scrub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 23:50:48.000000 nasa-scrub-2.6.5/nasa_scrub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 23:50:48.000000 nasa-scrub-2.6.5/nasa_scrub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 23:50:48.000000 nasa-scrub-2.6.5/nasa_scrub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.463542 nasa-scrub-2.6.5/scrub/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/scrub_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/scrubme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.463542 nasa-scrub-2.6.5/scrub/targets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/targets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.463542 nasa-scrub-2.6.5/scrub/targets/collaborator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/targets/collaborator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/targets/collaborator/do_collaborator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.463542 nasa-scrub-2.6.5/scrub/targets/scrub_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/targets/scrub_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/targets/scrub_gui/do_scrub_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.463542 nasa-scrub-2.6.5/scrub/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.467542 nasa-scrub-2.6.5/scrub/tools/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/csv_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_codesonar_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_coverity_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_gbuild_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_gcc_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_javac_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_pylint_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/get_sonarqube_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21844 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/parsers/translate_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.467542 nasa-scrub-2.6.5/scrub/tools/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/codeql.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/codesonar.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/coverity.template
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/gbuild.template
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/gcc.template
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/javac.template
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/pylint.template
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/tools/templates/sonarqube.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.471542 nasa-scrub-2.6.5/scrub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/diff_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/do_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:48.471542 nasa-scrub-2.6.5/scrub/utils/filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/filtering/FilteringDefaults
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/filtering/create_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/filtering/do_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/filtering/filter_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/scrub_defaults.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/scrub/utils/scrub_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-08 23:50:48.471542 nasa-scrub-2.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 23:50:30.000000 nasa-scrub-2.6.5/setup.py
```

### Comparing `nasa-scrub-2.6.4/LICENSE` & `nasa-scrub-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/PKG-INFO` & `nasa-scrub-2.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasa-scrub
-Version: 2.6.4
+Version: 2.6.5
 Summary: SCRUB is an orchestration and aggregation tool for static code analysis tools.
 Home-page: https://github.com/nasa/scrub
 Author: Lyle Barner
 Author-email: lyle.barner@jpl.nasa.gov
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/nasa/scrub/issues
 Project-URL: Documentation, https://nasa.github.io/scrub
```

### Comparing `nasa-scrub-2.6.4/README.md` & `nasa-scrub-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/docs/README.md` & `nasa-scrub-2.6.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/docs/configuration-inputs.md` & `nasa-scrub-2.6.5/docs/configuration-inputs.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/docs/configuration.md` & `nasa-scrub-2.6.5/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/docs/contributing.md` & `nasa-scrub-2.6.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/docs/faq.md` & `nasa-scrub-2.6.5/docs/faq.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/docs/filtering.md` & `nasa-scrub-2.6.5/docs/filtering.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/docs/installation.md` & `nasa-scrub-2.6.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/docs/output.md` & `nasa-scrub-2.6.5/docs/output.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/docs/release-checklist.md` & `nasa-scrub-2.6.5/docs/release-checklist.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/docs/reviewing.md` & `nasa-scrub-2.6.5/docs/reviewing.md`

 * *Files 18% similar despite different names*

```diff
@@ -28,7 +28,16 @@
 
 Please refer to the [Detailed Configuration](configuration.md) page for more information about Collaborator configuration inputs.
 
 
 ### Automated Invocation
 
 There is a section of the `scrub.cfg` file that can be used for pushing results to Collaborator automatically. For more information about the expected inputs for this process, please refer to the [Detailed Configuration](configuration.md) page. SCRUB analysis will be performed normally, but before execution is completed SCRUB will create a new Collaborator review that is initialized with all of the SCRUB results.
+
+### Collaborator Review Templates
+The Collaborator section of the `scrub.cfg` includes a section where users may define a review template to be used for Collaborator uploads. This can be any template on the Collaborator server, so long as it has the custom fields SCRUB expects. These fields are listed below, along with information to configure them on the Collaborator instance. Collaborator uploads may fail if these are not configured appropriately.
+
+| Collaborator Template Section | Field Name | Type                                                                | Default Value |
+| ----------------------------- | ---------- | ------------------------------------------------------------------- | ------------- |
+| Review Custom Fields          | Overview   | String (Multi-line)                                                 | None          |
+| Defect Custom Fields          | Severity   | Drop-down List (Blocker, Critical, Major, Moderate, Minor, Trivial) | Moderate      |
+
```

### Comparing `nasa-scrub-2.6.4/docs/troubleshooting.md` & `nasa-scrub-2.6.5/docs/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/docs/usage.md` & `nasa-scrub-2.6.5/docs/usage.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/docs/utilities.md` & `nasa-scrub-2.6.5/docs/utilities.md`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/nasa_scrub.egg-info/PKG-INFO` & `nasa-scrub-2.6.5/nasa_scrub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasa-scrub
-Version: 2.6.4
+Version: 2.6.5
 Summary: SCRUB is an orchestration and aggregation tool for static code analysis tools.
 Home-page: https://github.com/nasa/scrub
 Author: Lyle Barner
 Author-email: lyle.barner@jpl.nasa.gov
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/nasa/scrub/issues
 Project-URL: Documentation, https://nasa.github.io/scrub
```

### Comparing `nasa-scrub-2.6.4/nasa_scrub.egg-info/SOURCES.txt` & `nasa-scrub-2.6.5/nasa_scrub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/scrub_cli.py` & `nasa-scrub-2.6.5/scrub/scrub_cli.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/scrubme.py` & `nasa-scrub-2.6.5/scrub/scrubme.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,19 +254,21 @@
         if viewable_results_dir.exists():
             shutil.rmtree(viewable_results_dir)
         viewable_results_dir.mkdir()
         viewable_results_dir.chmod(0o755)
 
         # Copy SCRUB format output files
         for scrub_file in scrub_conf_data.get('scrub_analysis_dir').glob('*.scrub'):
-            os.symlink(scrub_file, viewable_results_dir.joinpath(scrub_file.name))
+            os.symlink(os.path.relpath(str(scrub_file), str(viewable_results_dir)),
+                       viewable_results_dir.joinpath(scrub_file.name))
 
         # Copy the SARIF format output files
         for sarif_file in scrub_conf_data.get('sarif_results_dir').glob('*.sarif'):
-            os.symlink(sarif_file, viewable_results_dir.joinpath(sarif_file.name))
+            os.symlink(os.path.relpath(str(sarif_file), str(viewable_results_dir)),
+                       viewable_results_dir.joinpath(sarif_file.name))
 
         # Print a status message
         tool_failure_count = 0
         total_execution_time = 0
         print('\nTool Execution Status:\n')
         for status in execution_status:
             # Track the execution time
```

### Comparing `nasa-scrub-2.6.4/scrub/targets/collaborator/do_collaborator.py` & `nasa-scrub-2.6.5/scrub/targets/collaborator/do_collaborator.py`

 * *Files 8% similar despite different names*

```diff
@@ -179,112 +179,104 @@
                              '        <url>{}</url>\n'.format(url) +
                              '        <user>{}</user>\n'.format(username) +
                              '    </global-options>\n')
 
     return global_options_string
 
 
-def create_batch_xml_file_upload(output_file, file_list, review_id, url, username, source_root):
+def create_batch_xml_file_upload(file_list, review_id, source_root):
     """This function creates the XML file that is used to upload review files to Collaborator.
 
     Inputs:
-        - output_file: Absolute path to the desired XML output file location [string]
         - file_list: List of files to be uploaded to Collaborator [list of strings]
         - review_id: ID of review to upload files [string]
-        - url: URL of the Collaborator server [string]
-        - username: Username for the Collaborator user [string]
         - source_root: Absolute path to the source code root directory [string]
     """
 
-    with open(output_file, 'w') as output_fh:
-        # Start the XML
-        output_fh.write('<batch-commands>\n')
+    # Initialize the variables
+    file_upload_xml_batch = ('    <addfiles>\n' +
+                             '        <review>{}</review>\n'.format(review_id) +
+                             '        <relative-to>{}</relative-to>\n'.format(source_root) +
+                             '        <upload-comment>Initial SCRUB upload</upload-comment>\n')
+
+    # Iterate through every file and add it to the upload
+    for file in file_list:
+        file_upload_xml_batch = file_upload_xml_batch + '        <file-path>{}</file-path>\n'.format(file.strip())
+
+    file_upload_xml_batch = file_upload_xml_batch + '    </addfiles>\n'
 
-        # Write out the global options
-        output_fh.write('{}'.format(construct_xml_global_options(url, username)))
+    return file_upload_xml_batch
 
-        # Write out all of the file upload commands
-        output_fh.write('    <addfiles>\n')
-        output_fh.write('        <review>{}</review>\n'.format(review_id))
-        output_fh.write('        <relative-to>{}</relative-to>\n'.format(source_root))
-        output_fh.write('        <upload-comment>Initial SCRUB upload</upload-comment>\n')
 
-        for file in file_list:
-            output_fh.write('        <file-path>{}</file-path>\n'.format(file.strip()))
+def create_batch_xml_comment_upload(file_list, comment_list, review_id):
+    """This function creates the XML snippet that is used to upload review comments to Collaborator.
+
+    Inputs:
+        - file_list: List of files that are present within the review [list of string]
+        - defect_list: List of defects to be uploaded to the Collaborator review [list of dicts]
+        - review_id: ID of review to upload files [string]
+    """
+
+    # Initialize variables
+    comment_xml_list = ''
+
+    # Write out every defect for files of interest
+    for comment in comment_list:
+        if comment.get('file') in file_list:
+            # Construct the comment xml
+            comment_xml = ('    <admin_review_comment_create>\n' +
+                           '        <review>{}</review>\n'.format(review_id) +
+                           '        <file>{}</file>\n'.format(comment.get('file')) +
+                           '        <line-number>{}</line-number>\n'.format(comment.get('line')) +
+                           '        <comment>{}: {}</comment>\n'.format(comment.get('tool'), comment.get('description')) +
+                           '    </admin_review_comment_create>\n')
 
-        output_fh.write('    </addfiles>\n')
+            # Add it to the list
+            comment_xml_list = comment_xml_list + comment_xml
 
-        # Close out the file
-        output_fh.write('</batch-commands>\n')
+    return comment_xml_list
 
 
-def create_batch_xml_defect_upload(output_file, file_list, defect_list, review_id, finding_level, url, username):
-    """This function creates the XML file that is used to upload review defects to Collaborator.
+def create_batch_xml_defect_upload(file_list, defect_list, review_id):
+    """This function creates the XML snippet that is used to upload review defects to Collaborator.
 
     Inputs:
-        - output_file: Absolute path to the desired XML output file location [string]
+        - file_list: List of files that are present within the review [list of string]
         - defect_list: List of defects to be uploaded to the Collaborator review [list of dicts]
         - review_id: ID of review to upload files [string]
-        - finding_level: Should findings be uploaded as comments or defects? ['comment'/'defect']
-        - url: URL of the Collaborator server [string]
-        - username: Username for the Collaborator user [string]
     """
 
-    with open(output_file, 'w') as output_fh:
-        # Start the XML
-        output_fh.write('<batch-commands>\n')
+    # Initialize variables
+    defect_xml_list = ''
+
+    # Write out every defect for files of interest
+    for defect in defect_list:
+        if defect.get('file') in file_list:
+            # Parse the priority level
+            if defect.get('priority') == 'High':
+                severity = 'Major'
+            elif defect.get('priority') == 'Med':
+                severity = 'Moderate'
+            else:
+                severity = 'Minor'
+
+            # Create the defect XML
+            defect_xml = ('    <admin_review_defect_create>\n'+
+                                 '        <custom-field>Severity={}</custom-field>\n'.format(severity) +
+                                 '        <review>{}</review>\n'.format(review_id) +
+                                 '        <file>{}</file>\n'.format(defect.get('file')) +
+                                 '        <line-number>{}</line-number>\n'.format(defect.get('line')) +
+                                 '        <comment>{}: {}</comment>\n'.format(defect.get('tool'),
+                                                                              defect.get('description')) +
+                                 '    </admin_review_defect_create>\n')
 
-        # Write out the global options
-        output_fh.write('{}'.format(construct_xml_global_options(url, username)))
-        
-        # Track if we're including any warnings
-        uploaded_warnings = False
-
-        # Write out every defect for files of interest
-        for defect in defect_list:
-            if defect.get('file') in file_list:
-                uploaded_warnings = True
-                if finding_level.lower() == 'defect':
-                    # Parse the priority level
-                    if defect.get('priority') == 'High':
-                        severity = 'Major'
-                    elif defect.get('priority') == 'Med':
-                        severity = 'Moderate'
-                    else:
-                        severity = 'Minor'
-
-                    output_fh.write('    <admin_review_defect_create>\n')
-                    output_fh.write('        <custom-field>Severity={}</custom-field>\n'.format(severity))
-                else:
-                    output_fh.write('    <admin_review_comment_create>\n')
-
-                output_fh.write('        <review>{}</review>\n'.format(review_id))
-                output_fh.write('        <file>{}</file>\n'.format(defect.get('file')))
-
-                # Check for a line number
-                if int(defect.get('line')) > 0:
-                    output_fh.write('        <line-number>{}</line-number>\n'.format(defect.get('line')))
-
-                output_fh.write('        <comment>{}: {}</comment>\n'.format(defect.get('tool'),
-                                                                             defect.get('description')))
-
-                if finding_level.lower() == 'defect':
-                    output_fh.write('    </admin_review_defect_create>')
-                else:
-                    output_fh.write('    </admin_review_comment_create>\n')
-
-        # Add a general comment if there are no uploaded warnings
-        if not uploaded_warnings:
-            output_fh.write('    <admin_review_comment_create>\n')
-            output_fh.write('        <review>{}</review>\n'.format(review_id))
-            output_fh.write('        <comment>No warnings were found to include in this review.</comment>\n')
-            output_fh.write('    </admin_review_comment_create>\n')
-                    
-        # Close out the file
-        output_fh.write('</batch-commands>\n')
+            # Update the list of defects
+            defect_xml_list = defect_xml_list + defect_xml
+
+    return defect_xml_list
 
 
 def initialize_upload(tool_conf_data):
     """This function prepares to upload review data to Collaborator.
 
     Inputs:
         - tool_conf_data: Dictionary of scrub.cfg input variables [dict]
@@ -309,20 +301,18 @@
     execute_ccollab(tool_conf_data.get('collaborator_ccollab_location'), subcommand)
 
     # Get the review ID and add it to the configuration data
     review_id = get_review_id(tool_conf_data.get('collaborator_log_file'))
     tool_conf_data.update({'collaborator_review_id': int(review_id)})
 
     # Set the review xml file path
-    files_xml = tool_conf_data.get('scrub_analysis_dir').joinpath('collaborator_review_' + str(review_id) +
-                                                                  '_files.xml')
-    comments_xml = tool_conf_data.get('scrub_analysis_dir').joinpath('collaborator_review_' + str(review_id) +
-                                                                     '_comments.xml')
-    tool_conf_data.update({'collaborator_review_xml_files': files_xml})
-    tool_conf_data.update({'collaborator_review_xml_comments': comments_xml})
+    batch_command_file = tool_conf_data.get('collaborator_upload_dir').joinpath('collaborator_review_' +
+                                                                                str(review_id) + '_batch.xml')
+    tool_conf_data.update({'batch_command_file': batch_command_file})
+    # tool_conf_data.update({'collaborator_review_xml_comments': comments_xml})
 
     # Set the author of the review
     subcommand = ('admin review set-participants ' + review_id + ' --participant author=' +
                   tool_conf_data.get('collaborator_username'))
     execute_ccollab(tool_conf_data.get('collaborator_ccollab_location'), subcommand)
 
 
@@ -355,35 +345,44 @@
     # Get the defects
     for tool_name in tool_defect_types:
         scrub_file = tool_conf_data.get('scrub_analysis_dir').joinpath(tool_name + '.scrub')
 
         # Add the defects to the review
         defect_list = defect_list + get_defects(scrub_file)
 
-    # Create XML batch file for uploading files
-    create_batch_xml_file_upload(tool_conf_data.get('collaborator_review_xml_files'), file_list,
-                                 tool_conf_data.get('collaborator_review_id'),
-                                 tool_conf_data.get('collaborator_server'), tool_conf_data.get('collaborator_username'),
-                                 tool_conf_data.get('source_dir'))
-
-    # Create the XML batch file for uploading defects
-    create_batch_xml_defect_upload(tool_conf_data.get('collaborator_review_xml_comments'), file_list, defect_list,
-                                   tool_conf_data.get('collaborator_review_id'),
-                                   tool_conf_data.get('collaborator_finding_level'),
-                                   tool_conf_data.get('collaborator_server'),
-                                   tool_conf_data.get('collaborator_username'))
-
-    # Find the xml files of interest
-    xml_files = [tool_conf_data.get('collaborator_review_xml_files'),
-                 tool_conf_data.get('collaborator_review_xml_comments')]
-
-    # Perform all the batch commands
-    for xml_file in xml_files:
-        subcommand = ('admin batch ' + str(xml_file))
-        execute_ccollab(tool_conf_data.get('collaborator_ccollab_location'), subcommand)
+    # Create XML data for uploading files
+    file_xml_data = create_batch_xml_file_upload(file_list, tool_conf_data.get('collaborator_review_id'),
+                                                 tool_conf_data.get('source_dir'))
+
+    if tool_conf_data.get('collaborator_finding_level').lower() == 'defect':
+        finding_xml_data = create_batch_xml_defect_upload(file_list, defect_list,
+                                                          tool_conf_data.get('collaborator_review_id'))
+    else:
+        finding_xml_data = create_batch_xml_comment_upload(file_list, defect_list,
+                                                           tool_conf_data.get('collaborator_review_id'))
+
+    # Add a generic comment if the finding upload list is empty
+    if finding_xml_data == '':
+        finding_xml_data = ('    <admin_review_comment_create>\n' +
+                            '        <review>{}</review>\n'.format(tool_conf_data.get('collaborator_review_id')) +
+                            '        <comment>No findings were found to include in this review.</comment>\n' +
+                            '    </admin_review_comment_create>\n')
+
+    # Create the XML batch file
+    with open(tool_conf_data.get('batch_command_file'), 'w+') as output_fh:
+        output_fh.write('<batch-commands>\n')
+        output_fh.write('{}'.format(construct_xml_global_options(tool_conf_data.get('collaborator_server'),
+                                                                 tool_conf_data.get('collaborator_username'))))
+        output_fh.write('{}'.format(file_xml_data))
+        output_fh.write('{}'.format(finding_xml_data))
+        output_fh.write('</batch-commands>')
+
+    # Perform the upload
+    subcommand = ('admin batch ' + str(tool_conf_data.get('batch_command_file')))
+    execute_ccollab(tool_conf_data.get('collaborator_ccollab_location'), subcommand)
 
 
 def create_filtering_files(tool_conf_data):
     """This function creates the filtering files needed for Collaborator upload.
 
     Inputs:
         - tool_conf_data: Dictionary of scrub.cfg input variables [dict]
@@ -499,26 +498,32 @@
 
     Inputs:
         - tool_conf_data: Dictionary of scrub.cfg input variables [dict]
     """
 
     # Initialize the derived variables
     current_user = pwd.getpwuid(os.getuid()).pw_name
+    collaborator_upload_dir = tool_conf_data.get('scrub_analysis_dir').joinpath('collaborator_upload')
     collaborator_log_file = tool_conf_data.get('scrub_log_dir').joinpath('collaborator_' + current_user + '.log')
-    collaborator_filtering_output_file = tool_conf_data.get('scrub_analysis_dir').joinpath('SCRUBCollaboratorFilteringList')
+    collaborator_filtering_output_file = collaborator_upload_dir.joinpath('SCRUBCollaboratorFilteringList')
 
     # Add derived values to the dictionary
     tool_conf_data.update({'collaborator_log_file': collaborator_log_file})
+    tool_conf_data.update({'collaborator_upload_dir': collaborator_upload_dir})
     tool_conf_data.update({'collaborator_filtering_output_file': collaborator_filtering_output_file})
     tool_conf_data.update({'collaborator_review_id': 0})
 
     # Set the username if necessary
     if tool_conf_data.get('collaborator_username') == '':
         tool_conf_data.update({'collaborator_username': current_user})
 
+    # Create the working directory if it doesn't already exist
+    if not collaborator_upload_dir.exists():
+        collaborator_upload_dir.mkdir()
+
     # Determine if Collaborator can be run
     if not (tool_conf_data.get('collaborator_server')):
         # Update the analysis flag if necessary
         if tool_conf_data.get('collaborator_export'):
             tool_conf_data.update({'collaborator_export': False})
 
             # Print a status message
```

### Comparing `nasa-scrub-2.6.4/scrub/targets/scrub_gui/do_scrub_gui.py` & `nasa-scrub-2.6.5/scrub/targets/scrub_gui/do_scrub_gui.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import pathlib
 import logging
 import traceback
 from scrub.utils import scrub_utilities
+from scrub.tools.parsers import translate_results
 
 
 def distribute_warnings(warning_file, source_dir):
     """This function moves warnings to be co-located with the source file of interest.
 
     Inputs:
         - warning_file: Full path to the file containing SCRUB-formatted warnings [string]
@@ -14,70 +15,56 @@
 
     Outputs:
         - A series of .scrub directories and output files will be created as necessary
     """
 
     # Initialize the variables
     warning_type = warning_file.stem
+    distributed_files_list = []
 
     # Print a status message
     logging.info('')
     logging.info('\tMoving results...')
     logging.info('\t>> Executing command: do_gui.distribute_warnings(%s, %s)', str(warning_file), str(source_dir))
     logging.info('\t>> From directory: %s', str(pathlib.Path().absolute()))
 
-    # Import the warning file
-    with open(warning_file, 'r') as input_fh:
-        input_data = input_fh.readlines()
-
     # Update the source root to make it absolute
     source_dir = source_dir.resolve()
 
-    # Iterate through every line of the file
-    for i in range(0, len(input_data)):
-        # Set the line
-        line = input_data[i]
-
-        # Check to see if the line contains a warning
-        if re.search(r'<.*>.*:.*:.*:', line):
-            # Add the line to the warning text
-            warning = line
-
-            # Get the warning file
-            warning_file = pathlib.Path(line.split(":")[1].strip())
-            warning_file_absolute = source_dir.joinpath(warning_file)
-
-            # Make sure the warning file is within the source root, but not at the source root
-            if warning_file_absolute.exists() and (source_dir != warning_file_absolute.parent):
-                # Get the rest of the warning text
-                j = i + 1
-                while input_data[j].strip() != '':
-                    warning = warning + input_data[j]
-
-                    # Increment the line
-                    j = j + 1
-
-                # Get the warning directory
-                warning_directory = warning_file_absolute.parent
-
-                # Create the scrub output paths
-                local_scrub_directory = warning_directory.joinpath('.scrub')
-                local_scrub_warning_file = local_scrub_directory.joinpath(warning_type)
-
-                # Create a .scrub directory if it doesn't already exists
-                if not local_scrub_directory.exists():
-                    local_scrub_directory.mkdir()
-                    local_scrub_directory.chmod(0o755)
-
-                # Write the warning to the output file
-                with open(local_scrub_warning_file, 'a') as output_fh:
-                    output_fh.write('%s\n' % warning_file.name)
+    # Parse all the findings from the warning file
+    warnings = translate_results.parse_scrub(warning_file, source_dir)
+
+    # Iterate through everything warning
+    for warning in warnings:
+        # Make sure the warning file is within the source root, but not at the source root
+        if warning['file'].exists() and (source_dir != warning['file'].parent):
+            # Get the warning directory
+            warning_directory = warning['file'].parent
+
+            # Create the scrub output paths
+            local_scrub_directory = warning_directory.joinpath('.scrub')
+            local_scrub_warning_file = local_scrub_directory.joinpath(warning_type + '.scrub')
+
+            # Create a .scrub directory if it doesn't already exists
+            if not local_scrub_directory.exists():
+                local_scrub_directory.mkdir()
+                local_scrub_directory.chmod(0o755)
+
+            # Write the warning to the output file
+            with open(local_scrub_warning_file, 'a') as output_fh:
+                output_fh.write('%s' % translate_results.format_scrub_warning(warning))
+
+            # Add the file to the list if it hasn't been added already
+            if local_scrub_warning_file not in distributed_files_list:
+                distributed_files_list.append(local_scrub_warning_file)
 
-                # Change the permissions of the output file
-                local_scrub_warning_file.chmod(0o644)
+            # Change the permissions of the output file
+            local_scrub_warning_file.chmod(0o644)
+
+    return distributed_files_list
 
 
 def initialize_analysis(tool_conf_data):
     """The purpose of this function is to prepare the tool to perform analysis.
 
     Inputs:
         - tool_conf_data: Dictionary of scrub.cfg input variables [dict]
@@ -118,15 +105,20 @@
             logging.info('Perform GUI export...')
 
             # Get a list of the filtered SCRUB output files
             filtered_output_files = tool_conf_data.get('scrub_analysis_dir').glob('*.scrub')
 
             # Move the warnings to the appropriate directories
             for filtered_output_file in filtered_output_files:
-                distribute_warnings(filtered_output_file, tool_conf_data.get('source_dir'))
+                distributed_files = distribute_warnings(filtered_output_file, tool_conf_data.get('source_dir'))
+
+                # Check each of the generated files for formatting
+                for distributed_file in distributed_files:
+                    if len(translate_results.parse_scrub(distributed_file, tool_conf_data.get('source_dir'))) == 0:
+                        raise AssertionError
 
             # Set the exit code
             gui_exit_code = 0
 
         except:     # lgtm [py/catch-base-exception]
             # Print a warning message
             logging.warning('GUI export could not be performed. Please see log file %s for more information.',
```

### Comparing `nasa-scrub-2.6.4/scrub/tools/parsers/csv_parser.py` & `nasa-scrub-2.6.5/scrub/tools/parsers/csv_parser.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/tools/parsers/get_coverity_warnings.py` & `nasa-scrub-2.6.5/scrub/tools/parsers/get_coverity_warnings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 import json
 import pathlib
 from scrub.tools.parsers import translate_results
 
-WARNING_LEVEL = 'Low'
 ID_PREFIX = 'coverity'
 
 
 def parse_json(raw_input_file, parsed_output_file):
     """This function parses the Coverity internal JSON results format into SCRUB formatted results.
 
     Inputs:
@@ -28,22 +27,33 @@
         # Parse issue data
         warning_id = '%s%03d' % (ID_PREFIX, warning_count)
         warning_file = pathlib.Path(issue['mainEventFilePathname'])
         warning_line = int(issue['mainEventLineNumber'])
         warning_checker = issue['checkerName']
         warning_description = []
 
+        if issue['checkerProperties']['impact'].lower() == 'high':
+            ranking = 'High'
+        elif issue['checkerProperties']['impact'].lower() == 'medium':
+            ranking = 'Med'
+        elif issue['checkerProperties']['impact'].lower() == 'low':
+            ranking = 'Low'
+        elif issue['checkerProperties']['impact'].lower() == 'audit':
+            ranking = 'Low'
+        else:
+            ranking = 'Low'
+
         # Get the warning description
         for event in issue['events']:
             if event['eventTag'] != 'caretline':
                 warning_description.append('%s:%s:' % (event['strippedFilePathname'], event['lineNumber']))
                 warning_description.append('%s: %s' % (event['eventTag'], event['eventDescription']))
 
         coverity_issues.append(translate_results.create_warning(warning_id, warning_file, warning_line,
-                                                                warning_description, 'coverity', WARNING_LEVEL,
+                                                                warning_description, 'coverity', ranking,
                                                                 warning_checker))
 
         # Increment the warning count
         warning_count = warning_count + 1
 
     # Create the output file
     translate_results.create_scrub_output_file(coverity_issues, parsed_output_file)
```

### Comparing `nasa-scrub-2.6.4/scrub/tools/parsers/get_gbuild_warnings.py` & `nasa-scrub-2.6.5/scrub/tools/parsers/get_gbuild_warnings.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/tools/parsers/get_gcc_warnings.py` & `nasa-scrub-2.6.5/scrub/tools/parsers/get_gcc_warnings.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/tools/parsers/get_javac_warnings.py` & `nasa-scrub-2.6.5/scrub/tools/parsers/get_javac_warnings.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/tools/parsers/get_pylint_warnings.py` & `nasa-scrub-2.6.5/scrub/tools/parsers/get_pylint_warnings.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/tools/parsers/translate_results.py` & `nasa-scrub-2.6.5/scrub/tools/parsers/translate_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         warning_lines = list(filter(None, re.split('\n', raw_warning.strip())))
 
         # Get the location information
         warning_info = list(filter(None, re.split(':', warning_lines[0].strip())))
 
         # Get the query name if it exists
         if len(warning_info) > 3:
-            warning_query = list(warning_lines[0].strip().split(' '))[-1]
+            warning_query = list(warning_lines[0].split(': '))[-1].strip()
         else:
             warning_query = ''
 
         # Get the warning description
         warning_description = []
         for line in warning_lines[1:]:
             warning_description.append(line.rstrip())
@@ -351,25 +351,36 @@
 
                     # Find the line number
                     if 'region' in location.keys():
                         warning_line = location['region']['startLine']
                     else:
                         warning_line = 0
 
+                    # Set the ranking
+                    if 'rank' in result.keys():
+                        if int(result['rank']) > 56:
+                            ranking = 'High'
+                        elif 21 < int(result['rank']) <= 56:
+                            ranking = 'Med'
+                        else:
+                            ranking = 'Low'
+                    else:
+                        ranking = 'Low'
+
                     # Fix the filepath
                     warning_file = pathlib.Path(warning_file.replace('file://', ''))
                     if warning_file.anchor != '/':
                         warning_file = updated_source_dir.joinpath(warning_file)
 
                     # Set the warning ID
                     warning_id = tool_name + str(warning_count).zfill(3)
 
                     # Add to the warning dictionary
                     results.append(create_warning(warning_id, warning_file.resolve(), warning_line, warning_description,
-                                                  tool_name, 'Low', warning_query, suppress_warning))
+                                                  tool_name, ranking, warning_query, suppress_warning))
 
                     # Update the warning count
                     warning_count = warning_count + 1
 
         else:
             results = []
```

### Comparing `nasa-scrub-2.6.4/scrub/tools/templates/codeql.template` & `nasa-scrub-2.6.5/scrub/tools/templates/codeql.template`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/tools/templates/codesonar.template` & `nasa-scrub-2.6.5/scrub/tools/templates/codesonar.template`

 * *Files 16% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 cd ${{TOOL_ANALYSIS_DIR}}
 
 # Get the results
 results_template='${{CODESONAR_RESULTS_TEMPLATE}}'
 re='^[0-9]+$'
 if [[ $results_template =~ $re ]] ; then
     # Get the results from the CodeSonar Hub
-    ${{CODESONAR_PATH}}/codesonar get -auth certificate -hubcert ${{CODESONAR_CERT}} -hubkey ${{CODESONAR_KEY}} ${{CODESONAR_GET_FLAGS}} ${{CODESONAR_HUB}}/report/aid-$aid-$results_template.xml
+    ${{CODESONAR_PATH}}/codesonar get -auth certificate -hubcert ${{CODESONAR_CERT}} -hubkey ${{CODESONAR_KEY}} ${{CODESONAR_GET_FLAGS}} "${{CODESONAR_HUB}}/search.xml?swarnings=%7B%0A%20%20%22visible%22%3A%20%7B%0A%20%20%20%20%22%2A%22%3A%20true%0A%20%20%7D%0A%7D&scope=aid%3A$aid&filter=%22active%22"
 
     # Parse the results into SCRUB format
-    python3 -m scrub.tools.parsers.get_codesonar_warnings ${{TOOL_ANALYSIS_DIR}}/*.xml ${{RAW_RESULTS_DIR}}/codesonar_raw.scrub
+    python3 -m scrub.tools.parsers.get_codesonar_warnings ${{TOOL_ANALYSIS_DIR}}/*.xml ${{RAW_RESULTS_DIR}}/codesonar_raw.scrub ${{CODESONAR_HUB}}
 else
     # Get the results from the CodeSonar Hub
-    ${{CODESONAR_PATH}}/codesonar get -auth certificate -hubcert ${{CODESONAR_CERT}} -hubkey ${{CODESONAR_KEY}} ${{CODESONAR_GET_FLAGS}} ${{CODESONAR_HUB}}/analysis/$aid-allwarnings.sarif
+    ${{CODESONAR_PATH}}/codesonar get -auth certificate -hubcert ${{CODESONAR_CERT}} -hubkey ${{CODESONAR_KEY}} ${{CODESONAR_GET_FLAGS}} "${{CODESONAR_HUB}}/warning_detail_search.sarif?scope=aid%3A$aid&filter=%22active%22"
 
     # Parse the results into SCRUB format
     python3 -m scrub.tools.parsers.translate_results ${{TOOL_ANALYSIS_DIR}}/*.sarif ${{RAW_RESULTS_DIR}}/codesonar_raw.scrub ${{SOURCE_DIR}} scrub
 fi
```

### Comparing `nasa-scrub-2.6.4/scrub/tools/templates/coverity.template` & `nasa-scrub-2.6.5/scrub/tools/templates/coverity.template`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/tools/templates/sonarqube.template` & `nasa-scrub-2.6.5/scrub/tools/templates/sonarqube.template`

 * *Files 6% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 done
 
 # Retrieve the hotspots from the SonarQube server
 PAGE=1
 MORE_RESULTS=true
 while $MORE_RESULTS; do
     # Get the page
-    RESULTS_FILE=${{TOOL_ANALYSIS_DIR}}/sonarqube_hotspots_search_$PAGE.json
+    RESULTS_FILE=${{TOOL_ANALYSIS_DIR}}/sonarqube_hotspots_$PAGE.json
     curl -u ${{SONARQUBE_TOKEN}}: "${{SONARQUBE_SERVER}}/api/hotspots/search?ps=500&projectKey=${{SONARQUBE_PROJECT}}&p=$PAGE&${{SONARQUBE_CURL_FLAGS}}" -o $RESULTS_FILE
     # Check to see if the file is empty
     if [ ! -s "$RESULTS_FILE" ]; then
         exit 1
     fi
     # Check the contents, verify file is not empty, and make sure the max page hasn't been reached
     if grep -q "Can return only the first 10000 results" $RESULTS_FILE; then
@@ -179,19 +179,9 @@
        rm -f $RESULTS_FILE
        MORE_RESULTS=false
     else
        PAGE=$((PAGE+1))
     fi
 done
 
-# Gather the hotspot keys
-grep -h -o -E '\"key\":\"[a-zA-Z0-9_-]{20}\",\"component' ${{TOOL_ANALYSIS_DIR}}/sonarqube_hotspots_search* | cut -c8-27 > ${{TOOL_ANALYSIS_DIR}}/sonarqube_hotspot_keys.txt
-
-# Get the hotspots
-count=1
-while read key; do
-    curl -u ${{SONARQUBE_TOKEN}}: "${{SONARQUBE_SERVER}}/api/hotspots/show?hotspot=$key" -o ${{TOOL_ANALYSIS_DIR}}/sonarqube_hotspot_$count.json
-    (( count++ ))
-done < ${{TOOL_ANALYSIS_DIR}}/sonarqube_hotspot_keys.txt
-
 # Parse the results
 python3 -m scrub.tools.parsers.get_sonarqube_warnings ${{TOOL_ANALYSIS_DIR}} ${{RAW_RESULTS_DIR}}/sonarqube_raw.scrub ${{SOURCE_DIR}} ${{SONARQUBE_SERVER}}
```

### Comparing `nasa-scrub-2.6.4/scrub/utils/diff_results.py` & `nasa-scrub-2.6.5/scrub/utils/diff_results.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/utils/do_clean.py` & `nasa-scrub-2.6.5/scrub/utils/do_clean.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/utils/filtering/create_file_list.py` & `nasa-scrub-2.6.5/scrub/utils/filtering/create_file_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     if initial_filtering_list:
         # Read in the list
         with open(initial_filtering_list, 'r') as input_fh:
             raw_file_list = input_fh.readlines()
 
     else:
         for root, dir_names, file_names, in os.walk(source_root_dir, topdown=True):
-            dir_names[:] = [d for d in dir_names if d not in ['.scrub']]
+            dir_names[:] = [d for d in dir_names if d not in ['.scrub', 'scrub_results']]
             for file_name in file_names:
                 raw_file_list.append(os.path.join(root, file_name))
 
     # Read in the values from the filtering file and add them to the list
     if filtering_options_file.exists():
         # Print a status message
         logging.info('')
@@ -86,18 +86,20 @@
         # Parse the filtering file
         filtering_options = parse_filtering_file(default_filtering_options_file)
 
     # Modify the list based on the include and exclude options
     filtered_file_list = raw_file_list.copy()
     for filtering_option in filtering_options:
         for file_path in list(filter(re.compile(filtering_option[1]).search, raw_file_list)):
-            if filtering_option[0] == '-':
+            if filtering_option[0] == '-' and os.path.exists(file_path):
+                logging.debug('\tRemoving file from filtering list: %s', file_path)
                 filtered_file_list.remove(file_path)
 
-            elif filtering_option[0] == '+':
+            elif filtering_option[0] == '+' and os.path.exists(file_path):
+                logging.debug('\tAdding file to filtering list: %s', file_path)
                 filtered_file_list.append(file_path)
 
     # Print the results to the output file
     filtered_file_list.sort()
     with open(filtering_output_file, 'w') as output_fh:
         for filtered_file in filtered_file_list:
             if pathlib.Path(filtered_file).anchor == '/':
```

### Comparing `nasa-scrub-2.6.4/scrub/utils/filtering/do_filtering.py` & `nasa-scrub-2.6.5/scrub/utils/filtering/do_filtering.py`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/utils/filtering/filter_results.py` & `nasa-scrub-2.6.5/scrub/utils/filtering/filter_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,28 +215,29 @@
     # Iterate through every warning in the list
     for warning in warning_list:
         # Check to see if it should be ignored
         if baseline_filtering_check(warning['file'], excluded_files):
             continue
 
         # Check to see if the warning is external to the source directory
-        if not enable_external_warnings \
-                and external_warning_check(warning['file'], source_root):
+        if not enable_external_warnings and external_warning_check(warning['file'], source_root):
             continue
 
         # Perform micro filtering checking
         if enable_micro_filtering and micro_filter_check(warning['file'], warning['line'], valid_warning_types):
             continue
 
         # Check to see if the query should be ignore
         if ignore_query_check(warning['tool'], warning['query'], ignore_query_file):
             continue
 
         # If we made it here we want the warning.
-        # Make the warning file path relative and append to filtered list
+        # Make the warning file path relative, make any description references relative, and append to filtered list
         warning['file'] = warning['file'].relative_to(source_root)
+        for i, line in enumerate(warning['description']):
+            warning['description'][i] = line.replace(str(source_root) + '/', '')
         filtered_warnings.append(warning)
 
     # Write out the results
     logging.info('\t>> Results filtered. Writing {}.'.format(output_file))
 
     translate_results.create_scrub_output_file(filtered_warnings, output_file)
```

### Comparing `nasa-scrub-2.6.4/scrub/utils/scrub_defaults.cfg` & `nasa-scrub-2.6.5/scrub/utils/scrub_defaults.cfg`

 * *Files identical despite different names*

### Comparing `nasa-scrub-2.6.4/scrub/utils/scrub_utilities.py` & `nasa-scrub-2.6.5/scrub/utils/scrub_utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pathlib
 import logging
 import threading
 import subprocess
 import configparser
 import argparse
 import urllib.request
-from scrub.tools.parsers import translate_results
 
 
 class Spinner:
     busy = False
     delay = 0.1
 
     @staticmethod
@@ -151,88 +150,14 @@
             raise CommandExecutionError(message)
         else:
             logging.warning('')
             logging.warning('\t%s is empty.', str(input_artifact.name))
             logging.warning('\tThis may or may not be a problem.')
 
 
-def split_results(baseline_file, subset_file, remainder_file, queries):
-    """This function splits a baseline set of SCRUB results into two separate files based on a given query list.
-
-    Inputs:
-        - baseline_file: Absolute path to the baseline file containing SCRUB warnings [string]
-        - subset_file: Absolute path to the output file to contain filtered warnings [string]
-        - remainder_file: Absolute path to the output file to contain remaining warnings not filtered [string]
-        - query_list: List of query strings to filter on [list of strings]
-    """
-
-    # Import the contents of the baseline input file
-    with open(baseline_file, 'r') as input_fh:
-        baseline_data = input_fh.readlines()
-
-    try:
-        # Open the output files
-        subset_fh = open(subset_file, 'w')
-        remainder_fh = open(remainder_file, 'w')
-
-        # Iterate through every line of the baseline data
-        for i in range(0, len(baseline_data)):
-            line = baseline_data[i]
-
-            # Check to see if the line contains a warning header
-            if re.search(translate_results.WARNING_LINE_REGEX, line):
-                # Get the current warning query
-                warning_query = list(filter(None, re.split(":", line)))[-1].strip()
-
-                # Get the full warning content
-                current_warning = get_warning(baseline_data, i)
-
-                # Check to see if the query is in the queries list of interest
-                if warning_query in queries:
-                    # Write the query to the output file
-                    subset_fh.write('%s' % current_warning)
-
-                else:
-                    # If not, write the result to to remaining output file
-                    remainder_fh.write('%s' % current_warning)
-
-    finally:
-        # Close the files
-        subset_fh.close()
-        remainder_fh.close()
-
-
-def get_warning(warning_data, index):
-    """This function gets a complete warning when passed the index of a warning header.
-
-    Inputs:
-        - warning_data: List of lines of warning file contents [list of strings]
-        - index: Index of warning header of interest [int]
-
-    Outputs:
-        - warning_content: Full warnings contents including header data [string]
-    """
-
-    # Initialize variables
-    warning_content = warning_data[index]
-
-    # Get the warning content
-    for i in range(index + 1, len(warning_data)):
-        # Get the line content
-        line = warning_data[i]
-
-        # Make sure you haven't hit the next warning header
-        if re.search(translate_results.WARNING_LINE_REGEX, line):
-            break
-        else:
-            warning_content = warning_content + line
-
-    return warning_content
-
-
 def execute_command(call_string, my_env, output_file=None, interactive=False):
     """This function executes a command string and captures the results.
 
     Inputs:
         - call_string: Command to execute in the shell [string]
         - my_env: Environment to use during execution [dict]
         - output_file: Absolute path to output file for storing results [string] [optional]
@@ -368,15 +293,16 @@
                 scrub_conf_data.update({section_key: user_conf_data.get(user_section, section_key)})
             elif section_key not in scrub_conf_data.keys():
                 # Add the key if it doesn't exist
                 scrub_conf_data.update({section_key: user_conf_data.get(user_section, section_key)})
 
     # Update the configuration data
     for key in scrub_conf_data.keys():
-        scrub_conf_data.update({key: os.path.expandvars(scrub_conf_data.get(key))})
+        if key != 'sonarqube_token':
+            scrub_conf_data.update({key: os.path.expandvars(scrub_conf_data.get(key))})
 
         # # Update boolean values
         if scrub_conf_data.get(key).lower() == 'true':
             scrub_conf_data.update({key: True})
         elif scrub_conf_data.get(key).lower() == 'false':
             scrub_conf_data.update({key: False})
 
@@ -421,24 +347,22 @@
         scrub_working_dir = pathlib.Path(scrub_conf_data.get('scrub_working_dir')).expanduser().resolve()
     scrub_conf_data.update({'scrub_working_dir': scrub_working_dir})
 
     # Make every *path variable absolute and make every *build_dir variable absolute
     for key in scrub_conf_data.keys():
         if re.search(r'.+path', key) and (scrub_conf_data.get(key) != ''):
             path_value = scrub_conf_data.get(key)
-            #path_value = os.path.abspath(os.path.expanduser(path_value))
             path_value = pathlib.Path(path_value).expanduser().resolve()
             scrub_conf_data.update({key: path_value})
 
         elif re.search(r'.+build_dir', key):
             if scrub_conf_data.get(key) == '':
                 scrub_conf_data.update({key: scrub_conf_data.get('source_dir')})
             elif not scrub_conf_data.get(key).startswith(str(scrub_conf_data.get('source_dir'))):
                 path_value = scrub_conf_data.get(key)
-                #path_value = os.path.abspath(os.path.expanduser(path_value))
                 path_value = pathlib.Path(path_value).expanduser().resolve()
                 scrub_conf_data.update({key: path_value})
 
     # Add SCRUB root path
     scrub_path = pathlib.Path(__file__).parents[1]
     scrub_conf_data.update({'scrub_path': scrub_path})
```

### Comparing `nasa-scrub-2.6.4/setup.cfg` & `nasa-scrub-2.6.5/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description_content_type = text/markdown
 name = nasa-scrub
 project_urls = 
 	Bug Tracker = https://github.com/nasa/scrub/issues
 	Documentation = https://nasa.github.io/scrub
 	Source = https://github.com/nasa/scrub
 url = https://github.com/nasa/scrub
-version = 2.6.4
+version = 2.6.5
 
 [options]
 include_package_data = True
 install_requires = 
 packages = find:
 setup_requires = 
 	setuptools
@@ -37,16 +37,16 @@
 	scrub = scrub.scrub_cli:main
 
 [options.packages.find]
 exclude = 
 	tests
 
 [bumpversion]
-new_version = 2.6.4
-current_version = 2.6.3.1
+new_version = 2.6.5
+current_version = 2.6.4
 commit = True
 tag = True
 
 [bumpversion:file:scrub/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
```

