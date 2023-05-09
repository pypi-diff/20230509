# Comparing `tmp/SAPsim-1.0.7.tar.gz` & `tmp/SAPsim-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPsim-1.0.7.tar", last modified: Mon May  8 03:22:36 2023, max compression
+gzip compressed data, was "SAPsim-1.0.8.tar", last modified: Tue May  9 00:05:22 2023, max compression
```

## Comparing `SAPsim-1.0.7.tar` & `SAPsim-1.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:36.414992 SAPsim-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 03:22:21.000000 SAPsim-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-08 03:22:36.414992 SAPsim-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-08 03:22:21.000000 SAPsim-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:36.402992 SAPsim-1.0.7/SAPsim/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:36.410992 SAPsim-1.0.7/SAPsim/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-08 03:22:21.000000 SAPsim-1.0.7/SAPsim/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:36.406992 SAPsim-1.0.7/SAPsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-08 03:22:36.000000 SAPsim-1.0.7/SAPsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-08 03:22:36.000000 SAPsim-1.0.7/SAPsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 03:22:36.000000 SAPsim-1.0.7/SAPsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 03:22:36.000000 SAPsim-1.0.7/SAPsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 03:22:36.000000 SAPsim-1.0.7/SAPsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-08 03:22:21.000000 SAPsim-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 03:22:36.414992 SAPsim-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-08 03:22:21.000000 SAPsim-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:36.414992 SAPsim-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 03:22:21.000000 SAPsim-1.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-08 03:22:21.000000 SAPsim-1.0.7/tests/test_example_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-08 03:22:21.000000 SAPsim-1.0.7/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-08 03:22:21.000000 SAPsim-1.0.7/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-08 03:22:21.000000 SAPsim-1.0.7/tests/test_instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 03:22:21.000000 SAPsim-1.0.7/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:05:22.426001 SAPsim-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 00:05:13.000000 SAPsim-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-09 00:05:22.426001 SAPsim-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-09 00:05:13.000000 SAPsim-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:05:22.422001 SAPsim-1.0.8/SAPsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-09 00:05:13.000000 SAPsim-1.0.8/SAPsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:05:22.426001 SAPsim-1.0.8/SAPsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:05:13.000000 SAPsim-1.0.8/SAPsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-09 00:05:13.000000 SAPsim-1.0.8/SAPsim/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-09 00:05:13.000000 SAPsim-1.0.8/SAPsim/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-09 00:05:13.000000 SAPsim-1.0.8/SAPsim/utils/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-09 00:05:13.000000 SAPsim-1.0.8/SAPsim/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-09 00:05:13.000000 SAPsim-1.0.8/SAPsim/utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-05-09 00:05:13.000000 SAPsim-1.0.8/SAPsim/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:05:22.426001 SAPsim-1.0.8/SAPsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-09 00:05:22.000000 SAPsim-1.0.8/SAPsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-09 00:05:22.000000 SAPsim-1.0.8/SAPsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:05:22.000000 SAPsim-1.0.8/SAPsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-09 00:05:22.000000 SAPsim-1.0.8/SAPsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 00:05:22.000000 SAPsim-1.0.8/SAPsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-09 00:05:13.000000 SAPsim-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:05:22.426001 SAPsim-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-09 00:05:13.000000 SAPsim-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:05:22.426001 SAPsim-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:05:13.000000 SAPsim-1.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-09 00:05:13.000000 SAPsim-1.0.8/tests/test_SAPsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-09 00:05:13.000000 SAPsim-1.0.8/tests/test_example_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-09 00:05:13.000000 SAPsim-1.0.8/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-09 00:05:13.000000 SAPsim-1.0.8/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-09 00:05:13.000000 SAPsim-1.0.8/tests/test_instructions.py
```

### Comparing `SAPsim-1.0.7/LICENSE` & `SAPsim-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.7/PKG-INFO` & `SAPsim-1.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 1.0.7
+Version: 1.0.8
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/SAPsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
@@ -35,40 +35,50 @@
 
 Your Python version needs to be 3.9+. Check with `python --version`.
 
 If `python` doesn't work, try `python3`. If `pip` doesn't work, try `pip3`.
 
 ## Usage
 
