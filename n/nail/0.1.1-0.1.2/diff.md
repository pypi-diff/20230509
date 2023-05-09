# Comparing `tmp/nail-0.1.1.tar.gz` & `tmp/nail-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nail-0.1.1.tar", last modified: Sat Apr 29 05:15:32 2023, max compression
+gzip compressed data, was "nail-0.1.2.tar", last modified: Tue May  9 01:58:10 2023, max compression
```

## Comparing `nail-0.1.1.tar` & `nail-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:32.463734 nail-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-29 05:15:19.000000 nail-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-29 05:15:32.463734 nail-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-29 05:15:19.000000 nail-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:32.459735 nail-0.1.1/nail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:19.000000 nail-0.1.1/nail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:32.459735 nail-0.1.1/nail/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:19.000000 nail-0.1.1/nail/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-29 05:15:19.000000 nail-0.1.1/nail/core/animation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-29 05:15:19.000000 nail-0.1.1/nail/core/chat_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-29 05:15:19.000000 nail-0.1.1/nail/core/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-29 05:15:19.000000 nail-0.1.1/nail/core/context_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-29 05:15:19.000000 nail-0.1.1/nail/core/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-29 05:15:19.000000 nail-0.1.1/nail/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:32.459735 nail-0.1.1/nail/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:19.000000 nail-0.1.1/nail/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:32.459735 nail-0.1.1/nail/tools/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:19.000000 nail-0.1.1/nail/tools/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-29 05:15:19.000000 nail-0.1.1/nail/tools/build/build_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-29 05:15:19.000000 nail-0.1.1/nail/tools/build/build_readme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:32.463734 nail-0.1.1/nail/tools/debug/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:19.000000 nail-0.1.1/nail/tools/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-29 05:15:19.000000 nail-0.1.1/nail/tools/debug/debug_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:32.463734 nail-0.1.1/nail/tools/modify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:19.000000 nail-0.1.1/nail/tools/modify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-29 05:15:19.000000 nail-0.1.1/nail/tools/modify/modify_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:32.463734 nail-0.1.1/nail/tools/spec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:19.000000 nail-0.1.1/nail/tools/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-29 05:15:19.000000 nail-0.1.1/nail/tools/spec/build_spec_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:32.459735 nail-0.1.1/nail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-29 05:15:32.000000 nail-0.1.1/nail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-29 05:15:32.000000 nail-0.1.1/nail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 05:15:32.000000 nail-0.1.1/nail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-29 05:15:32.000000 nail-0.1.1/nail.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-29 05:15:32.000000 nail-0.1.1/nail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 05:15:32.000000 nail-0.1.1/nail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 05:15:32.463734 nail-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-29 05:15:19.000000 nail-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:32.463734 nail-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:19.000000 nail-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:32.463734 nail-0.1.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 05:15:19.000000 nail-0.1.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-29 05:15:19.000000 nail-0.1.1/tests/core/test_chat_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-29 05:15:19.000000 nail-0.1.1/tests/core/test_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-29 05:15:19.000000 nail-0.1.1/tests/core/test_context_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-04-29 05:15:19.000000 nail-0.1.1/tests/core/test_file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-29 05:15:19.000000 nail-0.1.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:10.846253 nail-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 01:58:00.000000 nail-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-09 01:58:10.846253 nail-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-05-09 01:58:00.000000 nail-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:10.842253 nail-0.1.2/nail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:00.000000 nail-0.1.2/nail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:10.842253 nail-0.1.2/nail/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:10.842253 nail-0.1.2/nail/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/config/local_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/config/user_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/file_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:10.842253 nail-0.1.2/nail/core/language_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/language_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/language_models/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/language_models/open_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/language_models/supported_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/loading_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:10.842253 nail-0.1.2/nail/core/prompt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/prompt/context_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/prompt/formatting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-09 01:58:00.000000 nail-0.1.2/nail/core/prompt/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-09 01:58:00.000000 nail-0.1.2/nail/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:10.846253 nail-0.1.2/nail/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:00.000000 nail-0.1.2/nail/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-09 01:58:00.000000 nail-0.1.2/nail/tools/build_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-09 01:58:00.000000 nail-0.1.2/nail/tools/build_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-09 01:58:00.000000 nail-0.1.2/nail/tools/build_spec_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-09 01:58:00.000000 nail-0.1.2/nail/tools/debug_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-09 01:58:00.000000 nail-0.1.2/nail/tools/explain_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-09 01:58:00.000000 nail-0.1.2/nail/tools/modify_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:10.842253 nail-0.1.2/nail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-09 01:58:10.000000 nail-0.1.2/nail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-09 01:58:10.000000 nail-0.1.2/nail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 01:58:10.000000 nail-0.1.2/nail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-09 01:58:10.000000 nail-0.1.2/nail.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 01:58:10.000000 nail-0.1.2/nail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 01:58:10.000000 nail-0.1.2/nail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 01:58:10.846253 nail-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-09 01:58:00.000000 nail-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:10.846253 nail-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:00.000000 nail-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:10.846253 nail-0.1.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 01:58:00.000000 nail-0.1.2/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-09 01:58:00.000000 nail-0.1.2/tests/core/test_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-09 01:58:00.000000 nail-0.1.2/tests/core/test_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-09 01:58:00.000000 nail-0.1.2/tests/core/test_file_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-09 01:58:00.000000 nail-0.1.2/tests/test_main.py
```

### Comparing `nail-0.1.1/LICENSE` & `nail-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nail-0.1.1/PKG-INFO` & `nail-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nail
-Version: 0.1.1
+Version: 0.1.2
 Summary: A CLI tool for speeding up development using LLMs
 Home-page: https://github.com/edsaav/nail
 Author: Edward Saavedra
 Author-email: edsaav@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,19 +47,44 @@
 
 ```
 nail configure
 ```
 
 This will prompt you to enter your API key, which will be saved for future use.
 
