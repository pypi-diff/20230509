# Comparing `tmp/design.plone.policy-5.0.1.tar.gz` & `tmp/design.plone.policy-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.policy-5.0.1.tar", last modified: Thu May  4 11:42:29 2023, max compression
+gzip compressed data, was "design.plone.policy-5.0.2.tar", last modified: Tue May  9 14:20:42 2023, max compression
```

## Comparing `design.plone.policy-5.0.1.tar` & `design.plone.policy-5.0.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.483119 design.plone.policy-5.0.1/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5163 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/CHANGES.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       73 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/CONTRIBUTORS.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      585 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/DEVELOP.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/LICENSE.GPL
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/LICENSE.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      107 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/MANIFEST.in
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    15396 2023-05-04 11:42:29.483119 design.plone.policy-5.0.1/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9030 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/README.rst
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.479119 design.plone.policy-5.0.1/docs/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7993 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/docs/conf.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/docs/index.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       31 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/requirements.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      367 2023-05-04 11:42:29.487119 design.plone.policy-5.0.1/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2887 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.475118 design.plone.policy-5.0.1/src/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.479119 design.plone.policy-5.0.1/src/design/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.479119 design.plone.policy-5.0.1/src/design/plone/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.479119 design.plone.policy-5.0.1/src/design/plone/policy/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      173 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.479119 design.plone.policy-5.0.1/src/design/plone/policy/browser/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      119 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/browser/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    19901 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/browser/config.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      540 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/browser/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5622 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/browser/trasparenza.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1623 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      441 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.479119 design.plone.policy-5.0.1/src/design/plone/policy/locales/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/locales/README.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/locales/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/locales/design.plone.policy.pot
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.475118 design.plone.policy-5.0.1/src/design/plone/policy/locales/en/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.483119 design.plone.policy-5.0.1/src/design/plone/policy/locales/en/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1748 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/locales/update.py
--rwxrwxr-x   0 mauro     (1000) mauro     (1000)      494 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/locales/update.sh
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/permissions.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.475118 design.plone.policy-5.0.1/src/design/plone/policy/profiles/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.483119 design.plone.policy-5.0.1/src/design/plone/policy/profiles/default/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      584 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/profiles/default/actions.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      175 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/profiles/default/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      122 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/profiles/default/catalog.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1027 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/profiles/default/metadata.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1473 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/profiles/default/registry.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      341 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/profiles/default/rolemap.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.483119 design.plone.policy-5.0.1/src/design/plone/policy/profiles/to_1400/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      237 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/profiles/to_1400/registry.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.483119 design.plone.policy-5.0.1/src/design/plone/policy/profiles/uninstall/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      122 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      268 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/profiles/uninstall/registry.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      311 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/rejectanonymous.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.483119 design.plone.policy-5.0.1/src/design/plone/policy/restapi/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/restapi/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.483119 design.plone.policy-5.0.1/src/design/plone/policy/restapi/bandi_search_filters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/restapi/bandi_search_filters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      534 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      996 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/restapi/bandi_search_filters/get.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      288 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/restapi/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.483119 design.plone.policy-5.0.1/src/design/plone/policy/restapi/search_filters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/restapi/search_filters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      519 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/restapi/search_filters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3831 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/restapi/search_filters/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.483119 design.plone.policy-5.0.1/src/design/plone/policy/restapi/twitter_feed/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/restapi/twitter_feed/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      513 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/restapi/twitter_feed/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6581 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/restapi/twitter_feed/get.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2342 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/sensitive.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3306 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/setuphandlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5214 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/testing.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.483119 design.plone.policy-5.0.1/src/design/plone/policy/tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/tests/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4286 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/tests/test_bandi_search_filters_api.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4324 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/tests/test_initial_structure.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3864 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/tests/test_search_filters_api.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3720 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/tests/test_setup.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    11068 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/upgrades.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4771 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/upgrades.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    13046 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design/plone/policy/utils.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-04 11:42:29.479119 design.plone.policy-5.0.1/src/design.plone.policy.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    15396 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design.plone.policy.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2868 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design.plone.policy.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design.plone.policy.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       40 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design.plone.policy.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       20 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design.plone.policy.egg-info/namespace_packages.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design.plone.policy.egg-info/not-zip-safe
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      504 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design.plone.policy.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-05-04 11:42:29.000000 design.plone.policy-5.0.1/src/design.plone.policy.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5261 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/CHANGES.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       73 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/CONTRIBUTORS.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      585 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/DEVELOP.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/LICENSE.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      107 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/MANIFEST.in
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    15494 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9030 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/README.rst
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7993 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/docs/conf.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/docs/index.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       31 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/requirements.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      367 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2887 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/design/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/design/plone/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/design/plone/policy/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      173 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/browser/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      119 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/browser/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    19901 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/browser/config.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      540 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/browser/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5622 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/browser/trasparenza.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1623 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      441 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/locales/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/locales/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/locales/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/locales/design.plone.policy.pot
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/design/plone/policy/locales/en/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1748 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/locales/update.py
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      494 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/locales/update.sh
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/permissions.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/design/plone/policy/profiles/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      584 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/actions.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      175 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      122 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1027 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/metadata.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1473 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/registry.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      341 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/rolemap.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/profiles/to_1400/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      237 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/to_1400/registry.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/profiles/uninstall/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      122 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      268 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/uninstall/registry.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      311 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/rejectanonymous.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/restapi/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/restapi/bandi_search_filters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/bandi_search_filters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      534 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      996 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/bandi_search_filters/get.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      288 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/restapi/search_filters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/search_filters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      519 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/search_filters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3831 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/search_filters/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/restapi/twitter_feed/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/twitter_feed/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      513 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/twitter_feed/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6581 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/twitter_feed/get.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2342 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/sensitive.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3306 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/setuphandlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5214 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/tests/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4286 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/tests/test_bandi_search_filters_api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4324 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/tests/test_initial_structure.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3864 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/tests/test_search_filters_api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3720 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/tests/test_setup.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    11068 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/upgrades.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4771 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/upgrades.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    13116 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/utils.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    15494 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2868 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       40 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       20 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      504 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/top_level.txt
```

### Comparing `design.plone.policy-5.0.1/CHANGES.rst` & `design.plone.policy-5.0.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+5.0.2 (2023-05-09)
+------------------
+
+- Fix setuphandlers' utils for robotframework
+  [mamico]
+
+
 5.0.1 (2023-05-04)
 ------------------
 
 - Add X-ForceAuth header and iw.rejectanonymous
   [mamico]
 - Customize Access inactive portal content permission to allow access these contents also for not manager users.
   [cekk]