-Write a SAP program in the CSV file format shown below.
+Write a SAP program in the CSV file format shown below (templates are provided in COMP311's SAP assignment).
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/jesse-wei/SAPsim/main/docs/_static/ex1.jpg" alt="Screenshot of ex1.csv in Excel">
 </p>
 <p align="center">
     <a href="https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex1.csv">ex1.csv</a>
 </p>
 
-You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets, etc.), as long as you preserve the `.csv` extension. For a blank template, see [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv).
+You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets, etc.).
 
-Open a Python terminal. Import SAPsim's `run()` function, and pass the path to your SAP program as an argument.
+To run the SAP program, use `run()`. **Note**: There is a debug (step) mode, as shown below.
 
 ```py
 >>> from SAPsim import run
->>> run("ex1.csv")                 # Run ex1.csv at full speed (default)
+>>> run("ex1.csv")                  # Run ex1.csv at full speed (default)
 ...
->>> run("ex1.csv", debug=True)     # Run ex1.csv in debug (step) mode
+>>> run("ex1.csv", debug=True)      # Run ex1.csv in debug (step) mode
 ...
 ```
 
-**Note**: There is a debug (step) mode, as shown above.
+If you want a blank template, use `create_template()`.
+
+```py
+>>> from SAPsim import create_template
+>>> create_template()
+template.csv successfully created.
+```
 
 ## Settings
 
-Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., printed table format).
+Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings).
+
+`change` allows you to modify values in the SAP program without editing the CSV, which is convenient.
+
+`table_format` allows you to customize the appearance of the printed tables.
 
 ## Rules
 
 It's easy to just mimic the [example programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but if you need it, here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SAPsim Version: 1.0.7 Summary: Simulation of SAP
+Metadata-Version: 2.1 Name: SAPsim Version: 1.0.8 Summary: Simulation of SAP
 (Simple As Possible) computer programs from COMP311 (Computer Organization) @
 UNC Home-page: https://github.com/jesse-wei/SAPsim Download-URL: https://
 github.com/jesse-wei/SAPsim/releases Author: Jesse Wei Author-email: Jesse Wei
 cs.unc.edu> Project-URL: Homepage, https://github.com/jesse-wei/SAPsim Project-
 URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues Keywords:
 SAP,SAPsim,simple as possible,UNC,COMP311 Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -16,26 +16,28 @@
 SAPsim Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/
 img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://
 unc.edu).
                                  [SAPsim demo]
 ## Install `pip install SAPsim` Your Python version needs to be 3.9+. Check
 with `python --version`. If `python` doesn't work, try `python3`. If `pip`
 doesn't work, try `pip3`. ## Usage Write a SAP program in the CSV file format
-shown below.
+shown below (templates are provided in COMP311's SAP assignment).
                        [Screenshot of ex1.csv in Excel]
                                     ex1.csv
 You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets,
-etc.), as long as you preserve the `.csv` extension. For a blank template, see
-[template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv).
-Open a Python terminal. Import SAPsim's `run()` function, and pass the path to
-your SAP program as an argument. ```py >>> from SAPsim import run >>> run
-("ex1.csv") # Run ex1.csv at full speed (default) ... >>> run("ex1.csv",
-debug=True) # Run ex1.csv in debug (step) mode ... ``` **Note**: There is a
-debug (step) mode, as shown above. ## Settings Here's a list of [additional
-settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., printed
-table format). ## Rules It's easy to just mimic the [example programs](https://
-github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but if you need it,
-here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/
-en/latest/rules.html). ## SAP instruction set
+etc.). To run the SAP program, use `run()`. **Note**: There is a debug (step)
+mode, as shown below. ```py >>> from SAPsim import run >>> run("ex1.csv") # Run
+ex1.csv at full speed (default) ... >>> run("ex1.csv", debug=True) # Run
+ex1.csv in debug (step) mode ... ``` If you want a blank template, use
+`create_template()`. ```py >>> from SAPsim import create_template >>>
+create_template() template.csv successfully created. ``` ## Settings Here's a
+list of [additional settings](https://SAPsim.readthedocs.io/en/latest/
+#settings). `change` allows you to modify values in the SAP program without
+editing the CSV, which is convenient. `table_format` allows you to customize
+the appearance of the printed tables. ## Rules It's easy to just mimic the
+[example programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/
+public_prog), but if you need it, here's the list of [rules for SAPsim
+programs](https://SAPsim.readthedocs.io/en/latest/rules.html). ## SAP
+instruction set
                              [SAP instruction set]
 ## Documentation [https://SAPsim.readthedocs.io](https://SAPsim.readthedocs.io/
 en/latest/)