-## Usage
+## Basic Usage
+
+Once you have configured Nail, you can begin using it to generate code. To get started create and navigate to a new project directory. Create a new file and write out what you want the code in that file to do. For example:
+
+```
+# calculator.py
+A python class with addition, subtraction, and multiplication methods
+```
+
+Once you have created and saved your file, run the following command:
+
+```
+nail build calculator.py
+```
+
+After a moment, Nail will generate code meeting that specification and will prompt you to accept or reject the proposed code. If you accept, it will be saved to the file.
+
+What if we want to add to this file? Use the following command to ask Nail to add an additional method.
+
+```
+nail modify calculator.py -r "Add a division method"
+```
+
+Nail will then generate the changes and propose them as a diff that, if accepted, will be saved to the file. Continue reading below to learn about further ways to use Nail to assist in the coding process.
+
+## Usage Details
 
 Nail provides several commands to help you with your code:
 
-### Build 🔨
+### 🔨 Build 🔨
 
 To build a new file with optional context files, use the `build` command:
 
 ```
 nail build <file> [--context-files <file1> <file2> ...] [--model <model>]
 ```
 
@@ -73,71 +98,95 @@
 - returns an array of resulting headings
 ```
 
 If the file does not exist, nail will open your default editor to fill in the prompt in-line.
 
 The `--context-files` (or `-c`) option can be used to pass in one or more additional files that could provide useful reference. For example, you can pass in files containing modules that should be imported and used by the new file that is being built.
 
-### Modify 🔧
+### 🔧 Modify 🔧
 
 To modify an existing file, use the `modify` command:
 
 ```
 nail modify <file> [--request <request>] [--context-files <file1> <file2> ...] [--model <model>]
 ```
 
 The request should be in the form of a command, such as "Add a new function that..." or "Refactor the existing class to...".
 
-### Debug 🐛
+### 🐛 Debug 🐛
 
 To debug an existing file, use the `debug` command:
 
 ```
 nail debug <file> [--error <error_message>] [--model <model>]
 ```
 
 If an error message is not passed, this command will simply look for any possible issues in the given file.
 
-### Generate Unit Tests 🧪
+### 🧪 Generate Unit Tests 🧪
 
 To generate a unit test file for an existing file, use the `spec` command:
 
 ```
 nail spec <file> <target_path> [--model <model>]
 ```
 
 Once they have been generated, test files can be further adjusted with the `modify` command.
 
-### Generate README 📖
+### 🧐 Explain a File 🧐
+
+To explain the contents of a file, use the `explain` command:
+
+```
+nail explain <file> [--context-files <file1> <file2> ...] [--verbose] [--model <model>]
+```
+
+Output will be displayed in the console. More detailed explanations will be generated if the `--verbose` (or `-v`) flag is included.
+
+### 📖 Generate README 📖
 
 To generate a README file for your project, use the `readme` command:
 
 ```
 nail readme [--model <model>]
 ```
 
 This command will gather all application files into context automatically. It will exclude a number of files irrelevant to a README, such as tests and licenses. Please note, this currently only works for relatively small projects given the limited context window available for GPT.
 
+## Customization
+
+There may be situations in which you want Nail to apply specific additional instructions to the LLM. For example, when using the spec tool, you may wish to specify that tests are always written using a specific library. Or, you may wish to define style guidelines that the build and modify commands should always adhere to. Whatever the case, you can configure each Nail command with additional instructions.
+
+To do this, create a `.nail.yaml` file inside your project's root directory. There is a `.sample.nail.yaml` file inside of this repository showing the appropriate format. For any commands you would like to customize, simply add any desired instructions and they will be appended to requests to the LLM.
+
+For example:
+
+```
+prompt_instructions:
+  spec: Use rspec for all unit tests.
+  build: |
+    Do not include inline comments.
+    Avoid deeply nested conditionals wherever possible.
+```
+
 ## Models
 
 Nail currently supports the following models:
 
 - gpt-3.5-turbo (default)
 - gpt-4
 
-You can specify the model to use with the `--model` option for each command.
+You can specify the model to use with the `--model` (or `-m`) option for each command.
 
 ## Development
 
 To install Nail locally for development, clone the repo, then run this command from within the project directory:
 
 ```
 pip3 install -e .
 ```
 
-## Tests
-
 Run the test suite using `pytest`.
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `nail-0.1.1/README.md` & `nail-0.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -34,19 +34,44 @@
 
 ```
 nail configure
 ```
 
 This will prompt you to enter your API key, which will be saved for future use.
 
