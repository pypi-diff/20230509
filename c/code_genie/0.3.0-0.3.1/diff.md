# Comparing `tmp/code_genie-0.3.0.tar.gz` & `tmp/code_genie-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_genie-0.3.0.tar", last modified: Fri May  5 05:32:51 2023, max compression
+gzip compressed data, was "code_genie-0.3.1.tar", last modified: Tue May  9 06:30:34 2023, max compression
```

## Comparing `code_genie-0.3.0.tar` & `code_genie-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,44 @@
--rw-r--r--   0        0        0      399 2023-05-05 05:32:36.162791 code_genie-0.3.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1871 2023-04-29 16:20:39.492906 code_genie-0.3.0/.gitignore
--rw-r--r--   0        0        0      635 2023-04-27 10:15:39.147415 code_genie-0.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0      448 2023-05-05 05:32:36.163481 code_genie-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-04-20 10:01:19.112941 code_genie-0.3.0/LICENSE
--rw-r--r--   0        0        0     1549 2023-05-05 05:32:36.164274 code_genie-0.3.0/README.md
--rw-r--r--   0        0        0      484 2023-04-30 09:58:38.245553 code_genie-0.3.0/TODO.md
--rw-r--r--   0        0        0      102 2023-05-05 05:32:36.165170 code_genie-0.3.0/code_genie/__init__.py
--rw-r--r--   0        0        0     3431 2023-05-05 05:32:36.166104 code_genie-0.3.0/code_genie/_cache.py
--rw-r--r--   0        0        0     1678 2023-04-29 16:20:39.496137 code_genie-0.3.0/code_genie/client.py
--rw-r--r--   0        0        0     5723 2023-05-05 05:32:36.166922 code_genie-0.3.0/code_genie/genie.py
--rw-r--r--   0        0        0      679 2023-04-27 10:15:39.149821 code_genie-0.3.0/docs/Makefile
--rw-r--r--   0        0        0       47 2023-05-05 05:32:36.167856 code_genie-0.3.0/docs/api.rst
--rw-r--r--   0        0        0     1492 2023-04-27 10:15:39.151752 code_genie-0.3.0/docs/conf.py
--rw-r--r--   0        0        0       81 2023-04-27 10:15:39.152197 code_genie-0.3.0/docs/examples.rst
--rw-r--r--   0        0        0      284 2023-04-27 10:15:39.153008 code_genie-0.3.0/docs/generated/code_genie.client.rst
--rw-r--r--   0        0        0      226 2023-04-27 10:15:39.153533 code_genie-0.3.0/docs/generated/code_genie.genie.rst
--rw-r--r--   0        0        0     1154 2023-05-05 05:32:36.168709 code_genie-0.3.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-04-27 10:15:39.155023 code_genie-0.3.0/docs/make.bat
--rw-r--r--   0        0        0    64979 2023-05-05 05:32:36.170025 code_genie-0.3.0/docs/notebooks/Starter.ipynb
--rw-r--r--   0        0        0     1320 2023-05-05 05:32:36.171160 code_genie-0.3.0/docs/notebooks/_cache_starter/_meta.json
--rw-r--r--   0        0        0      377 2023-05-05 05:32:36.171751 code_genie-0.3.0/docs/notebooks/_cache_starter/count_missing_values_57234.py
--rw-r--r--   0        0        0      491 2023-05-05 05:32:36.172371 code_genie-0.3.0/docs/notebooks/_cache_starter/generate_employee_dataframe_16305.py
--rw-r--r--   0        0        0      125 2023-05-05 05:32:36.172714 code_genie-0.3.0/docs/notebooks/_cache_starter/high_earners_26869.py
--rw-r--r--   0        0        0      224 2023-05-05 05:32:36.173103 code_genie-0.3.0/docs/notebooks/_cache_starter/plot_salary_by_department_20090.py
--rw-r--r--   0        0        0      372 2023-05-05 05:32:36.173421 code_genie-0.3.0/docs/notebooks/_cache_starter/plot_salary_distribution_88606.py
--rw-r--r--   0        0        0       54 2023-04-27 10:15:39.156660 code_genie-0.3.0/docs/requirements.in
--rw-r--r--   0        0        0     3100 2023-04-27 10:15:39.156993 code_genie-0.3.0/docs/requirements.txt
--rw-r--r--   0        0        0     1245 2023-05-05 05:32:36.173897 code_genie-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 05:29:52.448133 code_genie-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      475 2023-04-29 16:20:39.501753 code_genie-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1176 2023-05-05 05:32:36.174627 code_genie-0.3.0/tests/test_genie.py
--rw-r--r--   0        0        0      839 2023-04-29 16:20:39.503091 code_genie-0.3.0/tox.ini
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 code_genie-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      399 2023-05-09 06:30:31.767724 code_genie-0.3.1/.bumpversion.cfg
+-rw-r--r--   0        0        0     1871 2023-05-09 06:20:04.190479 code_genie-0.3.1/.gitignore
+-rw-r--r--   0        0        0      635 2023-04-27 10:15:39.147415 code_genie-0.3.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      878 2023-05-09 06:30:31.768052 code_genie-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-04-20 10:01:19.112941 code_genie-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1549 2023-05-09 06:30:31.768370 code_genie-0.3.1/README.md
+-rw-r--r--   0        0        0      462 2023-05-09 06:30:31.769017 code_genie-0.3.1/TODO.md
+-rw-r--r--   0        0        0      102 2023-05-09 06:30:31.769437 code_genie-0.3.1/code_genie/__init__.py
+-rw-r--r--   0        0        0     3745 2023-05-09 06:30:31.770103 code_genie-0.3.1/code_genie/_cache.py
+-rw-r--r--   0        0        0     1487 2023-05-09 06:30:31.770784 code_genie-0.3.1/code_genie/client.py
+-rw-r--r--   0        0        0     7585 2023-05-09 06:30:31.771456 code_genie-0.3.1/code_genie/genie.py
+-rw-r--r--   0        0        0      679 2023-04-27 10:15:39.149821 code_genie-0.3.1/docs/Makefile
+-rw-r--r--   0        0        0      179 2023-05-09 06:30:31.772166 code_genie-0.3.1/docs/api.rst
+-rw-r--r--   0        0        0     1466 2023-05-09 06:30:31.772894 code_genie-0.3.1/docs/conf.py
+-rw-r--r--   0        0        0       81 2023-04-27 10:15:39.152197 code_genie-0.3.1/docs/examples.rst
+-rw-r--r--   0        0        0      284 2023-04-27 10:15:39.153008 code_genie-0.3.1/docs/generated/code_genie.client.rst
+-rw-r--r--   0        0        0      226 2023-04-27 10:15:39.153533 code_genie-0.3.1/docs/generated/code_genie.genie.rst
+-rw-r--r--   0        0        0     1758 2023-05-09 06:30:31.773394 code_genie-0.3.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-04-27 10:15:39.155023 code_genie-0.3.1/docs/make.bat
+-rw-r--r--   0        0        0       33 2023-05-09 06:30:31.773933 code_genie-0.3.1/docs/notebooks/.env.example
+-rw-r--r--   0        0        0   571332 2023-05-09 06:30:31.780435 code_genie-0.3.1/docs/notebooks/Starter.ipynb
+-rw-r--r--   0        0        0    12619 2023-05-09 06:30:31.783305 code_genie-0.3.1/docs/notebooks/_cache_starter/_meta.json
+-rw-r--r--   0        0        0      116 2023-05-09 06:30:31.784178 code_genie-0.3.1/docs/notebooks/_cache_starter/count_job_designations_83350.py
+-rw-r--r--   0        0        0       80 2023-05-09 06:30:31.784950 code_genie-0.3.1/docs/notebooks/_cache_starter/count_missing_values_26226.py
+-rw-r--r--   0        0        0      102 2023-05-09 06:30:31.785776 code_genie-0.3.1/docs/notebooks/_cache_starter/create_boxplot_24032.py
+-rw-r--r--   0        0        0      534 2023-05-09 06:30:31.786373 code_genie-0.3.1/docs/notebooks/_cache_starter/make_wordcloud_51022.py
+-rw-r--r--   0        0        0      291 2023-05-09 06:30:31.786954 code_genie-0.3.1/docs/notebooks/_cache_starter/map_experience_level_48687.py
+-rw-r--r--   0        0        0      186 2023-05-09 06:30:31.787739 code_genie-0.3.1/docs/notebooks/_cache_starter/pie_chart_47446.py
+-rw-r--r--   0        0        0      483 2023-05-09 06:30:31.788269 code_genie-0.3.1/docs/notebooks/_cache_starter/plot_emp_type_experience_level_31165.py
+-rw-r--r--   0        0        0      165 2023-05-09 06:30:31.789011 code_genie-0.3.1/docs/notebooks/_cache_starter/plot_salary_distribution_51861.py
+-rw-r--r--   0        0        0      173 2023-05-09 06:30:31.789633 code_genie-0.3.1/docs/notebooks/_cache_starter/process_dataframe_88292.py
+-rw-r--r--   0        0        0     1504 2023-05-09 06:30:31.790070 code_genie-0.3.1/docs/notebooks/_cache_starter/remote_ratio_by_work_years_96078.py
+-rw-r--r--   0        0        0      177 2023-05-09 06:30:31.790441 code_genie-0.3.1/docs/notebooks/_cache_starter/remote_ratio_mapper_69067.py
+-rw-r--r--   0        0        0      403 2023-05-09 06:30:31.790823 code_genie-0.3.1/docs/notebooks/_cache_starter/top_jobs_41202.py
+-rw-r--r--   0        0        0      145 2023-05-09 06:30:31.791299 code_genie-0.3.1/docs/notebooks/_cache_starter/unique_experience_count_96626.py
+-rw-r--r--   0        0        0       81 2023-05-09 06:30:31.791662 code_genie-0.3.1/docs/notebooks/_cache_starter/unique_remote_ratio_counts_63145.py
+-rw-r--r--   0        0        0       54 2023-04-27 10:15:39.156660 code_genie-0.3.1/docs/requirements.in
+-rw-r--r--   0        0        0     3100 2023-04-27 10:15:39.156993 code_genie-0.3.1/docs/requirements.txt
+-rw-r--r--   0        0        0     1327 2023-05-09 06:30:31.792425 code_genie-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 05:29:52.448133 code_genie-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      475 2023-04-29 16:20:39.501753 code_genie-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     1893 2023-05-09 06:30:31.793290 code_genie-0.3.1/tests/test_genie.py
+-rw-r--r--   0        0        0      863 2023-05-09 06:30:31.794175 code_genie-0.3.1/tox.ini
+-rw-r--r--   0        0        0     3222 1970-01-01 00:00:00.000000 code_genie-0.3.1/PKG-INFO
```

### Comparing `code_genie-0.3.0/.gitignore` & `code_genie-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `code_genie-0.3.0/.readthedocs.yaml` & `code_genie-0.3.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `code_genie-0.3.0/LICENSE` & `code_genie-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `code_genie-0.3.0/README.md` & `code_genie-0.3.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # code-genie
 This library is your copilot for jupyter notebooks
 
-Latest version: 0.3.0
+Latest version: 0.3.1
 
 ## Documentation
 
 - [Starter Notebook](https://code-genie.readthedocs.io/en/main/notebooks/Starter.html)
 - [All Examples](https://code-genie.readthedocs.io/en/main/examples.html)
 - [API Documentation](https://code-genie.readthedocs.io/en/main/api.html)
```

