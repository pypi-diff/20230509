# Comparing `tmp/struct_gpt-2.2.4.tar.gz` & `tmp/struct_gpt-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-2.2.4.tar", last modified: Mon May  8 21:28:04 2023, max compression
+gzip compressed data, was "struct_gpt-2.2.5.tar", last modified: Tue May  9 01:26:13 2023, max compression
```

## Comparing `struct_gpt-2.2.4.tar` & `struct_gpt-2.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-05-08 21:27:23.990857 struct_gpt-2.2.4/LICENSE
--rw-r--r--   0        0        0     3724 2023-05-08 21:27:23.990857 struct_gpt-2.2.4/README.md
--rw-r--r--   0        0        0      587 2023-05-08 21:28:04.103487 struct_gpt-2.2.4/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-08 21:27:23.990857 struct_gpt-2.2.4/struct_gpt/__init__.py
--rw-r--r--   0        0        0     4909 2023-05-08 21:27:23.994857 struct_gpt-2.2.4/struct_gpt/models.py
--rw-r--r--   0        0        0     6096 2023-05-08 21:27:23.994857 struct_gpt-2.2.4/tests/test_models.py
--rw-r--r--   0        0        0     5345 1970-01-01 00:00:00.000000 struct_gpt-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-09 01:25:31.509113 struct_gpt-2.2.5/LICENSE
+-rw-r--r--   0        0        0     3729 2023-05-09 01:25:31.509113 struct_gpt-2.2.5/README.md
+-rw-r--r--   0        0        0      587 2023-05-09 01:26:13.473596 struct_gpt-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-09 01:25:31.509113 struct_gpt-2.2.5/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     4909 2023-05-09 01:25:31.509113 struct_gpt-2.2.5/struct_gpt/models.py
+-rw-r--r--   0        0        0     6096 2023-05-09 01:25:31.513113 struct_gpt-2.2.5/tests/test_models.py
+-rw-r--r--   0        0        0     5350 1970-01-01 00:00:00.000000 struct_gpt-2.2.5/PKG-INFO
```

### Comparing `struct_gpt-2.2.4/LICENSE` & `struct_gpt-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.4/README.md` & `struct_gpt-2.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 }
 ```
 
 </details>
 
 ### Improving reliability with examples
 
-`create` can accept a list of examples to guide the model and improve its accuracy. 
+`from_openai` can accept a list of examples to guide the model and improve its accuracy. 
 
 Each example is a dictionary containing an `input` and `output` key. 
 
 `output` should be an instance of the model, a dictionary, or its json string representation,.
 
 ```python
 from struct_gpt import OpenAiBase
```

### Comparing `struct_gpt-2.2.4/pyproject.toml` & `struct_gpt-2.2.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dev = [
     "pytest>=7.3.1",
     "coverage>=7.2.5",
 ]
 
 [project]
 name = "struct-gpt"
-version = "2.2.4"
+version = "2.2.5"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-2.2.4/struct_gpt/models.py` & `struct_gpt-2.2.5/struct_gpt/models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.4/tests/test_models.py` & `struct_gpt-2.2.5/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.4/PKG-INFO` & `struct_gpt-2.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 2.2.4
+Version: 2.2.5
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Stephan Fitzpatrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -167,15 +167,15 @@
 }
 ```
 
 </details>
 
 ### Improving reliability with examples
 
-`create` can accept a list of examples to guide the model and improve its accuracy. 
+`from_openai` can accept a list of examples to guide the model and improve its accuracy. 
 
 Each example is a dictionary containing an `input` and `output` key. 
 
 `output` should be an instance of the model, a dictionary, or its json string representation,.
 
 ```python
 from struct_gpt import OpenAiBase
```

