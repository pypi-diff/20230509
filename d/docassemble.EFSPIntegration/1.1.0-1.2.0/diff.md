# Comparing `tmp/docassemble.EFSPIntegration-1.1.0.tar.gz` & `tmp/docassemble.EFSPIntegration-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.EFSPIntegration-1.1.0.tar", last modified: Thu Feb 23 20:38:51 2023, max compression
+gzip compressed data, was "docassemble.EFSPIntegration-1.2.0.tar", last modified: Tue May  9 20:24:58 2023, max compression
```

## Comparing `docassemble.EFSPIntegration-1.1.0.tar` & `docassemble.EFSPIntegration-1.2.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 20:38:51.059982 docassemble.EFSPIntegration-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-02-23 20:38:51.059982 docassemble.EFSPIntegration-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 20:38:51.055982 docassemble.EFSPIntegration-1.1.0/docassemble/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 20:38:51.055982 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26637 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 20:38:51.051982 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 20:38:51.055982 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/
--rw-r--r--   0 runner    (1001) docker     (122)    41267 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/admin_interview.yml
--rw-r--r--   0 runner    (1001) docker     (122)    26764 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/any_filing_interview.yml
--rw-r--r--   0 runner    (1001) docker     (122)    20187 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/case_search.yml
--rw-r--r--   0 runner    (1001) docker     (122)    32170 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/efiling_integration.yml
--rw-r--r--   0 runner    (1001) docker     (122)     7897 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/login_qs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/minimal_interview.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4186 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/toga_payments.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml
--rw-r--r--   0 runner    (1001) docker     (122)      729 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/unauthenticated_interview.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 20:38:51.059982 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/sources/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/sources/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/sources/admin_interview.feature
--rw-r--r--   0 runner    (1001) docker     (122)     8923 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/sources/any_filing_interview.feature
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/sources/example_upload.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/sources/unauthenticated_interview.feature
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 20:38:51.059982 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/static/
--rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/static/Ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 20:38:51.059982 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    13740 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/efm_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    15140 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/interview_logic.py
--rw-r--r--   0 runner    (1001) docker     (122)    35951 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/py_efsp_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 20:38:51.059982 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17006 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/test/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7090 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/test/peoria_to_cr.json
--rw-r--r--   0 runner    (1001) docker     (122)   238595 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/test/temp2.json
--rw-r--r--   0 runner    (1001) docker     (122)     5712 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/test/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    55792 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/test/vars.json
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/docassemble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 20:38:51.055982 docassemble.EFSPIntegration-1.1.0/docassemble.EFSPIntegration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-02-23 20:38:51.000000 docassemble.EFSPIntegration-1.1.0/docassemble.EFSPIntegration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-02-23 20:38:51.000000 docassemble.EFSPIntegration-1.1.0/docassemble.EFSPIntegration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-23 20:38:51.000000 docassemble.EFSPIntegration-1.1.0/docassemble.EFSPIntegration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-23 20:38:51.000000 docassemble.EFSPIntegration-1.1.0/docassemble.EFSPIntegration.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-23 20:38:50.000000 docassemble.EFSPIntegration-1.1.0/docassemble.EFSPIntegration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-02-23 20:38:51.000000 docassemble.EFSPIntegration-1.1.0/docassemble.EFSPIntegration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-23 20:38:51.000000 docassemble.EFSPIntegration-1.1.0/docassemble.EFSPIntegration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-02-23 20:38:51.059982 docassemble.EFSPIntegration-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-02-23 20:38:39.000000 docassemble.EFSPIntegration-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.953632 docassemble.EFSPIntegration-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-09 20:24:58.953632 docassemble.EFSPIntegration-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.945632 docassemble.EFSPIntegration-1.2.0/docassemble/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.949632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30386 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.941632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.949632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/
+-rw-r--r--   0 runner    (1001) docker     (122)    40916 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/admin_interview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    26764 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/any_filing_interview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    20187 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/case_search.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    32169 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/efiling_integration.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     8870 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/login_qs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/minimal_interview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12606 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/toga_payments.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/toga_payments_interview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/unauthenticated_interview.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.949632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/admin_interview.feature
+-rw-r--r--   0 runner    (1001) docker     (122)     8923 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/any_filing_interview.feature
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/example_upload.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/unauthenticated_interview.feature
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.953632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/static/
+-rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/static/Ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.953632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    14390 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/efm_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15778 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/interview_logic.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    38477 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/py_efsp_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.953632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18552 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7090 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/peoria_to_cr.json
+-rw-r--r--   0 runner    (1001) docker     (122)   238595 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/temp2.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5698 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55792 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/vars.json
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.945632 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2174 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-09 20:24:58.953632 docassemble.EFSPIntegration-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/setup.py
```

### Comparing `docassemble.EFSPIntegration-1.1.0/LICENSE` & `docassemble.EFSPIntegration-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/PKG-INFO` & `docassemble.EFSPIntegration-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.EFSPIntegration
-Version: 1.1.0
+Version: 1.2.0
 Home-page: https://github.com/SuffolkLITLab/docassemble-EFSPIntegration
 Author: Bryce Willey
 Author-email: bwilley@suffolk.edu
 License: The MIT License (MIT)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docassemble.EFSPIntegration-1.1.0/README.md` & `docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-# docassemble-EFSPIntegration
-
-A docassemble extension that talks to [a proxy e-filing server](https://github.com/SuffolkLITLab/EfileProxyServer/) easily within a docassemble interview.
-
-Main interviews of import:
-
-* any_filing_interview.yml: allows you to make any type of filing, initial or subsequent
-* admin_interview.yml: lets you handle admin / user functionality, outside of the context of cases and filings
-
-In progress!
-
-## Authors
-
-Quinten Steenhuis (qsteenhuis@suffolk.edu)
-Bryce Willey (bwilley@suffolk.edu)
+Metadata-Version: 2.1
+Name: docassemble.EFSPIntegration
+Version: 1.2.0
+Home-page: https://github.com/SuffolkLITLab/docassemble-EFSPIntegration
+Author: Bryce Willey
+Author-email: bwilley@suffolk.edu
+License: The MIT License (MIT)
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# docassemble-EFSPIntegration
+
+A docassemble extension that talks to [a proxy e-filing server](https://github.com/SuffolkLITLab/EfileProxyServer/) easily within a docassemble interview.
+
+Main interviews of import:
+
+* any_filing_interview.yml: allows you to make any type of filing, initial or subsequent
+* admin_interview.yml: lets you handle admin / user functionality, outside of the context of cases and filings
+
+In progress!
+
+## Authors
+
+Quinten Steenhuis (qsteenhuis@suffolk.edu)
+Bryce Willey (bwilley@suffolk.edu)
```

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/conversions.py` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/conversions.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     DADateTime,
     as_datetime,
     validation_error,
     log,
     as_datetime,
 )
 from docassemble.AssemblyLine.al_general import ALIndividual, ALAddress
-from docassemble.base.functions import get_config, illegal_variable_name, TypeType
+from docassemble.base.functions import get_config
 from .efm_client import ApiResponse, ProxyConnection
 import importlib
 import dateutil.parser
 
 __all__ = [
     "convert_court_to_id",
     "chain_xml",
@@ -28,24 +28,40 @@
     "debug_display",
     "parse_service_contacts",
     "tyler_daterep_to_datetime",
     "tyler_timestamp_to_datetime",
     "validate_tyler_regex",
     "parse_case_info",
     "fetch_case_info",
+    "_payment_type",
+    "_payment_labels",
+    "_payment_expiration",
     "filter_payment_accounts",
     "payment_account_labels",
     "filing_id_and_label",
     "get_tyler_roles",
 ]
 
 TypeType = type(type(None))
 
 
 def convert_court_to_id(trial_court) -> str:
+    """Converts a court type to the specific id string expected by Tyler.
+
+    A fairly ad-hoc function; it will check if the object has several attributes
+    ("tyler_court_code", "tyler_code", or "name"), or if it's already a string, it
+    tries to just make a lower case on the string. We strongly recommend that
+    your court object use the "tyler_court_code" attribute though.
+
+    Args:
+      trial_court: the court object
+
+    Returns:
+      the string that should be the Tyler EFM court id, i.e. `adams` or `peoria:cr`
+    """
     if hasattr(trial_court, "tyler_court_code"):
         return trial_court.tyler_court_code
     if hasattr(trial_court, "tyler_code"):
         return trial_court.tyler_code
     # The probably not right inputs
     if hasattr(trial_court, "name"):
         return str(trial_court.name).lower()
@@ -58,18 +74,30 @@
 
 class SafeDict(dict):
     def disp(self, elem, attr):
         return (self.get(elem) or {}).get(attr, elem)
 
 
 def choices_and_map(
-    codes_list: List, display: str = None, backing: str = None
+    codes_list: List[Dict[str, Any]], display: str = None, backing: str = None
 ) -> Tuple[List[Any], Dict]:
     """Takes the responses from the 'codes' service and make a DA ready list of choices and a map back
-    to the full code object"""
+    to the full code object
+
+    Args:
+      codes_list: should be the direct response from a 'codes' service, i.e. `proxy_conn.get_case_categories(court_id).data`
+      display: a python format string, where the input variables are the keys of the individual code elements. By
+          default, it's "{name}", but could be something else like "{name} ({code})"
+      backing: the key to each dict element in the codes_list that you want to use as the "canonical" representation
+          of the code, i.e. each is unique, and there aren't conflicts
+    Returns:
+      a tuple; first, a list of the codes that can be used at the `choices` in a docassemble field,
+          second, a map of each code, from the backing key to the full code element. Useful for getting
+          all of the information about a code after a user has selected it.
+    """
     if display is None:
         display = "{name}"
     if backing is None:
         backing = "code"
 
     if codes_list is None:
         return [], SafeDict({})
@@ -82,16 +110,27 @@
         (code_obj[backing], display.format(**code_obj)) for code_obj in codes_list
     ]
     codes_map = SafeDict({vv[backing]: vv for vv in codes_list})
     return choices_list, codes_map
 
 
 def pretty_display(data, tab_depth=0, skip_xml=True, item_name=None) -> str:
-    """Given an arbitrarily nested JSON structure, print it nicely.
-    Recursive, for subsequent calls `tab_depth` increases."""
+    """Given an arbitrarily nested JSON structure, print it nicely as markdown.
+    Recursive, for subsequent calls `tab_depth` increases.
+
+    Args:
+      data: the JSON structure (python dicts, lists, strings and ints) to print
+      tab_depth: how many spaces to add before each new line, to make the markdown correct
+      skip_xml: this function is mostly for printing responses from the EfileProxyServer, which
+          lazily returns XML as JSON. If this is true, we won't show the useless XML cruft
+      item_name: when recursing, will show the parent's name when showing elements in a list
+
+    Returns:
+      The string of markdown text that displays info about the given JSON structure
+    """
     tab_inc = 4
     out = ""
     tab_str = " " * tab_depth
     if isinstance(data, list):
         for idx, elem in enumerate(data):
             if item_name:
                 out += tab_str + f"* {item_name}: {idx}\n"
@@ -154,15 +193,16 @@
     else:
         out = tab_str + str(data) + "\n"
     return out
 
 
 def debug_display(resp: ApiResponse) -> str:
     """Returns a string with either the error of the response,
-    or it's data run through pretty_display"""
+    or it's data run through [pretty_display](#pretty_display)
+    """
     if resp.is_ok() and resp.data is None:
         return f"All ok! ({resp.response_code})"
     if not resp.is_ok():
         to_return = resp.error_msg if resp.error_msg is not None else ""
         if get_config("debug"):
             to_return += f"\nResponse Code: {resp.response_code}"
             if hasattr(resp, "data"):
@@ -182,15 +222,15 @@
 
 
 def tyler_timestamp_to_datetime(timestamp_ms: int) -> DADateTime:
     """Given a timestamp in milliseconds from epoch (in UTC), make a datetime from it"""
     return as_datetime(datetime.fromtimestamp(timestamp_ms / 1000, tz=timezone.utc))
 
 
-def validate_tyler_regex(data_field: Mapping) -> Callable:
+def validate_tyler_regex(data_field: Mapping) -> Callable[[str], Any]:
     """
     Return a function that validates a given input with the provided regex,
     suitable for use with Docassemble's `validate:` question modifier
     """
 
     def fn_validate(input_str):
         if not data_field:
@@ -212,15 +252,15 @@
             elif data_field.get("regularexpression") == r"^[0-9]*$":
                 validation_message = "Enter only digits"
         validation_error(validation_message)
 
     return fn_validate
 
 
-def _is_person(possible_person_entity: dict):
+def _is_person(possible_person_entity: dict) -> bool:
     """Helper for getting party ID"""
     # TODO(brycew): could also check the declaredType?
     return possible_person_entity.get("personOtherIdentification") is not None
 
 
 def chain_xml(xml_val, elems: List[Union[str, int]]):
     val = xml_val
@@ -477,30 +517,42 @@
     new_case: DAObject,
     entry: dict,
     court_id: str,
     *,
     fetch: bool = True,
     roles: dict = None,
 ):
+    """Given sparse information about a case, gets the full details about it
+
+    Args:
+      proxy_conn: the connection to the EFileProxyServer
+      new_case: the object to hold all of the information about the case
+      entry: the information we have about the case, usually from a call to `get_cases`
+      court_id: the id of the court that we searched in to get this info
+      fetch: if true, will fetch more detailed information about the case,
+          include the case title
+      roles: a dictionary of the party type codes to the party type name.
+          Used so we can filter and sort participants later
+    """
     if not roles:
         roles = {}
     new_case.details = entry
     new_case.court_id = court_id
     new_case.title = chain_xml(entry, ["value", "caseTitleText", "value"])
     new_case.tracking_id = chain_xml(entry, ["value", "caseTrackingID", "value"])
     new_case.docket_number = chain_xml(entry, ["value", "caseDocketID", "value"])
     new_case.category = chain_xml(entry, ["value", "caseCategoryText", "value"])
 
     if fetch:
         fetch_case_info(proxy_conn, new_case, roles)
 
 
 def fetch_case_info(
-    proxy_conn: ProxyConnection, new_case: DAObject, roles: dict = None
-):
+    proxy_conn: ProxyConnection, new_case: DAObject, roles: Optional[dict] = None
+) -> None:
     """Fills in these attributes with the full case details:
     * attorneys
     * party_to_attorneys
     * case_details_worked
     * case_details
     * case_type
     * title
@@ -612,48 +664,78 @@
                                 )
                             else:
                                 participant.existing_attorney_ids = [attorney_tyler_id]
     new_case.participants.gathered = True
     new_case.attorneys.gathered = True
 
 
-def _payment_labels(acc: Mapping) -> str:
+def _payment_labels(acc: Optional[Mapping]) -> str:
+    if not acc:
+        acc = {}
+    return f"{acc.get('accountName')} ({_payment_type(acc)})"
+
+
+def _payment_type(acc: Mapping) -> str:
     if acc.get("paymentAccountTypeCode") == "CC":
-        return f"{acc.get('accountName')} ({acc.get('cardType',{}).get('value')}, {acc.get('cardLast4')})"
+        return f"{acc.get('cardType',{}).get('value')}, {acc.get('cardLast4')}"
     elif acc.get("paymentAccountTypeCode") == "WV":
-        return f"{acc.get('accountName')} (Waiver account)"
+        return f"Waiver account"
+    else:
+        return f"{acc.get('paymentAccountTypeCode')}"
+
+
+def _payment_expiration(acc: Mapping) -> str:
+    if acc.get("paymentAccountTypeCode") == "CC":
+        return f"{(acc.get('cardMonth') or {}).get('value', '??')}/{(acc.get('cardYear') or {}).get('value', '????')}"
     else:
