# Comparing `tmp/peitho_data-2.1.4.tar.gz` & `tmp/peitho_data-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peitho_data-2.1.4.tar", last modified: Tue Apr 25 10:27:08 2023, max compression
+gzip compressed data, was "peitho_data-2.2.0.tar", last modified: Tue May  9 09:51:19 2023, max compression
```

## Comparing `peitho_data-2.1.4.tar` & `peitho_data-2.2.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.933914 peitho_data-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 10:27:08.000000 peitho_data-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 10:27:08.000000 peitho_data-2.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 10:27:08.933914 peitho_data-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-25 10:27:08.000000 peitho_data-2.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data/
--rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/Ubuntu-B.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/datafication/epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data/graph/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/graph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/graph/visualization/file_based_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/machine_learning/concept_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.933914 peitho_data-2.1.4/peitho_data/tests/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/datafication/test_epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.933914 peitho_data-2.1.4/peitho_data/tests/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.933914 peitho_data-2.1.4/peitho_data/tests/graph/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/graph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/graph/visualization/test_file_based_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.933914 peitho_data-2.1.4/peitho_data/tests/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/machine_learning/test_concept_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/test_trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/tests/test_word_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data/word_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:27:08.929914 peitho_data-2.1.4/peitho_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 10:27:08.000000 peitho_data-2.1.4/peitho_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 10:27:08.933914 peitho_data-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-25 10:27:08.000000 peitho_data-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.975470 peitho_data-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 09:51:18.000000 peitho_data-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 09:51:18.000000 peitho_data-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-09 09:51:19.975470 peitho_data-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-09 09:51:18.000000 peitho_data-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/Ubuntu-B.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/datafication/epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/graph/knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/graph/visualization/file_based_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/machine_learning/concept_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/tests/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/datafication/test_epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/tests/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/graph/test_knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data/tests/graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/graph/visualization/test_file_based_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.975470 peitho_data-2.2.0/peitho_data/tests/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/machine_learning/test_concept_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/test_trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/tests/test_word_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-09 09:51:18.000000 peitho_data-2.2.0/peitho_data/word_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:51:19.971470 peitho_data-2.2.0/peitho_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-09 09:51:19.000000 peitho_data-2.2.0/peitho_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-09 09:51:19.000000 peitho_data-2.2.0/peitho_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:51:19.000000 peitho_data-2.2.0/peitho_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:51:19.000000 peitho_data-2.2.0/peitho_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 09:51:19.000000 peitho_data-2.2.0/peitho_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 09:51:19.000000 peitho_data-2.2.0/peitho_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 09:51:19.975470 peitho_data-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-09 09:51:18.000000 peitho_data-2.2.0/setup.py
```

### Comparing `peitho_data-2.1.4/LICENSE` & `peitho_data-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.4/README.md` & `peitho_data-2.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,21 @@
     <img alt="永恒" src="./theme/韶光抚月-天下人间.png">
     Raiden Shogun (雷电将军), the character of eternity, themes my never-ending focus on data in general
 </a>
 
 <br>
 <br>
 
