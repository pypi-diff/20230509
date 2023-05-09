# Comparing `tmp/ethhelper-0.3.5.tar.gz` & `tmp/ethhelper-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethhelper-0.3.5.tar", max compression
+gzip compressed data, was "ethhelper-0.3.6.tar", max compression
```

## Comparing `ethhelper-0.3.5.tar` & `ethhelper-0.3.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-04-24 04:23:56.146270 ethhelper-0.3.5/LICENSE
--rw-r--r--   0        0        0     1708 2023-04-24 04:23:56.146270 ethhelper-0.3.5/README.md
--rw-r--r--   0        0        0     2137 2023-04-24 04:23:56.146270 ethhelper-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-24 04:23:56.146270 ethhelper-0.3.5/src/ethhelper/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 04:23:56.146270 ethhelper-0.3.5/src/ethhelper/connectors/__init__.py
--rw-r--r--   0        0        0     1565 2023-04-24 04:23:56.146270 ethhelper-0.3.5/src/ethhelper/connectors/http/__init__.py
--rw-r--r--   0        0        0    13216 2023-04-24 04:23:56.146270 ethhelper-0.3.5/src/ethhelper/connectors/http/base.py
--rw-r--r--   0        0        0     7712 2023-04-24 04:23:56.146270 ethhelper-0.3.5/src/ethhelper/connectors/http/custom.py
--rw-r--r--   0        0        0    16281 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/connectors/http/eth.py
--rw-r--r--   0        0        0     1743 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/connectors/http/net.py
--rw-r--r--   0        0        0     3958 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/connectors/http/txpool.py
--rw-r--r--   0        0        0      159 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/connectors/ws/__init__.py
--rw-r--r--   0        0        0     5912 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/connectors/ws/base.py
--rw-r--r--   0        0        0     3505 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/connectors/ws/block.py
--rw-r--r--   0        0        0        0 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/datatypes/__init__.py
--rw-r--r--   0        0        0     7579 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/datatypes/base.py
--rw-r--r--   0        0        0    17501 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/datatypes/eth.py
--rw-r--r--   0        0        0     6824 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/datatypes/geth.py
--rw-r--r--   0        0        0     5135 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/datatypes/txpool.py
--rw-r--r--   0        0        0        0 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/py.typed
--rw-r--r--   0        0        0     1387 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/types.py
--rw-r--r--   0        0        0        0 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/utils/__init__.py
--rw-r--r--   0        0        0      927 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/utils/convert.py
--rw-r--r--   0        0        0      498 2023-04-24 04:23:56.150270 ethhelper-0.3.5/src/ethhelper/utils/json.py
--rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 ethhelper-0.3.5/setup.py
--rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 ethhelper-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 05:07:50.736843 ethhelper-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1708 2023-05-09 05:07:50.736843 ethhelper-0.3.6/README.md
+-rw-r--r--   0        0        0     2155 2023-05-09 05:07:50.740844 ethhelper-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/__init__.py
+-rw-r--r--   0        0        0     1565 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/http/__init__.py
+-rw-r--r--   0        0        0    13216 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/http/base.py
+-rw-r--r--   0        0        0     7712 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/http/custom.py
+-rw-r--r--   0        0        0    16281 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/http/eth.py
+-rw-r--r--   0        0        0     1743 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/http/net.py
+-rw-r--r--   0        0        0     3958 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/http/txpool.py
+-rw-r--r--   0        0        0      159 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/ws/__init__.py
+-rw-r--r--   0        0        0     5912 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/ws/base.py
+-rw-r--r--   0        0        0     3505 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/ws/block.py
+-rw-r--r--   0        0        0        0 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/datatypes/__init__.py
+-rw-r--r--   0        0        0     7579 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/datatypes/base.py
+-rw-r--r--   0        0        0    17501 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/datatypes/eth.py
+-rw-r--r--   0        0        0     6824 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/datatypes/geth.py
+-rw-r--r--   0        0        0     5135 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/datatypes/txpool.py
+-rw-r--r--   0        0        0        0 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/py.typed
+-rw-r--r--   0        0        0     1387 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/types.py
+-rw-r--r--   0        0        0        0 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/utils/__init__.py
+-rw-r--r--   0        0        0      927 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/utils/convert.py
+-rw-r--r--   0        0        0      498 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/utils/json.py
+-rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 ethhelper-0.3.6/setup.py
+-rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 ethhelper-0.3.6/PKG-INFO
```

### Comparing `ethhelper-0.3.5/LICENSE` & `ethhelper-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/README.md` & `ethhelper-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/pyproject.toml` & `ethhelper-0.3.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ethhelper"
-version = "0.3.5"
+version = "0.3.6"
 description = "Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic."
 authors = ["XiaoHuiHui233 <1025184872@qq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/XiaoHuiHui233/ETHHelper"
 keywords = ["ethereum", "asyncio", "geth", "pydantic"]
 
 [tool.poetry.dependencies]
 eth-typing = "^3.3.0"
 httpx = "^0.23.3"
-orjson = "^3.8.10"
+orjson = "^3.8.12"
 pydantic = "^1.10.7"
 python = "^3.10"
-web3 = "^6.2.0"
+web3 = "^6.3.0"
 websockets = "^10.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.2.0"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.20.3"
 python-dotenv = "^1.0.0"
 ruff = "^0.0.253"
 
 [tool.poetry.group.docs.dependencies]
 docutils = "<0.19"
+sphinx = "^6.2.1"
 sphinx-pydantic = "^0.1.1"
 sphinx-rtd-theme = "^1.2.0"
 
 [tool.ruff]
 extend-select = ["Q", "RUF100", "C90"]
 flake8-quotes = {inline-quotes = "double", multiline-quotes = "double"}
 line-length = 79
```

### Comparing `ethhelper-0.3.5/src/ethhelper/connectors/http/__init__.py` & `ethhelper-0.3.6/src/ethhelper/connectors/http/__init__.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/connectors/http/base.py` & `ethhelper-0.3.6/src/ethhelper/connectors/http/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/connectors/http/custom.py` & `ethhelper-0.3.6/src/ethhelper/connectors/http/custom.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/connectors/http/eth.py` & `ethhelper-0.3.6/src/ethhelper/connectors/http/eth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/connectors/http/net.py` & `ethhelper-0.3.6/src/ethhelper/connectors/http/net.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/connectors/http/txpool.py` & `ethhelper-0.3.6/src/ethhelper/connectors/http/txpool.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/connectors/ws/base.py` & `ethhelper-0.3.6/src/ethhelper/connectors/ws/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/connectors/ws/block.py` & `ethhelper-0.3.6/src/ethhelper/connectors/ws/block.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/datatypes/base.py` & `ethhelper-0.3.6/src/ethhelper/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/datatypes/eth.py` & `ethhelper-0.3.6/src/ethhelper/datatypes/eth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/datatypes/geth.py` & `ethhelper-0.3.6/src/ethhelper/datatypes/geth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/datatypes/txpool.py` & `ethhelper-0.3.6/src/ethhelper/datatypes/txpool.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/types.py` & `ethhelper-0.3.6/src/ethhelper/types.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/src/ethhelper/utils/convert.py` & `ethhelper-0.3.6/src/ethhelper/utils/convert.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.5/setup.py` & `ethhelper-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['eth-typing>=3.3.0,<4.0.0',
  'httpx>=0.23.3,<0.24.0',
- 'orjson>=3.8.10,<4.0.0',
+ 'orjson>=3.8.12,<4.0.0',
  'pydantic>=1.10.7,<2.0.0',
- 'web3>=6.2.0,<7.0.0',
+ 'web3>=6.3.0,<7.0.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'ethhelper',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': 'Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.',
     'long_description': "# ETHHelper\n\n[![Build Status](https://img.shields.io/github/actions/workflow/status/XiaoHuiHui233/ETHHelper/publish.yml)](https://github.com/XiaoHuiHui233/ETHHelper/actions)\n[![Documentation Status](https://readthedocs.org/projects/ethhelper/badge/?version=latest)](https://ethhelper.readthedocs.io/en/latest/?badge=latest)\n![Python Version](https://img.shields.io/pypi/pyversions/ethhelper)\n![Wheel Status](https://img.shields.io/pypi/wheel/ethhelper)\n[![Latest Version](https://img.shields.io/github/v/release/XiaoHuiHui233/ETHHelper)](https://github.com/XiaoHuiHui233/ETHHelper/releases)\n[![License](https://img.shields.io/github/license/XiaoHuiHui233/ETHHelper)](https://github.com/XiaoHuiHui233/ETHHelper/blob/main/LICENSE)\n\nAsynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.\n\nQuickstart see [this](https://ethhelper.readthedocs.io/en/latest/quickstart.html).\n\n[中文](docs/README_cn.md) | English\n\n## Usage\n\n### pypi\n\nIf you prefer to use pypi to install this package, you can just run the following command:\n\n```bash\npip install ethhelper\n```\n\n### git\n\nThe project is managed by poetry. If you prefer to use git to install this package, you can use poetry to directly add a reference to the project's build package through git.\n\nThe command is as follow:\n\n```bash\npoetry add git+ssh://git@github.com:XiaoHuiHui233/ETHHelper.git\n```\n\n## Build\n\nYou can use poetry's tools to generate a build of this project (pure Python).\n\nThe command is as follow:\n\n```bash\npoetry build\n```\n\n## Author and License\n\nETHHelper was written by [XiaoHuiHui233](https://github.com/XiaoHuiHui233/), licensed under the Apache 2.0.\n",
     'author': 'XiaoHuiHui233',
     'author_email': '1025184872@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/XiaoHuiHui233/ETHHelper',
```

### Comparing `ethhelper-0.3.5/PKG-INFO` & `ethhelper-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ethhelper
-Version: 0.3.5
+Version: 0.3.6
 Summary: Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.
 Home-page: https://github.com/XiaoHuiHui233/ETHHelper
 License: Apache-2.0
 Keywords: ethereum,asyncio,geth,pydantic
 Author: XiaoHuiHui233
 Author-email: 1025184872@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: eth-typing (>=3.3.0,<4.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: orjson (>=3.8.10,<4.0.0)
+Requires-Dist: orjson (>=3.8.12,<4.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: web3 (>=6.2.0,<7.0.0)
+Requires-Dist: web3 (>=6.3.0,<7.0.0)
 Requires-Dist: websockets (>=10.4,<11.0)
 Project-URL: Repository, https://github.com/XiaoHuiHui233/ETHHelper
 Description-Content-Type: text/markdown
 
 # ETHHelper
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/XiaoHuiHui233/ETHHelper/publish.yml)](https://github.com/XiaoHuiHui233/ETHHelper/actions)
```

