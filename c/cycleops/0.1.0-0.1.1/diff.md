# Comparing `tmp/cycleops-0.1.0.tar.gz` & `tmp/cycleops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycleops-0.1.0.tar", max compression
+gzip compressed data, was "cycleops-0.1.1.tar", max compression
```

## Comparing `cycleops-0.1.0.tar` & `cycleops-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,13 @@
--rw-r--r--   0        0        0       20 2023-03-13 08:46:30.738691 cycleops-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-13 08:46:11.386394 cycleops-0.1.0/cycleops/__main__.py
--rw-r--r--   0        0        0      370 2023-03-13 08:45:33.796736 cycleops-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 cycleops-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-09 10:17:07.975552 cycleops-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3487 2023-05-09 10:17:07.975552 cycleops-0.1.1/README.md
+-rw-r--r--   0        0        0     1125 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/__main__.py
+-rw-r--r--   0        0        0      414 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/auth.py
+-rw-r--r--   0        0        0     5468 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/client.py
+-rw-r--r--   0        0        0     1113 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/exceptions.py
+-rw-r--r--   0        0        0     6626 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/services.py
+-rw-r--r--   0        0        0     4249 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/setups.py
+-rw-r--r--   0        0        0     3047 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/stacks.py
+-rw-r--r--   0        0        0      869 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/units.py
+-rw-r--r--   0        0        0      972 2023-05-09 10:17:07.975552 cycleops-0.1.1/cycleops/utils.py
+-rw-r--r--   0        0        0      556 2023-05-09 10:17:07.975552 cycleops-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4012 1970-01-01 00:00:00.000000 cycleops-0.1.1/PKG-INFO
```

