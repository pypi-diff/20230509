# Comparing `tmp/review-bot-0.0.dev3.tar.gz` & `tmp/review-bot-0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "review-bot-0.0.dev3.tar", last modified: Mon Apr 17 09:58:52 2023, max compression
+gzip compressed data, was "review-bot-0.0.dev4.tar", last modified: Tue May  9 07:58:33 2023, max compression
```

## Comparing `review-bot-0.0.dev3.tar` & `review-bot-0.0.dev4.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1089 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/LICENSE
--rw-r--r--   0        0        0     2929 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/README.rst
--rw-r--r--   0        0        0     1710 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/pyproject.toml
--rw-r--r--   0        0        0      298 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/src/review_bot/__init__.py
--rw-r--r--   0        0        0     3717 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/src/review_bot/gh_interface.py
--rw-r--r--   0        0        0     4864 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/src/review_bot/misc.py
--rw-r--r--   0        0        0     8120 2023-04-17 09:58:38.234545 review-bot-0.0.dev3/src/review_bot/open_ai_interface.py
--rw-r--r--   0        0        0     4321 1970-01-01 00:00:00.000000 review-bot-0.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-09 07:58:17.863319 review-bot-0.0.dev4/LICENSE
+-rw-r--r--   0        0        0     2929 2023-05-09 07:58:17.863319 review-bot-0.0.dev4/README.rst
+-rw-r--r--   0        0        0     1755 2023-05-09 07:58:17.863319 review-bot-0.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0      298 2023-05-09 07:58:17.863319 review-bot-0.0.dev4/src/review_bot/__init__.py
+-rw-r--r--   0        0        0     3717 2023-05-09 07:58:17.863319 review-bot-0.0.dev4/src/review_bot/gh_interface.py
+-rw-r--r--   0        0        0     4950 2023-05-09 07:58:17.863319 review-bot-0.0.dev4/src/review_bot/misc.py
+-rw-r--r--   0        0        0     8120 2023-05-09 07:58:17.863319 review-bot-0.0.dev4/src/review_bot/open_ai_interface.py
+-rw-r--r--   0        0        0       78 2023-05-09 07:58:17.863319 review-bot-0.0.dev4/src/review_bot/schema/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-09 07:58:17.867319 review-bot-0.0.dev4/src/review_bot/schema/resources/schema.json
+-rw-r--r--   0        0        0      770 2023-05-09 07:58:17.867319 review-bot-0.0.dev4/src/review_bot/schema/schema.py
+-rw-r--r--   0        0        0     4401 1970-01-01 00:00:00.000000 review-bot-0.0.dev4/PKG-INFO
```

### Comparing `review-bot-0.0.dev3/LICENSE` & `review-bot-0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `review-bot-0.0.dev3/README.rst` & `review-bot-0.0.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `review-bot-0.0.dev3/pyproject.toml` & `review-bot-0.0.dev4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "review-bot"
-version = "0.0.dev3"
+version = "0.0.dev4"
 description = "A python library to automatically generate suggestions and improvements for patches in GitHub PRs by leveraging the power of OpenAI."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -23,29 +23,31 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "importlib-metadata>=4.0,<5; python_version<='3.8'",
     "requests",
     "openai",
+    "jsonschema",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "pytest==7.2.2",
+    "pytest==7.3.1",
     "pytest-cov==4.0.0",
-    "requests==2.28.2",
-    "openai==0.27.2",
+    "pytest-retry==1.2.1",
+    "requests==2.30.0",
+    "openai==0.27.6",
 ]
 doc = [
-    "ansys_sphinx_theme==0.9.6",
+    "ansys_sphinx_theme==0.9.8",
     "numpydoc==1.5.0",
-    "Sphinx==5.3.0",
+    "Sphinx==7.0.0",
     "sphinx-autoapi==2.1.0",
-    "Sphinx-copybutton==0.5.1",
+    "Sphinx-copybutton==0.5.2",
 ]
 
 
 [tool.flit.module]
 name = "review_bot"
 
 [project.urls]
```

### Comparing `review-bot-0.0.dev3/src/review_bot/gh_interface.py` & `review-bot-0.0.dev4/src/review_bot/gh_interface.py`

 * *Files identical despite different names*

### Comparing `review-bot-0.0.dev3/src/review_bot/misc.py` & `review-bot-0.0.dev4/src/review_bot/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import logging
 import os
 import re
 from typing import Dict, List
 
 import openai
 
+from review_bot.schema import validate_output
+
 LOG = logging.getLogger(__name__)
 LOG.setLevel("DEBUG")
 
 
 def _get_gh_token():
     """Return the github access token from the GITHUB_TOKEN environment variable."""
     access_token = os.environ.get("GITHUB_TOKEN")
@@ -164,9 +166,9 @@
         suggestion = {
             "filename": match.group(1),
             "lines": match.group(2),
             "type": match.group(3),
             "text": match.group(4),
         }
         suggestions.append(suggestion)
-
+    validate_output(output=suggestions)
     return suggestions
```

### Comparing `review-bot-0.0.dev3/src/review_bot/open_ai_interface.py` & `review-bot-0.0.dev4/src/review_bot/open_ai_interface.py`

 * *Files identical despite different names*

### Comparing `review-bot-0.0.dev3/PKG-INFO` & `review-bot-0.0.dev4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: review-bot
-Version: 0.0.dev3
+Version: 0.0.dev4
 Summary: A python library to automatically generate suggestions and improvements for patches in GitHub PRs by leveraging the power of OpenAI.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.core@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: importlib-metadata>=4.0,<5; python_version<='3.8'
 Requires-Dist: requests
 Requires-Dist: openai
-Requires-Dist: ansys_sphinx_theme==0.9.6 ; extra == "doc"
+Requires-Dist: jsonschema
+Requires-Dist: ansys_sphinx_theme==0.9.8 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
+Requires-Dist: Sphinx==7.0.0 ; extra == "doc"
 Requires-Dist: sphinx-autoapi==2.1.0 ; extra == "doc"
-Requires-Dist: Sphinx-copybutton==0.5.1 ; extra == "doc"
-Requires-Dist: pytest==7.2.2 ; extra == "tests"
+Requires-Dist: Sphinx-copybutton==0.5.2 ; extra == "doc"
+Requires-Dist: pytest==7.3.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
-Requires-Dist: requests==2.28.2 ; extra == "tests"
-Requires-Dist: openai==0.27.2 ; extra == "tests"
+Requires-Dist: pytest-retry==1.2.1 ; extra == "tests"
+Requires-Dist: requests==2.30.0 ; extra == "tests"
+Requires-Dist: openai==0.27.6 ; extra == "tests"
 Project-URL: Homepage, https://github.com/ansys/hackathon-review-bot
 Project-URL: Source, https://github.com/ansys/hackathon-review-bot
 Project-URL: Tracker, https://github.com/ansys/hackathon-review-bot/issues
 Provides-Extra: doc
 Provides-Extra: tests
 
 Ansys Hackathon - Review bot
```

