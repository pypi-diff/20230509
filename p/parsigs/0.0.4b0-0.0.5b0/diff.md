# Comparing `tmp/parsigs-0.0.4b0.tar.gz` & `tmp/parsigs-0.0.5b0.tar.gz`

## Comparing `parsigs-0.0.4b0.tar` & `parsigs-0.0.5b0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/contributing.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/playground.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/requirements.txt
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/.github/workflows/starter-workflow.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/parsigs/__init__.py
--rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/parsigs/parse_sig_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/research/__init__.py
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/research/dosage_instructions_ner.ipynb
--rw-r--r--   0        0        0    10695 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/research/dosage_instructions_ner_bert.ipynb
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/research/pre_process_data.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/research/config/config.cfg
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/research/config/config_bert.cfg
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/research/config/config_compact_bert.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/tests/__init__.py
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/tests/test_parsig_api.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/LICENSE
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/README.md
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/pyproject.toml
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 parsigs-0.0.4b0/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/contributing.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/playground.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/requirements.txt
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/.github/workflows/starter-workflow.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/parsigs/__init__.py
+-rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/parsigs/parse_sig_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/research/__init__.py
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/research/dosage_instructions_ner.ipynb
+-rw-r--r--   0        0        0    10695 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/research/dosage_instructions_ner_bert.ipynb
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/research/pre_process_data.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/research/config/config.cfg
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/research/config/config_bert.cfg
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/research/config/config_compact_bert.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/tests/__init__.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/tests/test_parsig_api.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/LICENSE
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/README.md
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/pyproject.toml
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 parsigs-0.0.5b0/PKG-INFO
```

### Comparing `parsigs-0.0.4b0/.github/workflows/starter-workflow.yaml` & `parsigs-0.0.5b0/.github/workflows/starter-workflow.yaml`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.4b0/parsigs/parse_sig_api.py` & `parsigs-0.0.5b0/parsigs/parse_sig_api.py`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.4b0/research/dosage_instructions_ner.ipynb` & `parsigs-0.0.5b0/research/dosage_instructions_ner.ipynb`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.4b0/research/dosage_instructions_ner_bert.ipynb` & `parsigs-0.0.5b0/research/dosage_instructions_ner_bert.ipynb`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.4b0/research/pre_process_data.py` & `parsigs-0.0.5b0/research/pre_process_data.py`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.4b0/research/config/config.cfg` & `parsigs-0.0.5b0/research/config/config.cfg`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.4b0/research/config/config_bert.cfg` & `parsigs-0.0.5b0/research/config/config_bert.cfg`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.4b0/research/config/config_compact_bert.cfg` & `parsigs-0.0.5b0/research/config/config_compact_bert.cfg`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.4b0/tests/test_parsig_api.py` & `parsigs-0.0.5b0/tests/test_parsig_api.py`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.4b0/.gitignore` & `parsigs-0.0.5b0/.gitignore`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.4b0/LICENSE` & `parsigs-0.0.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.4b0/README.md` & `parsigs-0.0.5b0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 ## Installation
 For optimal usage, you will need to install the `parsigs` package and the underlying model
 (you can provide a different one by yourself, but this is not 
 recommended as the model was trained for the specific task of parsing dosage instructions from Sigs)
 ```
 pip install parsigs
-pip install https://huggingface.co/royashcenazi/en_parsigs/resolve/main/en_parsigs-any-py3-none-any.whl
 ```
 
 
 ## Usage
 Here are some examples of how to use the parse_sig method:
```

### Comparing `parsigs-0.0.4b0/pyproject.toml` & `parsigs-0.0.5b0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "parsigs"
-version = "0.0.4_beta"
+version = "0.0.5_beta"
 authors = [
     { name = "Roy Ashcenazi", email = "royashcenazi@gmail.com" },
 ]
 description = "The private, smart and easy Sig (Dosage Instructions) text-parser"
 readme = "README.md"
+
 [tool.hatch.metadata]
 allow-direct-references = true
-dependencies = [
-    "spacy>=3.0,<4.0",
-    "word2number",
-    "en-parsigs @ https://huggingface.co/royashcenazi/en_parsigs/resolve/main/en_parsigs-any-py3-none-any.whl"
-]
+
+#dependencies = [
+#    "spacy>=3.0,<4.0",
+#    "word2number",
+#    "en-parsigs @ https://huggingface.co/royashcenazi/en_parsigs/resolve/main/en_parsigs-any-py3-none-any.whl"
+#]
+
+dynamic = ["dependencies"]
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
 
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `parsigs-0.0.4b0/PKG-INFO` & `parsigs-0.0.5b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsigs
-Version: 0.0.4b0
+Version: 0.0.5b0
 Summary: The private, smart and easy Sig (Dosage Instructions) text-parser
 Project-URL: Homepage, https://github.com/royashcenazi/parsigs
 Project-URL: Bug Tracker, https://github.com/royashcenazi/parsigs/issues
 Author-email: Roy Ashcenazi <royashcenazi@gmail.com>
 License-File: LICENSE
 Description-Content-Type: text/markdown
 
@@ -21,15 +21,14 @@
 
 ## Installation
 For optimal usage, you will need to install the `parsigs` package and the underlying model
 (you can provide a different one by yourself, but this is not 
 recommended as the model was trained for the specific task of parsing dosage instructions from Sigs)
 ```
 pip install parsigs
-pip install https://huggingface.co/royashcenazi/en_parsigs/resolve/main/en_parsigs-any-py3-none-any.whl
 ```
 
 
 ## Usage
 Here are some examples of how to use the parse_sig method:
```

