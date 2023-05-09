# Comparing `tmp/phy_qcs-1.0.0.tar.gz` & `tmp/phy_qcs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phy_qcs-1.0.0.tar", last modified: Tue May  9 14:01:28 2023, max compression
+gzip compressed data, was "phy_qcs-1.0.1.tar", last modified: Tue May  9 14:12:16 2023, max compression
```

## Comparing `phy_qcs-1.0.0.tar` & `phy_qcs-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 14:01:28.992625 phy_qcs-1.0.0/
--rw-rw-rw-   0        0        0      867 2023-05-09 14:01:28.992625 phy_qcs-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-09 13:15:19.000000 phy_qcs-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 14:01:28.987638 phy_qcs-1.0.0/phy_qcs/
--rw-rw-rw-   0        0        0    54629 2023-05-09 13:49:52.000000 phy_qcs-1.0.0/phy_qcs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 14:01:28.991627 phy_qcs-1.0.0/phy_qcs.egg-info/
--rw-rw-rw-   0        0        0      867 2023-05-09 14:01:28.000000 phy_qcs-1.0.0/phy_qcs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-05-09 14:01:28.000000 phy_qcs-1.0.0/phy_qcs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 14:01:28.000000 phy_qcs-1.0.0/phy_qcs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-09 14:01:28.000000 phy_qcs-1.0.0/phy_qcs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-09 14:01:28.000000 phy_qcs-1.0.0/phy_qcs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 14:01:28.992625 phy_qcs-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1551 2023-05-09 13:48:07.000000 phy_qcs-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:12:16.495679 phy_qcs-1.0.1/
+-rw-rw-rw-   0        0        0     1011 2023-05-09 14:12:16.495679 phy_qcs-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-09 13:15:19.000000 phy_qcs-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 14:12:16.490694 phy_qcs-1.0.1/phy_qcs/
+-rw-rw-rw-   0        0        0    54629 2023-05-09 13:49:52.000000 phy_qcs-1.0.1/phy_qcs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:12:16.494683 phy_qcs-1.0.1/phy_qcs.egg-info/
+-rw-rw-rw-   0        0        0     1011 2023-05-09 14:12:16.000000 phy_qcs-1.0.1/phy_qcs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-05-09 14:12:16.000000 phy_qcs-1.0.1/phy_qcs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 14:12:16.000000 phy_qcs-1.0.1/phy_qcs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-09 14:12:16.000000 phy_qcs-1.0.1/phy_qcs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-09 14:12:16.000000 phy_qcs-1.0.1/phy_qcs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 14:12:16.496678 phy_qcs-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1692 2023-05-09 14:11:48.000000 phy_qcs-1.0.1/setup.py
```

### Comparing `phy_qcs-1.0.0/PKG-INFO` & `phy_qcs-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: phy_qcs
-Version: 1.0.0
+Version: 1.0.1
 Summary: QCS: Quantum Correlation Solver
 Home-page: 
 Author: ZhiGuang Lu
 Author-email: youngqlzg@gamil.com
 License: BSD
 Keywords: quantum physics higher-order equal-time correlation function
 Platform: Linux
 Platform: Mac OSX
 Platform: Unix
 Platform: Windows
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires: numpy (>=1.8)
 Requires: scipy (>=0.15)
 
 QCS is an open-source Python code that allows to study the single-photon transmission and reflection, as well as the nth-order equal-time correlation functions (ETCFs) in driven-dissipative quantum systems.
```

### Comparing `phy_qcs-1.0.0/phy_qcs/__init__.py` & `phy_qcs-1.0.1/phy_qcs/__init__.py`

 * *Files identical despite different names*

### Comparing `phy_qcs-1.0.0/phy_qcs.egg-info/PKG-INFO` & `phy_qcs-1.0.1/phy_qcs.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: phy-qcs
-Version: 1.0.0
+Version: 1.0.1
 Summary: QCS: Quantum Correlation Solver
 Home-page: 
 Author: ZhiGuang Lu
 Author-email: youngqlzg@gamil.com
 License: BSD
 Keywords: quantum physics higher-order equal-time correlation function
 Platform: Linux
 Platform: Mac OSX
 Platform: Unix
 Platform: Windows
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires: numpy (>=1.8)
 Requires: scipy (>=0.15)
 
 QCS is an open-source Python code that allows to study the single-photon transmission and reflection, as well as the nth-order equal-time correlation functions (ETCFs) in driven-dissipative quantum systems.
```

### Comparing `phy_qcs-1.0.0/setup.py` & `phy_qcs-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # # these things are needed for the README.md show on pypi
 # here = os.path.abspath(os.path.dirname(__file__))
 #
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'QCS: Quantum Correlation Solver'
 LONG_DESCRIPTION = 'QCS is an open-source Python code that allows to study the single-photon transmission and reflection, ' \
                    'as well as the nth-order equal-time correlation functions (ETCFs) in driven-dissipative quantum systems.'
 REQUIRES = ['numpy (>=1.8)', 'scipy (>=0.15)']
 INSTALL_REQUIRES = ['numpy>=1.8', 'scipy>=0.15']
 PLATFORMS = ["Linux", "Mac OSX", "Unix", "Windows"]
 KEYWORDS = "quantum physics higher-order equal-time correlation function"
@@ -27,17 +27,20 @@
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=INSTALL_REQUIRES,
     keywords=KEYWORDS,
     requires=REQUIRES,
     platforms=PLATFORMS,
     classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: BSD License",
+        "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Topic :: Scientific/Engineering",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     license="BSD",
     url="",
 )
```