-## Usage
+## Basic Usage
+
+Once you have configured Nail, you can begin using it to generate code. To get started create and navigate to a new project directory. Create a new file and write out what you want the code in that file to do. For example:
+
+```
+# calculator.py
+A python class with addition, subtraction, and multiplication methods
+```
+
+Once you have created and saved your file, run the following command:
+
+```
+nail build calculator.py
+```
+
+After a moment, Nail will generate code meeting that specification and will prompt you to accept or reject the proposed code. If you accept, it will be saved to the file.
+
+What if we want to add to this file? Use the following command to ask Nail to add an additional method.
+
+```
+nail modify calculator.py -r "Add a division method"
+```
+
+Nail will then generate the changes and propose them as a diff that, if accepted, will be saved to the file. Continue reading below to learn about further ways to use Nail to assist in the coding process.
+
+## Usage Details
 
 Nail provides several commands to help you with your code:
 
-### Build 🔨
+### 🔨 Build 🔨
 
 To build a new file with optional context files, use the `build` command:
 
 ```
 nail build <file> [--context-files <file1> <file2> ...] [--model <model>]
 ```
 
@@ -60,71 +85,95 @@
 - returns an array of resulting headings
 ```
 
 If the file does not exist, nail will open your default editor to fill in the prompt in-line.
 
 The `--context-files` (or `-c`) option can be used to pass in one or more additional files that could provide useful reference. For example, you can pass in files containing modules that should be imported and used by the new file that is being built.
 
-### Modify 🔧
+### 🔧 Modify 🔧
 
 To modify an existing file, use the `modify` command:
 
 ```
 nail modify <file> [--request <request>] [--context-files <file1> <file2> ...] [--model <model>]
 ```
 
 The request should be in the form of a command, such as "Add a new function that..." or "Refactor the existing class to...".
 
-### Debug 🐛
+### 🐛 Debug 🐛
 
 To debug an existing file, use the `debug` command:
 
 ```
 nail debug <file> [--error <error_message>] [--model <model>]
 ```
 
 If an error message is not passed, this command will simply look for any possible issues in the given file.
 
-### Generate Unit Tests 🧪
+### 🧪 Generate Unit Tests 🧪
 
 To generate a unit test file for an existing file, use the `spec` command:
 
 ```
 nail spec <file> <target_path> [--model <model>]
 ```
 
 Once they have been generated, test files can be further adjusted with the `modify` command.
 
-### Generate README 📖
+### 🧐 Explain a File 🧐
+
+To explain the contents of a file, use the `explain` command:
+
+```
+nail explain <file> [--context-files <file1> <file2> ...] [--verbose] [--model <model>]
+```
+
+Output will be displayed in the console. More detailed explanations will be generated if the `--verbose` (or `-v`) flag is included.
+
+### 📖 Generate README 📖
 
 To generate a README file for your project, use the `readme` command:
 
 ```
 nail readme [--model <model>]
 ```
 
 This command will gather all application files into context automatically. It will exclude a number of files irrelevant to a README, such as tests and licenses. Please note, this currently only works for relatively small projects given the limited context window available for GPT.
 
+## Customization
+
+There may be situations in which you want Nail to apply specific additional instructions to the LLM. For example, when using the spec tool, you may wish to specify that tests are always written using a specific library. Or, you may wish to define style guidelines that the build and modify commands should always adhere to. Whatever the case, you can configure each Nail command with additional instructions.
+
+To do this, create a `.nail.yaml` file inside your project's root directory. There is a `.sample.nail.yaml` file inside of this repository showing the appropriate format. For any commands you would like to customize, simply add any desired instructions and they will be appended to requests to the LLM.
+
+For example:
+
+```
+prompt_instructions:
+  spec: Use rspec for all unit tests.
+  build: |
+    Do not include inline comments.
+    Avoid deeply nested conditionals wherever possible.
+```
+
 ## Models
 
 Nail currently supports the following models:
 
 - gpt-3.5-turbo (default)
 - gpt-4
 
-You can specify the model to use with the `--model` option for each command.
+You can specify the model to use with the `--model` (or `-m`) option for each command.
 
 ## Development
 
 To install Nail locally for development, clone the repo, then run this command from within the project directory:
 
 ```
 pip3 install -e .
 ```
 
-## Tests
-
 Run the test suite using `pytest`.
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `nail-0.1.1/nail/core/config_utils.py` & `nail-0.1.2/nail/core/config/user_config_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import os
 import configparser
 from pathlib import Path
 
