# Comparing `tmp/networkx_query-1.0.1.tar.gz` & `tmp/networkx_query-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networkx_query-1.0.1.tar", last modified: Mon May  4 10:20:47 2020, max compression
+gzip compressed data, was "networkx_query-1.0.2.tar", max compression
```

## Comparing `networkx_query-1.0.1.tar` & `networkx_query-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1100 2020-05-01 17:30:55.612087 networkx_query-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     7131 2020-05-04 10:18:46.979052 networkx_query-1.0.1/README.md
--rw-r--r--   0        0        0      568 2020-05-04 10:18:46.996139 networkx_query-1.0.1/networkx_query/__init__.py
--rw-r--r--   0        0        0     4722 2020-05-04 10:20:35.486651 networkx_query-1.0.1/networkx_query/definition.py
--rw-r--r--   0        0        0     5851 2020-05-01 17:38:29.818462 networkx_query-1.0.1/networkx_query/operator.py
--rw-r--r--   0        0        0     2700 2020-05-04 10:20:35.422062 networkx_query-1.0.1/networkx_query/parser.py
--rw-r--r--   0        0        0     1310 2020-05-04 10:18:46.997524 networkx_query-1.0.1/networkx_query/query.py
--rw-r--r--   0        0        0     2060 2020-05-04 10:18:46.998067 networkx_query-1.0.1/networkx_query/relationship.py
--rw-r--r--   0        0        0     2136 2020-05-04 10:18:46.998562 networkx_query-1.0.1/networkx_query/utils.py
--rw-r--r--   0        0        0     4167 2020-05-04 10:18:47.000669 networkx_query-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8061 2020-05-04 10:20:47.262063 networkx_query-1.0.1/setup.py
--rw-r--r--   0        0        0     8106 2020-05-04 10:20:47.263034 networkx_query-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2020-09-09 06:59:30.189856 networkx_query-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     7131 2020-09-09 06:59:30.190132 networkx_query-1.0.2/README.md
+-rw-r--r--   0        0        0      568 2023-05-09 10:42:29.829423 networkx_query-1.0.2/networkx_query/__init__.py
+-rw-r--r--   0        0        0     4722 2020-09-09 06:59:30.234021 networkx_query-1.0.2/networkx_query/definition.py
+-rw-r--r--   0        0        0     5851 2020-09-09 06:59:30.234191 networkx_query-1.0.2/networkx_query/operator.py
+-rw-r--r--   0        0        0     2700 2020-09-09 06:59:30.234349 networkx_query-1.0.2/networkx_query/parser.py
+-rw-r--r--   0        0        0     1310 2020-09-09 06:59:30.234497 networkx_query-1.0.2/networkx_query/query.py
+-rw-r--r--   0        0        0     2060 2020-09-09 06:59:30.234632 networkx_query-1.0.2/networkx_query/relationship.py
+-rw-r--r--   0        0        0     2136 2020-09-09 06:59:30.234763 networkx_query-1.0.2/networkx_query/utils.py
+-rw-r--r--   0        0        0     3017 2023-05-09 11:15:01.856553 networkx_query-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8062 2023-05-09 11:16:18.585241 networkx_query-1.0.2/setup.py
+-rw-r--r--   0        0        0     8157 2023-05-09 11:16:18.585717 networkx_query-1.0.2/PKG-INFO
```

### Comparing `networkx_query-1.0.1/LICENSE.md` & `networkx_query-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.1/README.md` & `networkx_query-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.1/networkx_query/__init__.py` & `networkx_query-1.0.2/networkx_query/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """networkx-query."""
 from pkg_resources import DistributionNotFound, get_distribution
 
 from .definition import Evaluator, ParserException
 from .parser import prepare_query
