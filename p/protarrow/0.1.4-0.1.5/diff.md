# Comparing `tmp/protarrow-0.1.4.tar.gz` & `tmp/protarrow-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protarrow-0.1.4.tar", max compression
+gzip compressed data, was "protarrow-0.1.5.tar", max compression
```

## Comparing `protarrow-0.1.4.tar` & `protarrow-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    10140 2023-02-15 16:08:09.763474 protarrow-0.1.4/LICENSE
--rw-r--r--   0        0        0     3022 2023-02-15 16:08:09.763474 protarrow-0.1.4/README.md
--rw-r--r--   0        0        0      754 2023-02-15 16:08:31.507708 protarrow-0.1.4/protarrow/__init__.py
--rw-r--r--   0        0        0    19405 2023-02-15 16:08:09.763474 protarrow-0.1.4/protarrow/arrow_to_proto.py
--rw-r--r--   0        0        0     7596 2023-02-15 16:08:09.763474 protarrow-0.1.4/protarrow/cast_to_proto.py
--rw-r--r--   0        0        0     1236 2023-02-15 16:08:09.763474 protarrow-0.1.4/protarrow/common.py
--rw-r--r--   0        0        0     4621 2023-02-15 16:08:09.763474 protarrow-0.1.4/protarrow/message_extractor.py
--rw-r--r--   0        0        0    18792 2023-02-15 16:08:09.763474 protarrow-0.1.4/protarrow/proto_to_arrow.py
--rw-r--r--   0        0        0     1858 2023-02-15 16:08:31.507708 protarrow-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3859 1970-01-01 00:00:00.000000 protarrow-0.1.4/setup.py
--rw-r--r--   0        0        0     4285 1970-01-01 00:00:00.000000 protarrow-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    10140 2023-05-09 16:12:07.359680 protarrow-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3022 2023-05-09 16:12:07.359680 protarrow-0.1.5/README.md
+-rw-r--r--   0        0        0      754 2023-05-09 16:12:32.163744 protarrow-0.1.5/protarrow/__init__.py
+-rw-r--r--   0        0        0    19405 2023-05-09 16:12:07.359680 protarrow-0.1.5/protarrow/arrow_to_proto.py
+-rw-r--r--   0        0        0     7596 2023-05-09 16:12:07.359680 protarrow-0.1.5/protarrow/cast_to_proto.py
+-rw-r--r--   0        0        0     1236 2023-05-09 16:12:07.359680 protarrow-0.1.5/protarrow/common.py
+-rw-r--r--   0        0        0     4621 2023-05-09 16:12:07.359680 protarrow-0.1.5/protarrow/message_extractor.py
+-rw-r--r--   0        0        0    18792 2023-05-09 16:12:07.359680 protarrow-0.1.5/protarrow/proto_to_arrow.py
+-rw-r--r--   0        0        0     1858 2023-05-09 16:12:32.159743 protarrow-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4285 1970-01-01 00:00:00.000000 protarrow-0.1.5/PKG-INFO
```

### Comparing `protarrow-0.1.4/LICENSE` & `protarrow-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.4/README.md` & `protarrow-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 # Protarrow
 
 **Protarrow** is a python library for converting from protobuf to arrow and back.
 
 It is used at [Tradewell Technologies](https://www.tradewelltech.co/), 
-to share date between transactional and analytical applications,
+to share data between transactional and analytical applications,
 with little boilerplate code and zero data loss.
 
 # Installation
 
 ```shell
 pip install protarrow
 ```
```

### Comparing `protarrow-0.1.4/protarrow/__init__.py` & `protarrow-0.1.5/protarrow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from protarrow.proto_to_arrow import (
     message_type_to_schema,
     message_type_to_struct_type,
     messages_to_record_batch,
     messages_to_table,
 )
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 __all__ = [
     "MessageExtractor",
     "ProtarrowConfig",
     "cast_record_batch",
     "cast_struct_array",
     "cast_table",
     "message_type_to_schema",
```

### Comparing `protarrow-0.1.4/protarrow/arrow_to_proto.py` & `protarrow-0.1.5/protarrow/arrow_to_proto.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.4/protarrow/cast_to_proto.py` & `protarrow-0.1.5/protarrow/cast_to_proto.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.4/protarrow/common.py` & `protarrow-0.1.5/protarrow/common.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.4/protarrow/message_extractor.py` & `protarrow-0.1.5/protarrow/message_extractor.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.4/protarrow/proto_to_arrow.py` & `protarrow-0.1.5/protarrow/proto_to_arrow.py`

 * *Files identical despite different names*

### Comparing `protarrow-0.1.4/pyproject.toml` & `protarrow-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "protarrow"
-version = "0.1.4"
+version = "0.1.5"
 description = "Convert from protobuf to arrow and back"
 authors = ["Tradewell Tech <engineering@tradewelltech.co>"]
 maintainers = ["0x26res <0x26res@gmail.com>"]
 packages = [
     { include = "protarrow" }
 ]
 readme = "README.md"
```

### Comparing `protarrow-0.1.4/setup.py` & `protarrow-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,123 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['protarrow']
+Metadata-Version: 2.1
+Name: protarrow
+Version: 0.1.5
+Summary: Convert from protobuf to arrow and back
+Home-page: https://github.com/tradewelltech/protarrow
+License: Apache-2.0
+Keywords: apache-arrow,protobuf,data
+Author: Tradewell Tech
+Author-email: engineering@tradewelltech.co
+Maintainer: 0x26res
+Maintainer-email: 0x26res@gmail.com
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: googleapis-common-protos (>=1.53.0)
+Requires-Dist: protobuf (>=3.20.1)
+Requires-Dist: pyarrow (>=8.0.0)
+Project-URL: Documentation, https://protarrow.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/tradewelltech/protarrow
+Description-Content-Type: text/markdown
+
+[![PyPI Version][pypi-image]][pypi-url]
+[![Python Version][versions-image]][versions-url]
+[![Github Stars][stars-image]][stars-url]
+[![codecov][codecov-image]][codecov-url]
+[![Build Status][build-image]][build-url]
+[![Documentation][doc-image]][doc-url]
+[![License][license-image]][license-url]
+[![Downloads][downloads-image]][downloads-url]
+[![Downloads][downloads-month-image]][downloads-month-url]
+[![Code style: black][codestyle-image]][codestyle-url]
+[![snyk][snyk-image]][snyk-url]
+
+
+# Protarrow
+
+**Protarrow** is a python library for converting from protobuf to arrow and back.
+
+It is used at [Tradewell Technologies](https://www.tradewelltech.co/), 
+to share data between transactional and analytical applications,
+with little boilerplate code and zero data loss.
+
+# Installation
+
+```shell
+pip install protarrow
+```
+
+# Usage
+
+Taking a simple protobuf:
+
+```protobuf
+message MyProto {
+  string name = 1;
+  int32 id = 2;
+  repeated int32 values = 3;
+}
+```
 
-package_data = \
-{'': ['*']}
+It can be converted to a `pyarrow.Table`:
 
-install_requires = \
-['googleapis-common-protos>=1.53.0', 'protobuf>=3.20.1', 'pyarrow>=8.0.0']
-
-setup_kwargs = {
-    'name': 'protarrow',
-    'version': '0.1.4',
-    'description': 'Convert from protobuf to arrow and back',
-    'long_description': '[![PyPI Version][pypi-image]][pypi-url]\n[![Python Version][versions-image]][versions-url]\n[![Github Stars][stars-image]][stars-url]\n[![codecov][codecov-image]][codecov-url]\n[![Build Status][build-image]][build-url]\n[![Documentation][doc-image]][doc-url]\n[![License][license-image]][license-url]\n[![Downloads][downloads-image]][downloads-url]\n[![Downloads][downloads-month-image]][downloads-month-url]\n[![Code style: black][codestyle-image]][codestyle-url]\n[![snyk][snyk-image]][snyk-url]\n\n\n# Protarrow\n\n**Protarrow** is a python library for converting from protobuf to arrow and back.\n\nIt is used at [Tradewell Technologies](https://www.tradewelltech.co/), \nto share date between transactional and analytical applications,\nwith little boilerplate code and zero data loss.\n\n# Installation\n\n```shell\npip install protarrow\n```\n\n# Usage\n\nTaking a simple protobuf:\n\n```protobuf\nmessage MyProto {\n  string name = 1;\n  int32 id = 2;\n  repeated int32 values = 3;\n}\n```\n\nIt can be converted to a `pyarrow.Table`:\n\n```python\nimport protarrow\n\nmy_protos = [\n    MyProto(name="foo", id=1, values=[1, 2, 4]),\n    MyProto(name="bar", id=2, values=[3, 4, 5]),\n]\n\ntable = protarrow.messages_to_table(my_protos, MyProto)\n```\n\n\n| name   |   id | values   |\n|:-------|-----:|:---------|\n| foo    |    1 | [1 2 4]  |\n| bar    |    2 | [3 4 5]  |\n\nAnd the table can be converted back to proto:\n\n```python\nprotos_from_table = protarrow.table_to_messages(table, MyProto)\n```\n\nSee the [documentation](https://protarrow.readthedocs.io/en/latest/)\n\n\n<!-- Badges: -->\n\n[pypi-image]: https://img.shields.io/pypi/v/protarrow\n[pypi-url]: https://pypi.org/project/protarrow/\n[build-image]: https://github.com/tradewelltech/protarrow/actions/workflows/ci.yaml/badge.svg\n[build-url]: https://github.com/tradewelltech/protarrow/actions/workflows/ci.yaml\n[stars-image]: https://img.shields.io/github/stars/tradewelltech/protarrow\n[stars-url]: https://github.com/tradewelltech/protarrow\n[versions-image]: https://img.shields.io/pypi/pyversions/protarrow\n[versions-url]: https://pypi.org/project/protarrow/\n[doc-image]: https://readthedocs.org/projects/protarrow/badge/?version=latest\n[doc-url]: https://protarrow.readthedocs.io/en/latest/?badge=latest\n[license-image]: http://img.shields.io/:license-Apache%202-blue.svg\n[license-url]: https://github.com/tradewelltech/protarrow/blob/master/LICENSE\n[codecov-image]: https://codecov.io/gh/tradewelltech/protarrow/branch/master/graph/badge.svg?token=XMFH27IL70\n[codecov-url]: https://codecov.io/gh/tradewelltech/protarrow\n[downloads-image]: https://pepy.tech/badge/protarrow\n[downloads-url]: https://static.pepy.tech/badge/protarrow\n[downloads-month-image]: https://pepy.tech/badge/protarrow/month\n[downloads-month-url]: https://static.pepy.tech/badge/protarrow/month\n[codestyle-image]: https://img.shields.io/badge/code%20style-black-000000.svg\n[codestyle-url]: https://github.com/ambv/black\n[snyk-image]: https://snyk.io/advisor/python/protarrow/badge.svg\n[snyk-url]: https://snyk.io/advisor/python/protarrow\n',
-    'author': 'Tradewell Tech',
-    'author_email': 'engineering@tradewelltech.co',
-    'maintainer': '0x26res',
-    'maintainer_email': '0x26res@gmail.com',
-    'url': 'https://github.com/tradewelltech/protarrow',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.12',
-}
+```python
+import protarrow
 
+my_protos = [
+    MyProto(name="foo", id=1, values=[1, 2, 4]),
+    MyProto(name="bar", id=2, values=[3, 4, 5]),
+]
+
+table = protarrow.messages_to_table(my_protos, MyProto)
+```
+
+
+| name   |   id | values   |
+|:-------|-----:|:---------|
+| foo    |    1 | [1 2 4]  |
+| bar    |    2 | [3 4 5]  |
+
+And the table can be converted back to proto:
+
+```python
+protos_from_table = protarrow.table_to_messages(table, MyProto)
+```
+
+See the [documentation](https://protarrow.readthedocs.io/en/latest/)
+
+
+<!-- Badges: -->
+
+[pypi-image]: https://img.shields.io/pypi/v/protarrow
+[pypi-url]: https://pypi.org/project/protarrow/
+[build-image]: https://github.com/tradewelltech/protarrow/actions/workflows/ci.yaml/badge.svg
+[build-url]: https://github.com/tradewelltech/protarrow/actions/workflows/ci.yaml
+[stars-image]: https://img.shields.io/github/stars/tradewelltech/protarrow
+[stars-url]: https://github.com/tradewelltech/protarrow
+[versions-image]: https://img.shields.io/pypi/pyversions/protarrow
+[versions-url]: https://pypi.org/project/protarrow/
+[doc-image]: https://readthedocs.org/projects/protarrow/badge/?version=latest
+[doc-url]: https://protarrow.readthedocs.io/en/latest/?badge=latest
+[license-image]: http://img.shields.io/:license-Apache%202-blue.svg
+[license-url]: https://github.com/tradewelltech/protarrow/blob/master/LICENSE
+[codecov-image]: https://codecov.io/gh/tradewelltech/protarrow/branch/master/graph/badge.svg?token=XMFH27IL70
+[codecov-url]: https://codecov.io/gh/tradewelltech/protarrow
+[downloads-image]: https://pepy.tech/badge/protarrow
+[downloads-url]: https://static.pepy.tech/badge/protarrow
+[downloads-month-image]: https://pepy.tech/badge/protarrow/month
+[downloads-month-url]: https://static.pepy.tech/badge/protarrow/month
+[codestyle-image]: https://img.shields.io/badge/code%20style-black-000000.svg
+[codestyle-url]: https://github.com/ambv/black
+[snyk-image]: https://snyk.io/advisor/python/protarrow/badge.svg
+[snyk-url]: https://snyk.io/advisor/python/protarrow
 
-setup(**setup_kwargs)
```