-CONFIG_FILE = Path.home() / ".nailrc"
+USER_CONFIG_FILE = Path.home() / ".nailrc"
 
 
 def get_api_key():
     if "OPENAI_API_KEY" in os.environ:
         return os.environ["OPENAI_API_KEY"]
 
-    if CONFIG_FILE.is_file():
+    if USER_CONFIG_FILE.is_file():
         config = configparser.ConfigParser()
-        config.read(CONFIG_FILE)
+        config.read(USER_CONFIG_FILE)
         if "openai" in config and "api_key" in config["openai"]:
             return config["openai"]["api_key"]
 
     return None
 
 
 def save_api_key(api_key):
     config = configparser.ConfigParser()
-    if CONFIG_FILE.is_file():
-        config.read(CONFIG_FILE)
+    if USER_CONFIG_FILE.is_file():
+        config.read(USER_CONFIG_FILE)
 
     if "openai" not in config:
         config["openai"] = {}
 
     config["openai"]["api_key"] = api_key
 
-    with CONFIG_FILE.open("w") as config_file:
+    with USER_CONFIG_FILE.open("w") as config_file:
         config.write(config_file)
```

### Comparing `nail-0.1.1/nail/core/context_utils.py` & `nail-0.1.2/nail/core/prompt/context_compiler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from nail.core.file_utils import read_file
 import os
+import re
 
