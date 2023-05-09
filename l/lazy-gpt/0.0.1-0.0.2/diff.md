# Comparing `tmp/lazy-gpt-0.0.1.tar.gz` & `tmp/lazy-gpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy-gpt-0.0.1.tar", last modified: Tue May  9 21:34:55 2023, max compression
+gzip compressed data, was "lazy-gpt-0.0.2.tar", last modified: Tue May  9 21:43:37 2023, max compression
```

## Comparing `lazy-gpt-0.0.1.tar` & `lazy-gpt-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 21:34:55.880726 lazy-gpt-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-08 21:26:59.000000 lazy-gpt-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3491 2023-05-09 21:34:55.879725 lazy-gpt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1585 2023-05-09 21:30:33.000000 lazy-gpt-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 21:34:55.879725 lazy-gpt-0.0.1/lazy_gpt.egg-info/
--rw-rw-rw-   0        0        0     3491 2023-05-09 21:34:55.000000 lazy-gpt-0.0.1/lazy_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-05-09 21:34:55.000000 lazy-gpt-0.0.1/lazy_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 21:34:55.000000 lazy-gpt-0.0.1/lazy_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-09 21:34:55.000000 lazy-gpt-0.0.1/lazy_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 21:34:55.000000 lazy-gpt-0.0.1/lazy_gpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      785 2023-05-09 21:28:52.000000 lazy-gpt-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 21:34:55.880726 lazy-gpt-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 21:43:37.082510 lazy-gpt-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-08 21:26:59.000000 lazy-gpt-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3491 2023-05-09 21:43:37.081511 lazy-gpt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1585 2023-05-09 21:41:19.000000 lazy-gpt-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 21:43:37.081511 lazy-gpt-0.0.2/lazy_gpt.egg-info/
+-rw-rw-rw-   0        0        0     3491 2023-05-09 21:43:37.000000 lazy-gpt-0.0.2/lazy_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-05-09 21:43:37.000000 lazy-gpt-0.0.2/lazy_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 21:43:37.000000 lazy-gpt-0.0.2/lazy_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-09 21:43:37.000000 lazy-gpt-0.0.2/lazy_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 21:43:37.000000 lazy-gpt-0.0.2/lazy_gpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      785 2023-05-09 21:43:09.000000 lazy-gpt-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 21:43:37.082510 lazy-gpt-0.0.2/setup.cfg
```

### Comparing `lazy-gpt-0.0.1/LICENSE` & `lazy-gpt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lazy-gpt-0.0.1/PKG-INFO` & `lazy-gpt-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-gpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple package to make GPT API usage easier
 Author-email: Samuel Reeder <samuel.reeder@mail.utoronto.ca>
 License: MIT License
         
         Copyright (c) 2023 Samuel Reeder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,15 +46,15 @@
 ```python
 lazygpt.config("your_api_key", "your_organization")
 ```
 
 Next, create a GPT instance using the LazyGPT class. You can choose the GPT model by accessing the Model enum:
 
 ```python
-gpt_instance = lazygpt.EasyGPT(model=lazygpt.Model.GPT_4)
+gpt_instance = lazygpt.EasyGPT(model=lazygpt.Model.GPT4)
 ```
 
 Now you can obtain context-driven responses using the response function:
 
 ```python
 response = gpt_instance.response("What is the capital of France?")
 ```
@@ -64,15 +64,15 @@
 ```python
 json_response = gpt_instance.response("What is the capital of France?", just_reply=False, max_tokens=50, temperature=0.8)
 ```
 
 To change the GPT model, use the change_model function:
 
 ```python
-gpt_instance.change_model(lazygpt.Model.GPT_3)
+gpt_instance.change_model(lazygpt.Model.GPT3_5)
 ```
 
 To access the message history, use the get_messages function:
 
 ```python
 message_history = gpt_instance.get_messages()
 print(message_history)
```

### Comparing `lazy-gpt-0.0.1/README.md` & `lazy-gpt-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ```python
 lazygpt.config("your_api_key", "your_organization")
 ```
 
 Next, create a GPT instance using the LazyGPT class. You can choose the GPT model by accessing the Model enum:
 
 ```python
-gpt_instance = lazygpt.EasyGPT(model=lazygpt.Model.GPT_4)
+gpt_instance = lazygpt.EasyGPT(model=lazygpt.Model.GPT4)
 ```
 
 Now you can obtain context-driven responses using the response function:
 
 ```python
 response = gpt_instance.response("What is the capital of France?")
 ```
@@ -27,15 +27,15 @@
 ```python
 json_response = gpt_instance.response("What is the capital of France?", just_reply=False, max_tokens=50, temperature=0.8)
 ```
 
 To change the GPT model, use the change_model function:
 
 ```python
-gpt_instance.change_model(lazygpt.Model.GPT_3)
+gpt_instance.change_model(lazygpt.Model.GPT3_5)
 ```
 
 To access the message history, use the get_messages function:
 
 ```python
 message_history = gpt_instance.get_messages()
 print(message_history)
```

### Comparing `lazy-gpt-0.0.1/lazy_gpt.egg-info/PKG-INFO` & `lazy-gpt-0.0.2/lazy_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-gpt
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple package to make GPT API usage easier
 Author-email: Samuel Reeder <samuel.reeder@mail.utoronto.ca>
 License: MIT License
         
         Copyright (c) 2023 Samuel Reeder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,15 +46,15 @@
 ```python
 lazygpt.config("your_api_key", "your_organization")
 ```
 
 Next, create a GPT instance using the LazyGPT class. You can choose the GPT model by accessing the Model enum:
 
 ```python
-gpt_instance = lazygpt.EasyGPT(model=lazygpt.Model.GPT_4)
+gpt_instance = lazygpt.EasyGPT(model=lazygpt.Model.GPT4)
 ```
 
 Now you can obtain context-driven responses using the response function:
 
 ```python
 response = gpt_instance.response("What is the capital of France?")
 ```
@@ -64,15 +64,15 @@
 ```python
 json_response = gpt_instance.response("What is the capital of France?", just_reply=False, max_tokens=50, temperature=0.8)
 ```
 
 To change the GPT model, use the change_model function:
 
 ```python
-gpt_instance.change_model(lazygpt.Model.GPT_3)
+gpt_instance.change_model(lazygpt.Model.GPT3_5)
 ```
 
 To access the message history, use the get_messages function:
 
 ```python
 message_history = gpt_instance.get_messages()
 print(message_history)
```

### Comparing `lazy-gpt-0.0.1/pyproject.toml` & `lazy-gpt-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lazy-gpt"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Samuel Reeder", email="samuel.reeder@mail.utoronto.ca" },
 ]
 description = "A simple package to make GPT API usage easier"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