-from .query import search_nodes, search_edges
+from .query import search_edges, search_nodes
 from .relationship import search_direct_relationships
 
 __all__ = [
     'search_nodes',
     'search_edges',
     'search_direct_relationships',
     'prepare_query',
```

### Comparing `networkx_query-1.0.1/networkx_query/definition.py` & `networkx_query-1.0.2/networkx_query/definition.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.1/networkx_query/operator.py` & `networkx_query-1.0.2/networkx_query/operator.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.1/networkx_query/parser.py` & `networkx_query-1.0.2/networkx_query/parser.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.1/networkx_query/query.py` & `networkx_query-1.0.2/networkx_query/query.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.1/networkx_query/relationship.py` & `networkx_query-1.0.2/networkx_query/relationship.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.1/networkx_query/utils.py` & `networkx_query-1.0.2/networkx_query/utils.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.1/setup.py` & `networkx_query-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['networkx>=2.4,<3.0']
 
 setup_kwargs = {
     'name': 'networkx-query',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'NetworkX Query Tool',
     'long_description': '# networkx-query\n\n\n[![Unix Build Status](https://img.shields.io/travis/geronimo-iia/networkx-query/master.svg?label=unix)](https://travis-ci.com/geronimo-iia/networkx-query)[![Coverage Status](https://img.shields.io/coveralls/geronimo-iia/networkx-query/master.svg)](https://coveralls.io/r/geronimo-iia/networkx-query)\n[![Codacy Badge](https://api.codacy.com/project/badge/Grade/fe669a02b4aa46b5b1faf619ba2bf382)](https://www.codacy.com/app/geronimo-iia/networkx-query?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=geronimo-iia/networkx-query&amp;utm_campaign=Badge_Grade)[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/geronimo-iia/networkx-query.svg)](https://scrutinizer-ci.com/g/geronimo-iia/networkx-query/?branch=master)\n[![PyPI Version](https://img.shields.io/pypi/v/networkx-query.svg)](https://pypi.org/project/networkx-query)\n[![PyPI License](https://img.shields.io/pypi/l/networkx-query.svg)](https://pypi.org/project/networkx-query)\n\nVersions following [Semantic Versioning](https://semver.org/)\n\n## Overview\n\nNetworkX Query Tool (preview)\n\nSee [documentation](https://geronimo-iia.github.io/networkx-query).\n\n\n## Installation\n\nInstall this library directly into an activated virtual environment:\n\n```text\n$ pip install networkx-query\n```\n\nor add it to your [Poetry](https://poetry.eustace.io/) project:\n\n```text\n$ poetry add networkx-query\n```\n\n## Usage\n\n### Searching nodes\n\n```python\nimport networkx as nx\nfrom networkx_query import search_nodes, search_edges\n\ng = nx.DiGraph()\ng.add_node(1, product="chocolate")\ng.add_node(2, product="milk")\ng.add_node(3, product="coat")\ng.add_edge(1, 2, action="shake")\ng.add_edge(3, 2, action="produce")\n\n\nfor node_id in search_nodes(g, {"==": [("product",), "chocolate"]}):\n    print(node_id)\n\n>> 1\n```\n\n### Searching edges\n\n```python\nfor edge_id in search_edges(g, {"eq": [("action",), "produce"]}):\n    print(edge_id)\n\n>> (3, 2)\n```\n\n### Searching relation ship\n\nWith ```search_direct_relationships``` you can made a query which filter edges on their :\n - source node attributes\n - edge attributes\n - target node attributes\n\nWith this graph:\n\n```python\nimport networkx as nx\nfrom networkx_query import search_direct_relationships\n\ng = nx.DiGraph()\nfor i in range(30):\n    g.add_node(i, data=i)\n\nfor i in range(10, 30):\n    g.add_edge(i - 10, i, data=i)\n```\n\nWe can filtering all edges with source node with data < 3:\n\n```python\nlist(search_direct_relationships(graph=g, source={"lt": ["data", 3]}))\n\n[(0, 10), (1, 11), (2, 12)]\n```\n\n\nWe can filtering all edges with:\n - source node with data < 8\n - edge with data > 15\n\n```python\nlist(search_direct_relationships(graph=g, source={"lt": ["data", 8]}, edge={"gt": ["data", 15]}))\n\n>> [(6, 16), (7, 17)]\n```\n\nWe can filtering all edges with:\n - source node with data > 9\n - edge with data > 15\n - target node with data < 22\n\n```python\nsearch_direct_relationships(\n            graph=g, source={"gt": ["data", 9]}, edge={"gt": ["data", 15]}, target={\'lt\': ["data", 22]}\n        )\n    )\n\n>> [(10, 20), (11, 21)]\n```\n\n## API\n\nActually, we have:\n\n- [search_edges](https://geronimo-iia.github.io/networkx-query/api.html#networkx_query.search_edges)\n- [search_nodes](https://geronimo-iia.github.io/networkx-query/api.html#networkx_query.search_nodes) \n- [search_direct_relationships](https://geronimo-iia.github.io/networkx-query/api.html#networkx_query.search_direct_relationships) \n\n\nAll this function are based on [prepare_query](https://geronimo-iia.github.io/networkx-query/api.html#networkx_query.prepare_query) which return an Evaluator.\n\nQuickly, ```Evaluator``` are function with this signature: (context) -> bool, and ```Context``` is a dictionary like structure (with in and [] methods, and support __contains__ or  (__iter__ and __getitem__))\nWith networkX, node and edge attributes are dictionary like, so implementation of this three methods are very simple.\n\n\n\n## Query language\n\nWe define a little json query language like [json-query-language](https://github.com/clue/json-query-language/blob/master/SYNTAX.md) \nagainst nodes or edges attributes.\n\n\n### Expressions\n\nMain expression syntax turn around this:\n\n```\n{\n    operator_name : parameters\n}\n```\n\n### Basic matching expression\n\nTest if a node/edge has an attribute named "my_property":\n```\n{\n    "has" : "my_property"\n}\n```\n\n\nTest if a node/edge has an attribute product : { "definition": { "name": xxx }} with xxx equals to "chocolate".\n```\n{\n    "eq" : [ ("product", "definition", "name"), "chocolate"]\n}\n```\n\nThe tuple ```("product", "definition", "name")``` is a path in attribut dictionnary.\nA Path is a single string or a tuple of string which represente a path in a tree (here a dictionary).\n\nWe support this operators:\n\n| Name     | Alias | Parameters      | Description                                                                   |\n| -------- | :---: | --------------- | ----------------------------------------------------------------------------- |\n| has      |       | Path            | Check if path exists in context.                                              |\n| contains |       | Path, str       | Check if an attribut path exists and contains specified value.                |\n| eq       | `==`  | Path, Any       | Check if an attribut path exists and equals specified value.                  |\n| neq      | `!=`  | Path, Any       | Check if an attribut path did not exists or not equals specified value.       |\n| gt       |  `>`  | Path, Any       | Check if an attribut path exists and greather that specified value.           |\n| lt       |  `<`  | Path, Any       | Check if an attribut path exists and lower that specified value.              |\n| gte      | `>=`  | Path, Any       | Check if an attribut path exists and greather or equals that specified value. |\n| lte      | `<=`  | Path, Any       | Check if an attribut path exists and lower or equals that specified value.    |\n| in       | `:=`  | Path, List[Any] | Check if an attribut path exists and attribut value in specified values.      |\n\n\n### Boolean composition of matching expression\n\nWe support this operators:\n\n| Name | Alias | Parameters    | Description    |\n| ---- | :---: | ------------- | -------------- |\n| and  | `&&`  | list of query | And operator.  |\n| or   | \\|\\|  | list of query | Or operator.   |\n| xor  |       | list of query | xor operator.  |\n| nxor |       | list of query | nxor operator. |\n| not  |  `!`  | query         | Not operator.  |\n\n\nBy default, a list of expressions is equivalent of an "AND" of this expressions.\n\nExample:\n```\n{\n    \'not\': {\n        \'has\': [\'group\']\n    },\n    \'has\': \'application\',\n    \'eq\': [(\'_link\', \'other\', \'weight\'), 2]\n}\n```\nis equivalent to:\n\n```\n{\n    \'and\': [\n        {\n            \'not\': [\n                {\n                    \'has\': [\'group\']\n                }\n            ]\n        },\n        {\n            \'has\': [\'application\']\n        },\n        {\n            \'eq\': [(\'_link\', \'other\', \'weight\'), 2]\n        }\n    ]\n}\n```\n\n\n## Wished Features\n\n- add projection expression (a return like statement)\n- add join relation ship \n- add path condition between node\n\n\n',
     'author': 'Jerome Guibert',
     'author_email': 'jguibert@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://pypi.org/project/networkx_query',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `networkx_query-1.0.1/PKG-INFO` & `networkx_query-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: networkx-query
-Version: 1.0.1
+Version: 1.0.2
 Summary: NetworkX Query Tool
 Home-page: https://pypi.org/project/networkx_query
 License: MIT
 Keywords: networkx,graph,query
 Author: Jerome Guibert
 Author-email: jguibert@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: networkx (>=2.4,<3.0)
 Project-URL: Documentation, https://geronimo-iia.github.io/networkx-query/
 Project-URL: Repository, https://github.com/geronimo-iia/networkx-query
 Description-Content-Type: text/markdown
```

