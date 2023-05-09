# Comparing `tmp/cdk-valheim-0.0.26.tar.gz` & `tmp/cdk-valheim-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-valheim-0.0.26.tar", last modified: Tue May  9 16:58:15 2023, max compression
+gzip compressed data, was "/__w/cdk-valheim/cdk-valheim/dist/python/cdk-valheim-0.0.9.tar", last modified: Sat Feb 20 09:18:21 2021, max compression
```

## Comparing `cdk-valheim-0.0.26.tar` & `cdk-valheim-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:58:15.363360 cdk-valheim-0.0.26/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 16:57:59.000000 cdk-valheim-0.0.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 16:57:59.000000 cdk-valheim-0.0.26/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-09 16:58:15.363360 cdk-valheim-0.0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-09 16:57:59.000000 cdk-valheim-0.0.26/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-09 16:57:59.000000 cdk-valheim-0.0.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:58:15.363360 cdk-valheim-0.0.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-09 16:57:59.000000 cdk-valheim-0.0.26/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:58:15.359360 cdk-valheim-0.0.26/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:58:15.363360 cdk-valheim-0.0.26/src/cdk_valheim/
--rw-r--r--   0 runner    (1001) docker     (123)    28099 2023-05-09 16:57:59.000000 cdk-valheim-0.0.26/src/cdk_valheim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:58:15.363360 cdk-valheim-0.0.26/src/cdk_valheim/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-09 16:57:59.000000 cdk-valheim-0.0.26/src/cdk_valheim/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   374843 2023-05-09 16:57:59.000000 cdk-valheim-0.0.26/src/cdk_valheim/_jsii/cdk-valheim@0.0.26.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:57:59.000000 cdk-valheim-0.0.26/src/cdk_valheim/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:58:15.363360 cdk-valheim-0.0.26/src/cdk_valheim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-09 16:58:14.000000 cdk-valheim-0.0.26/src/cdk_valheim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-09 16:58:15.000000 cdk-valheim-0.0.26/src/cdk_valheim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:58:14.000000 cdk-valheim-0.0.26/src/cdk_valheim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-09 16:58:15.000000 cdk-valheim-0.0.26/src/cdk_valheim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 16:58:15.000000 cdk-valheim-0.0.26/src/cdk_valheim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-20 09:18:21.000000 cdk-valheim-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)       23 2021-02-20 09:18:16.000000 cdk-valheim-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1829 2021-02-20 09:18:21.000000 cdk-valheim-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      640 2021-02-20 09:18:16.000000 cdk-valheim-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-02-20 09:18:16.000000 cdk-valheim-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-02-20 09:18:21.000000 cdk-valheim-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2011 2021-02-20 09:18:16.000000 cdk-valheim-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-20 09:18:21.000000 cdk-valheim-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-20 09:18:21.000000 cdk-valheim-0.0.9/src/cdk_valheim/
+-rw-r--r--   0 root         (0) root         (0)    14666 2021-02-20 09:18:16.000000 cdk-valheim-0.0.9/src/cdk_valheim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-20 09:18:21.000000 cdk-valheim-0.0.9/src/cdk_valheim/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      589 2021-02-20 09:18:16.000000 cdk-valheim-0.0.9/src/cdk_valheim/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51843 2021-02-20 09:18:16.000000 cdk-valheim-0.0.9/src/cdk_valheim/_jsii/cdk-valheim@0.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-02-20 09:18:16.000000 cdk-valheim-0.0.9/src/cdk_valheim/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-20 09:18:21.000000 cdk-valheim-0.0.9/src/cdk_valheim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1829 2021-02-20 09:18:21.000000 cdk-valheim-0.0.9/src/cdk_valheim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      375 2021-02-20 09:18:21.000000 cdk-valheim-0.0.9/src/cdk_valheim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-02-20 09:18:21.000000 cdk-valheim-0.0.9/src/cdk_valheim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2021-02-20 09:18:21.000000 cdk-valheim-0.0.9/src/cdk_valheim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2021-02-20 09:18:21.000000 cdk-valheim-0.0.9/src/cdk_valheim.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

