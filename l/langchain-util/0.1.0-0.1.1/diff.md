# Comparing `tmp/langchain_util-0.1.0.tar.gz` & `tmp/langchain_util-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_util-0.1.0.tar", max compression
+gzip compressed data, was "langchain_util-0.1.1.tar", max compression
```

## Comparing `langchain_util-0.1.0.tar` & `langchain_util-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-07 23:32:05.575677 langchain_util-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-07 23:33:44.665502 langchain_util-0.1.0/langchain_util/__init__.py
--rw-r--r--   0        0        0      105 2023-05-08 00:49:14.383337 langchain_util-0.1.0/langchain_util/chains/__init__.py
--rw-r--r--   0        0        0      310 2023-05-08 00:49:16.495330 langchain_util-0.1.0/langchain_util/chains/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2873 2023-05-08 22:17:58.624591 langchain_util-0.1.0/langchain_util/chains/__pycache__/concatenate_chain.cpython-311.pyc
--rw-r--r--   0        0        0     1303 2023-05-08 22:17:54.772616 langchain_util-0.1.0/langchain_util/chains/concatenate_chain.py
--rw-r--r--   0        0        0      462 2023-05-08 00:34:15.203220 langchain_util-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 langchain_util-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-07 23:32:05.575677 langchain_util-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 23:33:44.665502 langchain_util-0.1.1/langchain_util/__init__.py
+-rw-r--r--   0        0        0      105 2023-05-08 00:49:14.383337 langchain_util-0.1.1/langchain_util/chains/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-08 00:49:16.495330 langchain_util-0.1.1/langchain_util/chains/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2873 2023-05-08 22:17:58.624591 langchain_util-0.1.1/langchain_util/chains/__pycache__/concatenate_chain.cpython-311.pyc
+-rw-r--r--   0        0        0     1303 2023-05-08 22:17:54.772616 langchain_util-0.1.1/langchain_util/chains/concatenate_chain.py
+-rw-r--r--   0        0        0      470 2023-05-09 00:19:56.311297 langchain_util-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 langchain_util-0.1.1/PKG-INFO
```

### Comparing `langchain_util-0.1.0/langchain_util/chains/__pycache__/concatenate_chain.cpython-311.pyc` & `langchain_util-0.1.1/langchain_util/chains/__pycache__/concatenate_chain.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `langchain_util-0.1.0/langchain_util/chains/concatenate_chain.py` & `langchain_util-0.1.1/langchain_util/chains/concatenate_chain.py`

 * *Files identical despite different names*