```

### Comparing `SAPsim-1.0.7/README.md` & `SAPsim-1.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,40 +15,50 @@
 
 Your Python version needs to be 3.9+. Check with `python --version`.
 
 If `python` doesn't work, try `python3`. If `pip` doesn't work, try `pip3`.
 
 ## Usage
 
-Write a SAP program in the CSV file format shown below.
+Write a SAP program in the CSV file format shown below (templates are provided in COMP311's SAP assignment).
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/jesse-wei/SAPsim/main/docs/_static/ex1.jpg" alt="Screenshot of ex1.csv in Excel">
 </p>
 <p align="center">
     <a href="https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex1.csv">ex1.csv</a>
 </p>
 
-You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets, etc.), as long as you preserve the `.csv` extension. For a blank template, see [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv).
+You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets, etc.).
 
-Open a Python terminal. Import SAPsim's `run()` function, and pass the path to your SAP program as an argument.
+To run the SAP program, use `run()`. **Note**: There is a debug (step) mode, as shown below.
 
 ```py
 >>> from SAPsim import run
->>> run("ex1.csv")                 # Run ex1.csv at full speed (default)
+>>> run("ex1.csv")                  # Run ex1.csv at full speed (default)
 ...
->>> run("ex1.csv", debug=True)     # Run ex1.csv in debug (step) mode
+>>> run("ex1.csv", debug=True)      # Run ex1.csv in debug (step) mode
 ...
 ```
 
-**Note**: There is a debug (step) mode, as shown above.
+If you want a blank template, use `create_template()`.
+
+```py
+>>> from SAPsim import create_template
+>>> create_template()
+template.csv successfully created.
+```
 
 ## Settings
 
-Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., printed table format).
+Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings).
+
+`change` allows you to modify values in the SAP program without editing the CSV, which is convenient.
+
+`table_format` allows you to customize the appearance of the printed tables.
 
 ## Rules
 
 It's easy to just mimic the [example programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but if you need it, here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
```

#### html2text {}

```diff
@@ -5,26 +5,28 @@
 Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/
 sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://
 unc.edu).
                                  [SAPsim demo]
 ## Install `pip install SAPsim` Your Python version needs to be 3.9+. Check
 with `python --version`. If `python` doesn't work, try `python3`. If `pip`
 doesn't work, try `pip3`. ## Usage Write a SAP program in the CSV file format