```

### Comparing `design.plone.policy-5.0.1/DEVELOP.rst` & `design.plone.policy-5.0.2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/LICENSE.GPL` & `design.plone.policy-5.0.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/LICENSE.rst` & `design.plone.policy-5.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/PKG-INFO` & `design.plone.policy-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.policy
-Version: 5.0.1
+Version: 5.0.2
 Summary: Pacchetto per creare un sito Agid su Plone
 Home-page: https://github.com/collective/design.plone.policy
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.policy
 Project-URL: Source, https://github.com/RedTurtle/design.plone.policy
@@ -323,14 +323,21 @@
 
 - RedTurtle Technology, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
+5.0.2 (2023-05-09)
+------------------
+
+- Fix setuphandlers' utils for robotframework
+  [mamico]
+
+
 5.0.1 (2023-05-04)
 ------------------
 
 - Add X-ForceAuth header and iw.rejectanonymous
   [mamico]
 - Customize Access inactive portal content permission to allow access these contents also for not manager users.
   [cekk]
```

### Comparing `design.plone.policy-5.0.1/README.rst` & `design.plone.policy-5.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/docs/conf.py` & `design.plone.policy-5.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/setup.py` & `design.plone.policy-5.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.policy",
-    version="5.0.1",
+    version="5.0.2",
     description="Pacchetto per creare un sito Agid su Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/browser/config.py` & `design.plone.policy-5.0.2/src/design/plone/policy/browser/config.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/browser/configure.zcml` & `design.plone.policy-5.0.2/src/design/plone/policy/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/browser/trasparenza.py` & `design.plone.policy-5.0.2/src/design/plone/policy/browser/trasparenza.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/configure.zcml` & `design.plone.policy-5.0.2/src/design/plone/policy/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/locales/README.rst` & `design.plone.policy-5.0.2/src/design/plone/policy/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/locales/update.py` & `design.plone.policy-5.0.2/src/design/plone/policy/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/profiles/default/actions.xml` & `design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/profiles/default/metadata.xml` & `design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/profiles/default/registry.xml` & `design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml` & `design.plone.policy-5.0.2/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/restapi/bandi_search_filters/get.py` & `design.plone.policy-5.0.2/src/design/plone/policy/restapi/bandi_search_filters/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/restapi/search_filters/configure.zcml` & `design.plone.policy-5.0.2/src/design/plone/policy/restapi/search_filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/restapi/search_filters/get.py` & `design.plone.policy-5.0.2/src/design/plone/policy/restapi/search_filters/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/restapi/twitter_feed/configure.zcml` & `design.plone.policy-5.0.2/src/design/plone/policy/restapi/twitter_feed/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/restapi/twitter_feed/get.py` & `design.plone.policy-5.0.2/src/design/plone/policy/restapi/twitter_feed/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/sensitive.py` & `design.plone.policy-5.0.2/src/design/plone/policy/sensitive.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/setuphandlers.py` & `design.plone.policy-5.0.2/src/design/plone/policy/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/testing.py` & `design.plone.policy-5.0.2/src/design/plone/policy/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/tests/test_bandi_search_filters_api.py` & `design.plone.policy-5.0.2/src/design/plone/policy/tests/test_bandi_search_filters_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/tests/test_initial_structure.py` & `design.plone.policy-5.0.2/src/design/plone/policy/tests/test_initial_structure.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/tests/test_search_filters_api.py` & `design.plone.policy-5.0.2/src/design/plone/policy/tests/test_search_filters_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/tests/test_setup.py` & `design.plone.policy-5.0.2/src/design/plone/policy/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/upgrades.py` & `design.plone.policy-5.0.2/src/design/plone/policy/upgrades.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/upgrades.zcml` & `design.plone.policy-5.0.2/src/design/plone/policy/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.1/src/design/plone/policy/utils.py` & `design.plone.policy-5.0.2/src/design/plone/policy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,15 +395,17 @@
     amministrazione = api.content.get(path="/amministrazione")
     servizi = api.content.get(path="/servizi")
     novita = api.content.get(path="/novita")
     vivere = api.content.get(path="/vivere-il-comune")
 
     items = []
     for x in [amministrazione, novita, servizi, vivere]:
-        json_serialized = getMultiAdapter((x, request), ISerializeToJsonSummary)()
+        json_serialized = getMultiAdapter(
+            (x, request or x.REQUEST), ISerializeToJsonSummary
+        )()
         items.append(create_default_menu_item(context=json_serialized, obj=x))
 
     mocked_payload = [
         {
             "rootPath": "/",
             "items": items,
         }
@@ -414,14 +416,16 @@
     )
 
 
 def create_secondary_menu():
     request = getRequest()
     items = []
     argomenti = api.content.get(path="/argomenti")
-    json_serialized = getMultiAdapter((argomenti, request), ISerializeToJsonSummary)()
+    json_serialized = getMultiAdapter(
+        (argomenti, request or argomenti.REQUEST), ISerializeToJsonSummary
+    )()
     items.append(create_default_menu_item(context=json_serialized, obj=argomenti))
     mocked_payload = [{"rootPath": "/", "items": items}]
     payload = json.dumps(mocked_payload)
     api.portal.set_registry_record(
         "secondary_menu_configuration", payload, interface=ISecondaryMenu
     )
```

### Comparing `design.plone.policy-5.0.1/src/design.plone.policy.egg-info/PKG-INFO` & `design.plone.policy-5.0.2/src/design.plone.policy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.policy
-Version: 5.0.1
+Version: 5.0.2
 Summary: Pacchetto per creare un sito Agid su Plone
 Home-page: https://github.com/collective/design.plone.policy
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.policy
 Project-URL: Source, https://github.com/RedTurtle/design.plone.policy
@@ -323,14 +323,21 @@
 
 - RedTurtle Technology, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
+5.0.2 (2023-05-09)
+------------------
+
+- Fix setuphandlers' utils for robotframework
+  [mamico]
+
+
 5.0.1 (2023-05-04)
 ------------------
 
 - Add X-ForceAuth header and iw.rejectanonymous
   [mamico]
 - Customize Access inactive portal content permission to allow access these contents also for not manager users.
   [cekk]
```

### Comparing `design.plone.policy-5.0.1/src/design.plone.policy.egg-info/SOURCES.txt` & `design.plone.policy-5.0.2/src/design.plone.policy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