-CONTEXT_PREFIX = "Existing files for context:\n\n"
-CONTEXT_SUFFIX = "Given the above context, draft a new file using " \
-    + "the following request:\n\n"
-
-
-def build_context_prefix(context_file_paths):
-    """
-    Build the context prefix string based on the provided context file paths.
-
-    :param context_file_paths: List of file paths to be used as context
-    :return: context_prefix: String containing the context prefix
-    """
-    context_prefix = ""
-    if context_file_paths:
-        context_prefix += CONTEXT_PREFIX
-        for context_file_path in context_file_paths:
-            context_content = read_file(context_file_path)
-            context_prefix += format_file_block(
-                context_file_path, context_content)
-        context_prefix += CONTEXT_SUFFIX
-    return context_prefix
-
-
-def format_file_label(file_path):
-    return f"[[{file_path}]]"
-
-
-def format_file_block(context_file_path, context_content):
-    label = format_file_label(context_file_path)
-    formatted_file_content = f"```\n{context_content}\n```"
-    return f"{label}\n{formatted_file_content}\n\n"
-
-
-def list_all_files(path=None, ignore_list=None):
-    """
-    Recursively list all file paths within the given directory, including files
-    nested within sub-directories, ignoring files or directories with names
-    starting with a period or matching any names in the ignore_list.
-
-    :param path: Optional path to the directory. If not provided, uses the
-    current path.
-    :param ignore_list: Optional list of strings containing names to ignore.
-    :return: List of strings containing file paths within the directory.
-    """
-    if path is None:
-        path = os.getcwd()
-
-    if ignore_list is None:
-        ignore_list = []
-
-    file_paths = []
-
-    for root, dirs, files in os.walk(path):
-        # Ignore directories starting with a period or in the ignore_list
-        dirs[:] = [d for d in dirs if not d.startswith(
-            '.') and d not in ignore_list]
-
-        for file in files:
-            # Ignore files starting with a period or in the ignore_list
-            if not file.startswith('.') and file not in ignore_list:
+from pathlib import Path
+from typing import List
+from nail.core.prompt.formatting_utils import file_block
+
+
+class ContextCompiler:
+    """
+    Compiles prompt context from the files in the given context_file_paths.
+
+    :param context_file_paths: A list of file paths to include in the context.
+    :param ignore_list: A list of file names or regex patterns to ignore.
+    """
+
+    CONTEXT_PREFIX = "Existing files for context:"
+    # TODO: Make this list configurable
+    DEFAULT_IGNORE_LIST = ["README", "LICENSE", "^[._]", "^test", "test$"]
+
+    def __init__(
+        self, context_file_paths=[os.getcwd()], ignore_list=DEFAULT_IGNORE_LIST
+    ):
+        self.context_file_paths = context_file_paths
+        self.ignore_list = ignore_list
+
+    def compile_all(self):
+        """
+        Compiles prompt context from all files in the given context_file_paths.
+        This includes a prefix explaining the context, and a code block
+        and file name label for each file.
+
+        :return: A string containing the prompt context.
+        """
+        all_files = self._list_all_files()
+        return self._compile_context(all_files)
+
+    def compile_all_minus_ignored(self):
+        """
+        Compiles prompt context from given context_file_paths. Includes all
+        files in the given paths, minus any that are included in the
+        ContextCompiler's ignore_list. Context includes a prefix explaining the
+        context, and a code block and file name label for each file.
+
+        :return: A string containing the prompt context.
+        """
+        relevant_files = self._filter_ignored(self._list_all_files())
+        return self._compile_context(relevant_files)
+
+    def _compile_context(self, files):
+        context = [file_block(file) for file in files]
+        return f"{self.CONTEXT_PREFIX}\n\n{''.join(context)}"
+
+    def _list_all_files(self):
+        all_file_paths = []
+        for path in self.context_file_paths:
+            file_paths = self._list_files_at_path(path)
+            all_file_paths.extend(file_paths)
+        return all_file_paths
+
+    def _list_files_at_path(self, path):
+        if os.path.isfile(path):
+            return [path]
+        file_paths = []
+        for root, dirs, files in os.walk(path):
+            dirs[:] = [d for d in dirs if not d.startswith(".")]
+            for file in files:
                 file_paths.append(os.path.join(root, file))
+        return file_paths
 
-    return file_paths
-
-
-def build_context_prefix_from_directory(path=None, ignore_list=None):
-    """
-    Build the context prefix string based on all the files in the
-    specified (or current) directory.
-
-    :param path: Optional path to directory. If not given, uses current path.
-    :param ignore_list: Optional list of strings containing names to ignore.
-    :return: context_prefix: String containing the context prefix
-    """
-    context_file_paths = list_all_files(path, ignore_list)
-    context_prefix = build_context_prefix(context_file_paths)
-    return context_prefix
+    def _filter_ignored(self, file_paths):
+        return [
+            file_path for file_path in file_paths if not self._is_ignored(file_path)
+        ]
+
+    def _is_ignored(self, file_path):
+        # Generate regexes for each item in the ignore list and
+        # return True if any of them match the given file path
+        file = os.path.basename(file_path)
+        return any(re.compile(item).search(file) for item in self.ignore_list)
```

### Comparing `nail-0.1.1/nail/main.py` & `nail-0.1.2/nail/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import click
-from nail.tools.build.build_file import build_file
-from nail.tools.build.build_readme import build_readme
-from nail.tools.modify.modify_file import modify_file
-from nail.tools.debug.debug_file import debug_file
-from nail.tools.spec.build_spec_file import build_spec_file
-from nail.core.config_utils import save_api_key
+from nail.tools.build_file import build_file
+from nail.tools.build_readme import build_readme
+from nail.tools.modify_file import modify_file
+from nail.tools.debug_file import debug_file
+from nail.tools.build_spec_file import build_spec_file
+from nail.tools.explain_file import explain_file
+from nail.core.config.user_config_utils import save_api_key
 