-shown below.
+shown below (templates are provided in COMP311's SAP assignment).
                        [Screenshot of ex1.csv in Excel]
                                     ex1.csv
 You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets,
-etc.), as long as you preserve the `.csv` extension. For a blank template, see
-[template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv).
-Open a Python terminal. Import SAPsim's `run()` function, and pass the path to
-your SAP program as an argument. ```py >>> from SAPsim import run >>> run
-("ex1.csv") # Run ex1.csv at full speed (default) ... >>> run("ex1.csv",
-debug=True) # Run ex1.csv in debug (step) mode ... ``` **Note**: There is a
-debug (step) mode, as shown above. ## Settings Here's a list of [additional
-settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., printed
-table format). ## Rules It's easy to just mimic the [example programs](https://
-github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but if you need it,
-here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/
-en/latest/rules.html). ## SAP instruction set
+etc.). To run the SAP program, use `run()`. **Note**: There is a debug (step)
+mode, as shown below. ```py >>> from SAPsim import run >>> run("ex1.csv") # Run
+ex1.csv at full speed (default) ... >>> run("ex1.csv", debug=True) # Run
+ex1.csv in debug (step) mode ... ``` If you want a blank template, use
+`create_template()`. ```py >>> from SAPsim import create_template >>>
+create_template() template.csv successfully created. ``` ## Settings Here's a
+list of [additional settings](https://SAPsim.readthedocs.io/en/latest/
+#settings). `change` allows you to modify values in the SAP program without
+editing the CSV, which is convenient. `table_format` allows you to customize
+the appearance of the printed tables. ## Rules It's easy to just mimic the
+[example programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/
+public_prog), but if you need it, here's the list of [rules for SAPsim
+programs](https://SAPsim.readthedocs.io/en/latest/rules.html). ## SAP
+instruction set
                              [SAP instruction set]
 ## Documentation [https://SAPsim.readthedocs.io](https://SAPsim.readthedocs.io/
 en/latest/)
```

### Comparing `SAPsim-1.0.7/SAPsim/__init__.py` & `SAPsim-1.0.8/SAPsim/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 from typing import Union, Any
 from SAPsim.utils.helpers import is_documented_by
+from SAPsim.utils.global_vars import MAX_PC
 import SAPsim.utils.execute as execute
 
 
 # Weird glitch, passing in the function doesn't actually get its docstring? Just append then
 @is_documented_by(execute.run, 0, "", execute.run.__doc__)
 def run(prog_path: str, **kwargs) -> Union[None, dict[str, Any]]:
     return execute.run(prog_path, **kwargs)
 
 
-def create_template() -> None:
+def create_template(path: str = "template.csv") -> None:
     r"""
-    Create blank ``template.csv`` file in SAPsim format in current directory.
+    Create blank template file in SAPsim format in current directory.
+
+    :param path: Path to create template file at. Defaults to ``template.csv``.
+    :type path: str
+    :return: None
     """
     # This will rarely be used so doesn't need to be imported at top level
     import csv
 
     header: list[str] = ["Address", "First Hexit", "Second Hexit", "Comments"]
-    with open("template.csv", "w") as f:
+    with open(path, "w") as f:
         writer = csv.writer(f)
         writer.writerow(header)
-        for i in range(16):
+        for i in range(MAX_PC):
             writer.writerow([f"{i}", "", "", ""])
+    print(f"{path} successfully created.")
```

### Comparing `SAPsim-1.0.7/SAPsim/utils/exceptions.py` & `SAPsim-1.0.8/SAPsim/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.7/SAPsim/utils/execute.py` & `SAPsim-1.0.8/SAPsim/utils/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                 * This is used to save computation time during unit testing
                 * If ``True``, then ``print()`` won't be called, except for error messages
             * *bits* (``int``) --
                 * Number of bits in unsigned registers
                 * Default value in ``global_vars`` is 8
 
     :return: ``None`` or program state if ``return_state``
