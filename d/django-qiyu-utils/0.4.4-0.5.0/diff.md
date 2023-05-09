# Comparing `tmp/django-qiyu-utils-0.4.4.tar.gz` & `tmp/django_qiyu_utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-qiyu-utils-0.4.4.tar", max compression
+gzip compressed data, was "django_qiyu_utils-0.5.0.tar", max compression
```

## Comparing `django-qiyu-utils-0.4.4.tar` & `django_qiyu_utils-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,10 @@
--rw-r--r--   0        0        0    35149 2022-09-18 13:27:43.936699 django-qiyu-utils-0.4.4/LICENSE
--rw-r--r--   0        0        0      596 2022-09-18 13:27:43.936699 django-qiyu-utils-0.4.4/README.md
--rw-r--r--   0        0        0      173 2022-09-18 13:27:43.936699 django-qiyu-utils-0.4.4/django_qiyu_utils/__init__.py
--rw-r--r--   0        0        0     1166 2022-09-18 13:27:43.936699 django-qiyu-utils-0.4.4/django_qiyu_utils/div_node/__init__.py
--rw-r--r--   0        0        0     1048 2022-09-18 13:27:43.936699 django-qiyu-utils-0.4.4/django_qiyu_utils/div_node/div_node.py
--rw-r--r--   0        0        0     1998 2022-09-18 13:27:43.936699 django-qiyu-utils-0.4.4/django_qiyu_utils/env.py
--rw-r--r--   0        0        0      534 2022-09-18 13:27:43.936699 django-qiyu-utils-0.4.4/django_qiyu_utils/http_header.py
--rw-r--r--   0        0        0     2028 2022-09-18 13:27:43.936699 django-qiyu-utils-0.4.4/django_qiyu_utils/paginator.py
--rw-r--r--   0        0        0      971 2022-09-18 13:27:43.936699 django-qiyu-utils-0.4.4/django_qiyu_utils/redirect.py
--rw-r--r--   0        0        0     3956 2022-09-18 13:27:43.936699 django-qiyu-utils-0.4.4/django_qiyu_utils/settings.py
--rw-r--r--   0        0        0      433 2022-09-18 13:27:43.936699 django-qiyu-utils-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 django-qiyu-utils-0.4.4/setup.py
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 django-qiyu-utils-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-09 14:59:10.327355 django_qiyu_utils-0.5.0/LICENSE
+-rw-r--r--   0        0        0      596 2023-05-09 14:59:10.327355 django_qiyu_utils-0.5.0/README.md
+-rw-r--r--   0        0        0      107 2023-05-09 14:59:10.327355 django_qiyu_utils-0.5.0/django_qiyu_utils/__init__.py
+-rw-r--r--   0        0        0     1166 2023-05-09 14:59:10.327355 django_qiyu_utils-0.5.0/django_qiyu_utils/div_node/__init__.py
+-rw-r--r--   0        0        0     1048 2023-05-09 14:59:10.327355 django_qiyu_utils-0.5.0/django_qiyu_utils/div_node/div_node.py
+-rw-r--r--   0        0        0     1998 2023-05-09 14:59:10.327355 django_qiyu_utils-0.5.0/django_qiyu_utils/env.py
+-rw-r--r--   0        0        0      971 2023-05-09 14:59:10.327355 django_qiyu_utils-0.5.0/django_qiyu_utils/redirect.py
+-rw-r--r--   0        0        0     3956 2023-05-09 14:59:10.327355 django_qiyu_utils-0.5.0/django_qiyu_utils/settings.py
+-rw-r--r--   0        0        0      433 2023-05-09 14:59:10.331356 django_qiyu_utils-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 django_qiyu_utils-0.5.0/PKG-INFO
```

### Comparing `django-qiyu-utils-0.4.4/LICENSE` & `django_qiyu_utils-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-qiyu-utils-0.4.4/README.md` & `django_qiyu_utils-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `django-qiyu-utils-0.4.4/django_qiyu_utils/div_node/__init__.py` & `django_qiyu_utils-0.5.0/django_qiyu_utils/div_node/__init__.py`

 * *Files identical despite different names*

### Comparing `django-qiyu-utils-0.4.4/django_qiyu_utils/div_node/div_node.py` & `django_qiyu_utils-0.5.0/django_qiyu_utils/div_node/div_node.py`

 * *Files identical despite different names*

### Comparing `django-qiyu-utils-0.4.4/django_qiyu_utils/env.py` & `django_qiyu_utils-0.5.0/django_qiyu_utils/env.py`

 * *Files identical despite different names*

### Comparing `django-qiyu-utils-0.4.4/django_qiyu_utils/redirect.py` & `django_qiyu_utils-0.5.0/django_qiyu_utils/redirect.py`

 * *Files identical despite different names*

### Comparing `django-qiyu-utils-0.4.4/django_qiyu_utils/settings.py` & `django_qiyu_utils-0.5.0/django_qiyu_utils/settings.py`

 * *Files identical despite different names*

### Comparing `django-qiyu-utils-0.4.4/PKG-INFO` & `django_qiyu_utils-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: django-qiyu-utils
-Version: 0.4.4
+Version: 0.5.0
 Summary: Django 辅助工具类
 Home-page: https://oss.qiyutech.tech/
 Author: dev
 Author-email: dev@qiyutech.tech
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: django (>=3.2,<4.2)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: django (>=4.0,<4.3)
 Description-Content-Type: text/markdown
 
 # 奇遇科技 Django 辅助工具箱
 
 ![PyPI - Version](https://img.shields.io/pypi/v/django-qiyu-utils)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-qiyu-utils)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/django-qiyu-utils)
```