-MODEL_HELP = "Optionally specify an LLM model. " \
+MODEL_HELP = (
+    "Optionally specify an LLM model. "
     + "Currently defaults to gpt-3.5-turbo and supports gpt-4."
+)
 
 
 @click.group()
 def main():
     pass
 
 
 @main.command()
-@click.option("--api_key", prompt=True, hide_input=True,
-              help="Your OpenAI API key.")
+@click.option("--api_key", prompt=True, hide_input=True, help="Your OpenAI API key.")
 def configure(api_key):
     save_api_key(api_key)
     click.echo("API key saved successfully.")
 
 
 @main.command()
 @click.argument("file")
-@click.option("--context-files", "-c", multiple=True, type=str,
-              help="Optional list of context file paths.")
+@click.option(
+    "--context-files",
+    "-c",
+    multiple=True,
+    type=str,
+    help="Optional list of context file paths.",
+)
 @click.option("--model", "-m", type=str, help=MODEL_HELP)
 def build(file, context_files, model):
     """Build a new file with optional context files."""
     click.echo(f"Building a new file: {file}")
     if context_files:
         click.echo(f"Using context files: {', '.join(context_files)}")
     build_file(file, context_files, model)
@@ -42,31 +49,41 @@
     """Build a new README file based on the currect directory."""
     click.echo("Generating README file.")
     build_readme("README.md", model)
 
 
 @main.command()
 @click.argument("file")
-@click.option("--request", "-r", prompt="Requested change",
-              help="The modification that you are requesting.")
-@click.option("--context-files", "-c", multiple=True, type=str,
-              help="Optional list of context file paths.")
+@click.option(
+    "--request",
+    "-r",
+    prompt="Requested change",
+    help="The modification that you are requesting.",
+)
+@click.option(
+    "--context-files",
+    "-c",
+    multiple=True,
+    type=str,
+    help="Optional list of context file paths.",
+)
 @click.option("--model", "-m", type=str, help=MODEL_HELP)
 def modify(file, request, context_files, model):
     """Modify an existing file."""
     click.echo(f"Modifying file: {file}")
     if context_files:
         click.echo(f"Using context files: {', '.join(context_files)}")
     modify_file(file, request, context_files, model)
 
 
 @main.command()
 @click.argument("file")
-@click.option("--error", "-e", default=None, prompt=False,
-              help="Optional error message to debug.")
+@click.option(
+    "--error", "-e", default=None, prompt=False, help="Optional error message to debug."
+)
 @click.option("--model", "-m", type=str, help=MODEL_HELP)
 def debug(file, error, model):
     """Debug an existing file. May include an optional error message"""
     click.echo(f"Debugging file: {file}")
     if error:
         click.echo(f"Error message: {error}")
     debug_file(file, error, model)
@@ -79,9 +96,26 @@
 def spec(file, target_path, model):
     """Build a unit test file for an existing file."""
     click.echo(f"Building spec file for: {file}")
     click.echo(f"Target path: {target_path}")
     build_spec_file(file, target_path, model)
 
 