-        return f"{acc.get('accountName')} ({acc.get('paymentAccountTypeCode')})"
+        return "N/A"
 
 
-def filter_payment_accounts(account_list, allowable_card_types) -> List:
+def filter_payment_accounts(account_list, allowable_card_types: List) -> List:
     """Gets a list of all payment accounts and filters them by if the card is
-    accepted at a particular court"""
+    accepted at a particular court.
+
+    Args:
+      account_list:
+      allowable_card_types: a list of the accepted card types at a court, usually
+        from the 'allowablecardtypes' dict entry in
+        [get_full_court_info](interview_logic#get_full_court_info)'s response
+
+    Returns:
+      the list of payment account choices that are valid for a particular court
+
+    """
     allowed_card = lambda acc: acc.get("paymentAccountTypeCode") != "CC" or (
         acc.get("paymentAccountTypeCode") == "CC"
         and acc.get("cardType", {}).get("value") in allowable_card_types
     )
     return [
         (acct.get("paymentAccountID"), _payment_labels(acct))
         for acct in account_list
         if acct.get("active", {}).get("value") and allowed_card(acct)
     ]
 
 
-def payment_account_labels(resp):
+def payment_account_labels(resp: ApiResponse) -> Optional[List[Dict]]:
+    """Returns all payment accounts as choices, without filters."""
     if resp.data:
         return [
             {account.get("paymentAccountID"): _payment_labels(account)}
             for account in resp.data
         ]
     else:
-        return None
+        log(f"payment_account_labels: {resp}")
+        return []
 
 
-def filing_id_and_label(case: Mapping, style="FILING_ID") -> Dict[str, str]:
+def filing_id_and_label(case: Mapping, style: str = "FILING_ID") -> Dict[str, str]:
+    """Converts a raw case information from [proxy_conn.get_filing_list()](py_efsp_client#get_filing_list)
+    into a key-value pair, where the key is the filing id and the value is the user-facing label
+    for that filing.
+    """
     tracking_id = case.get("caseTrackingID", {}).get("value")
     try:
         filing_id = (
             case.get("documentIdentification", [{}, {}])[1]
             .get("identificationID", {})
             .get("value")
         )
@@ -675,15 +757,15 @@
             == "{urn:tyler:ecf:extensions:Common}FilingCode",
             case.get("documentCategoryText", []),
         ),
         {},
     )
     filing_code = matching_category.get("value", {}).get("value")
     try:
-        filing_date = tyler_timestamp_to_datetime(
+        filing_date: Any = tyler_timestamp_to_datetime(
             case.get("documentFiledDate", {})
             .get("dateRepresentation", {})
             .get("value", {})
             .get("value", 1000)
         )
     except:
         filing_date = ""
@@ -694,15 +776,15 @@
         return {filing_id: filing_label}
     else:
         return {tracking_id: filing_label}
 
 
 def get_tyler_roles(
     proxy_conn: ProxyConnection,
-    login_data: Mapping,
+    login_data: Optional[Mapping],
     user_details: Optional[ApiResponse] = None,
 ) -> Tuple[bool, bool]:
     """Gets whether or not the user of this interview is a Tyler Admin, and a 'global' admin.
     The global admin means that they are allowed to change specific Global payment methods,
     and can be listed under the 'global server admins' section of the 'efile proxy' settings in the
     DAConfig"""
```

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/admin_interview.yml` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/admin_interview.yml`

 * *Files 2% similar despite different names*

```diff
@@ -72,26 +72,26 @@
     ('get_attorney_list', 'Get All Attorneys'),
     ('get_attorney', 'Get Attorney'),
     ('update_attorney', 'Update Attorney'),
     ('remove_attorney', 'Remove Attorney'),
   ]
   
   firm_admin_payment_list = [ 
-    ('get_payment_account_type_list', 'Get Payment Account Type List'),
-    ('get_payment_account', 'Get Payment Account'),
-    ('update_payment_account', 'Update Payment Account'),
-    ('remove_payment_account', 'Remove Payment Account'),
-    ('get_global_payment_account_list', 'Get Global Payment Account List'),
-    ('get_global_payment_account', 'Get Global Payment Account'),
+    ('get_payment_account_type_list', 'Get Payment Method Type List'),
+    ('get_payment_account', 'Get Payment Method'),
+    ('update_payment_account', 'Update Payment Method'),
+    ('remove_payment_account', 'Remove Payment Method'),
+    ('get_global_payment_account_list', 'Get Global Payment Method List'),
+    ('get_global_payment_account', 'Get Global Payment Method'),
   ]
   
   global_admin_payment_list = [
     *firm_admin_payment_list,
-    ('update_global_payment_account', 'Update Global Payment Account'),
-    ('remove_global_payment_account', 'Remove Global Payment Account'),
+    ('update_global_payment_account', 'Update Global Payment Method'),
+    ('remove_global_payment_account', 'Remove Global Payment Method'),
   ]
 ---
 need:
   - tyler_login
   - logged_in_user_is_global_admin
 id: Admin tasks
 question: | 
@@ -131,15 +131,15 @@
 ---
 template: login_status_template
 subject: Login
 content: |
   Logged in: ${ tyler_login }
 
   ${ action_button_html(url_ask(
-      [{'recompute': ['tyler_login','show_resp']}]),
+      [{'recompute': ['logout', 'tyler_login','show_resp']}]),
       label="Login") }
   
   As ${ my_username }
   
   ${ action_button_html(url_ask(
       [{'recompute': ['get_user_self', 'show_resp']}]),
       label="Get self") }
@@ -161,14 +161,19 @@
       [{'recompute': ['get_notification_preferences','show_resp']}]),
       label="Get notification preferences") }
 
    ${ action_button_html(url_ask(
       [{'recompute': ['update_notification_preferences','show_resp']}]),
       label="Update notification preferences") }
 ---
+code: |
+  tyler_header_name = f"TYLER-TOKEN-{jurisdiction_id.upper()}"
+  da_store.delete("EFSP-" + tyler_header_name)
+  logout = True
+---
 template: firm_admin_template
 subject: |
   Firm
 content: |
   % for elem in firm_admin_list:
   ${ action_button_html(url_ask(
       [{'recompute': [elem[0], 'show_resp']}]), 
@@ -299,44 +304,23 @@
     [{'recompute': ['detach_service_contact', 'show_resp']}]),
     label='Detach service contact', id_tag='detach_service_contact') }
 
   ${ action_button_html(url_ask(
     [{'recompute': ['get_attached_cases', 'show_resp']}]),
     label='View attached cases', id_tag='get_attached_cases') }
 ---
-template: payment_template
-subject: |
-  Payment accounts
-content: |
-  * Credit card
-  * Waiver
-  * eCheck
-
-  ${ action_button_html(url_ask([
-      {'undefine': ['new_payment_account', 'creation_status', 'new_account_type_code', 'new_account_name']},
-      {'recompute': ['new_payment_account']}
-    ]),
-    label='New payment Account') }
-
-  % for elem in firm_admin_payment_list:
-  ${ action_button_html(url_ask(
-      [{'recompute': [elem[0], 'show_resp']}]), 
-      label=elem[1]) }
-  
-  % endfor
----
 template: global_admin_payment_template
 subject: |
-  Payment accounts
+  Payment methods
 content: |
   ${ action_button_html(url_ask([
       {'undefine': ['new_payment_account', 'creation_status', 'new_account_type_code', 'new_account_name']},
       {'recompute': ['new_payment_account']}
     ]),
-    label='New payment Account', id_tag='new_payment_account') }
+    label='New payment Method', id_tag='new_payment_account') }
 
   % for elem in global_admin_payment_list:
   ${ action_button_html(url_ask(
       [{'recompute': [elem[0], 'show_resp']}]), 
       label=elem[1], id_tag=elem[0]) }
   
   % endfor
@@ -510,22 +494,22 @@
   Enter an attorney's GUID or select from attorneys in your firm.  
 fields:
   - Attorney id: attorney_id
     datatype: combobox
     code: |
       [{y.get('attorneyID'): f"{y.get('firstName')} {y.get('lastName')}" } for y in proxy_conn.get_attorney_list().data or []]
 ---
-id: payment account id
+id: payment method id
 question: |
-  Payment account id?
+  Payment method id?
 subquestion: |
-  Enter a payment account GUID or select from existing
-  payment accounts in your firm.
+  Enter a payment method GUID or select from existing
+  payment method in your firm.
 fields:
-  - Payment account id: payment_account_id
+  - Payment method id: payment_account_id
     datatype: combobox
     code: |
       payment_account_labels(proxy_conn.get_payment_account_list())
 ---
 depends on: payment_account_id
 code: |
   payment_account_id_resp = proxy_conn.get_payment_account(payment_account_id)
@@ -534,43 +518,43 @@
 code: |
   global_account_id_resp = proxy_conn.get_global_payment_account(global_payment_account_id)
 ---
 reconsider:
   - payment_account_id_resp
 depends on:
   - payment_account_id
-id: update payment account
+id: update payment method
 question: |
-  Update payment account
+  Update payment method
 fields:
-  - Account name: payment_account_name
+  - Payment method name: payment_account_name
     default: ${ payment_account_id_resp.data.get('accountName') if payment_account_id_resp.data else '' }
   - Active?: payment_account_active
     datatype: yesno
     default: ${ payment_account_id_resp.data.get('active',{}).get('value') if payment_account_id_resp.data else False}
 ---
 reconsider:
   - global_account_id_resp
 depends on:
   - global_payment_account_id
-id: update payment account
+id: update global payment method
 question: |
-  Update global payment account
+  Update global payment method
 fields:
-  - Account name: global_account_name
+  - Payment method name: global_account_name
     default: ${ global_account_id_resp.data.get('accountName') if global_account_id_resp.data else '' }
   - Active?: global_account_active
     datatype: yesno
     default: ${ global_account_id_resp.data.get('active',{}).get('value') if global_account_id_resp.data else False}
 ---
-id: global payment account id
+id: global payment method id
 question: |
-  Global payment account id?
+  Global payment method id?
 fields:
-  - Global payment account id: global_payment_account_id
+  - Global payment method id: global_payment_account_id
 ---
 code: |
   service_contact_options = proxy_conn.get_service_contact_list().data or []
 ---
 reconsider: service_contact_options
 id: service contact id
 question: |
@@ -1329,12 +1313,12 @@
 comment: |
   Overrides login_qs: all jurisdictions allowed here are Tyler
 depends on:
   - tyler_login
   - tyler_login_resp
 if: can_check_efile
 code: |
-  logged_in_user_is_admin, logged_in_user_is_global_admin = get_tyler_roles(proxy_conn, tyler_login_resp.data)
+  logged_in_user_is_admin, logged_in_user_is_global_admin = get_tyler_roles(proxy_conn, {"TYLER-ID": tyler_user_id})
 ---
 mandatory: True
 code: |
   all_done
```

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/any_filing_interview.yml` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/any_filing_interview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/case_search.yml` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/case_search.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/efiling_integration.yml` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/efiling_integration.yml`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
     else:
       log(f'Something went wrong: {check_resp.error_msg}')
   elif not remaining_to_check.get("required_vars") and not remaining_to_check.get("wrong_vars"):
     ready_to_efile = True
   else:
     if efile_author_mode:
       show_remaining
-      follow_up_setup 
+      follow_up_setup
       for key in follow_up_vars.keys():
         define(follow_up_vars[key].name, follow_up_vars[key].value)
       ready_to_efile = True
     else:
       ready_to_efile = False
       log(f"Couldn't efile, remaining_to_check: {remaining_to_check}")
       fallback_user_choice
```

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/login_qs.yml` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/login_qs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -86,409 +86,470 @@
 00000550: 6e0a 2020 2020 656c 7365 3a0a 2020 2020  n.    else:.    
 00000560: 2020 6c6f 6728 776f 7264 2822 596f 7520    log(word("You 
 00000570: 6172 6520 6e6f 7720 636f 6e6e 6563 7465  are now connecte
 00000580: 6420 746f 2079 6f75 7220 652d 6669 6c69  d to your e-fili
 00000590: 6e67 2061 6363 6f75 6e74 2229 2c20 2270  ng account"), "p
 000005a0: 7269 6d61 7279 2229 0a20 2074 796c 6572  rimary").  tyler
 000005b0: 5f6c 6f67 696e 203d 2054 7275 650a 2d2d  _login = True.--
-000005c0: 2d0a 636f 6465 3a20 7c0a 2020 7479 6c65  -.code: |.  tyle
-000005d0: 725f 6865 6164 6572 5f6e 616d 6520 3d20  r_header_name = 
-000005e0: 6622 5459 4c45 522d 544f 4b45 4e2d 7b6a  f"TYLER-TOKEN-{j
-000005f0: 7572 6973 6469 6374 696f 6e5f 6964 2e75  urisdiction_id.u
-00000600: 7070 6572 2829 7d22 0a20 2069 6620 6461  pper()}".  if da
-00000610: 5f73 746f 7265 2e64 6566 696e 6564 2822  _store.defined("
-00000620: 4546 5350 2d22 202b 2074 796c 6572 5f68  EFSP-" + tyler_h
-00000630: 6561 6465 725f 6e61 6d65 293a 0a20 2020  eader_name):.   
-00000640: 2070 726f 7879 5f63 6f6e 6e2e 7072 6f78   proxy_conn.prox
-00000650: 795f 636c 6965 6e74 2e68 6561 6465 7273  y_client.headers
-00000660: 5b74 796c 6572 5f68 6561 6465 725f 6e61  [tyler_header_na
-00000670: 6d65 5d20 3d20 6461 5f73 746f 7265 2e67  me] = da_store.g
-00000680: 6574 2822 4546 5350 2d22 202b 2074 796c  et("EFSP-" + tyl
-00000690: 6572 5f68 6561 6465 725f 6e61 6d65 290a  er_header_name).
-000006a0: 2020 2020 7479 6c65 725f 7573 6572 203d      tyler_user =
-000006b0: 2070 726f 7879 5f63 6f6e 6e2e 6765 745f   proxy_conn.get_
-000006c0: 7573 6572 2829 0a20 2020 2069 6620 7479  user().    if ty
-000006d0: 6c65 725f 7573 6572 2e69 735f 6f6b 2829  ler_user.is_ok()
-000006e0: 3a0a 2020 2020 2020 6d79 5f75 7365 726e  :.      my_usern
-000006f0: 616d 6520 3d20 7479 6c65 725f 7573 6572  ame = tyler_user
-00000700: 2e64 6174 612e 6765 7428 2765 6d61 696c  .data.get('email
-00000710: 2729 0a20 2020 2020 206c 6f67 2877 6f72  ').      log(wor
-00000720: 6428 2259 6f75 2061 7265 206e 6f77 2063  d("You are now c
-00000730: 6f6e 6e65 6374 6564 2074 6f20 796f 7572  onnected to your
-00000740: 2065 2d66 696c 696e 6720 6163 636f 756e   e-filing accoun
-00000750: 7422 2920 2b20 6622 2028 7b6d 795f 7573  t") + f" ({my_us
-00000760: 6572 6e61 6d65 7d29 222c 2022 7072 696d  ername})", "prim
-00000770: 6172 7922 290a 2020 2020 2020 6c6f 6767  ary").      logg
-00000780: 6564 5f69 6e5f 7573 6572 5f69 735f 6164  ed_in_user_is_ad
-00000790: 6d69 6e2c 206c 6f67 6765 645f 696e 5f75  min, logged_in_u
-000007a0: 7365 725f 6973 5f67 6c6f 6261 6c5f 6164  ser_is_global_ad
-000007b0: 6d69 6e20 3d20 6765 745f 7479 6c65 725f  min = get_tyler_
-000007c0: 726f 6c65 7328 7072 6f78 795f 636f 6e6e  roles(proxy_conn
-000007d0: 2c20 4e6f 6e65 2c20 7479 6c65 725f 7573  , None, tyler_us
-000007e0: 6572 290a 2020 2020 2020 7479 6c65 725f  er).      tyler_
-000007f0: 6c6f 6769 6e20 3d20 5472 7565 0a2d 2d2d  login = True.---
-00000800: 0a63 6f64 653a 207c 0a20 2063 6861 6e67  .code: |.  chang
-00000810: 655f 7265 7370 203d 2070 726f 7879 5f63  e_resp = proxy_c
-00000820: 6f6e 6e2e 7365 6c66 5f63 6861 6e67 655f  onn.self_change_
-00000830: 7061 7373 776f 7264 2863 7572 7265 6e74  password(current
-00000840: 5f70 6173 7377 6f72 642c 206e 6577 5f75  _password, new_u
-00000850: 7365 725f 7061 7373 776f 7264 290a 2020  ser_password).  
-00000860: 6465 6c20 6375 7272 656e 745f 7061 7373  del current_pass
-00000870: 776f 7264 2c20 6e65 775f 7573 6572 5f70  word, new_user_p
-00000880: 6173 7377 6f72 642c 2063 6f6e 6669 726d  assword, confirm
-00000890: 5f6e 6577 5f70 6173 7377 6f72 640a 2d2d  _new_password.--
-000008a0: 2d0a 636f 6465 3a20 7c0a 2020 6966 2063  -.code: |.  if c
-000008b0: 6861 6e67 655f 7265 7370 2e69 735f 6f6b  hange_resp.is_ok
-000008c0: 2829 3a0a 2020 2020 6368 616e 6765 645f  ():.    changed_
-000008d0: 7061 7373 776f 7264 5f73 6372 6565 6e0a  password_screen.
-000008e0: 2020 2020 7365 6c66 5f63 6861 6e67 655f      self_change_
-000008f0: 7061 7373 776f 7264 203d 2054 7275 650a  password = True.
-00000900: 2020 656c 7365 3a0a 2020 2020 6661 696c    else:.    fail
-00000910: 6564 5f63 6861 6e67 6564 5f70 6173 7377  ed_changed_passw
-00000920: 6f72 645f 7363 7265 656e 0a2d 2d2d 0a69  ord_screen.---.i
-00000930: 643a 2063 6861 6e67 6564 2070 6173 7377  d: changed passw
-00000940: 6f72 640a 7175 6573 7469 6f6e 3a20 7c0a  ord.question: |.
-00000950: 2020 2520 6966 2063 6861 6e67 655f 7265    % if change_re
-00000960: 7370 2e69 735f 6f6b 2829 3a0a 2020 596f  sp.is_ok():.  Yo
-00000970: 7572 2070 6173 7377 6f72 6420 6861 7320  ur password has 
-00000980: 6265 656e 2075 7064 6174 6564 0a20 2025  been updated.  %
-00000990: 2065 6c73 653a 0a20 2059 6f75 7220 7061   else:.  Your pa
-000009a0: 7373 776f 7264 2063 6861 6e67 6520 6661  ssword change fa
-000009b0: 696c 6564 0a20 2025 2065 6e64 6966 0a73  iled.  % endif.s
-000009c0: 7562 7175 6573 7469 6f6e 3a20 7c0a 2020  ubquestion: |.  
-000009d0: 247b 2064 6562 7567 5f64 6973 706c 6179  ${ debug_display
-000009e0: 2863 6861 6e67 655f 7265 7370 2920 7d0a  (change_resp) }.
-000009f0: 636f 6e74 696e 7565 2062 7574 746f 6e20  continue button 
-00000a00: 6669 656c 643a 2063 6861 6e67 6564 5f70  field: changed_p
-00000a10: 6173 7377 6f72 645f 7363 7265 656e 0a2d  assword_screen.-
-00000a20: 2d2d 0a69 643a 2066 6169 6c65 6420 6368  --.id: failed ch
-00000a30: 616e 6765 6420 7061 7373 776f 7264 0a65  anged password.e
-00000a40: 7665 6e74 3a20 6661 696c 6564 5f63 6861  vent: failed_cha
-00000a50: 6e67 6564 5f70 6173 7377 6f72 645f 7363  nged_password_sc
-00000a60: 7265 656e 0a71 7565 7374 696f 6e3a 207c  reen.question: |
-00000a70: 0a20 2059 6f75 7220 7061 7373 776f 7264  .  Your password
-00000a80: 2063 6861 6e67 6520 6661 696c 6564 2e20   change failed. 
-00000a90: 506c 6561 7365 2074 7279 2061 6761 696e  Please try again
-00000aa0: 2e0a 7375 6271 7565 7374 696f 6e3a 207c  ..subquestion: |
-00000ab0: 0a20 2024 7b20 6465 6275 675f 6469 7370  .  ${ debug_disp
-00000ac0: 6c61 7928 6368 616e 6765 5f72 6573 7029  lay(change_resp)
-00000ad0: 207d 0a2d 2d2d 0a69 643a 2070 6173 7377   }.---.id: passw
-00000ae0: 6f72 640a 7175 6573 7469 6f6e 3a20 7c0a  ord.question: |.
-00000af0: 2020 4e65 7720 5061 7373 776f 7264 3f0a    New Password?.
-00000b00: 6669 656c 6473 3a0a 2020 2d20 4e65 7720  fields:.  - New 
-00000b10: 7061 7373 776f 7264 3a20 6e65 775f 7573  password: new_us
-00000b20: 6572 5f70 6173 7377 6f72 640a 2020 2020  er_password.    
-00000b30: 6461 7461 7479 7065 3a20 414c 5669 7369  datatype: ALVisi
-00000b40: 626c 6550 6173 7377 6f72 640a 2020 2d20  blePassword.  - 
-00000b50: 436f 6e66 6972 6d20 6e65 7720 7061 7373  Confirm new pass
-00000b60: 776f 7264 3a20 636f 6e66 6972 6d5f 6e65  word: confirm_ne
-00000b70: 775f 7061 7373 776f 7264 0a20 2020 2064  w_password.    d
-00000b80: 6174 6174 7970 653a 2041 4c56 6973 6962  atatype: ALVisib
-00000b90: 6c65 5061 7373 776f 7264 0a76 616c 6964  lePassword.valid
-00000ba0: 6174 696f 6e20 636f 6465 3a20 7c0a 2020  ation code: |.  
-00000bb0: 6966 206e 6f74 206e 6577 5f75 7365 725f  if not new_user_
-00000bc0: 7061 7373 776f 7264 203d 3d20 636f 6e66  password == conf
-00000bd0: 6972 6d5f 6e65 775f 7061 7373 776f 7264  irm_new_password
-00000be0: 3a0a 2020 2020 7661 6c69 6461 7469 6f6e  :.    validation
-00000bf0: 5f65 7272 6f72 2822 596f 7572 2070 6173  _error("Your pas
-00000c00: 7377 6f72 6473 2064 6f20 6e6f 7420 6d61  swords do not ma
-00000c10: 7463 682e 222c 2066 6965 6c64 3d22 636f  tch.", field="co
-00000c20: 6e66 6972 6d5f 6e65 775f 7061 7373 776f  nfirm_new_passwo
-00000c30: 7264 2229 2020 2020 0a2d 2d2d 0a69 643a  rd")    .---.id:
-00000c40: 2063 6861 6e67 6520 7061 7373 776f 7264   change password
-00000c50: 0a71 7565 7374 696f 6e3a 207c 0a20 2043  .question: |.  C
-00000c60: 6861 6e67 6520 7061 7373 776f 7264 0a66  hange password.f
-00000c70: 6965 6c64 733a 0a20 202d 2043 7572 7265  ields:.  - Curre
-00000c80: 6e74 2070 6173 7377 6f72 643a 2063 7572  nt password: cur
-00000c90: 7265 6e74 5f70 6173 7377 6f72 640a 2020  rent_password.  
-00000ca0: 2020 6461 7461 7479 7065 3a20 414c 5669    datatype: ALVi
-00000cb0: 7369 626c 6550 6173 7377 6f72 640a 2020  siblePassword.  
-00000cc0: 2d20 4e65 7720 7061 7373 776f 7264 3a20  - New password: 
-00000cd0: 6e65 775f 7573 6572 5f70 6173 7377 6f72  new_user_passwor
-00000ce0: 640a 2020 2020 6461 7461 7479 7065 3a20  d.    datatype: 
-00000cf0: 414c 5669 7369 626c 6550 6173 7377 6f72  ALVisiblePasswor
-00000d00: 640a 2020 2d20 436f 6e66 6972 6d20 6e65  d.  - Confirm ne
-00000d10: 7720 7061 7373 776f 7264 3a20 636f 6e66  w password: conf
-00000d20: 6972 6d5f 6e65 775f 7061 7373 776f 7264  irm_new_password
-00000d30: 0a20 2020 2064 6174 6174 7970 653a 2041  .    datatype: A
-00000d40: 4c56 6973 6962 6c65 5061 7373 776f 7264  LVisiblePassword
-00000d50: 0a76 616c 6964 6174 696f 6e20 636f 6465  .validation code
-00000d60: 3a20 7c0a 2020 6966 206e 6f74 206e 6577  : |.  if not new
-00000d70: 5f75 7365 725f 7061 7373 776f 7264 203d  _user_password =
-00000d80: 3d20 636f 6e66 6972 6d5f 6e65 775f 7061  = confirm_new_pa
-00000d90: 7373 776f 7264 3a0a 2020 2020 7661 6c69  ssword:.    vali
-00000da0: 6461 7469 6f6e 5f65 7272 6f72 2877 6f72  dation_error(wor
-00000db0: 6428 2259 6f75 7220 7061 7373 776f 7264  d("Your password
-00000dc0: 7320 646f 206e 6f74 206d 6174 6368 2e22  s do not match."
-00000dd0: 292c 2066 6965 6c64 3d22 636f 6e66 6972  ), field="confir
-00000de0: 6d5f 6e65 775f 7061 7373 776f 7264 2229  m_new_password")
-00000df0: 0a20 2069 6620 6e6f 7420 7072 6f78 795f  .  if not proxy_
-00000e00: 636f 6e6e 2e69 735f 7661 6c69 645f 7061  conn.is_valid_pa
-00000e10: 7373 776f 7264 286e 6577 5f75 7365 725f  ssword(new_user_
-00000e20: 7061 7373 776f 7264 293a 0a20 2020 2070  password):.    p
-00000e30: 6173 7377 6f72 645f 7275 6c65 730a 2020  assword_rules.  
-00000e40: 2020 7661 6c69 6461 7469 6f6e 5f65 7272    validation_err
-00000e50: 6f72 2870 6173 7377 6f72 645f 7275 6c65  or(password_rule
-00000e60: 732e 6461 7461 2e67 6574 2822 7661 6c69  s.data.get("vali
-00000e70: 6461 7469 6f6e 6d65 7373 6167 6522 2929  dationmessage"))
-00000e80: 0a2d 2d2d 0a69 663a 206e 6f74 2063 616e  .---.if: not can
-00000e90: 5f63 6865 636b 5f65 6669 6c65 206f 7220  _check_efile or 
-00000ea0: 6675 6c6c 5f63 6f75 7274 5f69 6e66 6f2e  full_court_info.
-00000eb0: 6765 7428 2265 666d 5479 7065 222c 2022  get("efmType", "
-00000ec0: 6563 6622 2920 213d 2022 6563 6622 0a63  ecf") != "ecf".c
-00000ed0: 6f64 653a 207c 0a20 206c 6f67 6765 645f  ode: |.  logged_
-00000ee0: 696e 5f75 7365 725f 6973 5f61 646d 696e  in_user_is_admin
-00000ef0: 203d 2046 616c 7365 0a20 206c 6f67 6765   = False.  logge
-00000f00: 645f 696e 5f75 7365 725f 6973 5f67 6c6f  d_in_user_is_glo
-00000f10: 6261 6c5f 6164 6d69 6e20 3d20 4661 6c73  bal_admin = Fals
-00000f20: 650a 2d2d 2d0a 6465 7065 6e64 7320 6f6e  e.---.depends on
-00000f30: 3a0a 2020 2d20 7479 6c65 725f 6c6f 6769  :.  - tyler_logi
-00000f40: 6e0a 2020 2d20 7479 6c65 725f 6c6f 6769  n.  - tyler_logi
-00000f50: 6e5f 7265 7370 0a69 663a 2063 616e 5f63  n_resp.if: can_c
-00000f60: 6865 636b 5f65 6669 6c65 2061 6e64 2066  heck_efile and f
-00000f70: 756c 6c5f 636f 7572 745f 696e 666f 2e67  ull_court_info.g
-00000f80: 6574 2822 6566 6d54 7970 6522 2c20 2265  et("efmType", "e
-00000f90: 6366 2229 203d 3d20 2265 6366 220a 636f  cf") == "ecf".co
-00000fa0: 6465 3a20 7c0a 2020 6c6f 6767 6564 5f69  de: |.  logged_i
-00000fb0: 6e5f 7573 6572 5f69 735f 6164 6d69 6e2c  n_user_is_admin,
-00000fc0: 206c 6f67 6765 645f 696e 5f75 7365 725f   logged_in_user_
-00000fd0: 6973 5f67 6c6f 6261 6c5f 6164 6d69 6e20  is_global_admin 
-00000fe0: 3d20 6765 745f 7479 6c65 725f 726f 6c65  = get_tyler_role
-00000ff0: 7328 7072 6f78 795f 636f 6e6e 2c20 7479  s(proxy_conn, ty
-00001000: 6c65 725f 6c6f 6769 6e5f 7265 7370 2e64  ler_login_resp.d
-00001010: 6174 6129 0a2d 2d2d 0a65 7665 6e74 3a20  ata).---.event: 
-00001020: 7265 7365 745f 7061 7373 776f 7264 5f73  reset_password_s
-00001030: 6372 6565 6e0a 7175 6573 7469 6f6e 3a20  creen.question: 
-00001040: 7c0a 2020 2520 6966 2074 796c 6572 5f72  |.  % if tyler_r
-00001050: 6573 6574 5f70 6173 7377 6f72 645f 7265  eset_password_re
-00001060: 7370 2e69 735f 6f6b 2829 3a0a 2020 596f  sp.is_ok():.  Yo
-00001070: 7572 2070 6173 7377 6f72 6420 7265 7365  ur password rese
-00001080: 7420 7761 7320 7265 7175 6573 7465 640a  t was requested.
-00001090: 2020 0a20 2025 2065 6c73 653a 0a20 2053    .  % else:.  S
-000010a0: 6f6d 6574 6869 6e67 2077 656e 7420 7772  omething went wr
-000010b0: 6f6e 6720 7768 656e 2077 6520 7472 6965  ong when we trie
-000010c0: 6420 746f 2072 6573 6574 2079 6f75 7220  d to reset your 
-000010d0: 7061 7373 776f 7264 0a20 2025 2065 6e64  password.  % end
-000010e0: 6966 0a73 7562 7175 6573 7469 6f6e 3a20  if.subquestion: 
-000010f0: 7c0a 2020 247b 2074 796c 6572 5f72 6573  |.  ${ tyler_res
-00001100: 6574 5f70 6173 7377 6f72 645f 7265 7370  et_password_resp
-00001110: 2e65 7272 6f72 5f6d 7367 202b 2022 2e22  .error_msg + "."
-00001120: 2069 6620 6e6f 7420 7479 6c65 725f 7265   if not tyler_re
-00001130: 7365 745f 7061 7373 776f 7264 5f72 6573  set_password_res
-00001140: 702e 6973 5f6f 6b28 2920 656c 7365 2022  p.is_ok() else "
-00001150: 227d 0a0a 2020 596f 7520 6361 6e20 616c  "}..  You can al
-00001160: 736f 205b 7265 7365 6e64 2079 6f75 7220  so [resend your 
-00001170: 6163 7469 7661 7469 6f6e 2065 6d61 696c  activation email
-00001180: 5d28 247b 2075 726c 5f61 736b 280a 2020  ](${ url_ask(.  
-00001190: 2020 2020 5b7b 2772 6563 6f6d 7075 7465      [{'recompute
-000011a0: 273a 205b 2773 656c 665f 7265 7365 6e64  ': ['self_resend
-000011b0: 5f61 6374 6976 6174 696f 6e27 2c27 7368  _activation','sh
-000011c0: 6f77 5f61 6374 6976 6174 696f 6e5f 7265  ow_activation_re
-000011d0: 7370 275d 7d5d 2920 7d29 2e0a 2d2d 2d0a  sp']}]) })..---.
-000011e0: 6964 3a20 7265 7375 6c74 730a 7175 6573  id: results.ques
-000011f0: 7469 6f6e 3a20 7c0a 2020 2520 6966 2072  tion: |.  % if r
-00001200: 6573 656e 745f 6163 7469 7661 7469 6f6e  esent_activation
-00001210: 5f72 6573 702e 6973 5f6f 6b28 293a 0a20  _resp.is_ok():. 
-00001220: 2059 6f75 7220 6163 7469 7661 7469 6f6e   Your activation
-00001230: 2065 6d61 696c 2068 6173 2062 6565 6e20   email has been 
-00001240: 7265 7365 6e74 2e0a 2020 2520 656c 7365  resent..  % else
-00001250: 3a0a 2020 536f 6d65 7468 696e 6720 7765  :.  Something we
-00001260: 6e74 2077 726f 6e67 2077 6865 6e20 7765  nt wrong when we
-00001270: 2074 7269 6564 2074 6f20 7265 7365 6e64   tried to resend
-00001280: 2079 6f75 7220 6163 7469 7661 7469 6f6e   your activation
-00001290: 2065 6d61 696c 2e0a 2020 2520 656e 6469   email..  % endi
-000012a0: 660a 636f 6e74 696e 7565 2062 7574 746f  f.continue butto
-000012b0: 6e20 6669 656c 643a 2073 686f 775f 6163  n field: show_ac
-000012c0: 7469 7661 7469 6f6e 5f72 6573 700a 2d2d  tivation_resp.--
-000012d0: 2d0a 6964 3a20 4c6f 6769 6e20 6661 696c  -.id: Login fail
-000012e0: 6564 0a65 7665 6e74 3a20 6c6f 6769 6e5f  ed.event: login_
-000012f0: 6661 696c 6564 5f73 6372 6565 6e0a 7175  failed_screen.qu
-00001300: 6573 7469 6f6e 3a20 7c0a 2020 5479 6c65  estion: |.  Tyle
-00001310: 7220 4c6f 6769 6e20 6661 696c 6564 0a73  r Login failed.s
-00001320: 7562 7175 6573 7469 6f6e 3a20 7c0a 2020  ubquestion: |.  
-00001330: 2520 6966 2069 6e74 2874 796c 6572 5f6c  % if int(tyler_l
-00001340: 6f67 696e 5f72 6573 702e 7265 7370 6f6e  ogin_resp.respon
-00001350: 7365 5f63 6f64 6529 203d 3d20 3430 333a  se_code) == 403:
-00001360: 0a20 2059 6f75 7220 6c6f 6769 6e20 696e  .  Your login in
-00001370: 666f 726d 6174 696f 6e20 7761 7320 6e6f  formation was no
-00001380: 7420 636f 7272 6563 742e 2047 6f20 6261  t correct. Go ba
-00001390: 636b 2061 6e64 2074 7279 2061 6761 696e  ck and try again
-000013a0: 2e0a 2020 2520 656c 7365 3a0a 2020 536f  ..  % else:.  So
-000013b0: 6d65 7468 696e 6720 7765 6e74 2077 726f  mething went wro
-000013c0: 6e67 2077 6865 6e20 6c6f 6767 696e 6720  ng when logging 
-000013d0: 796f 7520 696e 2e20 5765 2077 696c 6c20  you in. We will 
-000013e0: 6e6f 7420 6265 2061 626c 6520 746f 2065  not be able to e
-000013f0: 2d66 696c 6520 796f 7572 2066 6f72 6d2e  -file your form.
-00001400: 2020 0a20 2025 2065 6e64 6966 0a2d 2d2d    .  % endif.---
-00001410: 0a23 2323 2323 2323 2323 230a 2323 2041  .##########.## A
-00001420: 7320 6120 7265 7375 6c74 206f 6620 6c6f  s a result of lo
-00001430: 6767 696e 6720 696e 2c20 7765 2063 616e  gging in, we can
-00001440: 2075 7365 2064 6566 6175 6c74 732e 2054   use defaults. T
-00001450: 6861 7427 7320 7768 7920 7468 6579 2772  hat's why they'r
-00001460: 6520 696e 2074 6869 7320 6669 6c65 2e0a  e in this file..
-00001470: 2d2d 2d0a 2320 544f 444f 3a20 636f 6e73  ---.# TODO: cons
-00001480: 6964 6572 2072 656d 6f76 696e 6720 6465  ider removing de
-00001490: 6661 756c 7420 7374 6174 650a 6966 3a20  fault state.if: 
-000014a0: 7c0a 2020 6361 6e5f 6368 6563 6b5f 6566  |.  can_check_ef
-000014b0: 696c 650a 6964 3a20 796f 7572 2061 6464  ile.id: your add
-000014c0: 7265 7373 0a73 6574 733a 0a20 202d 2075  ress.sets:.  - u
-000014d0: 7365 7273 5b30 5d2e 6164 6472 6573 732e  sers[0].address.
-000014e0: 6164 6472 6573 730a 2020 2d20 7573 6572  address.  - user
-000014f0: 735b 305d 2e61 6464 7265 7373 2e63 6974  s[0].address.cit
-00001500: 790a 2020 2d20 7573 6572 735b 305d 2e61  y.  - users[0].a
-00001510: 6464 7265 7373 2e7a 6970 0a20 202d 2075  ddress.zip.  - u
-00001520: 7365 7273 5b30 5d2e 6164 6472 6573 732e  sers[0].address.
-00001530: 756e 6974 0a20 202d 2075 7365 7273 5b30  unit.  - users[0
-00001540: 5d2e 6164 6472 6573 732e 7374 6174 650a  ].address.state.
-00001550: 2020 2d20 7573 6572 735b 305d 2e61 6464    - users[0].add
-00001560: 7265 7373 2e63 6f75 6e74 7279 0a71 7565  ress.country.que
-00001570: 7374 696f 6e3a 207c 0a20 2057 6861 7420  stion: |.  What 
-00001580: 6973 2079 6f75 7220 6164 6472 6573 733f  is your address?
-00001590: 0a73 7562 7175 6573 7469 6f6e 3a20 7c0a  .subquestion: |.
-000015a0: 2020 5573 6520 616e 2061 6464 7265 7373    Use an address
-000015b0: 2077 6865 7265 2079 6f75 2063 616e 2062   where you can b
-000015c0: 6520 636f 6e74 6163 7465 642e 0a66 6965  e contacted..fie
-000015d0: 6c64 733a 0a20 202d 2063 6f64 653a 207c  lds:.  - code: |
-000015e0: 0a20 2020 2020 2061 6464 7265 7373 5f66  .      address_f
-000015f0: 6965 6c64 735f 7769 7468 5f64 6566 6175  ields_with_defau
-00001600: 6c74 7328 7072 6f78 795f 636f 6e6e 2c20  lts(proxy_conn, 
-00001610: 7573 6572 735b 305d 2c20 6c6f 6767 6564  users[0], logged
-00001620: 5f69 6e5f 7573 6572 5f69 735f 6164 6d69  _in_user_is_admi
-00001630: 6e2c 2063 6f75 6e74 7279 5f63 6f64 653d  n, country_code=
-00001640: 414c 5f44 4546 4155 4c54 5f43 4f55 4e54  AL_DEFAULT_COUNT
-00001650: 5259 2c20 6465 6661 756c 745f 7374 6174  RY, default_stat
-00001660: 653d 414c 5f44 4546 4155 4c54 5f53 5441  e=AL_DEFAULT_STA
-00001670: 5445 290a 2d2d 2d0a 6964 3a20 636f 7572  TE).---.id: cour
-00001680: 740a 7175 6573 7469 6f6e 3a20 7c0a 2020  t.question: |.  
-00001690: 4368 6f6f 7365 2061 2063 6f75 7274 0a66  Choose a court.f
-000016a0: 6965 6c64 733a 0a20 202d 206e 6f20 6c61  ields:.  - no la
-000016b0: 6265 6c3a 2074 7269 616c 5f63 6f75 7274  bel: trial_court
-000016c0: 0a20 2020 2063 6f64 653a 207c 0a20 2020  .    code: |.   
-000016d0: 2020 2074 7269 616c 5f63 6f75 7274 5f6f     trial_court_o
-000016e0: 7074 696f 6e73 0a2d 2d2d 0a63 6f64 653a  ptions.---.code:
-000016f0: 207c 0a20 2074 7269 616c 5f63 6f75 7274   |.  trial_court
-00001700: 5f72 6573 7020 3d20 7072 6f78 795f 636f  _resp = proxy_co
-00001710: 6e6e 2e67 6574 5f63 6f75 7274 7328 6669  nn.get_courts(fi
-00001720: 6c65 6162 6c65 5f6f 6e6c 793d 5472 7565  leable_only=True
-00001730: 2c20 7769 7468 5f6e 616d 6573 3d54 7275  , with_names=Tru
-00001740: 6529 0a20 2074 7269 616c 5f63 6f75 7274  e).  trial_court
-00001750: 5f6f 7074 696f 6e73 203d 2073 6f72 7465  _options = sorte
-00001760: 6428 5b28 636f 7572 745b 2763 6f64 6527  d([(court['code'
-00001770: 5d2c 2063 6f75 7274 5b27 6e61 6d65 275d  ], court['name']
-00001780: 2920 666f 7220 636f 7572 7420 696e 2074  ) for court in t
-00001790: 7269 616c 5f63 6f75 7274 5f72 6573 702e  rial_court_resp.
-000017a0: 6461 7461 206f 7220 5b5d 5d2c 206b 6579  data or []], key
-000017b0: 3d6c 616d 6264 6120 633a 2063 5b31 5d29  =lambda c: c[1])
-000017c0: 0a20 2074 7269 616c 5f63 6f75 7274 5f6d  .  trial_court_m
-000017d0: 6170 203d 207b 636f 7572 745b 2763 6f64  ap = {court['cod
-000017e0: 6527 5d3a 2063 6f75 7274 5b27 6e61 6d65  e']: court['name
-000017f0: 275d 2066 6f72 2063 6f75 7274 2069 6e20  '] for court in 
-00001800: 7472 6961 6c5f 636f 7572 745f 7265 7370  trial_court_resp
-00001810: 2e64 6174 6120 6f72 205b 5d7d 0a2d 2d2d  .data or []}.---
-00001820: 0a69 663a 2064 6566 696e 6564 2827 636f  .if: defined('co
-00001830: 7572 745f 6964 2729 0a63 6f64 653a 207c  urt_id').code: |
-00001840: 0a20 2074 7269 616c 5f63 6f75 7274 203d  .  trial_court =
-00001850: 2074 7269 616c 5f63 6f75 7274 5f6d 6170   trial_court_map
-00001860: 5b63 6f75 7274 5f69 645d 0a2d 2d2d 0a69  [court_id].---.i
-00001870: 643a 2067 6574 2061 7661 696c 6162 6c65  d: get available
-00001880: 5f65 6669 6c65 5f63 6f75 7274 730a 636f  _efile_courts.co
-00001890: 6465 3a20 7c0a 2020 6176 6169 6c61 626c  de: |.  availabl
-000018a0: 655f 6566 696c 655f 636f 7572 7473 203d  e_efile_courts =
-000018b0: 2067 6574 5f61 7661 696c 6162 6c65 5f65   get_available_e
-000018c0: 6669 6c65 5f63 6f75 7274 7328 7072 6f78  file_courts(prox
-000018d0: 795f 636f 6e6e 290a 2d2d 2d0a 6465 7065  y_conn).---.depe
-000018e0: 6e64 7320 6f6e 3a0a 2020 2d20 7472 6961  nds on:.  - tria
-000018f0: 6c5f 636f 7572 740a 636f 6465 3a20 7c0a  l_court.code: |.
-00001900: 2020 636f 7572 745f 6964 203d 2063 6f6e    court_id = con
-00001910: 7665 7274 5f63 6f75 7274 5f74 6f5f 6964  vert_court_to_id
-00001920: 2874 7269 616c 5f63 6f75 7274 290a 2d2d  (trial_court).--
-00001930: 2d0a 636f 6465 3a20 7c0a 2020 616c 6c5f  -.code: |.  all_
-00001940: 7061 7274 795f 7479 7065 5f6f 7074 696f  party_type_optio
-00001950: 6e73 2c20 616c 6c5f 7061 7274 795f 7479  ns, all_party_ty
-00001960: 7065 5f6d 6170 203d 205c 0a20 2020 2063  pe_map = \.    c
-00001970: 686f 6963 6573 5f61 6e64 5f6d 6170 2870  hoices_and_map(p
-00001980: 726f 7879 5f63 6f6e 6e2e 6765 745f 7061  roxy_conn.get_pa
-00001990: 7274 795f 7479 7065 7328 636f 7572 745f  rty_types(court_
-000019a0: 6964 2c20 4e6f 6e65 292e 6461 7461 290a  id, None).data).
-000019b0: 2d2d 2d0a 6964 3a20 7573 6572 2d77 616e  ---.id: user-wan
-000019c0: 7473 2d65 6669 6c65 0a71 7565 7374 696f  ts-efile.questio
-000019d0: 6e3a 207c 0a20 2044 6f20 796f 7520 7761  n: |.  Do you wa
-000019e0: 6e74 2074 6f20 652d 6669 6c65 2074 6869  nt to e-file thi
-000019f0: 7320 646f 6375 6d65 6e74 2064 6972 6563  s document direc
-00001a00: 746c 7920 7769 7468 2074 6865 2063 6f75  tly with the cou
-00001a10: 7274 3f0a 7375 6271 7565 7374 696f 6e3a  rt?.subquestion:
-00001a20: 207c 0a20 2059 6f75 2061 7265 2061 626c   |.  You are abl
-00001a30: 6520 746f 2065 6c65 6374 726f 6e69 6361  e to electronica
-00001a40: 6c6c 792d 6669 6c65 2028 652d 6669 6c65  lly-file (e-file
-00001a50: 2920 7468 6973 2064 6f63 756d 656e 7420  ) this document 
-00001a60: 7769 7468 2024 7b20 6675 6c6c 5f63 6f75  with ${ full_cou
-00001a70: 7274 5f69 6e66 6f5b 276e 616d 6527 5d20  rt_info['name'] 
-00001a80: 7d21 0a0a 2020 5468 6973 206d 6561 6e73  }!..  This means
-00001a90: 2079 6f75 2064 6f6e 2774 2068 6176 6520   you don't have 
-00001aa0: 746f 2070 7269 6e74 206f 7574 2074 6865  to print out the
-00001ab0: 2064 6f63 756d 656e 742e 2054 6865 2063   document. The c
-00001ac0: 6f75 7274 0a20 2077 696c 6c20 636f 6d6d  ourt.  will comm
-00001ad0: 756e 6963 6174 6520 7769 7468 2079 6f75  unicate with you
-00001ae0: 2074 6872 6f75 6768 2079 6f75 7220 656d   through your em
-00001af0: 6169 6c20 6f72 2070 686f 6e65 2e0a 0a20  ail or phone... 
-00001b00: 2059 6f75 2077 696c 6c20 6861 7665 2074   You will have t
-00001b10: 6f20 7072 6f76 6964 6520 796f 7572 2065  o provide your e
-00001b20: 6d61 696c 2074 6f20 652d 6669 6c65 2074  mail to e-file t
-00001b30: 6869 7320 646f 6375 6d65 6e74 2e20 4966  his document. If
-00001b40: 2079 6f75 2064 6f6e 2774 2077 6973 6820   you don't wish 
-00001b50: 746f 2070 726f 7669 6465 2074 6861 742c  to provide that,
-00001b60: 0a20 2079 6f75 2063 616e 2063 686f 6f73  .  you can choos
-00001b70: 6520 6e6f 7420 746f 2065 6669 6c65 2e0a  e not to efile..
-00001b80: 6669 656c 6473 3a0a 2020 2d20 446f 2079  fields:.  - Do y
-00001b90: 6f75 2077 616e 7420 746f 2065 2d66 696c  ou want to e-fil
-00001ba0: 653f 3a20 7573 6572 5f77 616e 7473 5f65  e?: user_wants_e
-00001bb0: 6669 6c65 0a20 2020 2064 6174 6174 7970  file.    datatyp
-00001bc0: 653a 2079 6573 6e6f 7261 6469 6f0a 2d2d  e: yesnoradio.--
-00001bd0: 2d0a 6964 3a20 796f 752d 7769 6c6c 2d6e  -.id: you-will-n
-00001be0: 6f74 2d62 652d 6162 6c65 2d74 6f2d 6566  ot-be-able-to-ef
-00001bf0: 696c 650a 7175 6573 7469 6f6e 3a20 7c0a  ile.question: |.
-00001c00: 2020 596f 7520 7769 6c6c 202a 6e6f 742a    You will *not*
-00001c10: 2062 6520 6162 6c65 2074 6f20 652d 6669   be able to e-fi
-00001c20: 6c65 2074 6869 7320 646f 6375 6d65 6e74  le this document
-00001c30: 0a73 7562 7175 6573 7469 6f6e 3a20 7c0a  .subquestion: |.
-00001c40: 2020 556e 666f 7274 756e 6174 656c 792c    Unfortunately,
-00001c50: 2079 6f75 2063 616e 6e6f 7420 652d 6669   you cannot e-fi
-00001c60: 6c65 2074 6869 7320 646f 6375 6d65 6e74  le this document
-00001c70: 2061 7420 247b 2074 7269 616c 5f63 6f75   at ${ trial_cou
-00001c80: 7274 207d 2074 6872 6f75 6768 2074 6869  rt } through thi
-00001c90: 7320 7072 6f67 7261 6d2e 0a0a 2020 486f  s program...  Ho
-00001ca0: 7765 7665 722c 2079 6f75 2063 616e 2073  wever, you can s
-00001cb0: 7469 6c6c 2063 6f6e 7469 6e75 6520 616e  till continue an
-00001cc0: 6420 646f 776e 6c6f 6164 2061 2063 6f6d  d download a com
-00001cd0: 706c 6574 6564 2066 6f72 6d20 6174 2074  pleted form at t
-00001ce0: 6865 2065 6e64 2e0a 636f 6e74 696e 7565  he end..continue
-00001cf0: 2062 7574 746f 6e20 6669 656c 643a 2073   button field: s
-00001d00: 686f 775f 6e6f 5f65 6669 6c65 0a2d 2d2d  how_no_efile.---
-00001d10: 0a64 6570 656e 6473 206f 6e3a 0a20 202d  .depends on:.  -
-00001d20: 2063 6f75 7274 5f69 640a 2020 2d20 6176   court_id.  - av
-00001d30: 6169 6c61 626c 655f 6566 696c 655f 636f  ailable_efile_co
-00001d40: 7572 7473 0a6f 6e6c 7920 7365 7473 3a20  urts.only sets: 
-00001d50: 6566 696c 655f 7365 7475 700a 636f 6465  efile_setup.code
-00001d60: 3a20 7c0a 2020 6566 696c 655f 7365 7475  : |.  efile_setu
-00001d70: 7020 3d20 636f 7572 745f 6964 2069 6e20  p = court_id in 
-00001d80: 6176 6169 6c61 626c 655f 6566 696c 655f  available_efile_
-00001d90: 636f 7572 7473 0a2d 2d2d 0a69 643a 2063  courts.---.id: c
-00001da0: 6865 636b 2065 6669 6c65 2070 6f73 7369  heck efile possi
-00001db0: 6269 6c69 7479 0a73 6574 733a 0a20 202d  bility.sets:.  -
-00001dc0: 2063 616e 5f63 6865 636b 5f65 6669 6c65   can_check_efile
-00001dd0: 0a63 6f64 653a 207c 0a20 2069 6620 6566  .code: |.  if ef
-00001de0: 696c 655f 7365 7475 703a 0a20 2020 2023  ile_setup:.    #
-00001df0: 2041 736b 2074 6865 2075 7365 7220 6966   Ask the user if
-00001e00: 2074 6865 7920 7761 6e74 2074 6f20 6566   they want to ef
-00001e10: 696c 650a 2020 2020 6361 6e5f 6368 6563  ile.    can_chec
-00001e20: 6b5f 6566 696c 6520 3d20 7573 6572 5f77  k_efile = user_w
-00001e30: 616e 7473 5f65 6669 6c65 0a20 2065 6c73  ants_efile.  els
-00001e40: 653a 0a20 2020 2073 686f 775f 6e6f 5f65  e:.    show_no_e
-00001e50: 6669 6c65 0a20 2020 2063 616e 5f63 6865  file.    can_che
-00001e60: 636b 5f65 6669 6c65 203d 2046 616c 7365  ck_efile = False
-00001e70: 0a2d 2d2d 0a6f 6e6c 7920 7365 7473 3a20  .---.only sets: 
-00001e80: 6675 6c6c 5f63 6f75 7274 5f69 6e66 6f0a  full_court_info.
-00001e90: 636f 6465 3a20 7c0a 2020 6675 6c6c 5f63  code: |.  full_c
-00001ea0: 6f75 7274 5f69 6e66 6f20 3d20 6765 745f  ourt_info = get_
-00001eb0: 6675 6c6c 5f63 6f75 7274 5f69 6e66 6f28  full_court_info(
-00001ec0: 7072 6f78 795f 636f 6e6e 2c20 636f 7572  proxy_conn, cour
-00001ed0: 745f 6964 290a 2d2d 2d                   t_id).---
+000005c0: 2d0a 6e65 6564 3a0a 2020 2d20 7072 6f78  -.need:.  - prox
+000005d0: 795f 636f 6e6e 0a20 202d 2064 615f 7374  y_conn.  - da_st
+000005e0: 6f72 650a 636f 6465 3a20 7c0a 2020 2020  ore.code: |.    
+000005f0: 7479 6c65 725f 6865 6164 6572 5f6e 616d  tyler_header_nam
+00000600: 6520 3d20 6622 5459 4c45 522d 544f 4b45  e = f"TYLER-TOKE
+00000610: 4e2d 7b6a 7572 6973 6469 6374 696f 6e5f  N-{jurisdiction_
+00000620: 6964 2e75 7070 6572 2829 7d22 0a20 2020  id.upper()}".   
+00000630: 2074 7279 3a0a 2020 2020 2020 6966 2064   try:.      if d
+00000640: 615f 7374 6f72 652e 6465 6669 6e65 6428  a_store.defined(
+00000650: 2245 4653 502d 2220 2b20 7479 6c65 725f  "EFSP-" + tyler_
+00000660: 6865 6164 6572 5f6e 616d 6529 3a0a 2020  header_name):.  
+00000670: 2020 2020 2020 7072 6f78 795f 636f 6e6e        proxy_conn
+00000680: 2e70 726f 7879 5f63 6c69 656e 742e 6865  .proxy_client.he
+00000690: 6164 6572 735b 7479 6c65 725f 6865 6164  aders[tyler_head
+000006a0: 6572 5f6e 616d 655d 203d 2064 615f 7374  er_name] = da_st
+000006b0: 6f72 652e 6765 7428 2245 4653 502d 2220  ore.get("EFSP-" 
+000006c0: 2b20 7479 6c65 725f 6865 6164 6572 5f6e  + tyler_header_n
+000006d0: 616d 6529 0a20 2020 2020 2020 2074 796c  ame).        tyl
+000006e0: 6572 5f75 7365 7220 3d20 7072 6f78 795f  er_user = proxy_
+000006f0: 636f 6e6e 2e67 6574 5f75 7365 7228 290a  conn.get_user().
+00000700: 2020 2020 2020 2020 6966 2074 796c 6572          if tyler
+00000710: 5f75 7365 722e 6973 5f6f 6b28 293a 0a20  _user.is_ok():. 
+00000720: 2020 2020 2020 2020 206d 795f 7573 6572           my_user
+00000730: 6e61 6d65 203d 2074 796c 6572 5f75 7365  name = tyler_use
+00000740: 722e 6461 7461 2e67 6574 2827 656d 6169  r.data.get('emai
+00000750: 6c27 290a 2020 2020 2020 2020 2020 6c6f  l').          lo
+00000760: 6728 776f 7264 2822 596f 7520 6172 6520  g(word("You are 
+00000770: 6e6f 7720 636f 6e6e 6563 7465 6420 746f  now connected to
+00000780: 2079 6f75 7220 652d 6669 6c69 6e67 2061   your e-filing a
+00000790: 6363 6f75 6e74 2229 202b 2066 2220 287b  ccount") + f" ({
+000007a0: 6d79 5f75 7365 726e 616d 657d 2922 2c20  my_username})", 
+000007b0: 2270 7269 6d61 7279 2229 0a20 2020 2020  "primary").     
+000007c0: 2020 2020 206c 6f67 6765 645f 696e 5f75       logged_in_u
+000007d0: 7365 725f 6973 5f61 646d 696e 2c20 6c6f  ser_is_admin, lo
+000007e0: 6767 6564 5f69 6e5f 7573 6572 5f69 735f  gged_in_user_is_
+000007f0: 676c 6f62 616c 5f61 646d 696e 203d 2067  global_admin = g
+00000800: 6574 5f74 796c 6572 5f72 6f6c 6573 2870  et_tyler_roles(p
+00000810: 726f 7879 5f63 6f6e 6e2c 204e 6f6e 652c  roxy_conn, None,
+00000820: 2074 796c 6572 5f75 7365 7229 0a20 2020   tyler_user).   
+00000830: 2020 2020 2020 2074 796c 6572 5f6c 6f67         tyler_log
+00000840: 696e 203d 2054 7275 650a 2020 2020 6578  in = True.    ex
+00000850: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+00000860: 7320 6578 3a0a 2020 2020 2020 6c6f 6728  s ex:.      log(
+00000870: 6622 4572 726f 7220 7768 656e 2074 7279  f"Error when try
+00000880: 696e 6720 746f 2067 6574 2064 615f 7374  ing to get da_st
+00000890: 6f72 6520 5479 6c65 7220 746f 6b65 6e3a  ore Tyler token:
+000008a0: 207b 6578 7d22 290a 2d2d 2d0a 6f6e 6c79   {ex}").---.only
+000008b0: 2073 6574 733a 0a20 202d 2074 796c 6572   sets:.  - tyler
+000008c0: 5f75 7365 725f 6964 0a63 6f64 653a 207c  _user_id.code: |
+000008d0: 0a20 2074 796c 6572 5f75 7365 725f 6964  .  tyler_user_id
+000008e0: 5f6b 6579 203d 2066 2245 4653 502d 5459  _key = f"EFSP-TY
+000008f0: 4c45 522d 4944 2d7b 6a75 7269 7364 6963  LER-ID-{jurisdic
+00000900: 7469 6f6e 5f69 642e 6c6f 7765 7228 297d  tion_id.lower()}
+00000910: 220a 2020 6966 2064 615f 7374 6f72 652e  ".  if da_store.
+00000920: 6465 6669 6e65 6428 7479 6c65 725f 7573  defined(tyler_us
+00000930: 6572 5f69 645f 6b65 7929 3a0a 2020 2020  er_id_key):.    
+00000940: 7479 6c65 725f 7573 6572 5f69 6420 3d20  tyler_user_id = 
+00000950: 6461 5f73 746f 7265 2e67 6574 2874 796c  da_store.get(tyl
+00000960: 6572 5f75 7365 725f 6964 5f6b 6579 290a  er_user_id_key).
+00000970: 2020 656c 7365 3a0a 2020 2020 2320 6e6f    else:.    # no
+00000980: 7420 7468 6572 653a 2077 696c 6c20 6e65  t there: will ne
+00000990: 6564 2074 6f20 6c6f 6769 6e20 746f 2067  ed to login to g
+000009a0: 6574 2074 6865 2073 616d 6520 696e 666f  et the same info
+000009b0: 0a20 2020 2074 796c 6572 5f75 7365 725f  .    tyler_user_
+000009c0: 6964 203d 2074 796c 6572 5f6c 6f67 696e  id = tyler_login
+000009d0: 5f72 6573 702e 6461 7461 0a2d 2d2d 0a63  _resp.data.---.c
+000009e0: 6f64 653a 207c 0a20 2063 6861 6e67 655f  ode: |.  change_
+000009f0: 7265 7370 203d 2070 726f 7879 5f63 6f6e  resp = proxy_con
+00000a00: 6e2e 7365 6c66 5f63 6861 6e67 655f 7061  n.self_change_pa
+00000a10: 7373 776f 7264 2863 7572 7265 6e74 5f70  ssword(current_p
+00000a20: 6173 7377 6f72 642c 206e 6577 5f75 7365  assword, new_use
+00000a30: 725f 7061 7373 776f 7264 290a 2020 6465  r_password).  de
+00000a40: 6c20 6375 7272 656e 745f 7061 7373 776f  l current_passwo
+00000a50: 7264 2c20 6e65 775f 7573 6572 5f70 6173  rd, new_user_pas
+00000a60: 7377 6f72 642c 2063 6f6e 6669 726d 5f6e  sword, confirm_n
+00000a70: 6577 5f70 6173 7377 6f72 640a 2d2d 2d0a  ew_password.---.
+00000a80: 636f 6465 3a20 7c0a 2020 6966 2063 6861  code: |.  if cha
+00000a90: 6e67 655f 7265 7370 2e69 735f 6f6b 2829  nge_resp.is_ok()
+00000aa0: 3a0a 2020 2020 6368 616e 6765 645f 7061  :.    changed_pa
+00000ab0: 7373 776f 7264 5f73 6372 6565 6e0a 2020  ssword_screen.  
+00000ac0: 2020 7365 6c66 5f63 6861 6e67 655f 7061    self_change_pa
+00000ad0: 7373 776f 7264 203d 2054 7275 650a 2020  ssword = True.  
+00000ae0: 656c 7365 3a0a 2020 2020 6661 696c 6564  else:.    failed
+00000af0: 5f63 6861 6e67 6564 5f70 6173 7377 6f72  _changed_passwor
+00000b00: 645f 7363 7265 656e 0a2d 2d2d 0a69 643a  d_screen.---.id:
+00000b10: 2063 6861 6e67 6564 2070 6173 7377 6f72   changed passwor
+00000b20: 640a 7175 6573 7469 6f6e 3a20 7c0a 2020  d.question: |.  
+00000b30: 2520 6966 2063 6861 6e67 655f 7265 7370  % if change_resp
+00000b40: 2e69 735f 6f6b 2829 3a0a 2020 596f 7572  .is_ok():.  Your
+00000b50: 2070 6173 7377 6f72 6420 6861 7320 6265   password has be
+00000b60: 656e 2075 7064 6174 6564 0a20 2025 2065  en updated.  % e
+00000b70: 6c73 653a 0a20 2059 6f75 7220 7061 7373  lse:.  Your pass
+00000b80: 776f 7264 2063 6861 6e67 6520 6661 696c  word change fail
+00000b90: 6564 0a20 2025 2065 6e64 6966 0a73 7562  ed.  % endif.sub
+00000ba0: 7175 6573 7469 6f6e 3a20 7c0a 2020 247b  question: |.  ${
+00000bb0: 2064 6562 7567 5f64 6973 706c 6179 2863   debug_display(c
+00000bc0: 6861 6e67 655f 7265 7370 2920 7d0a 636f  hange_resp) }.co
+00000bd0: 6e74 696e 7565 2062 7574 746f 6e20 6669  ntinue button fi
+00000be0: 656c 643a 2063 6861 6e67 6564 5f70 6173  eld: changed_pas
+00000bf0: 7377 6f72 645f 7363 7265 656e 0a2d 2d2d  sword_screen.---
+00000c00: 0a69 643a 2066 6169 6c65 6420 6368 616e  .id: failed chan
+00000c10: 6765 6420 7061 7373 776f 7264 0a65 7665  ged password.eve
+00000c20: 6e74 3a20 6661 696c 6564 5f63 6861 6e67  nt: failed_chang
+00000c30: 6564 5f70 6173 7377 6f72 645f 7363 7265  ed_password_scre
+00000c40: 656e 0a71 7565 7374 696f 6e3a 207c 0a20  en.question: |. 
+00000c50: 2059 6f75 7220 7061 7373 776f 7264 2063   Your password c
+00000c60: 6861 6e67 6520 6661 696c 6564 2e20 506c  hange failed. Pl
+00000c70: 6561 7365 2074 7279 2061 6761 696e 2e0a  ease try again..
+00000c80: 7375 6271 7565 7374 696f 6e3a 207c 0a20  subquestion: |. 
+00000c90: 2024 7b20 6465 6275 675f 6469 7370 6c61   ${ debug_displa
+00000ca0: 7928 6368 616e 6765 5f72 6573 7029 207d  y(change_resp) }
+00000cb0: 0a2d 2d2d 0a69 643a 2070 6173 7377 6f72  .---.id: passwor
+00000cc0: 640a 7175 6573 7469 6f6e 3a20 7c0a 2020  d.question: |.  
+00000cd0: 4e65 7720 5061 7373 776f 7264 3f0a 6669  New Password?.fi
+00000ce0: 656c 6473 3a0a 2020 2d20 4e65 7720 7061  elds:.  - New pa
+00000cf0: 7373 776f 7264 3a20 6e65 775f 7573 6572  ssword: new_user
+00000d00: 5f70 6173 7377 6f72 640a 2020 2020 6461  _password.    da
+00000d10: 7461 7479 7065 3a20 414c 5669 7369 626c  tatype: ALVisibl
+00000d20: 6550 6173 7377 6f72 640a 2020 2d20 436f  ePassword.  - Co
+00000d30: 6e66 6972 6d20 6e65 7720 7061 7373 776f  nfirm new passwo
+00000d40: 7264 3a20 636f 6e66 6972 6d5f 6e65 775f  rd: confirm_new_
+00000d50: 7061 7373 776f 7264 0a20 2020 2064 6174  password.    dat
+00000d60: 6174 7970 653a 2041 4c56 6973 6962 6c65  atype: ALVisible
+00000d70: 5061 7373 776f 7264 0a76 616c 6964 6174  Password.validat
+00000d80: 696f 6e20 636f 6465 3a20 7c0a 2020 6966  ion code: |.  if
+00000d90: 206e 6f74 206e 6577 5f75 7365 725f 7061   not new_user_pa
+00000da0: 7373 776f 7264 203d 3d20 636f 6e66 6972  ssword == confir
+00000db0: 6d5f 6e65 775f 7061 7373 776f 7264 3a0a  m_new_password:.
+00000dc0: 2020 2020 7661 6c69 6461 7469 6f6e 5f65      validation_e
+00000dd0: 7272 6f72 2822 596f 7572 2070 6173 7377  rror("Your passw
+00000de0: 6f72 6473 2064 6f20 6e6f 7420 6d61 7463  ords do not matc
+00000df0: 682e 222c 2066 6965 6c64 3d22 636f 6e66  h.", field="conf
+00000e00: 6972 6d5f 6e65 775f 7061 7373 776f 7264  irm_new_password
+00000e10: 2229 2020 2020 0a2d 2d2d 0a69 643a 2063  ")    .---.id: c
+00000e20: 6861 6e67 6520 7061 7373 776f 7264 0a71  hange password.q
+00000e30: 7565 7374 696f 6e3a 207c 0a20 2043 6861  uestion: |.  Cha
+00000e40: 6e67 6520 7061 7373 776f 7264 0a66 6965  nge password.fie
+00000e50: 6c64 733a 0a20 202d 2043 7572 7265 6e74  lds:.  - Current
+00000e60: 2070 6173 7377 6f72 643a 2063 7572 7265   password: curre
+00000e70: 6e74 5f70 6173 7377 6f72 640a 2020 2020  nt_password.    
+00000e80: 6461 7461 7479 7065 3a20 414c 5669 7369  datatype: ALVisi
+00000e90: 626c 6550 6173 7377 6f72 640a 2020 2d20  blePassword.  - 
+00000ea0: 4e65 7720 7061 7373 776f 7264 3a20 6e65  New password: ne
+00000eb0: 775f 7573 6572 5f70 6173 7377 6f72 640a  w_user_password.
+00000ec0: 2020 2020 6461 7461 7479 7065 3a20 414c      datatype: AL
+00000ed0: 5669 7369 626c 6550 6173 7377 6f72 640a  VisiblePassword.
+00000ee0: 2020 2d20 436f 6e66 6972 6d20 6e65 7720    - Confirm new 
+00000ef0: 7061 7373 776f 7264 3a20 636f 6e66 6972  password: confir
+00000f00: 6d5f 6e65 775f 7061 7373 776f 7264 0a20  m_new_password. 
+00000f10: 2020 2064 6174 6174 7970 653a 2041 4c56     datatype: ALV
+00000f20: 6973 6962 6c65 5061 7373 776f 7264 0a76  isiblePassword.v
+00000f30: 616c 6964 6174 696f 6e20 636f 6465 3a20  alidation code: 
+00000f40: 7c0a 2020 6966 206e 6f74 206e 6577 5f75  |.  if not new_u
+00000f50: 7365 725f 7061 7373 776f 7264 203d 3d20  ser_password == 
+00000f60: 636f 6e66 6972 6d5f 6e65 775f 7061 7373  confirm_new_pass
+00000f70: 776f 7264 3a0a 2020 2020 7661 6c69 6461  word:.    valida
+00000f80: 7469 6f6e 5f65 7272 6f72 2877 6f72 6428  tion_error(word(
+00000f90: 2259 6f75 7220 7061 7373 776f 7264 7320  "Your passwords 
+00000fa0: 646f 206e 6f74 206d 6174 6368 2e22 292c  do not match."),
+00000fb0: 2066 6965 6c64 3d22 636f 6e66 6972 6d5f   field="confirm_
+00000fc0: 6e65 775f 7061 7373 776f 7264 2229 0a20  new_password"). 
+00000fd0: 2069 6620 6e6f 7420 7072 6f78 795f 636f   if not proxy_co
+00000fe0: 6e6e 2e69 735f 7661 6c69 645f 7061 7373  nn.is_valid_pass
+00000ff0: 776f 7264 286e 6577 5f75 7365 725f 7061  word(new_user_pa
+00001000: 7373 776f 7264 293a 0a20 2020 2070 6173  ssword):.    pas
+00001010: 7377 6f72 645f 7275 6c65 730a 2020 2020  sword_rules.    
+00001020: 7661 6c69 6461 7469 6f6e 5f65 7272 6f72  validation_error
+00001030: 2870 6173 7377 6f72 645f 7275 6c65 732e  (password_rules.
+00001040: 6461 7461 2e67 6574 2822 7661 6c69 6461  data.get("valida
+00001050: 7469 6f6e 6d65 7373 6167 6522 2929 0a2d  tionmessage")).-
+00001060: 2d2d 0a69 663a 206e 6f74 2063 616e 5f63  --.if: not can_c
+00001070: 6865 636b 5f65 6669 6c65 206f 7220 6675  heck_efile or fu
+00001080: 6c6c 5f63 6f75 7274 5f69 6e66 6f2e 6765  ll_court_info.ge
+00001090: 7428 2265 666d 5479 7065 222c 2022 6563  t("efmType", "ec
+000010a0: 6622 2920 213d 2022 6563 6622 0a63 6f64  f") != "ecf".cod
+000010b0: 653a 207c 0a20 206c 6f67 6765 645f 696e  e: |.  logged_in
+000010c0: 5f75 7365 725f 6973 5f61 646d 696e 203d  _user_is_admin =
+000010d0: 2046 616c 7365 0a20 206c 6f67 6765 645f   False.  logged_
+000010e0: 696e 5f75 7365 725f 6973 5f67 6c6f 6261  in_user_is_globa
+000010f0: 6c5f 6164 6d69 6e20 3d20 4661 6c73 650a  l_admin = False.
+00001100: 2d2d 2d0a 6465 7065 6e64 7320 6f6e 3a0a  ---.depends on:.
+00001110: 2020 2d20 7479 6c65 725f 6c6f 6769 6e0a    - tyler_login.
+00001120: 2020 2d20 7479 6c65 725f 6c6f 6769 6e5f    - tyler_login_
+00001130: 7265 7370 0a69 663a 2063 616e 5f63 6865  resp.if: can_che
+00001140: 636b 5f65 6669 6c65 2061 6e64 2066 756c  ck_efile and ful
+00001150: 6c5f 636f 7572 745f 696e 666f 2e67 6574  l_court_info.get
+00001160: 2822 6566 6d54 7970 6522 2c20 2265 6366  ("efmType", "ecf
+00001170: 2229 203d 3d20 2265 6366 220a 636f 6465  ") == "ecf".code
+00001180: 3a20 7c0a 2020 6c6f 6767 6564 5f69 6e5f  : |.  logged_in_
+00001190: 7573 6572 5f69 735f 6164 6d69 6e2c 206c  user_is_admin, l
+000011a0: 6f67 6765 645f 696e 5f75 7365 725f 6973  ogged_in_user_is
+000011b0: 5f67 6c6f 6261 6c5f 6164 6d69 6e20 3d20  _global_admin = 
+000011c0: 6765 745f 7479 6c65 725f 726f 6c65 7328  get_tyler_roles(
+000011d0: 7072 6f78 795f 636f 6e6e 2c20 7b22 5459  proxy_conn, {"TY
+000011e0: 4c45 522d 4944 223a 2074 796c 6572 5f75  LER-ID": tyler_u
+000011f0: 7365 725f 6964 7d29 0a2d 2d2d 0a65 7665  ser_id}).---.eve
+00001200: 6e74 3a20 7265 7365 745f 7061 7373 776f  nt: reset_passwo
+00001210: 7264 5f73 6372 6565 6e0a 7175 6573 7469  rd_screen.questi
+00001220: 6f6e 3a20 7c0a 2020 2520 6966 2074 796c  on: |.  % if tyl
+00001230: 6572 5f72 6573 6574 5f70 6173 7377 6f72  er_reset_passwor
+00001240: 645f 7265 7370 2e69 735f 6f6b 2829 3a0a  d_resp.is_ok():.
+00001250: 2020 596f 7572 2070 6173 7377 6f72 6420    Your password 
+00001260: 7265 7365 7420 7761 7320 7265 7175 6573  reset was reques
+00001270: 7465 640a 2020 0a20 2025 2065 6c73 653a  ted.  .  % else:
+00001280: 0a20 2053 6f6d 6574 6869 6e67 2077 656e  .  Something wen
+00001290: 7420 7772 6f6e 6720 7768 656e 2077 6520  t wrong when we 
+000012a0: 7472 6965 6420 746f 2072 6573 6574 2079  tried to reset y
+000012b0: 6f75 7220 7061 7373 776f 7264 0a20 2025  our password.  %
+000012c0: 2065 6e64 6966 0a73 7562 7175 6573 7469   endif.subquesti
+000012d0: 6f6e 3a20 7c0a 2020 247b 2074 796c 6572  on: |.  ${ tyler
+000012e0: 5f72 6573 6574 5f70 6173 7377 6f72 645f  _reset_password_
+000012f0: 7265 7370 2e65 7272 6f72 5f6d 7367 202b  resp.error_msg +
+00001300: 2022 2e22 2069 6620 6e6f 7420 7479 6c65   "." if not tyle
+00001310: 725f 7265 7365 745f 7061 7373 776f 7264  r_reset_password
+00001320: 5f72 6573 702e 6973 5f6f 6b28 2920 656c  _resp.is_ok() el
+00001330: 7365 2022 227d 0a0a 2020 596f 7520 6361  se ""}..  You ca
+00001340: 6e20 616c 736f 205b 7265 7365 6e64 2079  n also [resend y
+00001350: 6f75 7220 6163 7469 7661 7469 6f6e 2065  our activation e
+00001360: 6d61 696c 5d28 247b 2075 726c 5f61 736b  mail](${ url_ask
+00001370: 280a 2020 2020 2020 5b7b 2772 6563 6f6d  (.      [{'recom
+00001380: 7075 7465 273a 205b 2773 656c 665f 7265  pute': ['self_re
+00001390: 7365 6e64 5f61 6374 6976 6174 696f 6e27  send_activation'
+000013a0: 2c27 7368 6f77 5f61 6374 6976 6174 696f  ,'show_activatio
+000013b0: 6e5f 7265 7370 275d 7d5d 2920 7d29 2e0a  n_resp']}]) })..
+000013c0: 2d2d 2d0a 6964 3a20 7265 7375 6c74 730a  ---.id: results.
+000013d0: 7175 6573 7469 6f6e 3a20 7c0a 2020 2520  question: |.  % 
+000013e0: 6966 2072 6573 656e 745f 6163 7469 7661  if resent_activa
+000013f0: 7469 6f6e 5f72 6573 702e 6973 5f6f 6b28  tion_resp.is_ok(
+00001400: 293a 0a20 2059 6f75 7220 6163 7469 7661  ):.  Your activa
+00001410: 7469 6f6e 2065 6d61 696c 2068 6173 2062  tion email has b
+00001420: 6565 6e20 7265 7365 6e74 2e0a 2020 2520  een resent..  % 
+00001430: 656c 7365 3a0a 2020 536f 6d65 7468 696e  else:.  Somethin
+00001440: 6720 7765 6e74 2077 726f 6e67 2077 6865  g went wrong whe
+00001450: 6e20 7765 2074 7269 6564 2074 6f20 7265  n we tried to re
+00001460: 7365 6e64 2079 6f75 7220 6163 7469 7661  send your activa
+00001470: 7469 6f6e 2065 6d61 696c 2e0a 2020 2520  tion email..  % 
+00001480: 656e 6469 660a 636f 6e74 696e 7565 2062  endif.continue b
+00001490: 7574 746f 6e20 6669 656c 643a 2073 686f  utton field: sho
+000014a0: 775f 6163 7469 7661 7469 6f6e 5f72 6573  w_activation_res
+000014b0: 700a 2d2d 2d0a 6964 3a20 4c6f 6769 6e20  p.---.id: Login 
+000014c0: 6661 696c 6564 0a65 7665 6e74 3a20 6c6f  failed.event: lo
+000014d0: 6769 6e5f 6661 696c 6564 5f73 6372 6565  gin_failed_scree
+000014e0: 6e0a 7175 6573 7469 6f6e 3a20 7c0a 2020  n.question: |.  
+000014f0: 6546 696c 6524 7b20 7374 6174 655f 6e61  eFile${ state_na
+00001500: 6d65 5f74 6f5f 636f 6465 286a 7572 6973  me_to_code(juris
+00001510: 6469 6374 696f 6e5f 6964 2920 7d20 4c6f  diction_id) } Lo
+00001520: 6769 6e20 6661 696c 6564 0a73 7562 7175  gin failed.subqu
+00001530: 6573 7469 6f6e 3a20 7c0a 2020 2520 6966  estion: |.  % if
+00001540: 2069 6e74 2874 796c 6572 5f6c 6f67 696e   int(tyler_login
+00001550: 5f72 6573 702e 7265 7370 6f6e 7365 5f63  _resp.response_c
+00001560: 6f64 6529 203d 3d20 3430 333a 0a20 2059  ode) == 403:.  Y
+00001570: 6f75 7220 6c6f 6769 6e20 696e 666f 726d  our login inform
+00001580: 6174 696f 6e20 7761 7320 6e6f 7420 636f  ation was not co
+00001590: 7272 6563 742e 2047 6f20 6261 636b 2061  rrect. Go back a
+000015a0: 6e64 2074 7279 2061 6761 696e 2e0a 0a20  nd try again... 
+000015b0: 2059 6f75 2063 616e 2072 6573 6574 2079   You can reset y
+000015c0: 6f75 7220 7061 7373 776f 7264 2069 6620  our password if 
+000015d0: 796f 7520 7468 696e 6b20 796f 7572 2070  you think your p
+000015e0: 6173 7377 6f72 6420 6973 2077 726f 6e67  assword is wrong
+000015f0: 2e0a 2020 0a20 2024 7b20 6163 7469 6f6e  ..  .  ${ action
+00001600: 5f62 7574 746f 6e5f 6874 6d6c 2869 6e74  _button_html(int
+00001610: 6572 7669 6577 5f75 726c 2869 3d6c 6f67  erview_url(i=log
+00001620: 6765 645f 6f75 745f 696e 7465 7276 6965  ged_out_intervie
+00001630: 772c 2072 6573 6574 3d31 2c20 6a75 7269  w, reset=1, juri
+00001640: 7364 6963 7469 6f6e 5f69 643d 6a75 7269  sdiction_id=juri
+00001650: 7364 6963 7469 6f6e 5f69 6429 2c20 6c61  sdiction_id), la
+00001660: 6265 6c3d 2252 6573 6574 2079 6f75 7220  bel="Reset your 
+00001670: 7061 7373 776f 7264 222c 206e 6577 5f77  password", new_w
+00001680: 696e 646f 773d 5472 7565 297d 0a0a 2020  indow=True)}..  
+00001690: 596f 7520 6361 6e20 616c 736f 2072 6567  You can also reg
+000016a0: 6973 7465 7220 666f 7220 616e 2061 6363  ister for an acc
+000016b0: 6f75 6e74 2069 6620 796f 7520 646f 6e27  ount if you don'
+000016c0: 7420 6861 7665 206f 6e65 2079 6574 2e0a  t have one yet..
+000016d0: 0a20 2024 7b20 6163 7469 6f6e 5f62 7574  .  ${ action_but
+000016e0: 746f 6e5f 6874 6d6c 2869 6e74 6572 7669  ton_html(intervi
+000016f0: 6577 5f75 726c 2869 3d6c 6f67 6765 645f  ew_url(i=logged_
+00001700: 6f75 745f 696e 7465 7276 6965 772c 2072  out_interview, r
+00001710: 6573 6574 3d31 2c20 6a75 7269 7364 6963  eset=1, jurisdic
+00001720: 7469 6f6e 5f69 643d 6a75 7269 7364 6963  tion_id=jurisdic
+00001730: 7469 6f6e 5f69 6429 2c20 6c61 6265 6c3d  tion_id), label=
+00001740: 2252 6567 6973 7465 7220 666f 7220 6120  "Register for a 
+00001750: 6e65 7720 6163 636f 756e 7422 2c20 6e65  new account", ne
+00001760: 775f 7769 6e64 6f77 3d54 7275 6529 7d0a  w_window=True)}.
+00001770: 0a20 2025 2065 6c73 653a 0a20 2053 6f6d  .  % else:.  Som
+00001780: 6574 6869 6e67 2077 656e 7420 7772 6f6e  ething went wron
+00001790: 6720 7768 656e 206c 6f67 6769 6e67 2079  g when logging y
+000017a0: 6f75 2069 6e2e 2057 6520 7769 6c6c 206e  ou in. We will n
+000017b0: 6f74 2062 6520 6162 6c65 2074 6f20 652d  ot be able to e-
+000017c0: 6669 6c65 2079 6f75 7220 666f 726d 2e0a  file your form..
+000017d0: 2020 2520 656e 6469 660a 2d2d 2d0a 2323    % endif.---.##
+000017e0: 2323 2323 2323 2323 0a23 2320 4173 2061  ########.## As a
+000017f0: 2072 6573 756c 7420 6f66 206c 6f67 6769   result of loggi
+00001800: 6e67 2069 6e2c 2077 6520 6361 6e20 7573  ng in, we can us
+00001810: 6520 6465 6661 756c 7473 2e20 5468 6174  e defaults. That
+00001820: 2773 2077 6879 2074 6865 7927 7265 2069  's why they're i
+00001830: 6e20 7468 6973 2066 696c 652e 0a2d 2d2d  n this file..---
+00001840: 0a23 2054 4f44 4f3a 2063 6f6e 7369 6465  .# TODO: conside
+00001850: 7220 7265 6d6f 7669 6e67 2064 6566 6175  r removing defau
+00001860: 6c74 2073 7461 7465 0a69 663a 207c 0a20  lt state.if: |. 
+00001870: 2063 616e 5f63 6865 636b 5f65 6669 6c65   can_check_efile
+00001880: 0a69 643a 2079 6f75 7220 6164 6472 6573  .id: your addres
+00001890: 730a 7365 7473 3a0a 2020 2d20 7573 6572  s.sets:.  - user
+000018a0: 735b 305d 2e61 6464 7265 7373 2e61 6464  s[0].address.add
+000018b0: 7265 7373 0a20 202d 2075 7365 7273 5b30  ress.  - users[0
+000018c0: 5d2e 6164 6472 6573 732e 6369 7479 0a20  ].address.city. 
+000018d0: 202d 2075 7365 7273 5b30 5d2e 6164 6472   - users[0].addr
+000018e0: 6573 732e 7a69 700a 2020 2d20 7573 6572  ess.zip.  - user
+000018f0: 735b 305d 2e61 6464 7265 7373 2e75 6e69  s[0].address.uni
+00001900: 740a 2020 2d20 7573 6572 735b 305d 2e61  t.  - users[0].a
+00001910: 6464 7265 7373 2e73 7461 7465 0a20 202d  ddress.state.  -
+00001920: 2075 7365 7273 5b30 5d2e 6164 6472 6573   users[0].addres
+00001930: 732e 636f 756e 7472 790a 7175 6573 7469  s.country.questi
+00001940: 6f6e 3a20 7c0a 2020 5768 6174 2069 7320  on: |.  What is 
+00001950: 796f 7572 2061 6464 7265 7373 3f0a 7375  your address?.su
+00001960: 6271 7565 7374 696f 6e3a 207c 0a20 2055  bquestion: |.  U
+00001970: 7365 2061 6e20 6164 6472 6573 7320 7768  se an address wh
+00001980: 6572 6520 796f 7520 6361 6e20 6265 2063  ere you can be c
+00001990: 6f6e 7461 6374 6564 2e0a 6669 656c 6473  ontacted..fields
+000019a0: 3a0a 2020 2d20 636f 6465 3a20 7c0a 2020  :.  - code: |.  
+000019b0: 2020 2020 6164 6472 6573 735f 6669 656c      address_fiel
+000019c0: 6473 5f77 6974 685f 6465 6661 756c 7473  ds_with_defaults
+000019d0: 2870 726f 7879 5f63 6f6e 6e2c 2075 7365  (proxy_conn, use
+000019e0: 7273 5b30 5d2c 206c 6f67 6765 645f 696e  rs[0], logged_in
+000019f0: 5f75 7365 725f 6973 5f61 646d 696e 2c20  _user_is_admin, 
+00001a00: 636f 756e 7472 795f 636f 6465 3d41 4c5f  country_code=AL_
+00001a10: 4445 4641 554c 545f 434f 554e 5452 592c  DEFAULT_COUNTRY,
+00001a20: 2064 6566 6175 6c74 5f73 7461 7465 3d41   default_state=A
+00001a30: 4c5f 4445 4641 554c 545f 5354 4154 4529  L_DEFAULT_STATE)
+00001a40: 0a2d 2d2d 0a69 643a 2063 6f75 7274 0a71  .---.id: court.q
+00001a50: 7565 7374 696f 6e3a 207c 0a20 2043 686f  uestion: |.  Cho
+00001a60: 6f73 6520 6120 636f 7572 740a 6669 656c  ose a court.fiel
+00001a70: 6473 3a0a 2020 2d20 6e6f 206c 6162 656c  ds:.  - no label
+00001a80: 3a20 7472 6961 6c5f 636f 7572 740a 2020  : trial_court.  
+00001a90: 2020 636f 6465 3a20 7c0a 2020 2020 2020    code: |.      
+00001aa0: 7472 6961 6c5f 636f 7572 745f 6f70 7469  trial_court_opti
+00001ab0: 6f6e 730a 2d2d 2d0a 636f 6465 3a20 7c0a  ons.---.code: |.
+00001ac0: 2020 7472 6961 6c5f 636f 7572 745f 7265    trial_court_re
+00001ad0: 7370 203d 2070 726f 7879 5f63 6f6e 6e2e  sp = proxy_conn.
+00001ae0: 6765 745f 636f 7572 7473 2866 696c 6561  get_courts(filea
+00001af0: 626c 655f 6f6e 6c79 3d54 7275 652c 2077  ble_only=True, w
+00001b00: 6974 685f 6e61 6d65 733d 5472 7565 290a  ith_names=True).
+00001b10: 2020 7472 6961 6c5f 636f 7572 745f 6f70    trial_court_op
+00001b20: 7469 6f6e 7320 3d20 736f 7274 6564 285b  tions = sorted([
+00001b30: 2863 6f75 7274 5b27 636f 6465 275d 2c20  (court['code'], 
+00001b40: 636f 7572 745b 276e 616d 6527 5d29 2066  court['name']) f
+00001b50: 6f72 2063 6f75 7274 2069 6e20 7472 6961  or court in tria
+00001b60: 6c5f 636f 7572 745f 7265 7370 2e64 6174  l_court_resp.dat
+00001b70: 6120 6f72 205b 5d5d 2c20 6b65 793d 6c61  a or []], key=la
+00001b80: 6d62 6461 2063 3a20 635b 315d 290a 2020  mbda c: c[1]).  
+00001b90: 7472 6961 6c5f 636f 7572 745f 6d61 7020  trial_court_map 
+00001ba0: 3d20 7b63 6f75 7274 5b27 636f 6465 275d  = {court['code']
+00001bb0: 3a20 636f 7572 745b 276e 616d 6527 5d20  : court['name'] 
+00001bc0: 666f 7220 636f 7572 7420 696e 2074 7269  for court in tri
+00001bd0: 616c 5f63 6f75 7274 5f72 6573 702e 6461  al_court_resp.da
+00001be0: 7461 206f 7220 5b5d 7d0a 2d2d 2d0a 6966  ta or []}.---.if
+00001bf0: 3a20 6465 6669 6e65 6428 2763 6f75 7274  : defined('court
+00001c00: 5f69 6427 290a 636f 6465 3a20 7c0a 2020  _id').code: |.  
+00001c10: 7472 6961 6c5f 636f 7572 7420 3d20 7472  trial_court = tr
+00001c20: 6961 6c5f 636f 7572 745f 6d61 705b 636f  ial_court_map[co
+00001c30: 7572 745f 6964 5d0a 2d2d 2d0a 6964 3a20  urt_id].---.id: 
+00001c40: 6765 7420 6176 6169 6c61 626c 655f 6566  get available_ef
+00001c50: 696c 655f 636f 7572 7473 0a63 6f64 653a  ile_courts.code:
+00001c60: 207c 0a20 2061 7661 696c 6162 6c65 5f65   |.  available_e
+00001c70: 6669 6c65 5f63 6f75 7274 7320 3d20 6765  file_courts = ge
+00001c80: 745f 6176 6169 6c61 626c 655f 6566 696c  t_available_efil
+00001c90: 655f 636f 7572 7473 2870 726f 7879 5f63  e_courts(proxy_c
+00001ca0: 6f6e 6e29 0a2d 2d2d 0a64 6570 656e 6473  onn).---.depends
+00001cb0: 206f 6e3a 0a20 202d 2074 7269 616c 5f63   on:.  - trial_c
+00001cc0: 6f75 7274 0a63 6f64 653a 207c 0a20 2063  ourt.code: |.  c
+00001cd0: 6f75 7274 5f69 6420 3d20 636f 6e76 6572  ourt_id = conver
+00001ce0: 745f 636f 7572 745f 746f 5f69 6428 7472  t_court_to_id(tr
+00001cf0: 6961 6c5f 636f 7572 7429 0a2d 2d2d 0a63  ial_court).---.c
+00001d00: 6f64 653a 207c 0a20 2061 6c6c 5f70 6172  ode: |.  all_par
+00001d10: 7479 5f74 7970 655f 6f70 7469 6f6e 732c  ty_type_options,
+00001d20: 2061 6c6c 5f70 6172 7479 5f74 7970 655f   all_party_type_
+00001d30: 6d61 7020 3d20 5c0a 2020 2020 6368 6f69  map = \.    choi
+00001d40: 6365 735f 616e 645f 6d61 7028 7072 6f78  ces_and_map(prox
+00001d50: 795f 636f 6e6e 2e67 6574 5f70 6172 7479  y_conn.get_party
+00001d60: 5f74 7970 6573 2863 6f75 7274 5f69 642c  _types(court_id,
+00001d70: 204e 6f6e 6529 2e64 6174 6129 0a2d 2d2d   None).data).---
+00001d80: 0a69 643a 2075 7365 722d 7761 6e74 732d  .id: user-wants-
+00001d90: 6566 696c 650a 7175 6573 7469 6f6e 3a20  efile.question: 
+00001da0: 7c0a 2020 446f 2079 6f75 2077 616e 7420  |.  Do you want 
+00001db0: 746f 2065 2d66 696c 6520 7468 6973 2064  to e-file this d
+00001dc0: 6f63 756d 656e 7420 6469 7265 6374 6c79  ocument directly
+00001dd0: 2077 6974 6820 7468 6520 636f 7572 743f   with the court?
+00001de0: 0a73 7562 7175 6573 7469 6f6e 3a20 7c0a  .subquestion: |.
+00001df0: 2020 596f 7520 6172 6520 6162 6c65 2074    You are able t
+00001e00: 6f20 656c 6563 7472 6f6e 6963 616c 6c79  o electronically
+00001e10: 2d66 696c 6520 2865 2d66 696c 6529 2074  -file (e-file) t
+00001e20: 6869 7320 646f 6375 6d65 6e74 2077 6974  his document wit
+00001e30: 6820 247b 2066 756c 6c5f 636f 7572 745f  h ${ full_court_
+00001e40: 696e 666f 5b27 6e61 6d65 275d 207d 210a  info['name'] }!.
+00001e50: 0a20 2054 6869 7320 6d65 616e 7320 796f  .  This means yo
+00001e60: 7520 646f 6e27 7420 6861 7665 2074 6f20  u don't have to 
+00001e70: 7072 696e 7420 6f75 7420 7468 6520 646f  print out the do
+00001e80: 6375 6d65 6e74 2e20 5468 6520 636f 7572  cument. The cour
+00001e90: 740a 2020 7769 6c6c 2063 6f6d 6d75 6e69  t.  will communi
+00001ea0: 6361 7465 2077 6974 6820 796f 7520 7468  cate with you th
+00001eb0: 726f 7567 6820 796f 7572 2065 6d61 696c  rough your email
+00001ec0: 206f 7220 7068 6f6e 652e 0a0a 2020 596f   or phone...  Yo
+00001ed0: 7520 7769 6c6c 2068 6176 6520 746f 2070  u will have to p
+00001ee0: 726f 7669 6465 2079 6f75 7220 656d 6169  rovide your emai
+00001ef0: 6c20 746f 2065 2d66 696c 6520 7468 6973  l to e-file this
+00001f00: 2064 6f63 756d 656e 742e 2049 6620 796f   document. If yo
+00001f10: 7520 646f 6e27 7420 7769 7368 2074 6f20  u don't wish to 
+00001f20: 7072 6f76 6964 6520 7468 6174 2c0a 2020  provide that,.  
+00001f30: 796f 7520 6361 6e20 6368 6f6f 7365 206e  you can choose n
+00001f40: 6f74 2074 6f20 6566 696c 652e 0a66 6965  ot to efile..fie
+00001f50: 6c64 733a 0a20 202d 2044 6f20 796f 7520  lds:.  - Do you 
+00001f60: 7761 6e74 2074 6f20 652d 6669 6c65 3f3a  want to e-file?:
+00001f70: 2075 7365 725f 7761 6e74 735f 6566 696c   user_wants_efil
+00001f80: 650a 2020 2020 6461 7461 7479 7065 3a20  e.    datatype: 
+00001f90: 7965 736e 6f72 6164 696f 0a2d 2d2d 0a69  yesnoradio.---.i
+00001fa0: 643a 2079 6f75 2d77 696c 6c2d 6e6f 742d  d: you-will-not-
+00001fb0: 6265 2d61 626c 652d 746f 2d65 6669 6c65  be-able-to-efile
+00001fc0: 0a71 7565 7374 696f 6e3a 207c 0a20 2059  .question: |.  Y
+00001fd0: 6f75 2077 696c 6c20 2a6e 6f74 2a20 6265  ou will *not* be
+00001fe0: 2061 626c 6520 746f 2065 2d66 696c 6520   able to e-file 
+00001ff0: 7468 6973 2064 6f63 756d 656e 740a 7375  this document.su
+00002000: 6271 7565 7374 696f 6e3a 207c 0a20 2055  bquestion: |.  U
+00002010: 6e66 6f72 7475 6e61 7465 6c79 2c20 796f  nfortunately, yo
+00002020: 7520 6361 6e6e 6f74 2065 2d66 696c 6520  u cannot e-file 
+00002030: 7468 6973 2064 6f63 756d 656e 7420 6174  this document at
+00002040: 2024 7b20 7472 6961 6c5f 636f 7572 7420   ${ trial_court 
+00002050: 7d20 7468 726f 7567 6820 7468 6973 2070  } through this p
+00002060: 726f 6772 616d 2e0a 0a20 2048 6f77 6576  rogram...  Howev
+00002070: 6572 2c20 796f 7520 6361 6e20 7374 696c  er, you can stil
+00002080: 6c20 636f 6e74 696e 7565 2061 6e64 2064  l continue and d
+00002090: 6f77 6e6c 6f61 6420 6120 636f 6d70 6c65  ownload a comple
+000020a0: 7465 6420 666f 726d 2061 7420 7468 6520  ted form at the 
+000020b0: 656e 642e 0a63 6f6e 7469 6e75 6520 6275  end..continue bu
+000020c0: 7474 6f6e 2066 6965 6c64 3a20 7368 6f77  tton field: show
+000020d0: 5f6e 6f5f 6566 696c 650a 2d2d 2d0a 6465  _no_efile.---.de
+000020e0: 7065 6e64 7320 6f6e 3a0a 2020 2d20 636f  pends on:.  - co
+000020f0: 7572 745f 6964 0a20 202d 2061 7661 696c  urt_id.  - avail
+00002100: 6162 6c65 5f65 6669 6c65 5f63 6f75 7274  able_efile_court
+00002110: 730a 6f6e 6c79 2073 6574 733a 2065 6669  s.only sets: efi
+00002120: 6c65 5f73 6574 7570 0a63 6f64 653a 207c  le_setup.code: |
+00002130: 0a20 2065 6669 6c65 5f73 6574 7570 203d  .  efile_setup =
+00002140: 2063 6f75 7274 5f69 6420 696e 2061 7661   court_id in ava
+00002150: 696c 6162 6c65 5f65 6669 6c65 5f63 6f75  ilable_efile_cou
+00002160: 7274 730a 2d2d 2d0a 6964 3a20 6368 6563  rts.---.id: chec
+00002170: 6b20 6566 696c 6520 706f 7373 6962 696c  k efile possibil
+00002180: 6974 790a 7365 7473 3a0a 2020 2d20 6361  ity.sets:.  - ca
+00002190: 6e5f 6368 6563 6b5f 6566 696c 650a 636f  n_check_efile.co
+000021a0: 6465 3a20 7c0a 2020 6966 2065 6669 6c65  de: |.  if efile
+000021b0: 5f73 6574 7570 3a0a 2020 2020 2320 4173  _setup:.    # As
+000021c0: 6b20 7468 6520 7573 6572 2069 6620 7468  k the user if th
+000021d0: 6579 2077 616e 7420 746f 2065 6669 6c65  ey want to efile
+000021e0: 0a20 2020 2063 616e 5f63 6865 636b 5f65  .    can_check_e
+000021f0: 6669 6c65 203d 2075 7365 725f 7761 6e74  file = user_want
+00002200: 735f 6566 696c 650a 2020 656c 7365 3a0a  s_efile.  else:.
+00002210: 2020 2020 7368 6f77 5f6e 6f5f 6566 696c      show_no_efil
+00002220: 650a 2020 2020 6361 6e5f 6368 6563 6b5f  e.    can_check_
+00002230: 6566 696c 6520 3d20 4661 6c73 650a 2d2d  efile = False.--
+00002240: 2d0a 6f6e 6c79 2073 6574 733a 2066 756c  -.only sets: ful
+00002250: 6c5f 636f 7572 745f 696e 666f 0a63 6f64  l_court_info.cod
+00002260: 653a 207c 0a20 2066 756c 6c5f 636f 7572  e: |.  full_cour
+00002270: 745f 696e 666f 203d 2067 6574 5f66 756c  t_info = get_ful
+00002280: 6c5f 636f 7572 745f 696e 666f 2870 726f  l_court_info(pro
+00002290: 7879 5f63 6f6e 6e2c 2063 6f75 7274 5f69  xy_conn, court_i
+000022a0: 6429 0a2d 2d2d                           d).---
```

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/minimal_interview.yml` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/minimal_interview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/questions/unauthenticated_interview.yml` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/unauthenticated_interview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/sources/admin_interview.feature` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/admin_interview.feature`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/sources/any_filing_interview.feature` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/any_filing_interview.feature`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/sources/example_upload.pdf` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/example_upload.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/data/static/Ajax-loader.gif` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/static/Ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/efm_client.py` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/efm_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,28 +116,31 @@
         doc.pop("filing_component_options", None)
         doc.pop("optional_service_map", None)
 
     return all_vars_dict
 
 
 class ProxyConnection(EfspConnection):
+    """The main class you use to communicate with the E-file proxy server from docassemble.
+
+    Many methods are unchanged from the parent class, [EfspConnection](py_efsp_client#EfspConnection),
+    and are documented there.
+    """
+
     def __init__(
         self,
         *,
         url: str = None,
         api_key: str = None,
         credentials_code_block: str = "tyler_login",
         default_jurisdiction: str = None,
     ):
         """
-        Params:
-          url (str)
-          api_key (str)
-          credentials_code_block (str)
-          default_jurisdiction (str)
+        Creates the connection. Tries to get params from docassemble's config, but can
+        be overriden with parameters to __init__.
         """
         temp_efile_config = get_config("efile proxy", {})
         if url is None:
             url = temp_efile_config.get("url", "")
         if api_key is None:
             api_key = temp_efile_config.get("api key")
 
@@ -205,56 +208,67 @@
     ) -> ApiResponse:
         """
         registration_type needs to be INDIVIDUAL, FIRM_ADMINISTRATOR, or FIRM_ADMIN_NEW_MEMBER.
         If registration_type is INDIVIDUAL or FIRM_ADMINISTRATOR, you need a password.
         If it's FIRM_ADMINISTRATOR or FIRM_ADMIN_NEW_MEMBER, you need a firm_name_or_id
         """
         if isinstance(person, Individual) or isinstance(person, ALIndividual):
-            person = person.as_serializable()
+            person_dict = person.as_serializable()
+        else:
+            person_dict = person
         return super().register_user(
-            person,
+            person_dict,
             registration_type,
             password=password,
             firm_name_or_id=firm_name_or_id,
         )
 
     #### Managing Firm Users
 
-    def update_firm(self, firm: Person) -> ApiResponse:
+    def update_firm(self, firm: Union[Dict, Person]) -> ApiResponse:
         # firm is stateful
-        update = serialize_person(firm)
-        return super().update_firm(update)
+        if isinstance(firm, dict):
+            firm_dict = firm
+        else:
+            firm_dict = serialize_person(firm)
+        return super().update_firm(firm_dict)
 
     # Managing Service Contacts
     def update_service_contact(
         self,
         service_contact_id: str,
-        service_contact: Individual,
+        service_contact: Union[Individual, Dict],
         is_public: bool = None,
         is_in_master_list: bool = None,
         admin_copy: str = None,
     ) -> ApiResponse:
-        service_contact_dict = serialize_person(service_contact)
+        if isinstance(service_contact, dict):
+            service_contact_dict = service_contact
+        else:
+            service_contact_dict = serialize_person(service_contact)
         return super().update_service_contact(
             service_contact_id,
             service_contact_dict,
             is_public=is_public,
             is_in_master_list=is_in_master_list,
             admin_copy=admin_copy,
         )
 
     def create_service_contact(
         self,
-        service_contact: Individual,
+        service_contact: Union[Dict, Individual],
         *,
         is_public: bool,
         is_in_master_list: bool,
         admin_copy: str = None,
     ) -> ApiResponse:
-        service_contact_dict = serialize_person(service_contact)
+        if isinstance(service_contact, dict):
+            service_contact_dict = service_contact
+        else:
+            service_contact_dict = serialize_person(service_contact)
         return super().create_service_contact(
             service_contact_dict,
             is_public=is_public,
             is_in_master_list=is_in_master_list,
             admin_copy=admin_copy,
         )
```

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/interview_logic.py` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/interview_logic.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,24 @@
 
 from docassemble.base.util import CustomDataType, DAObject, DAList, log, word
 from .conversions import parse_case_info, fetch_case_info, chain_xml
 from docassemble.AssemblyLine.al_general import ALPeopleList, ALIndividual
 
 
 class EFCaseSearch(DAObject):
+    """A data-class that has holds all of the information and state for a single case search"""
+
     court_id: str
     can_file_non_indexed_case: bool
     do_what_choice: str
     found_case: DAObject
     case_was_found: bool
 
     def search_went_wrong(self) -> bool:
+        """Returns true if something errored during the case search process"""
         if (
             hasattr(self, "docket_case_response")
             and not self.docket_case_response.is_ok()
         ):
             return True
         if (
             hasattr(self, "found_cases")
@@ -31,14 +34,22 @@
         ):
             return True
         return False
 
     def get_lookup_choices(
         self, can_file_non_indexed_case: bool
     ) -> List[Dict[str, str]]:
+        """Returns the DA choice list of what ways you are allowed to search for a case;
+        By default, this is "party_search", and "docket_lookup", and depending on the
+        court, it could also include "non_indexed_case".
+
+        Not passed as direct arguments, but the object attributes `party_search_choice`,
+        `docket_lookup_choice`, and `non_indexed_choice` are the user-facing labels
+        for each choice.
+        """
         lookup_choices = [
             {"party_search": str(self.party_search_choice)},
             {"docket_lookup": str(self.docket_lookup_choice)},
         ]
         if can_file_non_indexed_case:
             lookup_choices.append({"non_indexed_case": str(self.non_indexed_choice)})
         return lookup_choices
@@ -260,15 +271,15 @@
 
 def get_full_court_info(proxy_conn, court_id: str) -> Dict:
     """Gets all of the information about the court from the id"""
     full_court_resp = proxy_conn.get_court(court_id)
     if full_court_resp.is_ok():
         return full_court_resp.data
     else:
-        log(f"Couldn't get full court info for {court_id}")
+        log(f"Couldn't get full court info for {court_id}: {full_court_resp}")
         return {}
 
 
 def _scale_byte_units(value: Union[str, int], unit: str) -> int:
     """Idk if these are right, but there's no examples out there.
     Niem suggests they might not matter:
     https://docs.oasis-open.org/legalxml-courtfiling/ecf/v5.0/csprd03/model/class137602.html
```

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/py_efsp_client.py` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/py_efsp_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 #!/usr/bin/env python3
 
+"""
+The base python client used to communicate with the E-file proxy server.
+
+Doesn't include anything from docassemble, and can be used without having it installed.
+"""
+
 import re
-import json
 import logging
 import isodate
 import requests
 from requests import Response
 from datetime import datetime
 from typing import Optional, Union, List, Dict
 import http.client as http_client
@@ -45,17 +50,19 @@
         data = resp.json()
         return ApiResponse(resp.status_code, None, data)
     except:
         return ApiResponse(resp.status_code, resp.text, None)
 
 
 class EfspConnection:
+    """A python client that communicates with the E-file proxy server."""
+
     def __init__(self, *, url: str, api_key: str, default_jurisdiction: str = None):
         """
-        Params:
+        Args:
           url (str)
           api_key (str)
           default_jurisdiction (str)
         """
         if not url.endswith("/"):
             url = url + "/"
 
@@ -114,17 +121,22 @@
         elif self.verbose and not turn_on:
             EfspConnection.verbose_logging(turn_on)
         self.verbose = turn_on
 
     def full_url(self, endpoint: str, jurisdiction: str = None) -> str:
         if jurisdiction is None:
             jurisdiction = self.default_jurisdiction
-        if endpoint.startswith("authenticate_user") or endpoint.startswith("messages"):
+        if any(
+            [
+                endpoint.startswith(service)
+                for service in ["authenticate_user", "messages", "api_user_settings"]
+            ]
+        ):
             return self.base_url + endpoint
-        return self.base_url + f"/jurisdictions/{jurisdiction}/{endpoint}"
+        return self.base_url + f"jurisdictions/{jurisdiction}/{endpoint}"
 
     def tyler_token(self) -> Optional[str]:
         token = self.proxy_client.headers.get(
             "TYLER-TOKEN-" + str(self.default_jurisdiction).upper()
         )
         if isinstance(token, bytes):
             return token.decode()
@@ -135,18 +147,15 @@
         *,
         tyler_email: Optional[str] = None,
         tyler_password: Optional[str] = None,
         jeffnet_key: Optional[str] = None,
         jurisdiction: str = None,
     ) -> ApiResponse:
         """
-        Params:
-            tyler_email (str)
-            tyler_password (str)
-            jeffnet_key (str)
+        Authenticates the user with the EFM server (not the E-file proxy).
         """
 
         if jurisdiction is None:
             jurisdiction = self.default_jurisdiction
         logging.info(f"authing with jurisdiction: {jurisdiction}")
         auth_obj: Dict[str, Union[str, Dict[str, str]]] = {}
         auth_obj["api_key"] = self.api_key
@@ -377,14 +386,17 @@
         send = lambda: self.proxy_client.post(
             self.full_url("adminusers/user/password/reset"), data=email
         )
         return self._call_proxy(send)
 
     ### Managing a Firm
     def get_firm(self) -> ApiResponse:
+        """Gets info about the "firm" for an associated user. If a user is a pro-se, this
+        contains their address information.
+        """
         send = lambda: self.proxy_client.get(self.full_url("firmattorneyservice/firm"))
         return self._call_proxy(send)
 
     def update_firm(self, firm: dict) -> ApiResponse:
         """
         firm should have the below keys:
         * firstName, middleName, lastName if it's a person
@@ -641,37 +653,42 @@
             self.full_url("firmattorneyservice/service-contacts/public")
         )
         return self._call_proxy(send)
 
     def get_courts(
         self, fileable_only: bool = False, with_names: bool = False
     ) -> ApiResponse:
+        """Gets the list of courts."""
         params = {"fileable_only": fileable_only, "with_names": with_names}
         send = lambda: self.proxy_client.get(
             self.full_url("codes/courts"), params=params
         )
         return self._call_proxy(send)
 
     def get_court(self, court_id: str) -> ApiResponse:
+        """Gets codes for a specific court"""
         send = lambda: self.proxy_client.get(
             self.full_url(f"codes/courts/{court_id}/codes")
         )
         return self._call_proxy(send)
 
-    def get_court_list(self):
+    def get_court_list(self) -> ApiResponse:
+        """Gets a list of all of the courts that you can file into. Slightly more limited than
+        [get_courts](#get_courts)"""
         send = lambda: self.proxy_client.get(self.full_url(f"filingreview/courts"))
         return self._call_proxy(send)
 
     def get_filing_list(
         self,
         court_id: str,
         user_id: str = None,
         start_date: datetime = None,
         before_date: datetime = None,
     ) -> ApiResponse:
+        """Returns a list of filings that a particular user has made with a court."""
         params = {
             "user_id": user_id,
             "start_date": start_date.strftime("%Y-%m-%d") if start_date else None,
             "before_date": before_date.strftime("%Y-%m-%d") if before_date else None,
         }
         send = lambda: self.proxy_client.get(
             self.full_url(f"filingreview/courts/{court_id}/filings"), params=params
@@ -946,18 +963,67 @@
         send = lambda: self.proxy_client.get(
             self.full_url(
                 f"codes/courts/{court_id}/casetypes/{case_type}/cross_references"
             )
         )
         return self._call_proxy(send)
 
+    def get_damage_amounts(
+        self, court_id: str, case_category: Optional[str] = None
+    ) -> ApiResponse:
+        params = {"category_id": case_category}
+        send = lambda: self.proxy_client.get(
+            self.full_url(
+                f"codes/courts/{court_id}/damage_amounts",
+            ),
+            params=params,
+        )
+        return self._call_proxy(send)
+
+    def get_procedure_or_remedies(
+        self, court_id: str, case_category: Optional[str] = None
+    ) -> ApiResponse:
+        params = {"category_id": case_category}
+        send = lambda: self.proxy_client.get(
+            self.full_url(
+                f"codes/courts/{court_id}/procedure_or_remedies",
+            ),
+            params=params,
+        )
+        return self._call_proxy(send)
+
     def get_datafield(self, court_id: str, field_name: str) -> ApiResponse:
         send = lambda: self.proxy_client.get(
             self.full_url(f"codes/courts/{court_id}/datafields/{field_name}")
         )
         return self._call_proxy(send)
 
     def get_disclaimers(self, court_id: str) -> ApiResponse:
         send = lambda: self.proxy_client.get(
             self.full_url(f"codes/courts/{court_id}/disclaimer_requirements")
         )
         return self._call_proxy(send)
+
+    def get_server_id(self) -> ApiResponse:
+        send = lambda: self.proxy_client.get(
+            self.full_url(f"api_user_settings/serverid")
+        )
+        return self._call_proxy(send)
+
+    def get_server_name(self) -> ApiResponse:
+        send = lambda: self.proxy_client.get(self.full_url(f"api_user_settings/name"))
+        return self._call_proxy(send)
+
+    def get_logs(self) -> ApiResponse:
+        send = lambda: self.proxy_client.get(
+            self.full_url(f"api_user_settings/logs"),
+            headers={
+                "Accept": "application/octet-stream",
+                "X-API-KEY": self.proxy_client.headers["X-API-KEY"],
+            },
+        )
+        # This resp has the logs as the error message: split by line and put in data
+        resp = self._call_proxy(send)
+        if resp.is_ok() and resp.error_msg and resp.error_msg != "":
+            resp.data = resp.error_msg[1:].split("|\n|")
+            resp.error_msg = None
+        return resp
```

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/test/integration_test.py` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/integration_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #! /usr/bin/env python3
 
-from docassemble.base.util import Address, Person, Individual, IndividualName, Address
-from docassemble.AssemblyLine.al_general import ALIndividual
-from ..efm_client import ProxyConnection, ApiResponse
+from ..py_efsp_client import EfspConnection, ApiResponse
 import sys
 import subprocess
 import json
 import os
 from pathlib import Path
 from datetime import datetime, timedelta
 
@@ -17,67 +15,81 @@
     info_json = subprocess.check_output(
         ["docker", "inspect", "efileproxyserver_efspjava_1"]
     )
     if info_json:
         info_dict = json.loads(info_json)
         base_url = (
             "http://"
-            + info_dict[0]["NetworkSettings"]["Networks"]["efileproxyserver_default"][
-                "IPAddress"
-            ]
+            # + info_dict[0]["NetworkSettings"]["Networks"]["efileproxyserver_default"]["IPAddress"]
+            + "localhost"
             + ":9000/"
         )
         print("Using URL: " + base_url)
         return base_url
     else:
         print("FAILED Can't find the docker image!")
         return None
 
 
-class MockPerson(ALIndividual):
-    def __init__(self):
-        self.email = "fakeemail@example.com"
-        self.instanceName = "mock_person"
-        # Neat trick: https://stackoverflow.com/a/24448351/11416267
-        self.name = IndividualName()
-        self.name.first = "B"
-        self.name.middle = "S"
-        self.name.last = "W"
-        self.address = Address()
-        self.address.address = "123 Fakestreet Ave"
-        self.address.unit = "Apt 1"
-        self.address.city = "Boston"
-        self.address.state = "MA"
-        self.address.zip = "12345"
-        self.address.country = "US"
-        self.mobile_number = "1234567890"
+def mock_person():
+    per = {}
+    per["email"] = "fakeemail@example.com"
+    # Neat trick: https://stackoverflow.com/a/24448351/11416267
+    per["name"] = {
+        "first": "B",
+        "middle": "S",
+        "last": "W",
+    }
+    per["address"] = {
+        "addressLine1": "123 Fakestreet Ave",
+        "addressLine2": "Apt 1",
+        "city": "Boston",
+        "state": "MA",
+        "zipCode": "12345",
+        "country": "US",
+    }
+    per["phoneNumber"] = "1234567890"
+    return per
 
 
 class TestClass:
     def __init__(self, proxy_conn, verbose: bool = True):
         self.proxy_conn = proxy_conn
         self.verbose = verbose
 
     def basic_assert(self, resp: ApiResponse):
         if self.verbose:
             print(resp)
         assert resp.is_ok()
         return resp
 
+    def test_authenticate(self):
+        print("\n\n### Authenticate ###\n\n")
+        empty_resp = self.proxy_conn.authenticate_user()
+        self.basic_assert(empty_resp)
+        assert len(empty_resp.data["tokens"]) == 0
+        resp = self.proxy_conn.authenticate_user(
+            tyler_email=os.getenv("bryce_user_email"),
+            tyler_password=os.getenv("bryce_user_password"),
+        )
+        self.basic_assert(resp)
+
     def test_hateos(self):
+        print("\n\n### Hateos ###\n\n")
         base_url = self.proxy_conn.base_url
         base_send = lambda: self.proxy_conn.proxy_client.get(base_url)
         next_level_urls = self.basic_assert(self.proxy_conn._call_proxy(base_send)).data
         for url in next_level_urls.values():
             if "authenticate" in url:
                 continue
             send = lambda: self.proxy_conn.proxy_client.get(url)
             self.basic_assert(self.proxy_conn._call_proxy(send))
 
     def test_self_user(self):
+        print("\n\n### Self user ###\n\n")
         myself = self.basic_assert(self.proxy_conn.get_user())
         assert myself.data["middleName"] == "Steven"
         nm = self.basic_assert(
             self.proxy_conn.update_user(myself.data["userID"], middle_name="Stephen")
         )
         bad_spelling = self.basic_assert(self.proxy_conn.get_user())
         assert bad_spelling.data["middleName"] == "Stephen"
@@ -122,41 +134,47 @@
         )
         last_update = self.proxy_conn.update_notification_preferences(
             [{"code": "SERVICEUNDELIVERABLE", "isActive": True}]
         )
         assert last_update.response_code == 200
 
     def test_service_contacts(self):
+        print("\n\n### Service Contacts ###\n\n")
         public = self.basic_assert(
             self.proxy_conn.get_public_service_contacts(first_name="John")
         )
-        new_contact = Individual()
-        new_contact.name.first = "Ella"
-        new_contact.name.last = "Doe"
-        new_contact.email = "ella.doe@example.com"
-        new_contact.address.address = "123 Fakestreet Ave"
-        new_contact.address.unit = "Unit 999"
-        new_contact.address.city = "Boston"
-        new_contact.address.state = "MA"
-        new_contact.address.zip = "12345"
-        new_contact.address.country = "US"
-        new_contact.phone_number = "9727133770"
+        new_contact = {
+            "firstName": "Ella",
+            "lastName": "Doe",
+            "email": "ella.doe@example.com",
+            "address": {
+                "addressLine1": "123 Fakestreet Ave",
+                "addressLine2": "Unit 999",
+                "city": "Boston",
+                "state": "MA",
+                "zipCode": "12345",
+                "country": "US",
+            },
+            "phoneNumber": "9727133770",
+        }
         new_c = self.basic_assert(
             self.proxy_conn.create_service_contact(
                 new_contact,
                 is_public=False,
                 is_in_master_list=True,
                 admin_copy="ella.doe@example.com",
             )
         )
         contact_id = new_c.data
-        new_contact.name.middle = '"Lorde"'
-        new_contact.email = "different@example.com"
+        new_contact["middleName"] = '"Lorde"'
+        new_contact["email"] = "different@example.com"
         self.basic_assert(
-            self.proxy_conn.update_service_contact(contact_id, new_contact, False, True)
+            self.proxy_conn.update_service_contact(
+                contact_id, new_contact, is_public=False, is_in_master_list=True
+            )
         )
 
         my_list = self.basic_assert(self.proxy_conn.get_service_contact_list())
         assert len(my_list.data) >= 1
         updated_contact = self.basic_assert(
             self.proxy_conn.get_service_contact(contact_id)
         )
@@ -173,51 +191,59 @@
                 contact_id, "c6d795d1-3f89-411d-8c86-fa1a33fb88e5"
             )
         )
 
         self.basic_assert(self.proxy_conn.remove_service_contact(contact_id))
 
     def test_firm(self):
-        update_firm = Person()
-        update_firm.name.text = "Suffolk FIT Lab"
-        update_firm.address.address = "121 Tremont Street"
+        print("\n\n### Firm ###\n\n")
+        update_firm = {}
+        update_firm["firmName"] = "Suffolk FIT Lab"
+        update_firm["address"] = {"addressLine1": "121 Tremont Street"}
         resp = self.proxy_conn.update_firm(update_firm)
         assert resp.response_code == 200
 
         new_firm = self.basic_assert(self.proxy_conn.get_firm())
         assert new_firm.data["firmName"] == "Suffolk FIT Lab"
         assert new_firm.data["address"]["addressLine1"] == "121 Tremont Street"
 
-        update_firm.name.text = "Suffolk LIT Lab"
-        update_firm.address.address = "120 Tremont Street"
+        update_firm["firmName"] = "Suffolk LIT Lab"
+        update_firm["address"]["addressLine1"] = "120 Tremont Street"
         self.basic_assert(self.proxy_conn.update_firm(update_firm))
 
         firm = self.basic_assert(self.proxy_conn.get_firm())
         assert firm.data["firmName"] == "Suffolk LIT Lab"
         assert firm.data["isIndividual"] == False
         assert firm.data["address"]["addressLine1"] == "120 Tremont Street"
 
     def test_users(self):
-        mock_person = MockPerson()
+        print("\n\n### Users ###\n\n")
+        all_initial_users = self.basic_assert(self.proxy_conn.get_users())
+        person = mock_person()
+        for u in all_initial_users.data:
+            if u["email"] == person["email"]:
+                self.basic_assert(self.proxy_conn.remove_user(u["userID"]))
+                all_initial_users = self.basic_assert(self.proxy_conn.get_users())
+                break
         firm_id = self.proxy_conn.get_firm().data["firmID"]
         new_user = self.proxy_conn.register_user(
-            mock_person,
+            person,
             registration_type="FIRM_ADMIN_NEW_MEMBER",
             firm_name_or_id=firm_id,
         )
         assert new_user.response_code == 201
         new_id = new_user.data["userID"]
 
         self.basic_assert(self.proxy_conn.resend_activation_email(new_id))
 
         full_user = self.basic_assert(self.proxy_conn.get_user(new_id))
         assert full_user.data["middleName"] == "S"
 
         all_users = self.basic_assert(self.proxy_conn.get_users())
-        assert len(all_users.data) >= 2
+        assert len(all_users.data) == len(all_initial_users.data) + 1
 
         roles = self.basic_assert(self.proxy_conn.get_user_roles(new_id))
         assert len(roles.data) == 1
         assert roles.data[0]["roleName"] == "FILER"
 
         new_role_add = self.proxy_conn.add_user_roles(
             new_id, [{"roleName": "FIRM_ADMIN"}]
@@ -238,14 +264,15 @@
         self.basic_assert(self.proxy_conn.remove_user(new_id))
 
     def test_get_courts(self):
         courts = self.basic_assert(self.proxy_conn.get_courts())
         assert "jefferson" in courts.data
 
     def test_global_payment_accounts(self):
+        print("\n\n### Global payment accounts ###\n\n")
         all_accounts = self.proxy_conn.get_global_payment_account_list()
         if self.verbose:
             print(all_accounts)
         assert all_accounts.response_code == 200
         assert all_accounts.data[0]["firmID"] is None
         account_id = all_accounts.data[0]["paymentAccountID"]
         account = self.proxy_conn.get_global_payment_account(
@@ -277,14 +304,15 @@
             )
         )
         self.basic_assert(
             self.proxy_conn.remove_global_payment_account(global_account.data)
         )
 
     def test_payment_accounts(self):
+        print("\n\n### Payment accounts ###\n\n")
         self.basic_assert(self.proxy_conn.get_payment_account_type_list())
         self.basic_assert(self.proxy_conn.get_payment_account_list())
         self.basic_assert(self.proxy_conn.get_payment_account_list("adams"))
 
         new_account = self.basic_assert(
             self.proxy_conn.create_waiver_account("New Integration Test account", False)
         )
@@ -303,19 +331,21 @@
             self.proxy_conn.update_payment_account(
                 id, account_name=one_account.data["accountName"]
             )
         )
         self.basic_assert(self.proxy_conn.remove_payment_account(new_account.data))
 
     def test_court_record(self):