### Comparing `code_genie-0.3.0/code_genie/_cache.py` & `code_genie-0.3.1/code_genie/_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import json
 import logging
 import os
 from hashlib import blake2b
 from tempfile import mkdtemp
-from typing import Dict, Optional
+from typing import Dict, List, Optional
 
 from pydantic import BaseModel
 
 logger = logging.getLogger(__name__)
 
 
 class _MetaValue(BaseModel):
     id: str
     fn_name: str
+    instructions: List[str]
+    inputs: List[str]
 
     class Config:
         frozen = True
 
     def toJson(self):
         return json.dumps(self, default=lambda o: o.__dict__)
 
@@ -86,31 +88,38 @@
 
     def update(self, key: str, value: _CacheValue):
         _cache_meta = self._load_meta()
         key_hash = self._consistent_hash(key)
 
         # if key is present in, delete the file which is currently cashed
         if key_hash in _cache_meta:
-            os.remove(self._get_filename(_cache_meta[key_hash].id))
+            filename = self._get_filename(_cache_meta[key_hash].id)
+            if os.path.exists(filename):
+                os.remove(filename)
 
         # add new cash entry
         _cache_meta[key_hash] = value
         # write to code file
         with open(self._get_filename(value.id), "w") as f:
             f.write(value.code)
         # update metadata
         with open(self.meta_path, "w") as f:
             json.dump(_cache_meta, f, indent=4, default=self._json_encoder)
 
     def get(self, key: str) -> Optional[_CacheValue]:
         _cache_meta = self._load_meta()
         meta = _cache_meta.get(self._consistent_hash(key), None)
         if meta is not None:
