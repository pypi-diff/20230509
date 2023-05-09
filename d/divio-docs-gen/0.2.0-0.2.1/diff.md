# Comparing `tmp/divio_docs_gen-0.2.0.tar.gz` & `tmp/divio_docs_gen-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divio_docs_gen-0.2.0.tar", last modified: Tue May  9 06:34:28 2023, max compression
+gzip compressed data, was "divio_docs_gen-0.2.1.tar", last modified: Tue May  9 07:05:56 2023, max compression
```

## Comparing `divio_docs_gen-0.2.0.tar` & `divio_docs_gen-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6045 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5251 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)      907 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:34:28.733783 divio_docs_gen-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/src/divio_docs_gen/
--rw-r--r--   0 root         (0) root         (0)     7676 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/Args.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/src/divio_docs_gen/Repo/
--rw-r--r--   0 root         (0) root         (0)     3135 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/Repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1754 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/Repo/files.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/Repo/sections.py
--rw-r--r--   0 root         (0) root         (0)     5417 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/Section.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/index.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/markdown_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/
--rw-r--r--   0 root         (0) root         (0)     1732 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3312 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/nav.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-05-09 06:34:18.000000 divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:34:28.737783 divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6045 2023-05-09 06:34:28.000000 divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-09 06:34:28.000000 divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 06:34:28.000000 divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-09 06:34:28.000000 divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-09 06:34:28.000000 divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6069 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      907 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/src/divio_docs_gen/
+-rw-r--r--   0 root         (0) root         (0)     7711 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/Args.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/files.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/sections.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/Section.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/index.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/markdown_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/nav.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6069 2023-05-09 07:05:56.000000 divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      662 2023-05-09 07:05:56.000000 divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 07:05:56.000000 divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-09 07:05:56.000000 divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-09 07:05:56.000000 divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/top_level.txt
```

### Comparing `divio_docs_gen-0.2.0/LICENSE` & `divio_docs_gen-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.0/PKG-INFO` & `divio_docs_gen-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divio_docs_gen
-Version: 0.2.0
+Version: 0.2.1
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
@@ -18,27 +18,27 @@
 
 # Divio Docs Generator
 
 Automatically collect, aggregate and structure all your [divio-style documentation](https://documentation.divio.com/) into a tree of .md files.
 ```
 /{reponame}
     /tutorials
-    /howtos
-    /explanations
-    /references
+    /how_to_guides
+    /explanation
+    /reference
 ```
 
 On a basic level, this repo will only need a list of git url's!
 
 - Any input structure: this script will scan your entire repository for .md files
     - If you have a how-to section in your README, that'll get extracted and put in the right spot
     - Or, if you have an how-to.md file, it'll get added in its entirety!
 - Any output structure: this script generates a simple markdown tree. Nothing proprietary, no vendor-lockin. It can be generated from GitHub Actions and put into a Jekyll pages site just as easily as it is run from a Raspberry Pi and used to render the contents of an Ember application.
 
-All you have to do is simply name your headers and/or files after the divio sections (`tutorial`, `how-to`, `explanation`, `reference`). (Oh, don't worry, the search is done through a case insensitive regex. Add more words as you please) 
+All you have to do is simply name your headers and/or files after the divio sections (`tutorials`, `how_to_guides`, `explanation`, `reference`). (Oh, don't worry, the search is done through a case insensitive regex. Add more words as you please) 
 
 ## Getting-Started / tutorial
 - Install the package (`python3 -m pip install divio_docs_gen`)
 - And then either...
     - Setup the docs.conf file (See the [reference below](#docsconf) and/or the [docs.conf.example](docs.conf.example) file)
     - Use throught the cli (`python3 -m divio_docs_gen --help`)
 
@@ -73,17 +73,17 @@
 If you want to know more about the design principles of this project, feel free to check out my writeup [here](https://github.com/Denperidge-Redpencil/Learning.md/blob/main/Notes/docs.md#design-principles)!
 
 Further expansion could be done to this project. For example, a structure like the following...
 ```
 /{reponame}
     /0.0.1
         /tutorials
-        /how-tos
-        /explanations
-        /references
+        /how_to_guides
+        /explanation
+        /reference
 ```
 ... should not be impossible to achieve with some tweaking!
 
 
 ## Reference
 
 ### docs.conf
@@ -91,42 +91,42 @@
 This section is on the top of the file, and defines options that affect the entire configuration
 | Parameter     | Functionality                    |
 | ------------- | -------------------------------- |
 | DefaultOwner  | (string) Defines which user or org has to be checked for the repository in case its Path does not explicitly define an owner |
 | GenerateNav   | (boolean) Whether to add internal navigation to the top of each generated file. Defaults to `False` |
 | DocsBasedir   | What folder to output the docs in. Defaults to `docs/` |
 | Tutorials     | Sets the output folder name for tutorials. Defaults to `tutorials`    |
-| Howtos        | Sets the output folder name for how-tos. Defaults to `how-tos`    |
-| explanations  | Sets the output folder name for explanations. Defaults to `explanations`    |
-| references    | Sets the output folder name for references. Defaults to `references`    |
+| how_to_guides | Sets the output folder name for how-to guides. Defaults to `how_to_guides`    |
+| explanation   | Sets the output folder name for explanation. Defaults to `explanation`    |
+| reference     | Sets the output folder name for reference. Defaults to `reference`    |
 
 
 #### [repo] section
 You can add as many of these as you want. Each one represents a repo you want parsed. You can give any name to `[the-section-header]`, but you should probably avoid duplicates. If no repo sections are defined but you've defined DefaultOwner, all repos of that user or organisation will be parsed.
 
 | Parameter | Functionality                              |
 | --------- | ------------------------------------------ |
 | Path      | (string) Defines which repository to parse |
 | Move      | (string) Files in the repository that should be copied to a specific section. Syntax: `docs/file.md/section_id//file2.md/section_id/output_filename` |
 | Ignore      | (string) Files in the repository that should be ignored. Syntax: `file.md//file2.md` |
 
 
 **Example Ignore:** `Ignore=building-a-template.md//why-semantic-microservices.md`
-**Example Move:** `Move=documentation.md/references`
+**Example Move:** `Move=documentation.md/reference`
 
 
 *Note: for `Move` and `Ignore` you can choose to be more specific by writing `sub/folder/filename.md`. The check is a `provided_path in full_filepath`, so `sub/folder/filename.md` will apply to `even/further/sub/folder/filename.md`.*
 
 
 
 
 ### Synonyms
 For ease of use and freedom of implementation, every section has synonyms.
 
 | Section       | Synonyms                        |
 | ------------- | ------------------------------- |
 | Tutorials     | Getting started                 |
-| How-To's      | How-To, Guide, Usage            |
+| How-to Guides | How-To, Guide, Usage            |
 | Explanation   | Discussion, background material | 
 | Reference     | Technical                       |
```

### Comparing `divio_docs_gen-0.2.0/README.md` & `divio_docs_gen-0.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Divio Docs Generator
 
 Automatically collect, aggregate and structure all your [divio-style documentation](https://documentation.divio.com/) into a tree of .md files.
 ```
 /{reponame}
     /tutorials
-    /howtos
-    /explanations
-    /references
+    /how_to_guides
+    /explanation
+    /reference
 ```
 
 On a basic level, this repo will only need a list of git url's!
 
 - Any input structure: this script will scan your entire repository for .md files
     - If you have a how-to section in your README, that'll get extracted and put in the right spot
     - Or, if you have an how-to.md file, it'll get added in its entirety!
 - Any output structure: this script generates a simple markdown tree. Nothing proprietary, no vendor-lockin. It can be generated from GitHub Actions and put into a Jekyll pages site just as easily as it is run from a Raspberry Pi and used to render the contents of an Ember application.
 
-All you have to do is simply name your headers and/or files after the divio sections (`tutorial`, `how-to`, `explanation`, `reference`). (Oh, don't worry, the search is done through a case insensitive regex. Add more words as you please) 
+All you have to do is simply name your headers and/or files after the divio sections (`tutorials`, `how_to_guides`, `explanation`, `reference`). (Oh, don't worry, the search is done through a case insensitive regex. Add more words as you please) 
 
 ## Getting-Started / tutorial
 - Install the package (`python3 -m pip install divio_docs_gen`)
 - And then either...
     - Setup the docs.conf file (See the [reference below](#docsconf) and/or the [docs.conf.example](docs.conf.example) file)
     - Use throught the cli (`python3 -m divio_docs_gen --help`)
 
@@ -55,17 +55,17 @@
 If you want to know more about the design principles of this project, feel free to check out my writeup [here](https://github.com/Denperidge-Redpencil/Learning.md/blob/main/Notes/docs.md#design-principles)!
 
 Further expansion could be done to this project. For example, a structure like the following...
 ```
 /{reponame}
     /0.0.1
         /tutorials
-        /how-tos
-        /explanations
-        /references
+        /how_to_guides
+        /explanation
+        /reference
 ```
 ... should not be impossible to achieve with some tweaking!
 
 
 ## Reference
 
 ### docs.conf
@@ -73,42 +73,42 @@
 This section is on the top of the file, and defines options that affect the entire configuration
 | Parameter     | Functionality                    |
 | ------------- | -------------------------------- |
 | DefaultOwner  | (string) Defines which user or org has to be checked for the repository in case its Path does not explicitly define an owner |
 | GenerateNav   | (boolean) Whether to add internal navigation to the top of each generated file. Defaults to `False` |
 | DocsBasedir   | What folder to output the docs in. Defaults to `docs/` |
 | Tutorials     | Sets the output folder name for tutorials. Defaults to `tutorials`    |
-| Howtos        | Sets the output folder name for how-tos. Defaults to `how-tos`    |
-| explanations  | Sets the output folder name for explanations. Defaults to `explanations`    |
-| references    | Sets the output folder name for references. Defaults to `references`    |
+| how_to_guides | Sets the output folder name for how-to guides. Defaults to `how_to_guides`    |
+| explanation   | Sets the output folder name for explanation. Defaults to `explanation`    |
+| reference     | Sets the output folder name for reference. Defaults to `reference`    |
 
 
 #### [repo] section
 You can add as many of these as you want. Each one represents a repo you want parsed. You can give any name to `[the-section-header]`, but you should probably avoid duplicates. If no repo sections are defined but you've defined DefaultOwner, all repos of that user or organisation will be parsed.
 
 | Parameter | Functionality                              |
 | --------- | ------------------------------------------ |
 | Path      | (string) Defines which repository to parse |
 | Move      | (string) Files in the repository that should be copied to a specific section. Syntax: `docs/file.md/section_id//file2.md/section_id/output_filename` |
 | Ignore      | (string) Files in the repository that should be ignored. Syntax: `file.md//file2.md` |
 
 
 **Example Ignore:** `Ignore=building-a-template.md//why-semantic-microservices.md`
-**Example Move:** `Move=documentation.md/references`
+**Example Move:** `Move=documentation.md/reference`
 
 
 *Note: for `Move` and `Ignore` you can choose to be more specific by writing `sub/folder/filename.md`. The check is a `provided_path in full_filepath`, so `sub/folder/filename.md` will apply to `even/further/sub/folder/filename.md`.*
 
 
 
 
 ### Synonyms
 For ease of use and freedom of implementation, every section has synonyms.
 
 | Section       | Synonyms                        |
 | ------------- | ------------------------------- |
 | Tutorials     | Getting started                 |
-| How-To's      | How-To, Guide, Usage            |
+| How-to Guides | How-To, Guide, Usage            |
 | Explanation   | Discussion, background material | 
 | Reference     | Technical                       |
```

### Comparing `divio_docs_gen-0.2.0/pyproject.toml` & `divio_docs_gen-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "divio_docs_gen"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name="Denperidge", email="denperidge@gmail.com" },
 ]
 description = "Turn all the markdown files in your repos into one big, divio structrured documentation"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `divio_docs_gen-0.2.0/src/divio_docs_gen/Args.py` & `divio_docs_gen-0.2.1/src/divio_docs_gen/Args.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # Native imports
 from configparser import ConfigParser
 from os import getcwd, path
 from argparse import ArgumentParser
 
 """Code to handle configuration, through docs.conf or args"""
 
-section_keys = ["tutorials", "howtos", "explanations", "references"]
+section_keys = ["tutorials", "how_to_guides", "explanation", "reference"]
 class Args:
     def __init__(self) -> None:
         # store_true default is False, which means save_conf's output will be too verbose. Use None instead
         self.save_conf = None  
         self.write_to_disk = None
         self.docs_basedir = "docs/"
         self.generate_nav = None
 
-        self.tutorials, self.howtos, self.explanations, self.references = section_keys
+        self.tutorials, self.how_to_guides, self.explanation, self.reference = section_keys
 
         self.repos = []
     
     def get_configured_section_name(self, section_id: str):
         # TODO look for a cleaner solution
         if section_id == section_keys[0]:
             return self.tutorials
         elif section_id == section_keys[1]:
-            return self.howtos
+            return self.how_to_guides
         elif section_id == section_keys[2]:
-            return self.explanations
+            return self.explanation
         elif section_id == section_keys[3]:
-            return self.references
+            return self.reference
         print(section_id)
 
 
     
     def __str__(self) -> str:
         return f"""
         Configured args:
 
         - save_conf: {self.save_conf} 
         - write_to_disk: {self.write_to_disk} 
         - docs_basedir: {self.docs_basedir} 
         - generate_nav: {self.generate_nav}
 
         - tutorials: {self.tutorials}
-        - howtos: {self.howtos}
-        - explanations: {self.explanations}
-        - references: {self.references}
+        - how_to_guides: {self.how_to_guides}
+        - explanation: {self.explanation}
+        - reference: {self.reference}
 
         - repos: {self.repos} 
         """
 
     def __repr__(self) -> str:
         return self.__str__()
 
@@ -126,50 +126,50 @@
         section = conf_sections[section_key]
         if section not in conf:
             conf.add_section(section)
 
 
 """ Get config, save if desired, apply"""
 def get_conf_value(section_id, value_id):
-    return conf[section_id][value_id] if value_id in conf[section_id] else ""
+    return conf[section_id][value_id] if value_id in conf[section_id] else None
 
 def get_cli_arg_value(value_id):
     return getattr(cli_args, value_id) if hasattr(cli_args, value_id) else None
 
 def get_value(section_id, value_id, default):
     """Gets the arg, whether it be from the config file or CLI"""
     # Get the value from cli if defined. Cli > conf
     value = get_cli_arg_value(value_id)
     # If it's undefined in the CLI, check if conf can be used
     if value is None and use_conf:
         value = get_conf_value(section_id, value_id)
-    elif value is None:
+    if value is None:
         value = default
 
     if args.save_conf:
         # If it should be saved, do that
         conf[section_id][value_id] = str(value)
         
     return value
 
 args.write_to_disk = bool(get_value(conf_sections["output"], "WriteToDisk", False))
 args.generate_nav = bool(get_value(conf_sections["output"], "GenerateNav", False))
 args.docs_basedir = get_value(conf_sections["output"], "DocsBasedir", "docs/")
 
-for i, section_name in enumerate(["tutorials", "howtos", "explanations", "references"]):
+for i, section_name in enumerate(["tutorials", "how_to_guides", "explanation", "reference"]):
     # TODO cleaner solution
     value = get_value(conf_sections["naming"], value_id=section_name, default=section_name)
     if i == 0:
         args.tutorials = value
     elif i == 1:
-        args.howtos = value
+        args.how_to_guides = value
     elif i == 2:
-        args.explanations = value
+        args.explanation = value
     elif i == 3:
-        args.references = value
+        args.reference = value
 
 
 if get_cli_arg_value("repos"):
     for repo_arg in get_cli_arg_value("repos"):
         repo_config = dict()
         repo_config.url = repo_arg[0]
         for arg in repo_arg[1:]:
```

### Comparing `divio_docs_gen-0.2.0/src/divio_docs_gen/Repo/__init__.py` & `divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/__init__.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.0/src/divio_docs_gen/Repo/files.py` & `divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/files.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.0/src/divio_docs_gen/Repo/sections.py` & `divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/sections.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.0/src/divio_docs_gen/Section.py` & `divio_docs_gen-0.2.1/src/divio_docs_gen/Section.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from re import search, RegexFlag, sub, escape
 from .Args import args
 
-"""Defines section (how-to, getting started...) classes"""
+"""Defines section (how_to_guides, tutorials...) classes"""
 
 def regex(needle: r"str", haystack: str, flags):
     """Base regex helper"""
     return search(needle, haystack, flags)
 
 def regexIM(needle: r"str", haystack: str):
     """Helper for case insensitive & multiline regex"""
@@ -114,15 +114,15 @@
 
         
     
 
 """Section definitions. This is where you can customise synonyms"""
 sections = {
     "tutorials": Section(args.tutorials,       r"(tutorial|getting\W*started)"),
-    "howtos": Section(args.howtos,             r"(how\W*to|guide|usage)"),
-    "explanations": Section(args.explanations, r"(explanation|discussion|background\W*material)"),
-    "references": Section(args.references,     r"(reference|technical)")
+    "how_to_guides": Section(args.how_to_guides,             r"(how\W*to|guide|usage)"),
+    "explanation": Section(args.explanation, r"(explanation|discussion|background\W*material)"),
+    "reference": Section(args.reference,     r"(reference|technical)")
 }
```

### Comparing `divio_docs_gen-0.2.0/src/divio_docs_gen/index.py` & `divio_docs_gen-0.2.1/src/divio_docs_gen/index.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.0/src/divio_docs_gen/markdown_parser.py` & `divio_docs_gen-0.2.1/src/divio_docs_gen/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/__init__.py` & `divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/__init__.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/nav.py` & `divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/nav.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.0/src/divio_docs_gen/write_to_disk/utils.py` & `divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/utils.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/PKG-INFO` & `divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divio-docs-gen
-Version: 0.2.0
+Version: 0.2.1
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
@@ -18,27 +18,27 @@
 
 # Divio Docs Generator
 
 Automatically collect, aggregate and structure all your [divio-style documentation](https://documentation.divio.com/) into a tree of .md files.
 ```
 /{reponame}
     /tutorials
-    /howtos
-    /explanations
-    /references
+    /how_to_guides
+    /explanation
+    /reference
 ```
 
 On a basic level, this repo will only need a list of git url's!
 
 - Any input structure: this script will scan your entire repository for .md files
     - If you have a how-to section in your README, that'll get extracted and put in the right spot
     - Or, if you have an how-to.md file, it'll get added in its entirety!
 - Any output structure: this script generates a simple markdown tree. Nothing proprietary, no vendor-lockin. It can be generated from GitHub Actions and put into a Jekyll pages site just as easily as it is run from a Raspberry Pi and used to render the contents of an Ember application.
 
-All you have to do is simply name your headers and/or files after the divio sections (`tutorial`, `how-to`, `explanation`, `reference`). (Oh, don't worry, the search is done through a case insensitive regex. Add more words as you please) 
+All you have to do is simply name your headers and/or files after the divio sections (`tutorials`, `how_to_guides`, `explanation`, `reference`). (Oh, don't worry, the search is done through a case insensitive regex. Add more words as you please) 
 
 ## Getting-Started / tutorial
 - Install the package (`python3 -m pip install divio_docs_gen`)
 - And then either...
     - Setup the docs.conf file (See the [reference below](#docsconf) and/or the [docs.conf.example](docs.conf.example) file)
     - Use throught the cli (`python3 -m divio_docs_gen --help`)
 
@@ -73,17 +73,17 @@
 If you want to know more about the design principles of this project, feel free to check out my writeup [here](https://github.com/Denperidge-Redpencil/Learning.md/blob/main/Notes/docs.md#design-principles)!
 
 Further expansion could be done to this project. For example, a structure like the following...
 ```
 /{reponame}
     /0.0.1
         /tutorials
-        /how-tos
-        /explanations
-        /references
+        /how_to_guides
+        /explanation
+        /reference
 ```
 ... should not be impossible to achieve with some tweaking!
 
 
 ## Reference
 
 ### docs.conf
@@ -91,42 +91,42 @@
 This section is on the top of the file, and defines options that affect the entire configuration
 | Parameter     | Functionality                    |
 | ------------- | -------------------------------- |
 | DefaultOwner  | (string) Defines which user or org has to be checked for the repository in case its Path does not explicitly define an owner |
 | GenerateNav   | (boolean) Whether to add internal navigation to the top of each generated file. Defaults to `False` |
 | DocsBasedir   | What folder to output the docs in. Defaults to `docs/` |
 | Tutorials     | Sets the output folder name for tutorials. Defaults to `tutorials`    |
-| Howtos        | Sets the output folder name for how-tos. Defaults to `how-tos`    |
-| explanations  | Sets the output folder name for explanations. Defaults to `explanations`    |
-| references    | Sets the output folder name for references. Defaults to `references`    |
+| how_to_guides | Sets the output folder name for how-to guides. Defaults to `how_to_guides`    |
+| explanation   | Sets the output folder name for explanation. Defaults to `explanation`    |
+| reference     | Sets the output folder name for reference. Defaults to `reference`    |
 
 
 #### [repo] section
 You can add as many of these as you want. Each one represents a repo you want parsed. You can give any name to `[the-section-header]`, but you should probably avoid duplicates. If no repo sections are defined but you've defined DefaultOwner, all repos of that user or organisation will be parsed.
 
 | Parameter | Functionality                              |
 | --------- | ------------------------------------------ |
 | Path      | (string) Defines which repository to parse |
 | Move      | (string) Files in the repository that should be copied to a specific section. Syntax: `docs/file.md/section_id//file2.md/section_id/output_filename` |
 | Ignore      | (string) Files in the repository that should be ignored. Syntax: `file.md//file2.md` |
 
 
 **Example Ignore:** `Ignore=building-a-template.md//why-semantic-microservices.md`
-**Example Move:** `Move=documentation.md/references`
+**Example Move:** `Move=documentation.md/reference`
 
 
 *Note: for `Move` and `Ignore` you can choose to be more specific by writing `sub/folder/filename.md`. The check is a `provided_path in full_filepath`, so `sub/folder/filename.md` will apply to `even/further/sub/folder/filename.md`.*
 
 
 
 
 ### Synonyms
 For ease of use and freedom of implementation, every section has synonyms.
 
 | Section       | Synonyms                        |
 | ------------- | ------------------------------- |
 | Tutorials     | Getting started                 |
-| How-To's      | How-To, Guide, Usage            |
+| How-to Guides | How-To, Guide, Usage            |
 | Explanation   | Discussion, background material | 
 | Reference     | Technical                       |
```

### Comparing `divio_docs_gen-0.2.0/src/divio_docs_gen.egg-info/SOURCES.txt` & `divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

