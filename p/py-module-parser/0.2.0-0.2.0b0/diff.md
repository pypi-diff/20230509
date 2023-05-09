# Comparing `tmp/py-module-parser-0.2.0.tar.gz` & `tmp/py-module-parser-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-module-parser-0.2.0.tar", max compression
+gzip compressed data, was "py-module-parser-0.2.0b0.tar", max compression
```

## Comparing `py-module-parser-0.2.0.tar` & `py-module-parser-0.2.0b0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1093 2023-05-09 19:52:20.665429 py-module-parser-0.2.0/LICENSE
--rw-r--r--   0        0        0     4004 2023-05-09 19:50:56.096364 py-module-parser-0.2.0/README.md
--rw-r--r--   0        0        0      153 2023-05-09 19:35:44.746055 py-module-parser-0.2.0/py_module_parser/__init__.py
--rw-r--r--   0        0        0     1255 2023-05-09 19:42:22.221129 py-module-parser-0.2.0/py_module_parser/models.py
--rw-r--r--   0        0        0     8767 2023-05-09 19:46:22.296262 py-module-parser-0.2.0/py_module_parser/parser.py
--rw-r--r--   0        0        0      406 2023-05-09 19:23:59.461629 py-module-parser-0.2.0/py_module_parser/utils.py
--rw-r--r--   0        0        0     1104 2023-05-09 19:55:52.231761 py-module-parser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4977 2023-05-09 19:55:55.156420 py-module-parser-0.2.0/setup.py
--rw-r--r--   0        0        0     5084 2023-05-09 19:55:55.156870 py-module-parser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-09 19:52:20.665429 py-module-parser-0.2.0b0/LICENSE
+-rw-r--r--   0        0        0     4004 2023-05-09 19:50:56.096364 py-module-parser-0.2.0b0/README.md
+-rw-r--r--   0        0        0      153 2023-05-09 19:35:44.746055 py-module-parser-0.2.0b0/py_module_parser/__init__.py
+-rw-r--r--   0        0        0     1255 2023-05-09 19:42:22.221129 py-module-parser-0.2.0b0/py_module_parser/models.py
+-rw-r--r--   0        0        0     8767 2023-05-09 19:46:22.296262 py-module-parser-0.2.0b0/py_module_parser/parser.py
+-rw-r--r--   0        0        0      406 2023-05-09 19:23:59.461629 py-module-parser-0.2.0b0/py_module_parser/utils.py
+-rw-r--r--   0        0        0     1105 2023-05-09 19:54:49.297724 py-module-parser-0.2.0b0/pyproject.toml
+-rw-r--r--   0        0        0     4979 2023-05-09 19:54:51.573483 py-module-parser-0.2.0b0/setup.py
+-rw-r--r--   0        0        0     5086 2023-05-09 19:54:51.573934 py-module-parser-0.2.0b0/PKG-INFO
```

### Comparing `py-module-parser-0.2.0/LICENSE` & `py-module-parser-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-module-parser-0.2.0/README.md` & `py-module-parser-0.2.0b0/README.md`

 * *Files identical despite different names*

### Comparing `py-module-parser-0.2.0/py_module_parser/models.py` & `py-module-parser-0.2.0b0/py_module_parser/models.py`

 * *Files identical despite different names*

### Comparing `py-module-parser-0.2.0/py_module_parser/parser.py` & `py-module-parser-0.2.0b0/py_module_parser/parser.py`

 * *Files identical despite different names*

### Comparing `py-module-parser-0.2.0/pyproject.toml` & `py-module-parser-0.2.0b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-module-parser"
-version = "0.2.0"
+version = "0.2.0b"
 description = "Python Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code."
 authors = ["Iuliia Volkova <xnuinside@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/xnuinside/py-module-parser"
 repository = "https://github.com/xnuinside/py-module-parser"
 classifiers = [
```

### Comparing `py-module-parser-0.2.0/setup.py` & `py-module-parser-0.2.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['py_module_parser']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'py-module-parser',
-    'version': '0.2.0',
+    'version': '0.2.0b0',
     'description': 'Python Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code.',
     'long_description': '# Python Module Parser\n![badge1](https://img.shields.io/pypi/v/py-module-parser) ![badge2](https://img.shields.io/pypi/l/py-module-parser) ![badge3](https://img.shields.io/pypi/pyversions/py-module-parser)![workflow](https://github.com/xnuinside/py-module-parser/actions/workflows/main.yml/badge.svg)\n\nPython Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code.\n\nTo get more samples of output - check tests: tests/test_py_module_parser.py\n\nThis project inspired by https://github.com/xnuinside/codegraph and https://github.com/xnuinside/py-models-parser and will be used as a parser inside them in the future. \n\n## Features\n\n- Parse Python modules and extract information about imports, functions, and variables\n- Identify line numbers for each import, function, and variable\n- Represent the extracted information in a structured format\n\n## Installation\n\nTo install the Python Module Parser library, use `pip`:\n\n```bash\n    pip install py-module-parser\n```\n\n\n## Usage\nHere\'s a simple example of how to use the Python Module Parser library:\n\n```python\nfrom py_module_parser import PyModulesParser\n\nsource_code = """from django.db import models\n\n\nclass Musician(models.Model):\n    first_name = models.CharField(max_length=50)\n    last_name = models.CharField(max_length=50)\n    instrument = models.CharField(max_length=100)\n\n"""\nparsed_output = PyModulesParser(source_code).parse()\nprint(parsed_output)\n```\n\nThis will output:\n\n```python\n[\n    FromImportOutput(\n        lineno_start=1,\n        lineno_end=1,\n        module=\'django.db\',\n        imports=[\n            ImportOutput(\n                lineno_start=1,\n                lineno_end=1,\n                name=\'models\',\n                alias=None,\n                node_type=\'import\'\n            )\n        ],\n        node_type=\'from_import\'\n    ),\n    ClassOutput(\n        lineno_start=4,\n        lineno_end=7,\n        name=\'Musician\',\n        parents=[\'models.Model\'],\n        attrs=[\n            VariableOutput(\n                lineno_start=5,\n                lineno_end=5,\n                name=\'first_name\',\n                type_annotation=None,\n                default=FuncCallOutput(\n                    lineno_start=5,\n                    lineno_end=5,\n                    func_name=\'models.CharField\',\n                    args=[],\n                    kwargs={\'max_length\': 50},\n                    node_type=\'func_call\'\n                ),\n                properties={},\n                node_type=\'variable\'\n            ),\n            VariableOutput(\n                lineno_start=6,\n                lineno_end=6,\n                name=\'last_name\',\n                type_annotation=None,\n                default=FuncCallOutput(\n                    lineno_start=6,\n                    lineno_end=6,\n                    func_name=\'models.CharField\',\n                    args=[],\n                    kwargs={\'max_length\': 50},\n                    node_type=\'func_call\'\n                ),\n                properties={},\n                node_type=\'variable\'\n            ),\n            VariableOutput(\n                lineno_start=7,\n                lineno_end=7,\n                name=\'instrument\',\n                type_annotation=None,\n                default=FuncCallOutput(\n                    lineno_start=7,\n                    lineno_end=7,\n                    func_name=\'models.CharField\',\n                    args=[],\n                    kwargs={\'max_length\': 100},\n                    node_type=\'func_call\'\n                ),\n                properties={},\n                node_type=\'variable\'\n            )\n        ],\n        node_type=\'class\'\n    )\n]\n```\n\nTo parse from file, you can use method `parse_from_file`\n\n```python\nfrom py_module_parser import parse_from_file\n\nparsed_output = parse_from_file(file_path=\'path_to/python_module.py\')\nprint(parsed_output)\n```\n',
     'author': 'Iuliia Volkova',
     'author_email': 'xnuinside@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/xnuinside/py-module-parser',
```

### Comparing `py-module-parser-0.2.0/PKG-INFO` & `py-module-parser-0.2.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-module-parser
-Version: 0.2.0
+Version: 0.2.0b0
 Summary: Python Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code.
 Home-page: https://github.com/xnuinside/py-module-parser
 License: MIT
 Author: Iuliia Volkova
 Author-email: xnuinside@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