-            code = self._load_code(meta.id)
-            return _CacheValue(code=code, id=meta.id, fn_name=meta.fn_name)
+            try:
+                code = self._load_code(meta.id)
+                return _CacheValue(
+                    code=code, id=meta.id, fn_name=meta.fn_name, instructions=meta.instructions, inputs=meta.inputs
+                )
+            except FileNotFoundError:
+                return None
         return None
 
     def num_items(self):
         return len(self._load_meta())
 
     def get_all_code_segments(self) -> Dict[str, str]:
         _cache_meta = self._load_meta()
```

### Comparing `code_genie-0.3.0/code_genie/client.py` & `code_genie-0.3.1/code_genie/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,29 +22,24 @@
     code: str
     fn_name: str
 
 
 class Client:
     TOKEN_ENV_VAR = "CODE_GENIE_TOKEN"
     URL = "https://code-scribe-pzj44qvhfa-el.a.run.app"
-    ENDPOINT_GENERIC = "get-executable/generic"
-    ENDPOINT_PANDAS = "get-executable/pandas"
+    ENDPOINT = "get-executable/generic"
 
     def __init__(self, token: Optional[str] = None):
         self._token = token or os.environ[self.TOKEN_ENV_VAR]
 
     def _get_response(self, endpoint, data):
         headers = {"token": self._token, "Content-Type": "application/json"}
         response = requests.post(url=f"{self.URL}/{endpoint}", data=data.json(), headers=headers)
         # if error found, raise the error
         response.raise_for_status()
         return GetExecutableResponse.parse_obj(response.json())
 