+@main.command()
+@click.argument("file")
+@click.option(
+    "--context-files",
+    "-c",
+    multiple=True,
+    type=str,
+    help="Optional list of context file paths.",
+)
+@click.option("--verbose", "-v", is_flag=True, help="Verbose output.")
+@click.option("--model", "-m", type=str, help=MODEL_HELP)
+def explain(file, context_files, verbose, model):
+    """Explain the contents of a file."""
+    click.echo(f"Explaining: {file}")
+    explain_file(file, context_files, {"verbose": verbose}, model)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `nail-0.1.1/nail.egg-info/PKG-INFO` & `nail-0.1.2/nail.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nail
-Version: 0.1.1
+Version: 0.1.2
 Summary: A CLI tool for speeding up development using LLMs
 Home-page: https://github.com/edsaav/nail
 Author: Edward Saavedra
 Author-email: edsaav@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,19 +47,44 @@
 
 ```
 nail configure
 ```
 
 This will prompt you to enter your API key, which will be saved for future use.
 
-## Usage
+## Basic Usage
+
+Once you have configured Nail, you can begin using it to generate code. To get started create and navigate to a new project directory. Create a new file and write out what you want the code in that file to do. For example:
+
+```
+# calculator.py
+A python class with addition, subtraction, and multiplication methods
+```
+
+Once you have created and saved your file, run the following command:
+
+```
+nail build calculator.py
+```
+
+After a moment, Nail will generate code meeting that specification and will prompt you to accept or reject the proposed code. If you accept, it will be saved to the file.
+
+What if we want to add to this file? Use the following command to ask Nail to add an additional method.
+
+```
+nail modify calculator.py -r "Add a division method"
+```
+
+Nail will then generate the changes and propose them as a diff that, if accepted, will be saved to the file. Continue reading below to learn about further ways to use Nail to assist in the coding process.
+
+## Usage Details
 
 Nail provides several commands to help you with your code:
 
-### Build 🔨
+### 🔨 Build 🔨
 
 To build a new file with optional context files, use the `build` command:
 
 ```
 nail build <file> [--context-files <file1> <file2> ...] [--model <model>]
 ```
 
@@ -73,71 +98,95 @@
 - returns an array of resulting headings
 ```
 
 If the file does not exist, nail will open your default editor to fill in the prompt in-line.
 
 The `--context-files` (or `-c`) option can be used to pass in one or more additional files that could provide useful reference. For example, you can pass in files containing modules that should be imported and used by the new file that is being built.
 
-### Modify 🔧
+### 🔧 Modify 🔧
 
 To modify an existing file, use the `modify` command:
 
 ```
 nail modify <file> [--request <request>] [--context-files <file1> <file2> ...] [--model <model>]
 ```
 
 The request should be in the form of a command, such as "Add a new function that..." or "Refactor the existing class to...".
 
-### Debug 🐛
+### 🐛 Debug 🐛
 
 To debug an existing file, use the `debug` command:
 
 ```
 nail debug <file> [--error <error_message>] [--model <model>]
 ```
 
 If an error message is not passed, this command will simply look for any possible issues in the given file.
 
-### Generate Unit Tests 🧪
+### 🧪 Generate Unit Tests 🧪
 
 To generate a unit test file for an existing file, use the `spec` command:
 
 ```
 nail spec <file> <target_path> [--model <model>]
 ```
 
 Once they have been generated, test files can be further adjusted with the `modify` command.
 
-### Generate README 📖
+### 🧐 Explain a File 🧐
+
+To explain the contents of a file, use the `explain` command:
+
+```
+nail explain <file> [--context-files <file1> <file2> ...] [--verbose] [--model <model>]
+```
+
+Output will be displayed in the console. More detailed explanations will be generated if the `--verbose` (or `-v`) flag is included.
+
+### 📖 Generate README 📖
 
 To generate a README file for your project, use the `readme` command:
 
 ```
 nail readme [--model <model>]
 ```
 
 This command will gather all application files into context automatically. It will exclude a number of files irrelevant to a README, such as tests and licenses. Please note, this currently only works for relatively small projects given the limited context window available for GPT.
 
+## Customization
+
+There may be situations in which you want Nail to apply specific additional instructions to the LLM. For example, when using the spec tool, you may wish to specify that tests are always written using a specific library. Or, you may wish to define style guidelines that the build and modify commands should always adhere to. Whatever the case, you can configure each Nail command with additional instructions.
+
+To do this, create a `.nail.yaml` file inside your project's root directory. There is a `.sample.nail.yaml` file inside of this repository showing the appropriate format. For any commands you would like to customize, simply add any desired instructions and they will be appended to requests to the LLM.
+
+For example:
+
+```
+prompt_instructions:
+  spec: Use rspec for all unit tests.
+  build: |
+    Do not include inline comments.
+    Avoid deeply nested conditionals wherever possible.
+```
+
 ## Models
 
 Nail currently supports the following models:
 
 - gpt-3.5-turbo (default)
 - gpt-4
 
