# Comparing `tmp/release_verchk_vijkan-0.0.1.tar.gz` & `tmp/release_verchk_vijkan-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "release_verchk_vijkan-0.0.1.tar", last modified: Mon May  8 09:09:44 2023, max compression
+gzip compressed data, was "release_verchk_vijkan-0.0.2.tar", last modified: Tue May  9 14:50:56 2023, max compression
```

## Comparing `release_verchk_vijkan-0.0.1.tar` & `release_verchk_vijkan-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 09:09:44.395530 release_verchk_vijkan-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-25 09:16:43.000000 release_verchk_vijkan-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      616 2023-05-08 09:09:44.395530 release_verchk_vijkan-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-05-04 09:39:16.000000 release_verchk_vijkan-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 09:09:44.395530 release_verchk_vijkan-0.0.1/release_verchk_vijkan.egg-info/
--rw-rw-rw-   0        0        0      616 2023-05-08 09:09:43.000000 release_verchk_vijkan-0.0.1/release_verchk_vijkan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-05-08 09:09:44.000000 release_verchk_vijkan-0.0.1/release_verchk_vijkan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 09:09:43.000000 release_verchk_vijkan-0.0.1/release_verchk_vijkan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 09:09:44.000000 release_verchk_vijkan-0.0.1/release_verchk_vijkan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 09:09:44.395530 release_verchk_vijkan-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1281 2023-05-08 09:09:00.000000 release_verchk_vijkan-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:50:56.880777 release_verchk_vijkan-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 14:50:33.000000 release_verchk_vijkan-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-09 14:50:56.880777 release_verchk_vijkan-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-09 14:50:33.000000 release_verchk_vijkan-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:50:56.880777 release_verchk_vijkan-0.0.2/release_verchk_vijkan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-09 14:50:56.000000 release_verchk_vijkan-0.0.2/release_verchk_vijkan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-09 14:50:56.000000 release_verchk_vijkan-0.0.2/release_verchk_vijkan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:50:56.000000 release_verchk_vijkan-0.0.2/release_verchk_vijkan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:50:56.000000 release_verchk_vijkan-0.0.2/release_verchk_vijkan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:50:56.880777 release_verchk_vijkan-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-09 14:50:33.000000 release_verchk_vijkan-0.0.2/setup.py
```

### Comparing `release_verchk_vijkan-0.0.1/LICENSE.txt` & `release_verchk_vijkan-0.0.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `release_verchk_vijkan-0.0.1/setup.py` & `release_verchk_vijkan-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from setuptools import setup, find_packages
-
-# try:
-#    import pypandoc
-#    long_description = pypandoc.convert_file('README.md', 'rst')
-# except(IOError, ImportError):
-#    long_description = open('README.md').read()
-
-VERSION = '0.0.1' 
-DESCRIPTION = 'Python package to learn Version'
-LONG_DESCRIPTION = 'Python package for Calculation and Display'
-
-# Setting up
-setup(
-       # the name must match the folder name 'vijsamplepackage'
-        name="release_verchk_vijkan", 
-        version=VERSION,
-        author="Vijai Kannan",
-        author_email="vijaik.nd@gmail.com",
-        description="Setting up a python package to learn version",
-        long_description=LONG_DESCRIPTION,
-        packages=find_packages(),
-        install_requires=[], # add any additional packages that 
-        # needs to be installed along with your package. Eg: 'caer'
-        
-        keywords=['python', 'sample package'],
-        classifiers= [
-            "Development Status :: 3 - Alpha",
-            "Intended Audience :: Education",
-            "Programming Language :: Python :: 2",
-            "Programming Language :: Python :: 3",
-            "Operating System :: MacOS :: MacOS X",
-            "Operating System :: Microsoft :: Windows",
-        ]
+from setuptools import setup, find_packages
+
+# try:
+#    import pypandoc
+#    long_description = pypandoc.convert_file('README.md', 'rst')
+# except(IOError, ImportError):
+#    long_description = open('README.md').read()
+
+VERSION = '0.0.2' 
+DESCRIPTION = 'Python package to learn Version'
+LONG_DESCRIPTION = 'Python package for Calculation and Display'
+
+# Setting up
+setup(
+       # the name must match the folder name 'vijsamplepackage'
+        name="release_verchk_vijkan", 
+        version=VERSION,
+        author="Vijai Kannan",
+        author_email="vijaik.nd@gmail.com",
+        description="Setting up a python package to learn version",
+        long_description=LONG_DESCRIPTION,
+        packages=find_packages(),
+        install_requires=[], # add any additional packages that 
+        # needs to be installed along with your package. Eg: 'caer'
+        
+        keywords=['python', 'sample package'],
+        classifiers= [
+            "Development Status :: 3 - Alpha",
+            "Intended Audience :: Education",
+            "Programming Language :: Python :: 2",
+            "Programming Language :: Python :: 3",
+            "Operating System :: MacOS :: MacOS X",
+            "Operating System :: Microsoft :: Windows",
+        ]
 )
```

