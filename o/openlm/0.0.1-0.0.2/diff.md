# Comparing `tmp/openlm-0.0.1.tar.gz` & `tmp/openlm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlm-0.0.1.tar", max compression
+gzip compressed data, was "openlm-0.0.2.tar", max compression
```

## Comparing `openlm-0.0.1.tar` & `openlm-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-05-08 15:56:49.714425 openlm-0.0.1/LICENSE
--rw-r--r--   0        0        0       91 2023-05-08 16:01:30.637360 openlm-0.0.1/README.md
--rw-r--r--   0        0        0       37 2023-05-08 16:00:36.097722 openlm-0.0.1/openlm/__init__.py
--rw-r--r--   0        0        0       28 2023-05-08 15:58:19.203559 openlm-0.0.1/openlm/openlm.py
--rw-r--r--   0        0        0      348 2023-05-08 15:56:24.009313 openlm-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 openlm-0.0.1/setup.py
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 openlm-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-08 15:56:49.714425 openlm-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1518 2023-05-08 22:18:45.011135 openlm-0.0.2/README.md
+-rw-r--r--   0        0        0      132 2023-05-08 21:54:25.618285 openlm-0.0.2/openlm/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-08 19:53:27.996546 openlm-0.0.2/openlm/llm/__init__.py
+-rw-r--r--   0        0        0     1472 2023-05-08 18:39:43.818023 openlm-0.0.2/openlm/llm/base.py
+-rw-r--r--   0        0        0     3051 2023-05-08 22:27:11.789761 openlm-0.0.2/openlm/llm/cohere.py
+-rw-r--r--   0        0        0     3526 2023-05-08 22:27:16.866957 openlm-0.0.2/openlm/llm/huggingface.py
+-rw-r--r--   0        0        0     3374 2023-05-08 22:25:22.904394 openlm-0.0.2/openlm/llm/openai.py
+-rw-r--r--   0        0        0     7734 2023-05-08 22:26:26.647266 openlm-0.0.2/openlm/openlm.py
+-rw-r--r--   0        0        0     1174 2023-05-08 22:27:44.245701 openlm-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 openlm-0.0.2/setup.py
+-rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 openlm-0.0.2/PKG-INFO
```

### Comparing `openlm-0.0.1/LICENSE` & `openlm-0.0.2/LICENSE`

 * *Files identical despite different names*

