# Comparing `tmp/struct_gpt-2.2.6.tar.gz` & `tmp/struct_gpt-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-2.2.6.tar", last modified: Tue May  9 01:28:39 2023, max compression
+gzip compressed data, was "struct_gpt-2.2.7.tar", last modified: Tue May  9 17:05:57 2023, max compression
```

## Comparing `struct_gpt-2.2.6.tar` & `struct_gpt-2.2.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-05-09 01:27:56.458064 struct_gpt-2.2.6/LICENSE
--rw-r--r--   0        0        0     3729 2023-05-09 01:27:56.462062 struct_gpt-2.2.6/README.md
--rw-r--r--   0        0        0      587 2023-05-09 01:28:39.262019 struct_gpt-2.2.6/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-09 01:27:56.462062 struct_gpt-2.2.6/struct_gpt/__init__.py
--rw-r--r--   0        0        0     4854 2023-05-09 01:27:56.462062 struct_gpt-2.2.6/struct_gpt/models.py
--rw-r--r--   0        0        0     6096 2023-05-09 01:27:56.462062 struct_gpt-2.2.6/tests/test_models.py
--rw-r--r--   0        0        0     5350 1970-01-01 00:00:00.000000 struct_gpt-2.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-09 17:05:11.795020 struct_gpt-2.2.7/LICENSE
+-rw-r--r--   0        0        0     3650 2023-05-09 17:05:11.795020 struct_gpt-2.2.7/README.md
+-rw-r--r--   0        0        0      587 2023-05-09 17:05:57.651840 struct_gpt-2.2.7/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-09 17:05:11.795020 struct_gpt-2.2.7/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     4854 2023-05-09 17:05:11.795020 struct_gpt-2.2.7/struct_gpt/models.py
+-rw-r--r--   0        0        0     6096 2023-05-09 17:05:11.795020 struct_gpt-2.2.7/tests/test_models.py
+-rw-r--r--   0        0        0     5271 1970-01-01 00:00:00.000000 struct_gpt-2.2.7/PKG-INFO
```

### Comparing `struct_gpt-2.2.6/LICENSE` & `struct_gpt-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.6/README.md` & `struct_gpt-2.2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -53,20 +53,14 @@
 ```python
 from struct_gpt import OpenAiBase, OpenAiMixin
 from pydantic import Field, BaseModel
 from typing import Mapping
 
 
 class SentimentSchema(OpenAiBase):
-    """
-    Determine the sentiment of the given text:
-
-    {content}
-    """
-
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
 
 class SentimentAnalysis(BaseModel, OpenAiMixin):
     """
     Determine the sentiment of each word in the following: {text}
```

### Comparing `struct_gpt-2.2.6/pyproject.toml` & `struct_gpt-2.2.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dev = [
     "pytest>=7.3.1",
     "coverage>=7.2.5",
 ]
 
 [project]
 name = "struct-gpt"
-version = "2.2.6"
+version = "2.2.7"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-2.2.6/struct_gpt/models.py` & `struct_gpt-2.2.7/struct_gpt/models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.6/tests/test_models.py` & `struct_gpt-2.2.7/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.6/PKG-INFO` & `struct_gpt-2.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 2.2.6
+Version: 2.2.7
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Stephan Fitzpatrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -86,20 +86,14 @@
 ```python
 from struct_gpt import OpenAiBase, OpenAiMixin
 from pydantic import Field, BaseModel
 from typing import Mapping
 
 
 class SentimentSchema(OpenAiBase):
-    """
-    Determine the sentiment of the given text:
-
-    {content}
-    """
-
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
 
 class SentimentAnalysis(BaseModel, OpenAiMixin):
     """
     Determine the sentiment of each word in the following: {text}
```