-        contact = ALIndividual()
-        contact.name.first = "John"
-        contact.name.last = "Brown"
-        contact.person_type = "ALIndividual"
-        cases = self.basic_assert(self.proxy_conn.get_cases("adams", person=contact))
+        print("\n\n### Court record ###\n\n")
+        contact = {}
+        contact["first"] = "John"
+        contact["last"] = "Brown"
+        cases = self.basic_assert(
+            self.proxy_conn.get_cases_raw("adams", person_name=contact)
+        )
         assert len(cases.data) > 0
         case_id = cases.data[0]["value"]["caseTrackingID"]["value"]
         case = self.basic_assert(self.proxy_conn.get_case("adams", case_id))
         doc_resp = self.proxy_conn.get_document("adams", case_id)
         assert doc_resp.response_code == 405
         serv_info = self.basic_assert(
             self.proxy_conn.get_service_information("adams", case_id)
@@ -329,14 +359,15 @@
             attach_cases = self.proxy_conn.get_service_attach_case_list(
                 "adams", serv_id
             )
             if self.verbose:
                 print(attach_cases)
 
     def test_attorneys(self):
+        print("\n\n### Attorneys ###\n\n")
         new_attorney = self.proxy_conn.create_attorney(
             bar_number="6224951",
             first_name="Valarie",
             middle_name="DONTUSE_IS_REAL_PERSON",
             last_name="Franklin",
         )
         assert new_attorney.response_code == 200
@@ -355,14 +386,15 @@
         )
         assert full_new_attorney.data["middleName"] == "Lobert"
 
         deleted_maybe = self.proxy_conn.remove_attorney(new_attorney_id)
         assert deleted_maybe.response_code == 200
 
     def test_filings(self):