-[ ![PyPI](https://img.shields.io/pypi/v/peitho-data?logo=pypi&logoColor=white&style=for-the-badge) ](https://pypi.org/project/peitho-data/)
-[ ![Read the Docs (version)](https://img.shields.io/readthedocs/peitho-data/latest?logo=Read%20the%20Docs&logoColor=white&style=for-the-badge) ](https://peitho-data.readthedocs.io/en/latest/)
-[ ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/QubitPi/peitho-data/Release?logo=github&style=for-the-badge) ](https://github.com/QubitPi/peitho-data/actions/workflows/release.yml)
+[![PyPI](https://img.shields.io/pypi/v/peitho-data?logo=pypi&logoColor=white&style=for-the-badge)](https://pypi.org/project/peitho-data/)
+[![Read the Docs (version)](https://img.shields.io/readthedocs/peitho-data/latest?logo=Read%20the%20Docs&logoColor=white&style=for-the-badge)](https://peitho-data.readthedocs.io/en/latest/)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/QubitPi/peitho-data/release.yml?logo=github&style=for-the-badge)](https://github.com/QubitPi/peitho-data/actions/workflows/release.yml)
 
-[ ![Discord](https://img.shields.io/discord/1005754525942030366?logo=discord&logoColor=white&style=for-the-badge) ](https://discord.com/widget?id=1005754525942030366&theme=dark)
-[ ![Project Management](https://img.shields.io/badge/Project%20Management-0052CC?style=for-the-badge&logo=trello&logoColor=white) ](https://trello.com/b/ersqV9rd)
-[![License Badge](https://img.shields.io/badge/Apache%202.0-F25910.svg?style=for-the-badge&logo=Apache&logoColor=white) ](https://www.apache.org/licenses/LICENSE-2.0)
+[![Discord](https://img.shields.io/discord/1005754525942030366?logo=discord&logoColor=white&style=for-the-badge)](https://discord.com/widget?id=1005754525942030366&theme=dark)
+[![Project Management](https://img.shields.io/badge/Project%20Management-0052CC?style=for-the-badge&logo=trello&logoColor=white)](https://trello.com/b/ersqV9rd)
+[![License Badge](https://img.shields.io/badge/Apache%202.0-F25910.svg?style=for-the-badge&logo=Apache&logoColor=white)](https://www.apache.org/licenses/LICENSE-2.0)
 ![GitHub last commit (branch)](https://img.shields.io/github/last-commit/QubitPi/peitho-data/master?logo=github&style=for-the-badge)
 
 [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-data&metric=bugs)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
 [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-data&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
 [![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-data&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-data&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-data&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
   [æ°¸æ]_Raiden_Shogun_(é·çµå°å),_the_character_of_eternity,_themes_my
                     never-ending_focus_on_data_in_general
 
-                [ ![PyPI](https://img.shields.io/pypi/v/peitho-
-data?logo=pypi&logoColor=white&style=for-the-badge) ](https://pypi.org/project/
-peitho-data/) [ ![Read the Docs (version)](https://img.shields.io/readthedocs/
-peitho-data/latest?logo=Read%20the%20Docs&logoColor=white&style=for-the-badge)
- ](https://peitho-data.readthedocs.io/en/latest/) [ ![GitHub Workflow Status]
-      (https://img.shields.io/github/workflow/status/QubitPi/peitho-data/
- Release?logo=github&style=for-the-badge) ](https://github.com/QubitPi/peitho-
-   data/actions/workflows/release.yml) [ ![Discord](https://img.shields.io/
-discord/1005754525942030366?logo=discord&logoColor=white&style=for-the-badge) ]
-  (https://discord.com/widget?id=1005754525942030366&theme=dark) [ ![Project
+                [![PyPI](https://img.shields.io/pypi/v/peitho-
+data?logo=pypi&logoColor=white&style=for-the-badge)](https://pypi.org/project/
+ peitho-data/) [![Read the Docs (version)](https://img.shields.io/readthedocs/
+peitho-data/latest?logo=Read%20the%20Docs&logoColor=white&style=for-the-badge)]
+  (https://peitho-data.readthedocs.io/en/latest/) [![GitHub Workflow Status]
+  (https://img.shields.io/github/actions/workflow/status/QubitPi/peitho-data/
+   release.yml?logo=github&style=for-the-badge)](https://github.com/QubitPi/
+peitho-data/actions/workflows/release.yml) [![Discord](https://img.shields.io/
+discord/1005754525942030366?logo=discord&logoColor=white&style=for-the-badge)]
+   (https://discord.com/widget?id=1005754525942030366&theme=dark) [![Project
 Management](https://img.shields.io/badge/Project%20Management-0052CC?style=for-
-  the-badge&logo=trello&logoColor=white) ](https://trello.com/b/ersqV9rd) [!
+   the-badge&logo=trello&logoColor=white)](https://trello.com/b/ersqV9rd) [!
 [License Badge](https://img.shields.io/badge/Apache%202.0-F25910.svg?style=for-
-   the-badge&logo=Apache&logoColor=white) ](https://www.apache.org/licenses/
+   the-badge&logo=Apache&logoColor=white)](https://www.apache.org/licenses/
 LICENSE-2.0) ![GitHub last commit (branch)](https://img.shields.io/github/last-
   commit/QubitPi/peitho-data/master?logo=github&style=for-the-badge) [![Bugs]
    (https://sonarcloud.io/api/project_badges/measure?project=QubitPi_peitho-
  data&metric=bugs)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-
       data) [![Vulnerabilities](https://sonarcloud.io/api/project_badges/
      measure?project=QubitPi_peitho-data&metric=vulnerabilities)](https://
 sonarcloud.io/summary/new_code?id=QubitPi_peitho-data) [![Duplicated Lines (%)]
```

### Comparing `peitho_data-2.1.4/peitho_data/Ubuntu-B.ttf` & `peitho_data-2.2.0/peitho_data/Ubuntu-B.ttf`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.4/peitho_data/datafication/epub.py` & `peitho_data-2.2.0/peitho_data/datafication/epub.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.4/peitho_data/graph/visualization/file_based_visualization.py` & `peitho_data-2.2.0/peitho_data/graph/visualization/file_based_visualization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-from pathlib import Path
+# Copyright Jiaqi Liu
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 import json
 
 import matplotlib.pyplot as plt
 import networkx as nx
 
 
 def __get_data(json_abs_path: str) -> dict[str, list[dict]]:
@@ -84,15 +96,12 @@
         graph,
         pos,
         edge_labels={(link["source"], link["target"]): link["fields"]["label"] for link in data["links"]},
         font_color='red'
     )
     plt.axis('off')
 
-    filename: str = Path(json_abs_path).stem
-
-    plt.savefig(filename + ".png", format="PNG")
     plt.show()
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `peitho_data-2.1.4/peitho_data/machine_learning/concept_learning.py` & `peitho_data-2.2.0/peitho_data/machine_learning/concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.4/peitho_data/tests/machine_learning/test_concept_learning.py` & `peitho_data-2.2.0/peitho_data/tests/machine_learning/test_concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.4/peitho_data/tests/test_trello_api.py` & `peitho_data-2.2.0/peitho_data/tests/test_trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.4/peitho_data/tests/test_word_cloud.py` & `peitho_data-2.2.0/peitho_data/tests/test_word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.4/peitho_data/trello_api.py` & `peitho_data-2.2.0/peitho_data/trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.4/peitho_data/word_cloud.py` & `peitho_data-2.2.0/peitho_data/word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.1.4/peitho_data.egg-info/SOURCES.txt` & `peitho_data-2.2.0/peitho_data.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 peitho_data.egg-info/dependency_links.txt
 peitho_data.egg-info/not-zip-safe
 peitho_data.egg-info/requires.txt
 peitho_data.egg-info/top_level.txt
 peitho_data/datafication/__init__.py
 peitho_data/datafication/epub.py
 peitho_data/graph/__init__.py
+peitho_data/graph/knowledge_graph_spec.py
 peitho_data/graph/visualization/__init__.py
 peitho_data/graph/visualization/file_based_visualization.py
 peitho_data/machine_learning/__init__.py
 peitho_data/machine_learning/concept_learning.py
 peitho_data/tests/__init__.py
 peitho_data/tests/test_trello_api.py
 peitho_data/tests/test_word_cloud.py
 peitho_data/tests/datafication/__init__.py
 peitho_data/tests/datafication/test_epub.py
 peitho_data/tests/graph/__init__.py
+peitho_data/tests/graph/test_knowledge_graph_spec.py
 peitho_data/tests/graph/visualization/__init__.py
 peitho_data/tests/graph/visualization/test_file_based_visualization.py
 peitho_data/tests/machine_learning/__init__.py
 peitho_data/tests/machine_learning/test_concept_learning.py
```

### Comparing `peitho_data-2.1.4/setup.py` & `peitho_data-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="peitho_data",
-    version="2.1.4",
+    version="2.2.0",
     description="An opinionated Python package on Big Data Analytics",
     url="https://github.com/QubitPi/peitho-data",
     author="Jiaqi liu",
     author_email="jack20191124@proton.me",
     license="Apache-2.0",
     packages=find_packages(),
     python_requires='>=3.10',
```

