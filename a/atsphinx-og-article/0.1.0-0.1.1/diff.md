# Comparing `tmp/atsphinx-og-article-0.1.0.tar.gz` & `tmp/atsphinx-og-article-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atsphinx-og-article-0.1.0.tar", last modified: Tue May  9 18:26:28 2023, max compression
+gzip compressed data, was "atsphinx-og-article-0.1.1.tar", last modified: Tue May  9 18:37:39 2023, max compression
```

## Comparing `atsphinx-og-article-0.1.0.tar` & `atsphinx-og-article-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      517 2023-05-09 18:26:24.593003 atsphinx-og-article-0.1.0/.editorconfig
--rw-r--r--   0        0        0     3338 2023-05-09 18:26:24.593003 atsphinx-og-article-0.1.0/.gitignore
--rw-r--r--   0        0        0      543 2023-05-09 18:26:24.593003 atsphinx-og-article-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      444 2023-05-09 18:26:24.593003 atsphinx-og-article-0.1.0/.readthedocs.yml
--rw-r--r--   0        0        0      298 2023-05-09 18:26:24.593003 atsphinx-og-article-0.1.0/CHANGES.rst
--rw-r--r--   0        0        0     9161 2023-05-09 18:26:24.593003 atsphinx-og-article-0.1.0/LICENSE
--rw-r--r--   0        0        0     1718 2023-05-09 18:26:24.593003 atsphinx-og-article-0.1.0/README.rst
--rw-r--r--   0        0        0      634 2023-05-09 18:26:24.593003 atsphinx-og-article-0.1.0/docs/Makefile
--rw-r--r--   0        0        0       14 2023-05-09 18:26:24.593003 atsphinx-og-article-0.1.0/docs/_static/.gitignore
--rw-r--r--   0        0        0       14 2023-05-09 18:26:24.593003 atsphinx-og-article-0.1.0/docs/_templates/.gitignore
--rw-r--r--   0        0        0      914 2023-05-09 18:26:24.597003 atsphinx-og-article-0.1.0/docs/conf.py
--rw-r--r--   0        0        0     1875 2023-05-09 18:26:24.597003 atsphinx-og-article-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-09 18:26:24.597003 atsphinx-og-article-0.1.0/docs/make.bat
--rw-r--r--   0        0        0     1057 2023-05-09 18:26:24.597003 atsphinx-og-article-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      364 2023-05-09 18:26:24.597003 atsphinx-og-article-0.1.0/setup.cfg
--rw-r--r--   0        0        0      919 2023-05-09 18:26:24.597003 atsphinx-og-article-0.1.0/src/atsphinx/og_article/__init__.py
--rw-r--r--   0        0        0     2021 2023-05-09 18:26:24.597003 atsphinx-og-article-0.1.0/src/atsphinx/og_article/models.py
--rw-r--r--   0        0        0     1233 2023-05-09 18:26:24.597003 atsphinx-og-article-0.1.0/src/atsphinx/og_article/processors.py
--rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 atsphinx-og-article-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      517 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/.editorconfig
+-rw-r--r--   0        0        0     3338 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/.gitignore
+-rw-r--r--   0        0        0      543 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      444 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/.readthedocs.yml
+-rw-r--r--   0        0        0      395 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/CHANGES.rst
+-rw-r--r--   0        0        0     9161 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1718 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/README.rst
+-rw-r--r--   0        0        0      634 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0       14 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/docs/_static/.gitignore
+-rw-r--r--   0        0        0       14 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/docs/_templates/.gitignore
+-rw-r--r--   0        0        0      914 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0     1875 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0     1130 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      364 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/setup.cfg
+-rw-r--r--   0        0        0      919 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/src/atsphinx/og_article/__init__.py
+-rw-r--r--   0        0        0     2021 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/src/atsphinx/og_article/models.py
+-rw-r--r--   0        0        0     1233 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/src/atsphinx/og_article/processors.py
+-rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 atsphinx-og-article-0.1.1/PKG-INFO
```

### Comparing `atsphinx-og-article-0.1.0/.editorconfig` & `atsphinx-og-article-0.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.0/.gitignore` & `atsphinx-og-article-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.0/.pre-commit-config.yaml` & `atsphinx-og-article-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.0/LICENSE` & `atsphinx-og-article-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.0/README.rst` & `atsphinx-og-article-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.0/docs/Makefile` & `atsphinx-og-article-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.0/docs/conf.py` & `atsphinx-og-article-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.0/docs/index.rst` & `atsphinx-og-article-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.0/docs/make.bat` & `atsphinx-og-article-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.0/pyproject.toml` & `atsphinx-og-article-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "atsphinx-og-article"
 authors = [{name = "Kazuya Takei", email = "myself@attakei.net"}]
 license = {file = "LICENSE"}
 classifiers = [
-  "Development Status :: 3 - Alpha",
+  "Development Status :: 4 - Beta",
   "Framework :: Sphinx",
   "Framework :: Sphinx :: Extension",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
@@ -33,14 +33,15 @@
 doc = [
   "furo",
   "rst-pypi-ref",
   "sphinx",
 ]
 
 [project.urls]
-Home = "https://github.com/atsphinx/og-article"
+Documentation = "https://atsphinx-og-article.readthedocs.io/en/stable/"
+Source = "https://github.com/atsphinx/og-article"
 
 [tool.flit.module]
 name = "atsphinx.og_article"
 
 [tool.flit.sdist]
 exclude = [".github", "tests"]
```

### Comparing `atsphinx-og-article-0.1.0/src/atsphinx/og_article/__init__.py` & `atsphinx-og-article-0.1.1/src/atsphinx/og_article/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Support article tpye's properties of Open Graph for Sphinx."""
 
 from docutils import nodes
 from sphinx.application import Sphinx
 
 from . import models, processors
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 
 def skip_node(self, node: models.og_article):
     """Minimum function to skip when builder visit it."""
     raise nodes.SkipNode()
```

### Comparing `atsphinx-og-article-0.1.0/src/atsphinx/og_article/models.py` & `atsphinx-og-article-0.1.1/src/atsphinx/og_article/models.py`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.0/src/atsphinx/og_article/processors.py` & `atsphinx-og-article-0.1.1/src/atsphinx/og_article/processors.py`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.0/PKG-INFO` & `atsphinx-og-article-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: atsphinx-og-article
-Version: 0.1.0
+Version: 0.1.1
 Summary: Support article tpye's properties of Open Graph for Sphinx.
 Author-email: Kazuya Takei <myself@attakei.net>
 Description-Content-Type: text/x-rst
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,15 +17,16 @@
 Requires-Dist: python-dateutil
 Requires-Dist: sphinx
 Requires-Dist: furo ; extra == "doc"
 Requires-Dist: rst-pypi-ref ; extra == "doc"
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: beautifulsoup4 == 4.* ; extra == "test"
 Requires-Dist: pytest ==7.* ; extra == "test"
-Project-URL: Home, https://github.com/atsphinx/og-article
+Project-URL: Documentation, https://atsphinx-og-article.readthedocs.io/en/stable/
+Project-URL: Source, https://github.com/atsphinx/og-article
 Provides-Extra: doc
 Provides-Extra: test
 
 ===================
 atsphinx-og-article
 ===================
```