-    def get_generic(self, request: GetExecutableRequest) -> Tuple[str, str]:
+    def get(self, instructions: List[str], inputs: Dict[str, str]) -> Tuple[str, str]:
+        request = GetExecutableRequest(instructions=instructions, inputs=inputs, allowed_imports=[])
         # send a request with given data
-        response = self._get_response(self.ENDPOINT_GENERIC, request)
-        return response.code, response.fn_name
-
-    def get_pandas(self, request: GetPandasExecutableRequest) -> Tuple[str, str]:
-        # send a request with given data
-        response = self._get_response(self.ENDPOINT_PANDAS, request)
+        response = self._get_response(self.ENDPOINT, request)
         return response.code, response.fn_name
```

### Comparing `code_genie-0.3.0/docs/Makefile` & `code_genie-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `code_genie-0.3.0/docs/conf.py` & `code_genie-0.3.1/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,27 +19,25 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.napoleon',
               'sphinx.ext.autodoc',
               'sphinx.ext.viewcode',
               'sphinx.ext.autosummary',
               "nbsphinx",
-              "sphinx_gallery.load_style"]
+              "sphinx_gallery.load_style",
+              "sphinxcontrib.autodoc_pydantic"]
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-autodoc_default_options = {
-    'members': True,
-    'member-order': 'bysource',
-    'special-members': '__init__',
-    'exclude-members': '__weakref__',
-    'inherited-members': True,
-}
 
 # Napoleon settings
 napoleon_google_docstring = True
 napoleon_numpy_docstring = False
 
+# autodoc-pydantic settings
+autodoc_pydantic_model_show_json = False
+autodoc_pydantic_model_show_config = False
+
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'sphinx_rtd_theme'
 html_static_path = ['_static']
```

### Comparing `code_genie-0.3.0/docs/index.rst` & `code_genie-0.3.1/docs/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -16,27 +16,38 @@
 
 code-genie will help you bring the power of chatGPT technology to your notebooks.
 
 Look how easy it is to use::
 
    from code_genie import Genie
    df = load_your_df()
-   genie = Genie(inputs={"df": df})
-   df_missing = genie.plz("create a dataframe with number of missing values per column")
-   genie.plz("make scatter plot of col1 vs col2")
+   genie = Genie(data=df)
+   gr_miss = genie.plz("create a dataframe with number of missing values per column")
+   gr_miss.result  # show the result of computation
+   print(gr_miss.code)  # print the code which was generated
+   genie.plz("make scatter plot of col1 vs col2").result  # directly make the plot without storing into interim variable
 
