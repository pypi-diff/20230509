# Comparing `tmp/struct_gpt-2.2.5.tar.gz` & `tmp/struct_gpt-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-2.2.5.tar", last modified: Tue May  9 01:26:13 2023, max compression
+gzip compressed data, was "struct_gpt-2.2.6.tar", last modified: Tue May  9 01:28:39 2023, max compression
```

## Comparing `struct_gpt-2.2.5.tar` & `struct_gpt-2.2.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-05-09 01:25:31.509113 struct_gpt-2.2.5/LICENSE
--rw-r--r--   0        0        0     3729 2023-05-09 01:25:31.509113 struct_gpt-2.2.5/README.md
--rw-r--r--   0        0        0      587 2023-05-09 01:26:13.473596 struct_gpt-2.2.5/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-09 01:25:31.509113 struct_gpt-2.2.5/struct_gpt/__init__.py
--rw-r--r--   0        0        0     4909 2023-05-09 01:25:31.509113 struct_gpt-2.2.5/struct_gpt/models.py
--rw-r--r--   0        0        0     6096 2023-05-09 01:25:31.513113 struct_gpt-2.2.5/tests/test_models.py
--rw-r--r--   0        0        0     5350 1970-01-01 00:00:00.000000 struct_gpt-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-09 01:27:56.458064 struct_gpt-2.2.6/LICENSE
+-rw-r--r--   0        0        0     3729 2023-05-09 01:27:56.462062 struct_gpt-2.2.6/README.md
+-rw-r--r--   0        0        0      587 2023-05-09 01:28:39.262019 struct_gpt-2.2.6/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-09 01:27:56.462062 struct_gpt-2.2.6/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     4854 2023-05-09 01:27:56.462062 struct_gpt-2.2.6/struct_gpt/models.py
+-rw-r--r--   0        0        0     6096 2023-05-09 01:27:56.462062 struct_gpt-2.2.6/tests/test_models.py
+-rw-r--r--   0        0        0     5350 1970-01-01 00:00:00.000000 struct_gpt-2.2.6/PKG-INFO
```

### Comparing `struct_gpt-2.2.5/LICENSE` & `struct_gpt-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.5/README.md` & `struct_gpt-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.5/pyproject.toml` & `struct_gpt-2.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dev = [
     "pytest>=7.3.1",
     "coverage>=7.2.5",
 ]
 
 [project]
 name = "struct-gpt"
-version = "2.2.5"
+version = "2.2.6"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-2.2.5/struct_gpt/models.py` & `struct_gpt-2.2.6/struct_gpt/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import io
 import json
 import logging
-from pprint import pprint
 from typing import TypeVar, TypedDict
 
 import openai
 from pydantic import BaseModel, ValidationError
 from ruamel.yaml import YAML
 
 Model = TypeVar("Model", bound=BaseModel)
@@ -143,13 +142,12 @@
                 logger.error(error_msg)
                 messages.append(
                     {"role": "user", "content": f"{e.__class__.__name__}: {e}"}
                 )
                 attempt += 1
 
         if last_exception:
-            pprint(messages)
             raise last_exception
 
 
 class OpenAiBase(BaseModel, OpenAiMixin):
     ...
```

### Comparing `struct_gpt-2.2.5/tests/test_models.py` & `struct_gpt-2.2.6/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.5/PKG-INFO` & `struct_gpt-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 2.2.5
+Version: 2.2.6
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Stephan Fitzpatrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