+        print("\n\n### Filings ###\n\n")
         filing_list = self.basic_assert(
             self.proxy_conn.get_filing_list(
                 "illinois",
                 "adams",
                 start_date=datetime.today() - timedelta(days=3),
                 before_date=datetime.today(),
             )
@@ -402,43 +434,57 @@
                 self.proxy_conn.get_filing(court, filing_id)
             )
             cancel_resp = self.basic_assert(
                 self.proxy_conn.cancel_filing_status(court, filing_id)
             )
 
     def test_codes(self):
+        print("\n\n### Codes ###\n\n")
         self.basic_assert(self.proxy_conn.get_court_list())
         self.basic_assert(self.proxy_conn.get_case_categories("adams"))
 
+    def test_logs(self):
+        print("\n\n### Test Logs ###\n\n")
+        server_id = self.basic_assert(self.proxy_conn.get_server_id()).data
+        all_logs = self.basic_assert(self.proxy_conn.get_logs())
+        for l in all_logs.data:
+            assert l.split("|")[1].strip() == server_id
+
 
 def main(args):
     base_url = get_proxy_server_ip()
     api_key = os.getenv("PROXY_API_KEY")
-    proxy_conn = ProxyConnection(
-        url=base_url, api_key=api_key, default_jurisdiction="illinois"
+    if not api_key:
+        print("You need to have the PROXY_API_KEY env var set; not running tests")
+        return
+    bad_proxy = EfspConnection(
+        url=base_url, api_key="IntenionallyWrongKey", default_jurisdiction="illinois"
     )
-    proxy_conn.set_verbose_logging(True)
-    intentional_bad_resp = proxy_conn.authenticate_user()
+    intentional_bad_resp = bad_proxy.authenticate_user()
+    if intentional_bad_resp.response_code != 403:
+        print(intentional_bad_resp)
     assert intentional_bad_resp.response_code == 403
-    resp = proxy_conn.authenticate_user(
-        tyler_email=os.getenv("bryce_user_email"),
-        tyler_password=os.getenv("bryce_user_password"),
+    proxy_conn = EfspConnection(
+        url=base_url, api_key=api_key, default_jurisdiction="illinois"
     )
-    assert resp.response_code == 200
+    proxy_conn.set_verbose_logging(True)
     tc = TestClass(proxy_conn, verbose=True)
+    tc.test_authenticate()
     tc.test_hateos()
     tc.test_self_user()
     tc.test_firm()
     tc.test_service_contacts()
     tc.test_get_courts()
-    tc.test_global_payment_accounts()
     tc.test_payment_accounts()
     tc.test_attorneys()
     tc.test_court_record()
     tc.test_users()
     tc.test_codes()
+    tc.test_logs()
     # TODO(brycew): needs a more up to date JSON from any filing interiview
     # tc.test_filings()
+    # TODO(brycew): Tyler issue, have to wait on them
+    # tc.test_global_payment_accounts()
 
 
 if __name__ == "__main__":
     main(sys.argv)
```

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/test/peoria_to_cr.json` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/peoria_to_cr.json`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/test/temp2.json` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/temp2.json`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/test/test_conversions.py` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/test_conversions.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from docassemble.base.core import DAObject
 from docassemble.AssemblyLine.al_general import ALIndividual
 from ..efm_client import ProxyConnection, ApiResponse
 from ..conversions import parse_case_info, parse_service_contacts
 
 
 class TestConversions(unittest.TestCase):
-    """Tests conversions.py on the "vars.json" file"""
+    # Tests conversions.py on the "vars.json" file
 
     def setUp(self):
         with open(Path(__file__).parent / "vars.json", "r") as file:
             full_json = json.load(file).get("variables")
             self.my_var = full_json.get("my_var").get("data")
         self.my_service_contacts = full_json.get("my_service_contacts")
         self.proxy_conn = ProxyConnection()
         self.proxy_conn.get_case = MagicMock(
             "get_case", return_value=ApiResponse(200, "", self.my_var)
         )
 
     def test_parse_case_info(self):
-        """Makes sure that participants of the case are parsed fully, needed"""
+        # Makes sure that participants of the case are parsed fully, needed
         case = DAObject("case")
         parse_case_info(self.proxy_conn, case, self.my_var, "adams")
         self.assertEqual(len(case.participants), 2)
         for partip in case.participants:
             self.assertIsInstance(partip, ALIndividual)
             self.assertIn(partip.person_type, ["ALIndividual", "business"])
             self.assertNotEqual(partip.name.first, None)
@@ -55,50 +55,50 @@
         service_contacts = parse_service_contacts(self.my_service_contacts)
         self.assertEqual(len(service_contacts), 1)
         self.assertEqual(service_contacts[0][0], "6707a4f8-9f4c-4bbb-8498-ed4890208c6d")
         self.assertEqual(service_contacts[0][1], "Bryce Willey")
 
 
 class TestNoneResp(unittest.TestCase):
-    """Tests with none responses conversions.py on the "vars.json" file"""
+    # Tests with none responses conversions.py on the "vars.json" file
 
     def setUp(self):
         with open(Path(__file__).parent / "vars.json", "r") as file:
             full_json = json.load(file).get("variables")
             self.my_var = full_json.get("my_var").get("data")
         self.my_service_contacts = full_json.get("my_service_contacts")
         self.proxy_conn = ProxyConnection()
         self.proxy_conn.get_case = MagicMock(
             "get_case", return_value=ApiResponse(200, "", None)
         )
 
     def test_none(self):
-        """Makes sure that participants of the case are parsed fully, needed"""
+        # Makes sure that participants of the case are parsed fully, needed
         case = DAObject("case")
         parse_case_info(self.proxy_conn, case, None, "peoria")
         # no throw!
 
 
 class TestCourtSwitching(unittest.TestCase):
-    """Tests that if we search a case in a grouped court (say peoria) and
-    get back a court from a sub court (peariacr), that the
-    court_id from the found case reflects the sub court.
-
-    This is necessary, as filings can't be accepted to the grouped court."""
+    # Tests that if we search a case in a grouped court (say peoria) and
+    # get back a court from a sub court (peariacr), that the
+    # court_id from the found case reflects the sub court.
+    #
+    # This is necessary, as filings can't be accepted to the grouped court."""
 
     def setUp(self):
         with open(Path(__file__).parent / "peoria_to_cr.json", "r") as file:
             self.my_var = json.load(file)
         self.proxy_conn = ProxyConnection()
         self.proxy_conn.get_case = MagicMock(
             "get_case", return_value=ApiResponse(200, "", self.my_var)
         )
 
     def test_switched_court(self):
-        """Makes sure that participants of the case are parsed fully, needed"""
+        # Makes sure that participants of the case are parsed fully, needed
         case = DAObject("case")
         parse_case_info(self.proxy_conn, case, self.my_var, "peoria")
         self.assertEqual(case.court_id, "peoriacr")
         self.assertEqual(case.docket_number, "02-CM-02778-1")
         self.assertEqual(case.category, "135493")
 
 
@@ -110,13 +110,13 @@
             self.more_details = full_json.get("case_details")
         self.proxy_conn = ProxyConnection()
         self.proxy_conn.get_case = MagicMock(
             "get_case", return_value=ApiResponse(200, "", self.more_details)
         )
 
     def test_ignore_attorneys(self):
-        """Attorneys are just stuck in the middle with normal case participants. You can't attach service contacts to them, so"""
+        # Attorneys are just stuck in the middle with normal case participants. You can't attach service contacts to them, so
         case = DAObject("case")
         parse_case_info(self.proxy_conn, case, self.first_resp, "peoria")
         self.assertEqual(len(case.attorneys.keys()), 2)
         self.assertTrue("e650827f-3a2b-4550-b76c-f7d22ed479ff" in case.attorneys.keys())
         self.assertTrue("7ff43f9b-53ff-4e6d-9253-e393318549d0" in case.attorneys.keys())
```

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble/EFSPIntegration/test/vars.json` & `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/vars.json`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.1.0/docassemble.EFSPIntegration.egg-info/SOURCES.txt` & `docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 docassemble.EFSPIntegration.egg-info/not-zip-safe
 docassemble.EFSPIntegration.egg-info/requires.txt
 docassemble.EFSPIntegration.egg-info/top_level.txt
 docassemble/EFSPIntegration/__init__.py
 docassemble/EFSPIntegration/conversions.py
 docassemble/EFSPIntegration/efm_client.py
 docassemble/EFSPIntegration/interview_logic.py
+docassemble/EFSPIntegration/py.typed
 docassemble/EFSPIntegration/py_efsp_client.py
 docassemble/EFSPIntegration/requirements.txt
 docassemble/EFSPIntegration/data/questions/admin_interview.yml
 docassemble/EFSPIntegration/data/questions/any_filing_interview.yml
 docassemble/EFSPIntegration/data/questions/case_search.yml
 docassemble/EFSPIntegration/data/questions/efiling_integration.yml
 docassemble/EFSPIntegration/data/questions/login_qs.yml
 docassemble/EFSPIntegration/data/questions/minimal_interview.yml
 docassemble/EFSPIntegration/data/questions/toga_payments.yml
+docassemble/EFSPIntegration/data/questions/toga_payments_interview.yml
 docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml
 docassemble/EFSPIntegration/data/questions/unauthenticated_interview.yml
 docassemble/EFSPIntegration/data/sources/README.md
 docassemble/EFSPIntegration/data/sources/admin_interview.feature
 docassemble/EFSPIntegration/data/sources/any_filing_interview.feature
 docassemble/EFSPIntegration/data/sources/example_upload.pdf
 docassemble/EFSPIntegration/data/sources/unauthenticated_interview.feature
```

### Comparing `docassemble.EFSPIntegration-1.1.0/setup.py` & `docassemble.EFSPIntegration-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.EFSPIntegration',
-      version='1.1.0',
+      version='1.2.0',
       description=(''),
       long_description='# docassemble-EFSPIntegration\r\n\r\nA docassemble extension that talks to [a proxy e-filing server](https://github.com/SuffolkLITLab/EfileProxyServer/) easily within a docassemble interview.\r\n\r\nMain interviews of import:\r\n\r\n* any_filing_interview.yml: allows you to make any type of filing, initial or subsequent\r\n* admin_interview.yml: lets you handle admin / user functionality, outside of the context of cases and filings\r\n\r\nIn progress!\r\n\r\n## Authors\r\n\r\nQuinten Steenhuis (qsteenhuis@suffolk.edu)\r\nBryce Willey (bwilley@suffolk.edu)\r\n',
       long_description_content_type='text/markdown',
       author='Bryce Willey',
       author_email='bwilley@suffolk.edu',
       license='The MIT License (MIT)',
       url='https://github.com/SuffolkLITLab/docassemble-EFSPIntegration',
```