-Find more examples in the `examples` folder.
+Get started with this `notebook`_.
+
+.. _notebook: https://nbviewer.org/github/thismlguy/code-genie/blob/main/docs/notebooks/Starter.ipynb
 
 Installation
 ------------
 
 Install code-genie by running:
 
 ``pip install code_genie``
 
+
+Note on Privacy & Security
+------------
+Privacy of your data is of primte importance. This library has been specifically designed to NOT share any part of your data with the Genie APIs.
+Just the metadata about your data like name and types of columns of a pandas dataframe would be shared, which help in generating high quality results.
+
+
 Features
 --------
 
 - Create functions from text and re-use them as you want
 - No more spending hours searching for syntax on stack overflow
 
 Contribute
```

### Comparing `code_genie-0.3.0/docs/make.bat` & `code_genie-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `code_genie-0.3.0/docs/requirements.txt` & `code_genie-0.3.1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `code_genie-0.3.0/pyproject.toml` & `code_genie-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -39,19 +39,22 @@
     "bumpversion"
 ]
 docs = [
     "sphinx==5.3.0",
     "autodocsumm",
     "sphinx_rtd_theme",
     "nbsphinx",
-    "sphinx_gallery"
+    "sphinx_gallery",
+    "autodoc-pydantic"
 ]
 notebook = [
     "jupyterlab>=3.1,<4",
     "ipykernel>=6.0,<7",
+    "opendatasets>=0.1.22,<0.2",
+    "wordcloud>=1.8,<2",
 ]
 
 [project.urls]
 Documentation = "https://code-genie.readthedocs.io/en/latest/"
 Source = "https://github.com/thismlguy/code-genie"
 
 [tool.flit.sdist]
```

### Comparing `code_genie-0.3.0/tox.ini` & `code_genie-0.3.1/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 [testenv:check-format]
 basepython = python3.7
 deps =
     black
     isort
 skip_install = true
 commands =
-    isort code_genie -c --diff  --line-length 120
-    black code_genie --line-length 120 --diff --check
+    isort code_genie tests -c --diff  --line-length 120
+    black code_genie tests --line-length 120 --diff --check
 
 [testenv:format]
 basepython = python3.7
 deps =
     black
     isort
 skip_install = true
 commands =
-    isort code_genie  --line-length 120
-    black code_genie --line-length 120
+    isort code_genie tests  --line-length 120
+    black code_genie tests --line-length 120
 
 [flake8]
 show-source = true
 max-line-length = 120
 exclude = .tox,.git,dist,doc,*.egg,build
 
 [isort]
```

### Comparing `code_genie-0.3.0/PKG-INFO` & `code_genie-0.3.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code_genie
-Version: 0.3.0
+Version: 0.3.1
 Summary: Copilot to supercharge your notebooks
 Keywords: copilot,jupyter
 Author-email: Aarshay Jain <aarshay.jain@columbia.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,26 +24,29 @@
 Requires-Dist: pip-tools ; extra == "build"
 Requires-Dist: bumpversion ; extra == "build"
 Requires-Dist: sphinx==5.3.0 ; extra == "docs"
 Requires-Dist: autodocsumm ; extra == "docs"
 Requires-Dist: sphinx_rtd_theme ; extra == "docs"
 Requires-Dist: nbsphinx ; extra == "docs"
 Requires-Dist: sphinx_gallery ; extra == "docs"
+Requires-Dist: autodoc-pydantic ; extra == "docs"
 Requires-Dist: jupyterlab>=3.1,<4 ; extra == "notebook"
 Requires-Dist: ipykernel>=6.0,<7 ; extra == "notebook"
+Requires-Dist: opendatasets>=0.1.22,<0.2 ; extra == "notebook"
+Requires-Dist: wordcloud>=1.8,<2 ; extra == "notebook"
 Project-URL: Documentation, https://code-genie.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/thismlguy/code-genie
 Provides-Extra: build
 Provides-Extra: docs
 Provides-Extra: notebook
 
 # code-genie
 This library is your copilot for jupyter notebooks
 
-Latest version: 0.3.0
+Latest version: 0.3.1
 
 ## Documentation
 
 - [Starter Notebook](https://code-genie.readthedocs.io/en/main/notebooks/Starter.html)
 - [All Examples](https://code-genie.readthedocs.io/en/main/examples.html)
 - [API Documentation](https://code-genie.readthedocs.io/en/main/api.html)
```