-You can specify the model to use with the `--model` option for each command.
+You can specify the model to use with the `--model` (or `-m`) option for each command.
 
 ## Development
 
 To install Nail locally for development, clone the repo, then run this command from within the project directory:
 
 ```
 pip3 install -e .
 ```
 
-## Tests
-
 Run the test suite using `pytest`.
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `nail-0.1.1/setup.py` & `nail-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
-    name='nail',
-    version='0.1.1',
-    description='A CLI tool for speeding up development using LLMs',
+    name="nail",
+    version="0.1.2",
+    description="A CLI tool for speeding up development using LLMs",
     packages=find_packages(),
     install_requires=[
-        'click',
-        'openai',
-        'termcolor',
+        "click",
+        "openai",
+        "termcolor",
+        "PyYAML",
+        "rich",
     ],
-    entry_points='''
+    entry_points="""
         [console_scripts]
         nail=nail.main:main
-    ''',
+    """,
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    author='Edward Saavedra',
-    author_email='edsaav@gmail.com',
-    url='https://github.com/edsaav/nail',
+    long_description_content_type="text/markdown",
+    author="Edward Saavedra",
+    author_email="edsaav@gmail.com",
+    url="https://github.com/edsaav/nail",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `nail-0.1.1/tests/core/test_config_utils.py` & `nail-0.1.2/tests/core/test_config_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import configparser
 from unittest import mock
 from unittest.mock import patch
 import pytest
-from nail.core.config_utils import get_api_key, save_api_key
+from nail.core.config.user_config_utils import get_api_key, save_api_key
 
 
 @pytest.fixture
 def temp_config_file(tmp_path):
     temp_file = tmp_path / ".nailrc"
     temp_file.touch()
     return temp_file
@@ -20,26 +20,30 @@
 def test_get_api_key_with_config_file(monkeypatch, temp_config_file):
     monkeypatch.delenv("OPENAI_API_KEY", raising=False)
     config = configparser.ConfigParser()
     config["openai"] = {"api_key": "test_key"}
     with temp_config_file.open("w") as f:
         config.write(f)
 
-    with mock.patch("nail.core.config_utils.CONFIG_FILE", temp_config_file):
+    with mock.patch(
+        "nail.core.config.user_config_utils.USER_CONFIG_FILE", temp_config_file
+    ):
         assert get_api_key() == "test_key"
 
 
 def test_get_api_key_with_no_key(monkeypatch, temp_config_file):
     monkeypatch.delenv("OPENAI_API_KEY", raising=False)
-    with mock.patch("nail.core.config_utils.CONFIG_FILE", temp_config_file):
+    with mock.patch(
+        "nail.core.config.user_config_utils.USER_CONFIG_FILE", temp_config_file
+    ):
         assert get_api_key() is None
 
 
 def test_save_api_key(tmp_path):
     api_key = "test_api_key"
     temp_config_file = tmp_path / ".nailrc"
 
-    with patch("nail.core.config_utils.CONFIG_FILE", temp_config_file):
+    with patch("nail.core.config.user_config_utils.USER_CONFIG_FILE", temp_config_file):
         save_api_key(api_key)
         config = configparser.ConfigParser()
         config.read(temp_config_file)
         assert config["openai"]["api_key"] == api_key
```

### Comparing `nail-0.1.1/tests/test_main.py` & `nail-0.1.2/tests/test_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,24 +31,24 @@
         mock_build_readme.assert_called_once_with("README.md", None)
 
 
 def test_modify(runner):
     with patch("nail.main.modify_file") as mock_modify_file:
         result = runner.invoke(modify, ["test_file", "-r", "test_request"])
         assert result.exit_code == 0
-        mock_modify_file.assert_called_once_with(
-            "test_file", "test_request", ANY, None)
+        mock_modify_file.assert_called_once_with("test_file", "test_request", ANY, None)
 
 
 def test_debug(runner):
     with patch("nail.main.debug_file") as mock_debug_file:
         result = runner.invoke(debug, ["test_file"])
         assert result.exit_code == 0
         mock_debug_file.assert_called_once_with("test_file", None, None)
 
 
 def test_spec(runner):
     with patch("nail.main.build_spec_file") as mock_build_spec_file:
         result = runner.invoke(spec, ["test_file", "test_target_path"])
         assert result.exit_code == 0
         mock_build_spec_file.assert_called_once_with(
-            "test_file", "test_target_path", None)
+            "test_file", "test_target_path", None
+        )
```