-    :rtype: Union[None, dict[str, Any]]
+    :rtype: ``Union[None, dict[str, Any]]``
     """
     if not isinstance(prog_path, str):
         raise TypeError("Required parameter prog_path must be a str.")
     if "debug" in kwargs and not isinstance(kwargs["debug"], bool):
         raise TypeError("Keyword argument debug must be a bool.")
     if "change" in kwargs and not isinstance(kwargs["change"], str):
         raise TypeError("Keyword argument change must be a str.")
```

### Comparing `SAPsim-1.0.7/SAPsim/utils/global_vars.py` & `SAPsim-1.0.8/SAPsim/utils/global_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 # Same as number of full adders
 # This affects how FLAG_C, FLAG_Z, and result register work
 NUM_BITS_IN_REGISTERS: int = 8
 """This variable is the #bits in registers and affects how ``add``, ``sub``, ``ldi``, and ``lda`` work.
 Default value is 8."""
 EXECUTING: bool = True
 """Is the program executing? Set to ``False`` by ``hlt()``"""
+MAX_PC: int = 16
+"""Max PC value."""
 
 MNEMONIC_TO_OPCODE: bidict = bidict(
     {
         "NOP": 0,
         "LDA": 1,
         "ADD": 2,
         "SUB": 3,
```

### Comparing `SAPsim-1.0.7/SAPsim/utils/helpers.py` & `SAPsim-1.0.8/SAPsim/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.7/SAPsim/utils/instructions.py` & `SAPsim-1.0.8/SAPsim/utils/instructions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.7/SAPsim.egg-info/PKG-INFO` & `SAPsim-1.0.8/SAPsim.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 1.0.7
+Version: 1.0.8
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/SAPsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
@@ -35,40 +35,50 @@
 
 Your Python version needs to be 3.9+. Check with `python --version`.
 
 If `python` doesn't work, try `python3`. If `pip` doesn't work, try `pip3`.
 
 ## Usage
 
-Write a SAP program in the CSV file format shown below.
+Write a SAP program in the CSV file format shown below (templates are provided in COMP311's SAP assignment).
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/jesse-wei/SAPsim/main/docs/_static/ex1.jpg" alt="Screenshot of ex1.csv in Excel">
 </p>
 <p align="center">
     <a href="https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex1.csv">ex1.csv</a>
 </p>
 
-You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets, etc.), as long as you preserve the `.csv` extension. For a blank template, see [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv).
+You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets, etc.).
 
-Open a Python terminal. Import SAPsim's `run()` function, and pass the path to your SAP program as an argument.
+To run the SAP program, use `run()`. **Note**: There is a debug (step) mode, as shown below.
 
 ```py
 >>> from SAPsim import run
->>> run("ex1.csv")                 # Run ex1.csv at full speed (default)
+>>> run("ex1.csv")                  # Run ex1.csv at full speed (default)
 ...
->>> run("ex1.csv", debug=True)     # Run ex1.csv in debug (step) mode
+>>> run("ex1.csv", debug=True)      # Run ex1.csv in debug (step) mode
 ...
 ```
 
-**Note**: There is a debug (step) mode, as shown above.
+If you want a blank template, use `create_template()`.
+
+```py
+>>> from SAPsim import create_template
+>>> create_template()
+template.csv successfully created.
+```
 
 ## Settings
 
-Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., printed table format).
+Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings).
+
+`change` allows you to modify values in the SAP program without editing the CSV, which is convenient.
+
+`table_format` allows you to customize the appearance of the printed tables.
 
 ## Rules
 
 It's easy to just mimic the [example programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but if you need it, here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SAPsim Version: 1.0.7 Summary: Simulation of SAP
+Metadata-Version: 2.1 Name: SAPsim Version: 1.0.8 Summary: Simulation of SAP
 (Simple As Possible) computer programs from COMP311 (Computer Organization) @
 UNC Home-page: https://github.com/jesse-wei/SAPsim Download-URL: https://
 github.com/jesse-wei/SAPsim/releases Author: Jesse Wei Author-email: Jesse Wei
 cs.unc.edu> Project-URL: Homepage, https://github.com/jesse-wei/SAPsim Project-
 URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues Keywords:
 SAP,SAPsim,simple as possible,UNC,COMP311 Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -16,26 +16,28 @@
 SAPsim Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/
 img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://
 unc.edu).
                                  [SAPsim demo]
 ## Install `pip install SAPsim` Your Python version needs to be 3.9+. Check
 with `python --version`. If `python` doesn't work, try `python3`. If `pip`
 doesn't work, try `pip3`. ## Usage Write a SAP program in the CSV file format
-shown below.
+shown below (templates are provided in COMP311's SAP assignment).
                        [Screenshot of ex1.csv in Excel]
                                     ex1.csv
 You may edit the `.csv` file with any program (Microsoft Excel, Google Sheets,
-etc.), as long as you preserve the `.csv` extension. For a blank template, see
-[template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv).
-Open a Python terminal. Import SAPsim's `run()` function, and pass the path to
-your SAP program as an argument. ```py >>> from SAPsim import run >>> run
-("ex1.csv") # Run ex1.csv at full speed (default) ... >>> run("ex1.csv",
-debug=True) # Run ex1.csv in debug (step) mode ... ``` **Note**: There is a
-debug (step) mode, as shown above. ## Settings Here's a list of [additional
-settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., printed
-table format). ## Rules It's easy to just mimic the [example programs](https://
-github.com/jesse-wei/SAPsim/tree/main/tests/public_prog), but if you need it,
-here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/
-en/latest/rules.html). ## SAP instruction set
+etc.). To run the SAP program, use `run()`. **Note**: There is a debug (step)
+mode, as shown below. ```py >>> from SAPsim import run >>> run("ex1.csv") # Run
+ex1.csv at full speed (default) ... >>> run("ex1.csv", debug=True) # Run
+ex1.csv in debug (step) mode ... ``` If you want a blank template, use
+`create_template()`. ```py >>> from SAPsim import create_template >>>
+create_template() template.csv successfully created. ``` ## Settings Here's a
+list of [additional settings](https://SAPsim.readthedocs.io/en/latest/
+#settings). `change` allows you to modify values in the SAP program without
+editing the CSV, which is convenient. `table_format` allows you to customize
+the appearance of the printed tables. ## Rules It's easy to just mimic the
+[example programs](https://github.com/jesse-wei/SAPsim/tree/main/tests/
+public_prog), but if you need it, here's the list of [rules for SAPsim
+programs](https://SAPsim.readthedocs.io/en/latest/rules.html). ## SAP
+instruction set
                              [SAP instruction set]
 ## Documentation [https://SAPsim.readthedocs.io](https://SAPsim.readthedocs.io/
 en/latest/)
```

### Comparing `SAPsim-1.0.7/SAPsim.egg-info/SOURCES.txt` & `SAPsim-1.0.8/SAPsim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 SAPsim/utils/exceptions.py
 SAPsim/utils/execute.py
 SAPsim/utils/global_vars.py
 SAPsim/utils/helpers.py
 SAPsim/utils/instructions.py
 SAPsim/utils/parser.py
 tests/__init__.py
+tests/test_SAPsim.py
 tests/test_example_progs.py
 tests/test_exceptions.py
 tests/test_helpers.py
-tests/test_instructions.py
-tests/test_run.py
+tests/test_instructions.py
```

### Comparing `SAPsim-1.0.7/pyproject.toml` & `SAPsim-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.7/setup.py` & `SAPsim-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """All required (i.e., for functionality) dependencies that are installed when running `pip install SAPsim`.
 
 Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="SAPsim",
     # Check https://pypi.org/project/SAPsim/ for latest version number
-    version="1.0.7",
+    version="1.0.8",
     description="Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC.",
     author="Jesse Wei",
     author_email="jesse@cs.unc.edu",
     url="https://github.com/jesse-wei/SAPsim",
     download_url="https://github.com/jesse-wei/SAPsim/releases",
     keywords=[
         "SAP",
```

### Comparing `SAPsim-1.0.7/tests/test_example_progs.py` & `SAPsim-1.0.8/tests/test_example_progs.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.7/tests/test_exceptions.py` & `SAPsim-1.0.8/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.7/tests/test_helpers.py` & `SAPsim-1.0.8/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.7/tests/test_instructions.py` & `SAPsim-1.0.8/tests/test_instructions.py`

 * *Files identical despite different names*

