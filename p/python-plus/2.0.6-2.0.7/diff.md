# Comparing `tmp/python_plus-2.0.6.tar.gz` & `tmp/python_plus-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_plus-2.0.6.tar", last modified: Fri Apr 14 17:17:42 2023, max compression
+gzip compressed data, was "dist/python_plus-2.0.7.tar", last modified: Tue May  9 17:40:32 2023, max compression
```

## Comparing `python_plus-2.0.6.tar` & `python_plus-2.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:17:42.490855 python_plus-2.0.6/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6979 2023-04-14 17:17:42.490855 python_plus-2.0.6/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15133 2023-04-14 17:17:41.000000 python_plus-2.0.6/README.rst
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:17:42.490855 python_plus-2.0.6/python_plus/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8668 2023-03-25 15:58:03.000000 python_plus-2.0.6/python_plus/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1177 2023-03-25 15:58:03.000000 python_plus-2.0.6/python_plus/__main__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:17:42.490855 python_plus-2.0.6/python_plus/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       93 2022-12-09 05:08:44.000000 python_plus-2.0.6/python_plus/scripts/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    48185 2023-04-14 13:58:36.000000 python_plus-2.0.6/python_plus/scripts/list_requirements.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6398 2023-03-25 15:58:03.000000 python_plus-2.0.6/python_plus/scripts/main.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7581 2023-04-14 17:17:01.000000 python_plus-2.0.6/python_plus/scripts/setup.info
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 python_plus-2.0.6/python_plus/scripts/vem.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    66051 2023-04-14 17:14:36.000000 python_plus-2.0.6/python_plus/scripts/vem.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3696 2022-12-09 05:08:44.000000 python_plus-2.0.6/python_plus/vem.man
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:17:42.490855 python_plus-2.0.6/python_plus.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6979 2023-04-14 17:17:42.000000 python_plus-2.0.6/python_plus.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      519 2023-04-14 17:17:42.000000 python_plus-2.0.6/python_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-14 17:17:42.000000 python_plus-2.0.6/python_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      169 2023-04-14 17:17:42.000000 python_plus-2.0.6/python_plus.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:33:53.000000 python_plus-2.0.6/python_plus.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        6 2023-04-14 17:17:42.000000 python_plus-2.0.6/python_plus.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       12 2023-04-14 17:17:42.000000 python_plus-2.0.6/python_plus.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-14 17:17:42.490855 python_plus-2.0.6/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7581 2023-03-25 15:58:03.000000 python_plus-2.0.6/setup.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:40:32.000000 python_plus-2.0.7/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1177 2023-05-09 15:53:59.000000 python_plus-2.0.7/python_plus/__main__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7608 2023-05-09 11:58:50.000000 python_plus-2.0.7/python_plus/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-05-09 15:53:59.000000 python_plus-2.0.7/python_plus/scripts/main.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 python_plus-2.0.7/python_plus/scripts/vem.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    54303 2023-05-09 15:53:59.000000 python_plus-2.0.7/python_plus/scripts/list_requirements.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    68223 2023-05-09 15:53:59.000000 python_plus-2.0.7/python_plus/scripts/vem.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       93 2022-12-09 05:08:44.000000 python_plus-2.0.7/python_plus/scripts/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8668 2023-05-09 15:53:59.000000 python_plus-2.0.7/python_plus/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3696 2022-12-09 05:08:44.000000 python_plus-2.0.7/python_plus/vem.man
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       12 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:33:53.000000 python_plus-2.0.7/python_plus.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      169 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      519 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       26 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8055 2023-05-09 17:40:32.000000 python_plus-2.0.7/python_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-09 17:40:32.000000 python_plus-2.0.7/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7608 2023-05-09 15:53:59.000000 python_plus-2.0.7/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8055 2023-05-09 17:40:32.000000 python_plus-2.0.7/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15133 2023-05-09 17:40:32.000000 python_plus-2.0.7/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `python_plus-2.0.6/PKG-INFO` & `python_plus-2.0.7/python_plus.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,160 +1,158 @@
-Metadata-Version: 2.1
-Name: python_plus
-Version: 2.0.6
+Metadata-Version: 1.2
+Name: python-plus
+Version: 2.0.7
 Summary: python useful function
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
 Project-URL: Source, https://github.com/zeroincombenze/tools
+Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
+Description: 
+        Python supplemental features
+        ----------------------------
+        
+        python-plus adds various features to python 2 and python 3 programs.
+        It is designed to be used as integration of pypi future to help to port your code from Python 2 to Python 3 and still have it run on Python 2.
+        
+        
+        list_requirements.py: list environment requirements
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        This command is an internal command of python-plus but may be used as own command.
+        list_requirements.py displays the pypi and binaries packages needed to create a virtual environment.
+        It is specially designed to show Odoo requirements.
+        Passing Odoo path it reads requirements.txt files in path and setup directories of OCA repositories.
+        
+        vem: virtual environment manager
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        This command is an interactive tool with some nice features to manage standard virtual environment.
+        Mainly it works ad standard pip but inside a specific virtual environment.
+        
+        vem: virtual environment manager
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        ::
+        
+            Usage: vem.sh [-h][-a list][-BCD][-d paths][-E distro][-f][-F name][-gkIi][-l iso][-n][-O version][-o dir][-p pyver][-q][-r file][-stVvy] p3 p4 p5 p6 p7 p8 p9
+            Manage virtual environment
+            action may be: help amend cp check create exec info inspect install merge mv python shell rm show uninstall update test
+             -h --help            this help
+             -a list              bin packages to install (* means wkhtmltopdf,lessc)
+             -B                   use unstable packages: -B testpypi / -BB from ~/tools / -BBB from ~/pypi / -BBBB link to local ~/pypi
+             -C                   clear cache before executing pip command
+             -D --devel           create v.environment with development packages
+             -d --dep-path paths
+                                  odoo dependencies paths (comma separated)
+             -E --distro distro
+                                  simulate Linux distro: like Ubuntu20 Centos7 etc (requires -n switch)
+             -f --force           force v.environment create, even if exists or inside another virtual env
+             -F name              simulate Linux family: may be RHEL or Debian (requires -n switch)
+             -g --global          install npm packages globally
+             -k --keep            keep python2 executable as python (deprecated)
+             -I --indipendent     run pip in an isolated mode and set home virtual directory
+             -i --isolated        run pip in an isolated mode, ignoring environment variables and user configuration
+             -l --lang iso
+                                  set default language
+             -n --dry_run         do nothing (dry-run)
+             -O --odoo-ver version
+                                  install pypi required by odoo version (amend or create)
+             -o --odoo-path dir
+                                  odoo path used to search odoo requirements
+             -p --python pyver
+                                  python version
+             -q --quiet           silent mode
+             -r --requirement file
+                                  after created v.environment install from the given requirements file
+             -s --system-site-pack
+                                  create v.environment with access to the global site-packages
+             -t --travis          activate environment for travis test
+             -V --version         show version
+             -v --verbose         verbose mode
+             -y --yes             assume yes
+        
+        vem is an interactive tool with some nice features to manage standard virtual environment.
+        
+        Action is one of:
+        
+        * help
+        * amend [OPTIONS] [SRC_VENV]
+        * check [OPTIONS] [SRC_VENV]
+        * cp [OPTIONS] SRC_VENV TGT_ENV
+        * create -p PYVER [OPTIONS] [VENV]
+        * exec [OPTIONS] [VENV] CMD
+        * info [OPTIONS] [VENV] PKG
+        * install [OPTIONS] [VENV] PKG
+        * merge [OPTIONS] SRC_VENV TGT_ENV
+        * mv [OPTIONS] SRC_VENV TGT_ENV
+        * update [OPTIONS] [VENV] PKG
+        * uninstall [OPTIONS] [VENV] PKG
+        * test [OPTIONS] [VENV]
+        * reset [OPTIONS] [VENV]
+        * show [OPTIONS] [VENV] PKG
+        
+        amend [OPTIONS] [SRC_VENV]
+              Amend package versions against requirements.  May used after 'create' or 'reset' when requirements are changed.
+        
+        check [OPTIONS] [SRC_VENV]
+              Compare package versions against requirements.  May be used after 'create' or 'reset' to check virtual environment
+              consistency.
+        
+        cp [OPTIONS] SRC_VENV TGT_ENV
+              Copy SOURCE environment directory to TGT_ENV, like the bash command 'cp' and  set  relative  path  inside  virtual
+              environment to aim the new directory name.
+              Copying virtual environments is not well supported.
+              Each virtualenv has path information hard-coded into it, and there may be cases where the copy code does not know it needs to update a particular file.
+              Use with caution.
+        
+        create -p PYVER [OPTIONS] VENV
+              Create  a  new  virtual environment directory VENV like virtualenv command but with some nice features.  Switch -p
+              declare which python version will be used to create new environment.
+              This action can install various python packages to create a ready to use environment directory.
+              See -I -D -O -o -r switches to furthermore information.
+        
+        exec [OPTIONS] [SRC_VENV] CMD ...
+              Execute a command in virtual environment. Enclose command by quotes.
+        
+        info [OPTIONS] [SRC_VENV] PKG
+              Show information about pypi package if installed in virtual environment (alias of show)
+        
+        install [OPTIONS] [SRC_VENV] PKG
+              Install pypi package or bin package into virtual environment.
+              Warning! currently just 2 bin packages can be installed: wkhtmltopdf and lessc
+        
+        show [OPTIONS] [SRC_VENV] PKG
+              Show information about pypi package if installed in virtual environment (alias of info)
+        
+        uninstall [OPTIONS] [SRC_VENV] PKG
+              Uninstall pypi package from virtual environment.
+        
+        update [OPTIONS] [SRC_VENV] PKG
+              Upgrade pypi package in virtual environment.
+        
+        History
+        -------
+        
+        2.0.4 (2022-12-15)
+        ~~~~~~~~~~~~~~~~~~
+        
+        * [IMP] Package version adjustment
+        * [IMP] vem: amend show current package version
+        * [IMP] vem: no python2 warning in linux kernel 3
+        * [FIX] vem: best recognition of python version
+        
 Keywords: unit test virtual environment venv
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
-
-
-Python supplemental features
-----------------------------
-
-python-plus adds various features to python 2 and python 3 programs.
-It is designed to be used as integration of pypi future to help to port your code from Python 2 to Python 3 and still have it run on Python 2.
-
-
-list_requirements.py: list environment requirements
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-This command is an internal command of python-plus but may be used as own command.
-list_requirements.py dispays the pypi and binaries packages needed to create a virtual environment.
-It is specially designed to show Odoo requirements.
-Passing Odoo path it reads requirements.txt files in path and setup directories of OCA repositories.
-
-vem: virtual environment manager
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-This command is an interactive tool with some nice features to manage standard virtual environment.
-Mainly it works ad standard pip but inside a specific virtual environment.
-
-vem: virtual environment manager
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-::
-
-    Usage: vem.sh [-h][-a list][-BCD][-d paths][-E distro][-f][-F name][-gkIi][-l iso][-n][-O version][-o dir][-p pyver][-q][-r file][-stVvy] p3 p4 p5 p6 p7 p8 p9
-    Manage virtual environment
-    action may be: help amend cp check create exec info inspect install merge mv python shell rm show uninstall update test
-     -h --help            this help
-     -a list              bin packages to install (* means wkhtmltopdf,lessc)
-     -B                   use unstable packages: -B testpypi / -BB from ~/tools / -BBB from ~/pypi / -BBBB link to local ~/pypi
-     -C                   clear cache before executing pip command
-     -D --devel           create v.environment with development packages
-     -d --dep-path paths
-                          odoo dependencies paths (comma separated)
-     -E --distro distro
-                          simulate Linux distro: like Ubuntu20 Centos7 etc (requires -n switch)
-     -f --force           force v.environment create, even if exists or inside another virtual env
-     -F name              simulate Linux family: may be RHEL or Debian (requires -n switch)
-     -g --global          install npm packages globally
-     -k --keep            keep python2 executable as python (deprecated)
-     -I --indipendent     run pip in an isolated mode and set home virtual directory
-     -i --isolated        run pip in an isolated mode, ignoring environment variables and user configuration
-     -l --lang iso
-                          set default language
-     -n --dry_run         do nothing (dry-run)
-     -O --odoo-ver version
-                          install pypi required by odoo version (amend or create)
-     -o --odoo-path dir
-                          odoo path used to search odoo requirements
-     -p --python pyver
-                          python version
-     -q --quiet           silent mode
-     -r --requirement file
-                          after created v.environment install from the given requirements file
-     -s --system-site-pack
-                          create v.environment with access to the global site-packages
-     -t --travis          activate environment for travis test
-     -V --version         show version
-     -v --verbose         verbose mode
-     -y --yes             assume yes
-
-vem is an interactive tool with some nice features to manage standard virtual environment.
-
-Action is one of:
-
-* help
-* amend [OPTIONS] [SRC_VENV]
-* check [OPTIONS] [SRC_VENV]
-* cp [OPTIONS] SRC_VENV TGT_ENV
-* create -p PYVER [OPTIONS] [VENV]
-* exec [OPTIONS] [VENV] CMD
-* info [OPTIONS] [VENV] PKG
-* install [OPTIONS] [VENV] PKG
-* merge [OPTIONS] SRC_VENV TGT_ENV
-* mv [OPTIONS] SRC_VENV TGT_ENV
-* update [OPTIONS] [VENV] PKG
-* uninstall [OPTIONS] [VENV] PKG
-* test [OPTIONS] [VENV]
-* reset [OPTIONS] [VENV]
-* show [OPTIONS] [VENV] PKG
-
-amend [OPTIONS] [SRC_VENV]
-      Amend package versions against requirements.  May used after 'create' or 'reset' when requirements are changed.
-
-check [OPTIONS] [SRC_VENV]
-      Compare package versions against requirements.  May be used after 'create' or 'reset' to check virtual environment
-      consistency.
-
-cp [OPTIONS] SRC_VENV TGT_ENV
-      Copy SOURCE environment directory to TGT_ENV, like the bash command 'cp' and  set  relative  path  inside  virtual
-      environment to aim the new directory name.
-      Copying virtual environments is not well supported.
-      Each virtualenv has path information hard-coded into it, and there may be cases where the copy code does not know it needs to update a particular file.
-      Use with caution.
-
-create -p PYVER [OPTIONS] VENV
-      Create  a  new  virtual environment directory VENV like virtualenv command but with some nice features.  Switch -p
-      declare which python version will be used to create new environment.
-      This action can install various python packages to create a ready to use environment directory.
-      See -I -D -O -o -r switches to furthermore information.
-
-exec [OPTIONS] [SRC_VENV] CMD ...
-      Execute a command in virtual environment. Enclose command by quotes.
-
-info [OPTIONS] [SRC_VENV] PKG
-      Show information about pypi package if installed in virtual environment (alias of show)
-
-install [OPTIONS] [SRC_VENV] PKG
-      Install pypi package or bin package into virtual environment.
-      Warning! currently just 2 bin packages can be installed: wkhtmltopdf and lessc
-
-show [OPTIONS] [SRC_VENV] PKG
-      Show information about pypi package if installed in virtual environment (alias of info)
-
-uninstall [OPTIONS] [SRC_VENV] PKG
-      Uninstall pypi package from virtual environment.
-
-update [OPTIONS] [SRC_VENV] PKG
-      Upgrade pypi package in virtual environment.
-
-History
--------
-
-2.0.4 (2022-12-15)
-~~~~~~~~~~~~~~~~~~
-
-* [IMP] Package version adjustment
-* [IMP] vem: amend show current package version
-* [IMP] vem: no python2 warning in linux kernel 3
-* [FIX] vem: best recognition of python version
-
-
```

### Comparing `python_plus-2.0.6/README.rst` & `python_plus-2.0.7/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2023-04-14
+Last Update / Ultimo aggiornamento: 2023-05-09
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Mature-green.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
 .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
     :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
```

### Comparing `python_plus-2.0.6/python_plus/__init__.py` & `python_plus-2.0.7/python_plus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 __author__ = 'Antonio Maria Vigliotti'
 __license__ = 'L-GPL'
 __copyright__ = 'Copyright 2018-2023 SHS-AV srl'
 __ver_major__ = 0
 __ver_minor__ = 1
 __ver_patch__ = 3
 __ver_sub__ = '6'
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 PYCODESET = 'utf-8'
 if PY3:
     text_type = unicode = str
     bytestr_type = bytes
 elif PY2:
     # unicode exist only for python2
```

### Comparing `python_plus-2.0.6/python_plus/__main__.py` & `python_plus-2.0.7/python_plus/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import os
 import subprocess
 import sys
 
 from zerobug import Z0BUG
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 STS_FAILED = 1
 STS_SUCCESS = 0
 
 if __name__ == "__main__":
     action = False
     if len(sys.argv) > 1:
         action = sys.argv[1]
```

### Comparing `python_plus-2.0.6/python_plus/scripts/list_requirements.py` & `python_plus-2.0.7/python_plus/scripts/list_requirements.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 #
 # This software manages 4 lists:
 # list['python'] -> Result list
 # list['python1'] -> is the list with packages w/o version
 # list['python2'] -> is the list with versioned packages
 #
 from __future__ import print_function, unicode_literals
+from past.builtins import basestring
+# from future.utils import PY2, PY3
 
 import ast
 import os
 import re
 import sys
 from subprocess import PIPE, Popen
 
@@ -20,50 +22,54 @@
     import python_plus
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 python_version = "%s.%s" % (sys.version_info[0], sys.version_info[1])
 
 #
 # known incompatibilities:
 # - requests: oca-maintainers-tools -> '==2.3.0',
 #             codecov -> '>=2.7.9'
-# Here we assume: Odoo 11.0 use python 3.5, Odoo 12.0 uses python 3.7
+# Here we assume: Odoo 11.0 use python 3.6, Odoo 12.0 -> 3.7, Odoo 16.0 -> 3.8
 # If version is 2.7 or 3.5 or 3.6 or 3.7 or 3.8 or 3.9 then it refers to python version
 REQVERSION = {
     "acme_tiny": {"6.1": ">=4.0.3"},
     "argparse": {"0": "==1.2.1"},
     "astroid": {"2.7": "==1.6.5", "3.5": "==2.2.0"},  # Version by test pkgs
     "autopep8": {"0": "==1.2"},
-    "Babel": {"6.1": "==1.3", "8.0": "==2.3.4", "16.0": ">=2.6.0<=2.9.1"},
+    "Babel": {"6.1": "==1.3", "8.0": "==2.3.4", "16.0": ">=2.6.0,<=2.9.1"},
     "beautifulsoup": {"6.1": "==3.2.1"},
     "bokeh": {
-        "11.0": "==0.12.7", "12.0": "==1.1.0", "14.0": "==2.3.1", "15.0": "2.4.2"
+        "10.0": "bokeh<1.4.0",
+        "11.0": "==0.12.7",
+        "12.0": "==1.1.0",
+        "14.0": "==2.3.1",
+        "15.0": "2.4.2"
     },
     "codicefiscale": {"6.1": "==0.9"},
     "coverage": {"2.7": "<5.6.0", "3.5": ">=5.0.0"},
-    "cryptography": {"2.7": ">=2.2.2", "3.7": ">=38.0<39.0"},
+    "cryptography": {"2.7": ">=2.2.2,<3.4", "3.7": ">=38.0,<39.0"},
     "decorator": {"6.1": "==3.4.0", "10.0": "==4.0.10"},
     "docutils": {"6.1": "==0.12", "0": "==0.14", "3.7": "==0.16"},       # By test pkgs
     "ebaysdk": {"6.1": "==2.1.4"},
     "email_validator": {"10.0": "<1.3.0", "12.0": ">=1.3"},
     "ERPpeek": {"0": "==1.6.1"},
     "feedparser": {"6.1": "==5.1.3", "10.0": "==5.2.1"},
     "flake8": {
         "6.1": "==3.4.1"     # Tested 3.5.0; 3.6.0 does not work
     },
     "gdata": {"6.1": "==2.0.18"},
     "gevent": {
         "6.1": "==1.0.1",
         "7.0": "==1.0.2",
-        "10.0": ">=1.1.2<=1.4.0",       # trying to test
+        "10.0": ">=1.1.2,<=1.4.0",       # trying to test
         "3.7": "==1.5.0",
     },
     "greenlet": {
         "6.1": "==0.4.2",
         "7.0": "==0.4.10",
         "3.7": ">=0.4.13",
     },
@@ -81,15 +87,15 @@
     },
     "MarkupSafe": {"6.1": "==0.23", "14.0": "==1.1.0", "0": "<2.1.0"},  # Tested 1.0
     "matplotlib": {
         "10.0": "==3.0.3",
         # "13.0": "==3.4.1",
         "3.6": "==3.0.3",
         # "3.7": "==3.4.1"
-        "3.7": "<3.4.0"     # Experimental!
+        "3.7": "<3.3.0"     # Experimental!
     },
     "mock": {"6.1": "==1.0.1", "8.0": "==2.0.0"},
     "nbconvert": {"0": "==6.0.7"},
     "odoo_score": {"6.1": "==1.0.1", "10.0": ">=2.0.0"},
     "ofxparse": {"6.1": "==0.16"},
     "pandas": {"3.7": ">=0.22.0,<=1.1.0"},
     "passlib": {"6.1": "==1.6.2", "10.0": "==1.6.5", "16.0": ">=1.7.0"},
@@ -102,16 +108,16 @@
         "3.6": "==4.0.0",
         "3.7": "==6.1.0",
         "3.8": ">=6.2.1",
     },
     "psutil": {"6.1": "==2.1.1", "7.0": "==2.2.0", "8.0": "==4.3.1"},
     "psycogreen": {"6.1": "==1.0"},
     "psycopg2-binary": {
-        "6.1": ">=2.0.0",
-        "8.0": ">=2.5.4",
+        "6.1": ">=2.0.0,<2.8.0",
+        "8.0": ">=2.5.4,<2.8.0",
         "10.0": ">=2.7.4",
         "12.0": ">=2.8.3",
         "0": ">=2.7.4",
     },
     "pycodestyle": {"0": "==2.3.1"},
     "pydot": {"6.1": "==1.0.2", "8.0": "==1.2.3"},
     "pyflakes": {"0": "pyflakes<1.6.0,>=1.5.0"},
@@ -125,22 +131,22 @@
         "3.5": "<2.7.0",
         "3.6": "<2.14.0",
         "3.7": "<2.15.0",
     },
     "pylint-odoo": {
         "2.7": "==3.5.0",
         "3.5": "<=8.0.0",
-        "3.8": ">=3.5.0<=8.0.0",
+        "3.8": ">=3.5.0,<=8.0.0",
     },
     "pylint-plugin-utils": {
         "2.7": "==0.2.6",
         "3.5": "==0.5",
         "3.6": ">=0.7",
     },
-    "pyopenssl": {"0": ">=16.2.0"},  # by MQT
+    "pyOpenSSL": {"0": ">=16.2.0", "16.0": ">=23.0"},  # by MQT
     "pyotp": {"2.7": "==2.3.0", "3.5": ">=2.4.0"},
     "pyPDF2": {"2.7": "==1.28.4", "3.5": "<2.0"},
     "pysftp": {"6.1": ">=0.2.9"},
     "pyparsing": {"6.1": "==1.5.7", "7.0": "==2.0.3", "10.0": "==2.1.10"},
     "pyPdf": {"6.1": "==1.13"},
     "pyserial": {"6.1": "==2.7", "10.0": ">=3.1.1"},
     "Python-Chart": {"6.1": "==1.39"},
@@ -153,15 +159,16 @@
         "10.0": "==2.4.27",
         "11.0": "==2.5.28",
         "13.0": "==3.1.0",
     },
     "python-openid": {"6.1": "==2.2.5"},
     "python-stdnum": {"6.1": ">=1.8.1"},
     "pytz": {"6.1": ">=2014.10", "10.0": ">=2016.7"},
-    "pyusb": {"6.1": ">=1.0.0b1", "10.0": "==1.0.0"},
+    # check for: Odoo requires >=1.0.0b1, but it does conflict with other packges
+    "pyusb": {"6.1": ">=1.0.0b1", "10.0": "==1.0.0", "16.0": ">=1.0.0b1"},
     "pyxb": {"6.1": "==1.2.5", "12.0": "==1.2.6"},
     "PyWebDAV": {"6.1": "<0.9.8"},
     "PyYAML": {"6.1": "==3.11", "8.0": "==3.12", "3.7": "==3.13"},
     "qrcode": {"6.1": "==5.0.1", "7.0": "==5.1", "10.0": "==5.3"},
     "readme-renderer" : {"2.7": "<25.0", "3.5": "<29.0", "3.6": ">=30.0"},
     "restructuredtext_lint": {"6.1": "==0.12.2", "0": "==1.1.3"},
     "reportlab": {"6.1": "==3.1.44", "10.0": "==3.3.0"},
@@ -183,14 +190,15 @@
     "Werkzeug": {
         "6.1": "==0.9.6",
         "10.0": "==0.11.11",
         "11.0": "==0.11.15",
         "3.7": "==0.14.1",
     },
     "wkhtmltopdf": {"6.1": "==0.12.1", "10.0": "==0.12.4", "12.0": "==0.12.5"},
+    "wok_code": {"6.1": "<2.0.6", "10.0": ">=2.0.0"},
     "wsgiref": {"6.1": "==0.1.2"},
     "XlsxWriter": {"6.1": "==0.9.3"},  # Tested 1.0.2
     "xlrd": {"6.1": "==1.0.0"},
     "xlwt": {"6.1": "==0.7.5", "10.0": "==1.1.2", "12.0": "==1.3"},
     "z0bug_odoo": {"6.1": "==1.0.1", "10.0": ">=2.0.0"},
     "zeep": {"0": "==2.4.0"},
     "zerobug": {"6.1": "==1.0.1", "10.0": ">=2.0.0"},
@@ -208,15 +216,15 @@
     "markupsafe": "MarkupSafe",
     "openid": "python-openid",
     "openupgradelib": "openupgradelib@git+https://github.com/OCA/openupgradelib.git",
     "past": "future",
     "pillow": "Pillow",
     "psycopg2": "psycopg2-binary",
     "py-asterisk": "py-Asterisk",
-    "pychart": "PyChart",
+    "pychart": "Python-Chart",
     "pypdf": "pyPdf",
     "pypdf2": "pyPDF2",
     "pygments": "Pygments",
     "pyldap": "python-ldap",  # pyldap is a fork!
     "python-chart": "Python-Chart",
     "python-docutils": "docutils",
     "python-levenshtein": "python-Levenshtein",
@@ -230,18 +238,36 @@
     "stdnum": "python-stdnum",
     "usb": "pyusb",
     "werkzeug": "Werkzeug",
     "xlsxwriter": "XlsxWriter",
 }
 ALIAS3 = {
     "PyWebDAV": "PyWebDAV3",
-    # "pyPdf": "pyPDF2",
     # "python-ldap": "pyldap",  # pyldap is a fork!
     "python-dev": "python3-dev",
     "python3-ldap": "ldap3",
+    "jsonlib": "jsonlib-python3",
+}
+ALIAS_RHEL = {
+    "build-essential": "groupinstall 'Development Tools'",
+    "expect-dev": "expect-devel",
+    "python-dev": "python-devel",
+    "python3-dev": "python3-devel",
+    "libcups2-dev": "cups-devel",
+    "libevent-dev": "libevent-devel",
+    "libffi-dev": "libffi-devel",
+    "libgeos-dev": "geos-devel",
+    "libldap2-dev": "openldap-devel",
+    "libpq-dev": "postgresql-devel",
+    "libsasl2-dev": "",
+    "libssl-dev": "",
+    "libxml2-dev": "libxml2-devel",
+    "libxslt-dev": "libxslt-devel",
+    "zlib1g": "epel-release --enablerepo=extras",
+    "zlib1g-dev": "zlib-devel",
 }
 FORCE_ALIAS2 = {
     "docutils==0.12": "docutils==0.14",
     "pytz==2014.4": "pytz>=2014.4",
     "pytz==2014.10": "pytz>=2014.10",
     "pytz==2016.7": "pytz>=2016.7",
     "zeep==4.0.0": "zeep==2.4.0",
@@ -271,24 +297,25 @@
     "cryptography",
     "pyOpenSSL",
     "idna",
     "certifi",
     "asn1crypto",
     "pyasn1",
 ]
-PIP_TEST_PACKAGES = [
+PIP2_TEST_PACKAGES = [
     "astroid",
     "Click",
     "configparser",
     # "codecov",
     "coverage",
     # "coveralls",
     "docopt",
     "docutils",
     "flake8",
+    "future",
     "GitPython",
     "isort",
     "lazy_object_proxy",
     "lxml",
     "MarkupSafe",
     "mock",
     "pbr",
@@ -324,14 +351,15 @@
     "configparser",
     # "codecov",
     "coverage",
     # "coveralls",
     "docopt",
     "docutils",
     "flake8",
+    "future",
     "GitPython",
     "isort",
     "lazy_object_proxy",
     "lxml",
     "MarkupSafe",
     "mock",
     "pbr",
@@ -367,19 +395,20 @@
     "expect-dev",
     "libffi-dev",
     "libpq-dev",
     "libssl-dev",
     "python-dev",
     "python-setuptools",
 ]
-RPC_PACKAGES2 = ["clodoo", "odoorpc", "oerplib", "os0"]
-RPC_PACKAGES3 = ["clodoo", "odoorpc", "os0"]
+RPC2_PACKAGES = ["clodoo", "odoorpc", "oerplib", "os0"]
+RPC3_PACKAGES = ["clodoo", "odoorpc", "os0"]
 PIP_BASE_PACKAGES = [
     "Babel",
     "chardet",
+    "Click",
     "configparser",
     "decorator",
     "docutils",
     "feedparser",
     "future",
     "gdata",
     "gevent",
@@ -396,29 +425,31 @@
     "python-dateutil",
     "python-openid",
     "python-plus",
     "pydot",
     "pyparsing",
     "simplejson",
     "six",
-    "stdnum",
-    "vatnumber",
+    "python-stdnum",
+    # "vatnumber",
 ]
+PIP3_BASE_PACKAGES = []
 PIP_ODOO_BASE_PACKAGES = [
     "Babel",
     "chardet",
     "configparser",
     "decorator",
     "docutils",
     "feedparser",
     "future",
     "gdata",
     "gevent",
     "html2text",
     "Jinja2",
+    "lessc; odoo_major>=10",
     "lxml",
     "Mako",
     "numpy",
     "num2words",
     "passlib",
     "Pillow",
     "psutil",
@@ -428,24 +459,26 @@
     "python-ldap",
     "python-dateutil",
     "python-openid",
     "python-plus",
     "pydot",
     "pyparsing",
     "pyPdf",
+    "pyPDF2",
     "pyserial",
     "pytz",
+    "qrcode; odoo_major>=16",
     "reportlab",
     "simplejson",
     "six",
-    "stdnum",
+    "python-stdnum",
     "vatnumber",
     "Werkzeug",
+    "zeep; odoo_major>=16"
 ]
-PIP3_BASE_PACKAGES = []
 BIN_BASE_PACKAGES = [
     "curl",
     "less-plugin-clean-css",
     "nodejs",
     "npm",
     "wkhtmltopdf",
     "zlib1g",
@@ -466,17 +499,16 @@
     "Crypto.Cipher": "pycrypto",
     "facturx": "factur-x",
     "past": "future",
     "u2flib_server": "python-u2flib-server",
     "voicent": "Voicent-Python",
 }
 # Retrieve python3 version
-cmd = ["python3", "--version"]
 try:
-    p = Popen(cmd, stdin=PIPE, stdout=PIPE, stderr=PIPE)
+    p = Popen(["python3", "--version"], stdin=PIPE, stdout=PIPE, stderr=PIPE)
     res, err = p.communicate()
     res = res.decode()
     i = res.find("3.")
     if i >= 0:
         PY3ID = res[i] + res[i + 2]
     else:
         PY3ID = "3"
@@ -489,71 +521,168 @@
     "gevent": {"bin": "libevent-dev"},
     "Pillow": {"python": "docutils"},
     "pycups": {"bin": "libcups2-dev"},
     "shapely": {"bin": "libgeos-dev"},
 }
 DEPS2 = {
     "invoice2data": {"python": "regex<2022.1.18"},
-    "lxml": {"bin": ("python-dev", "libxml2-dev", "libxslt1-dev", "zlib1g-dev")},
+    "lxml": {
+        "bin":
+            ("python-dev", "python-lxml", "libxml2-dev", "libxslt1-dev", "zlib1g-dev")
+    },
     "python-psycopg2": {"bin": ("python-dev", "libpq-dev")},
     "python-ldap": {"bin": ("libsasl2-dev", "libldap2-dev", "libssl-dev")},
 }
 DEPS3 = {
-    "lxml": {"bin": ("PY3_DEV", "libxml2-dev", "libxslt1-dev", "zlib1g-dev")},
+    "lxml": {
+        "bin": ("PY3_DEV", "python3-lxml", "libxml2-dev", "libxslt1-dev", "zlib1g-dev")
+    },
     "python-psycopg2": {"bin": ("PY3_DEV", "libpq-dev")},
-    # "python3-ldap": {"bin": ("libsasl2-dev", "libldap2-dev", "libssl-dev")},
+    "python3-ldap": {"bin": ("libsasl2-dev", "libldap2-dev", "libssl-dev")},
 }
-DEPS9 = [
-    "astroid==1.6.5",
-    "astroid==2.2.0",
-    "astroid==2.4.2",
-    "docutils==0.12",
-    "docutils==0.14",
-    "docutils==0.16",
-    "Pillow==3.4.1",
-    "Pygments==2.0.2",
-    # "pylint==1.9.3",
-    # "pylint==1.9.5",
-    # "pylint==2.3.0",
-    # "pylint==2.5.3",
-    # "pylint-plugin-utils==0.4",
-    "six==1.15.0",
-]
+# DEPS9 = [
+#     "astroid==1.6.5",
+#     "astroid==2.2.0",
+#     "astroid==2.4.2",
+#     "docutils==0.12",
+#     "docutils==0.14",
+#     "docutils==0.16",
+#     "Pillow==3.4.1",
+#     "Pygments==2.0.2",
+#     "six==1.15.0",
+# ]
+
+# PYCODESET = 'utf-8'
+# if PY3:
+#     text_type = unicode = str
+#     bytestr_type = bytes
+# elif PY2:
+#     # unicode exist only for python2
+#     text_type = unicode
+#     bytestr_type = str
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def get_naked_pkgname(pkg):
     return re.split('[!<=>@#;]', python_plus.qsplit(pkg)[0])[0].strip()
 
 
-def trim_pkgname(pkg):
-    pkg = (
-        pkg.replace(" =", "=")
-        .replace(" <", "<")
-        .replace(" >", ">")
-        .replace(" ;", ";")
-        .replace(" @", "@")
-        .replace("= ", "=")
-        .replace("< ", "<")
-        .replace("> ", ">")
-        .replace("; ", ";")
-        .replace("@ ", "@")
-    )
-    return pkg.replace(" !", "!").strip()
+# def _b(s):
+#     if isinstance(s, text_type):
+#         return s.encode(PYCODESET)
+#     return s
+#
+#
+# def _u(s):
+#     if isinstance(s, bytestr_type):
+#         if PY3:
+#             return s.decode(PYCODESET)
+#         return unicode(s, PYCODESET)
+#     return s
+#
+#
+# def bstrings(src):
+#     if isinstance(src, dict):
+#         src2 = src.copy()
+#         for x in src2.keys():
+#             if isinstance(x, text_type):
+#                 del src[x]
+#             src[_b(x)] = _b(src2[x])
+#     elif isinstance(src, (list, tuple)):
+#         for i, x in enumerate(src):
+#             src[i] = _b(x)
+#     return src
+#
+#
+# def unicodes(src):
+#     if isinstance(src, dict):
+#         src2 = src.copy()
+#         for x in src2.keys():
+#             if isinstance(x, bytestr_type):
+#                 del src[x]
+#             src[_u(x)] = _u(src2[x])
+#     elif isinstance(src, (list, tuple)):
+#         for i, x in enumerate(src):
+#             src[i] = _u(x)
+#     return src
+#
+#
+# def qsplit(*args, **kwargs):
+#     src = args[0]
+#     if len(args) > 1 and args[1]:
+#         sep = args[1]
+#         if isinstance(sep, (tuple, list)):
+#             sep = unicodes(sep)
+#         elif isinstance(sep, basestring):
+#             sep = _u(sep)
+#     else:
+#         sep = [' ', '\t', '\n', '\r']
+#     if len(args) > 2 and args[2]:
+#         maxsplit = args[2]
+#     else:
+#         maxsplit = -1
+#     quotes = kwargs.get('quotes', ["'", '"'])
+#     escape = kwargs.get('escape', False)
+#     enquote = kwargs.get('enquote', False)
+#     strip = kwargs.get('strip', False)
+#     source = _u(src)
+#     sts = False
+#     result = []
+#     item = ''
+#     esc_sts = False
+#     ctr = 0
+#     for ch in source:
+#         if maxsplit >= 0 and ctr >= maxsplit:
+#             item += ch
+#         elif esc_sts:
+#             esc_sts = False
+#             item += ch
+#         elif ch == escape:
+#             esc_sts = True
+#         elif ch == sts:
+#             sts = False
+#             if enquote:
+#                 item += ch
+#         elif sts:
+#             item += ch
+#         elif ch in quotes:
+#             sts = ch
+#             if enquote:
+#                 item += ch
+#         elif (isinstance(sep, (tuple, list)) and ch in sep) or (
+#             isinstance(sep, basestring) and ch == sep
+#         ):
+#             if strip:
+#                 result.append(item.strip())
+#             else:
+#                 result.append(item)
+#             item = ''
+#             ctr += 1
+#         else:
+#             item += ch
+#     if strip:
+#         result.append(item.strip())
+#     else:
+#         result.append(item)
+#     if isinstance(src, bytestr_type):
+#         return bstrings(result)
+#     return result
 
 
-def eval_requirement_cond(line, pyver=None):
+def eval_requirement_cond(line, pyver=None, odoo_ver=None):
     pyver = pyver or '3.7'
     items = line.split('#')[0].split(";")
     if len(items) == 1:
         return get_naked_pkgname(line)
-    testenv = {"sys_platform": sys.platform, "python_version": pyver}
+    testenv = {"sys_platform": sys.platform,
+               "python_version": pyver,
+               "odoo_major": int(odoo_ver.split(".")[0])}
     if eval(items[1], testenv):
         return get_naked_pkgname(line)
     return False
 
 
 def parse_setup(ctx, setup, pyver=None):
     # reqlist = []
@@ -600,33 +729,33 @@
     return reqlist
 
 
 def parse_requirements(ctx, reqfile, pyver=None):
     if reqfile == "openupgradelib":
         return [reqfile]
     reqlist = []
-    with open(reqfile, "r") as fd:
-        lines = fd.read().split("\n")
-        for line in lines:
-            if eval_requirement_cond(line, pyver=pyver):
-                if ctx["keep_cond"]:
-                    reqlist.append(line)
-                else:
-                    reqlist.append(line.split(";")[0].strip())
+    try:
+        with open(reqfile, "r") as fd:
+            lines = fd.read().split("\n")
+            for line in lines:
+                line = re.split('[#]', line)[0].strip()
+                if not line:
+                    continue
+                if eval_requirement_cond(line, pyver=pyver, odoo_ver=ctx["odoo_ver"]):
+                    if ctx["keep_cond"]:
+                        reqlist.append(line)
+                    else:
+                        reqlist.append(re.split('[#;]', line)[0].strip())
+    except BaseException as e:
+        print("File %s: error %s" % (reqfile, e))
     return reqlist
 
 
 def name_n_version(full_item, with_version=None, odoo_ver=None, pyver=None):
-    full_item = trim_pkgname(full_item)
-    item = re.split("[!=<>]", full_item)
-    # if len(item) == 1:
-    #     item_ver = ""
-    # else:
-    #     item_ver = item[-1]
-    item = os.path.basename(get_naked_pkgname(item[0]))
+    item = os.path.basename(get_naked_pkgname(re.split("[!=<>]", full_item)[0]))
     if item.endswith(".git"):
         item = item[:-4]
     if not filter(lambda x: item.startswith(x), PIP_WITH_DOT):
         if '.' in item:
             full_item = full_item.replace('.' + item.split(".")[1], '')
             item = item.split(".")[0].lower()
     item_l = item.lower()
@@ -757,26 +886,100 @@
                 if ver_left != ver_right:
                     if not ignore_error:
                         sys.stderr.write(
                             "Modules version requirements mismatch: <%s> <%s>\n"
                             % (left, right))
                     if ver_right > ver_left:
                         split_left[ix_left] = ver_right
-            elif "<" in op:
+            elif ">" in op:
                 split_left[ix_left] = maxver(ver_left, ver_right)
 
             else:
                 split_left[ix_left] = minver(ver_left, ver_right)
 
     if split_left[-1] == ",":
         split_left = split_left[: -1]
     return "".join(split_left)
 
 
-def add_package(deps_list, kw, item, with_version=None, odoo_ver=None, pyver=None):
+def add_dependencies(deps_list, item, with_version=None, odoo_ver=None, pyver=None):
+    if item in DEPS:
+        for kw1 in ("python", "bin"):
+            if kw1 not in DEPS[item]:
+                continue
+            if isinstance(DEPS[item][kw1], (tuple, list)):
+                for itm in DEPS[item][kw1]:
+                    deps_list = add_package(
+                        deps_list,
+                        kw1,
+                        itm,
+                        with_version=with_version,
+                        odoo_ver=odoo_ver,
+                        pyver=pyver,
+                    )
+            else:
+                deps_list = add_package(
+                    deps_list,
+                    kw1,
+                    DEPS[item][kw1],
+                    with_version=with_version,
+                    odoo_ver=odoo_ver,
+                    pyver=pyver,
+                )
+    if pyver and pyver.split(".")[0] == "2" and item in DEPS2:
+        for kw1 in ("python", "bin"):
+            if kw1 not in DEPS2[item]:
+                continue
+            if isinstance(DEPS2[item][kw1], (tuple, list)):
+                for itm in DEPS2[item][kw1]:
+                    deps_list = add_package(
+                        deps_list,
+                        kw1,
+                        itm,
+                        with_version=with_version,
+                        odoo_ver=odoo_ver,
+                        pyver=pyver,
+                    )
+            else:
+                deps_list = add_package(
+                    deps_list,
+                    kw1,
+                    DEPS2[item][kw1],
+                    with_version=with_version,
+                    odoo_ver=odoo_ver,
+                    pyver=pyver,
+                )
+    if pyver and pyver.split(".")[0] == "3" and item in DEPS3:
+        for kw1 in ("python", "bin"):
+            if kw1 not in DEPS3[item]:
+                continue
+            if isinstance(DEPS3[item][kw1], (tuple, list)):
+                for itm in DEPS3[item][kw1]:
+                    deps_list = add_package(
+                        deps_list,
+                        kw1,
+                        itm,
+                        with_version=with_version,
+                        odoo_ver=odoo_ver,
+                        pyver=pyver,
+                    )
+            else:
+                deps_list = add_package(
+                    deps_list,
+                    kw1,
+                    DEPS3[item][kw1],
+                    with_version=with_version,
+                    odoo_ver=odoo_ver,
+                    pyver=pyver,
+                )
+    return deps_list
+
+
+def add_package(deps_list, kw, item, with_version=None, odoo_ver=None, pyver=None,
+                ignore_deps=False):
 
     def add_full_item(deps_list, kw, with_version, full_item):
         kw1 = "%s1" % kw
         kw2 = "%s2" % kw
         if with_version and full_item:
             found = False
             for ix, kk in enumerate(deps_list[kw2]):
@@ -788,108 +991,50 @@
                 deps_list[kw2].append(full_item)
             if item in deps_list[kw1]:
                 del deps_list[kw1][deps_list[kw1].index(item)]
         elif item not in deps_list[kw1]:
             deps_list[kw1].append(item)
         return deps_list
 
-    if item in BUILTIN:
-        return deps_list
-    if item == "PY3_DEV":
-        item = PY3_DEV
+    if eval_requirement_cond(item, pyver=pyver, odoo_ver=odoo_ver):
+        item = re.split('[#;]', item)[0].strip()
+        if item in BUILTIN:
+            return deps_list
+        if item == "PY3_DEV":
+            item = PY3_DEV
 
-    item, full_item = name_n_version(
-        item, with_version=with_version, odoo_ver=odoo_ver, pyver=pyver
-    )
-    if item in BIN_PACKAGES or item in BIN_BASE_PACKAGES or item in BIN_TEST_PACKAGES:
-        kw = "bin"
+        item, full_item = name_n_version(
+            item, with_version=with_version, odoo_ver=odoo_ver, pyver=pyver
+        )
+        if (
+            item in BIN_PACKAGES
+            or item in BIN_BASE_PACKAGES
+            or item in BIN_TEST_PACKAGES
+        ):
+            kw = "bin"
 
-    if item not in deps_list[kw]:
-        deps_list[kw].append(item)
-        if kw == "python":
-            deps_list = add_full_item(deps_list, kw, with_version, full_item)
-
-            if item in DEPS:
-                for kw1 in ("python", "bin"):
-                    if kw1 not in DEPS[item]:
-                        continue
-                    if isinstance(DEPS[item][kw1], (tuple, list)):
-                        for itm in DEPS[item][kw1]:
-                            deps_list = add_package(
-                                deps_list,
-                                kw1,
-                                itm,
-                                with_version=with_version,
-                                odoo_ver=odoo_ver,
-                                pyver=pyver,
-                            )
-                    else:
-                        deps_list = add_package(
-                            deps_list,
-                            kw1,
-                            DEPS[item][kw1],
-                            with_version=with_version,
-                            odoo_ver=odoo_ver,
-                            pyver=pyver,
-                        )
-            if pyver and pyver.split(".")[0] == "2" and item in DEPS2:
-                for kw1 in ("python", "bin"):
-                    if kw1 not in DEPS2[item]:
-                        continue
-                    if isinstance(DEPS2[item][kw1], (tuple, list)):
-                        for itm in DEPS2[item][kw1]:
-                            deps_list = add_package(
-                                deps_list,
-                                kw1,
-                                itm,
-                                with_version=with_version,
-                                odoo_ver=odoo_ver,
-                                pyver=pyver,
-                            )
-                    else:
-                        deps_list = add_package(
-                            deps_list,
-                            kw1,
-                            DEPS2[item][kw1],
-                            with_version=with_version,
-                            odoo_ver=odoo_ver,
-                            pyver=pyver,
-                        )
-            if pyver and pyver.split(".")[0] == "3" and item in DEPS3:
-                for kw1 in ("python", "bin"):
-                    if kw1 not in DEPS3[item]:
-                        continue
-                    if isinstance(DEPS3[item][kw1], (tuple, list)):
-                        for itm in DEPS3[item][kw1]:
-                            deps_list = add_package(
-                                deps_list,
-                                kw1,
-                                itm,
-                                with_version=with_version,
-                                odoo_ver=odoo_ver,
-                                pyver=pyver,
-                            )
-                    else:
-                        deps_list = add_package(
-                            deps_list,
-                            kw1,
-                            DEPS3[item][kw1],
-                            with_version=with_version,
-                            odoo_ver=odoo_ver,
-                            pyver=pyver,
-                        )
-        elif kw == "bin":
-            deps_list = add_full_item(deps_list, kw, with_version, full_item)
+        if item not in deps_list[kw]:
+            deps_list[kw].append(item)
+            if kw == "python":
+                deps_list = add_full_item(deps_list, kw, with_version, full_item)
+                if not ignore_deps:
+                    deps_list = add_dependencies(
+                        deps_list, item,
+                        with_version=with_version, odoo_ver=odoo_ver, pyver=pyver)
+            elif kw == "bin":
+                deps_list = add_full_item(deps_list, kw, with_version, full_item)
 
     return deps_list
 
 
 def package_from_list(
     deps_list, kw, pkg_list, with_version=None, odoo_ver=None, pyver=None
 ):
+    if isinstance(pkg_list, basestring):
+        pkg_list = [pkg_list]
     for item in pkg_list:
         if isinstance(item, (list, tuple)):
             for sub in item:
                 deps_list = add_package(
                     deps_list,
                     kw,
                     sub,
@@ -993,23 +1138,14 @@
     def parse_manifest(manifests, reqfiles, setups, root, files, no_deep):
         if "/setup/" in root and "setup.py" in files:
             fn = os.path.join(root, "setup.py")
             if fn not in setups:
                 setups.append(os.path.join(root, "setup.py"))
         if root.startswith(no_deep):
             return manifests, reqfiles, setups, no_deep
-        # basename = os.path.basename(root)
-        # if (
-        #     basename.startswith('.')
-        #     or basename.startswith('_')
-        #     or basename.endswith('~')
-        #     or basename in ("doc", "tmp", "venv_odoo")
-        # ):
-        #     no_deep = root
-        #     return manifests, reqfiles, setups, no_deep
         if (
             not read_from_manifest
             and "__init__.py" in files
             and ("__manifest__.py" in files or "__openerp__.py" in files)
         ):
             no_deep = root
             return manifests, reqfiles, setups, no_deep
@@ -1063,22 +1199,22 @@
 
 
 def get_pyver(ctx):
     if not ctx.get("odoo_ver"):
         global python_version
         ctx["pyver"] = python_version
     else:
-        odoo_majver = int(ctx["odoo_ver"].split(".")[0])
-        if odoo_majver <= 10:
+        odoo_major = int(ctx["odoo_ver"].split(".")[0])
+        if odoo_major <= 10:
             ctx["pyver"] = "2.7"
-        elif odoo_majver == 11:
-            ctx["pyver"] = "3.5"
-        elif odoo_majver >= 12:
+        elif odoo_major == 11:
+            ctx["pyver"] = "3.6"
+        elif odoo_major >= 12:
             ctx["pyver"] = "3.7"
-        elif odoo_majver >= 14:
+        elif odoo_major >= 14:
             ctx["pyver"] = "3.8"
     return ctx
 
 
 def get_def_odoo_ver(ctx):
     py_majver = int(ctx["pyver"].split(".")[0])
     if py_majver == 3:
@@ -1093,17 +1229,19 @@
         sys.stderr.write("Please, declare odoo path to write requirements.txt file!\n")
         sys.exit(1)
     ctx["sep"] = "\n"
     ctx["from_manifest"] = True
     ctx["with_version"] = True
     ctx["itypes"] = "python"
     ctx["opt_verbose"] = False
-    ctx["base_pkgs"] = False
-    ctx["rpc_pkgs"] = False
-    ctx["test_pkgs"] = False
+    ctx["base_packages"] = False
+    ctx["rpc_packages"] = False
+    ctx["secure_packages"] = False
+    ctx["test_packages"] = False
+    ctx["exclude_devel"] = False
     ctx["oca_dependencies"] = False
     if os.path.isdir(os.path.join(ctx["odoo_dir"], "venv_odoo")):
         ctx["opt_fn"] = os.path.join(ctx["odoo_dir"], "venv_odoo", "requirements.txt")
     else:
         ctx["opt_fn"] = os.path.join(ctx["odoo_dir"], "requirements.txt")
     return ctx
 
@@ -1119,40 +1257,46 @@
     return ctx
 
 
 def main(cli_args=None):
     # if not cli_args:
     #     cli_args = sys.argv[1:]
     parser = z0lib.parseoptargs(
-        "List Odoo requirements", "© 2017-2022 by SHS-AV s.r.l.", version=__version__
+        "List Odoo requirements", "© 2017-2023 by SHS-AV s.r.l.", version=__version__
     )
     parser.add_argument("-h")
     parser.add_argument("-b", "--odoo-branch", action="store", dest="odoo_ver")
     parser.add_argument(
         "-B",
         "--base-packages",
         help="Add base & secure packages",
         action="store_true",
-        dest="base_pkgs",
+        dest="base_packages",
     )
     parser.add_argument(
         "-C",
         "--check-current-packages",
         help="Check for current installed packages",
         action="store_true",
-        dest="current_pkgs",
+        dest="check_current_packages",
     )
     parser.add_argument(
         "-d",
         "--dependencies-path",
         help="Follow oca dependency repositories in directory list",
         metavar="directory list (comma separated)",
         dest="oca_dependencies",
     )
     parser.add_argument(
+        "-j",
+        "--just-package",
+        help="Return just info of supplied package",
+        dest="pypi_name",
+    )
+    parser.add_argument(
         "-k",
         "--keep-condition",
         help="Keep condition",
         action="store_true",
         dest="keep_cond",
     )
     parser.add_argument(
@@ -1202,22 +1346,22 @@
         dest="recurse",
     )
     parser.add_argument(
         "-R",
         "--rpc-packages",
         help="Add packages for xmlrpc/jsonrpc management",
         action="store_true",
-        dest="rpc_pkgs",
+        dest="rpc_packages",
     )
     parser.add_argument(
         "-S",
         "--secure-packages",
         help="Add secure packages",
         action="store_true",
-        dest="secure_pkgs",
+        dest="secure_packages",
     )
     parser.add_argument(
         "-s",
         "--sep",
         help="Separator character of list",
         dest="sep",
         metavar="character",
@@ -1229,36 +1373,82 @@
         help="File type: may be bin,python,both or modules",
         dest="itypes",
         metavar="keyword",
         default="both",
     )
     parser.add_argument(
         "-T",
-        "--tests-packages",
-        help="Add packages for test",
+        "--test-packages",
+        help="Add packages for test environment",
         action="store_true",
-        dest="test_pkgs",
+        dest="test_packages",
+    )
+    parser.add_argument(
+        "-X",
+        "--exclude-devel",
+        help="Exclude base,rpc,secure and test packages from output list",
+        action="store_true",
+        dest="exclude_devel",
     )
     parser.add_argument("-V")
     parser.add_argument("-v")
     parser.add_argument("-y", "--python-version", action="store", dest="pyver")
     ctx = parser.parseoptargs(sys.argv[1:], apply_conf=False)
     if ctx["pyver"]:
         global PY3_DEV
         PY3_DEV = "python%s-dev" % ctx["pyver"]
     if ctx["odoo_ver"] and not ctx["pyver"]:
         ctx = get_pyver(ctx)
     if ctx["out_file"]:
         ctx = set_def_outfile(ctx)
-    if not ctx["odoo_dir"] and ctx["odoo_ver"]:
+    if (
+        not ctx["odoo_dir"]
+        and ctx["odoo_ver"]
+        and (not ctx["base_packages"]
+             and not ctx["rpc_packages"]
+             and not ctx["secure_packages"]
+             and not ctx["test_packages"])
+        or ctx["pypi_name"]
+    ):
         ctx = search_4_odoo_dir(ctx)
+
     manifests = []
     reqfiles = []
     setups = []
-    if ctx["manifests"]:
+    deps_list = {}
+    for kw in (
+        "python",
+        "python1",
+        "python2",
+        "bin",
+        "bin1",
+        "bin2",
+        "modules",
+    ):
+        deps_list[kw] = []
+
+    if ctx["pypi_name"]:
+        if ctx["itypes"] == "bin":
+            deps_list = add_dependencies(
+                deps_list,
+                ctx["pypi_name"],
+                with_version=ctx["with_version"],
+                odoo_ver=ctx["odoo_ver"],
+                pyver=ctx["pyver"])
+        else:
+            if ctx["itypes"] == "both":
+                ctx["itypes"] = "python"
+            add_package(deps_list,
+                        ctx["itypes"],
+                        ctx["pypi_name"],
+                        with_version=ctx["with_version"],
+                        odoo_ver=ctx["odoo_ver"],
+                        pyver=ctx["pyver"],
+                        ignore_deps=True)
+    elif ctx["manifests"]:
         for item in ctx["manifests"].split(","):
             if item.endswith(".py"):
                 manifests.append(os.path.expanduser(item))
             else:
                 reqfiles.append(os.path.expanduser(item))
     elif ctx["odoo_dir"]:
         if ctx["oca_dependencies"]:
@@ -1270,27 +1460,16 @@
             ctx["odoo_dir"],
             manifests,
             reqfiles,
             setups,
             ctx['from_manifest'],
             ctx['recurse'],
         )
-    deps_list = {}
-    for kw in (
-        "python",
-        "python1",
-        "python2",
-        "bin",
-        "bin1",
-        "bin2",
-        "modules",
-    ):
-        deps_list[kw] = []
 
-    if ctx["current_pkgs"]:
+    if ctx["check_current_packages"]:
         sts, stdout, stderr = z0lib.run_traced(
             "pip list", verbose=False, dry_run=ctx['dry_run'])
         if sts == 0:
             hdr = 2
             for ln in stdout.split("\n"):
                 if hdr:
                     hdr -= 1
@@ -1329,115 +1508,143 @@
         deps_list = package_from_manifest(
             deps_list,
             manifest_file,
             with_version=ctx["with_version"],
             odoo_ver=ctx["odoo_ver"],
             pyver=ctx["pyver"],
         )
-    if ctx["base_pkgs"]:
+    if ctx["secure_packages"]:
         deps_list = package_from_list(
             deps_list,
             "python",
-            PIP_ODOO_BASE_PACKAGES + PIP_SECURE_PACKAGES
-            if ctx["odoo_ver"] else PIP_BASE_PACKAGES + PIP_SECURE_PACKAGES,
+            PIP_SECURE_PACKAGES,
             with_version=ctx["with_version"],
             odoo_ver=ctx["odoo_ver"],
             pyver=ctx["pyver"],
         )
-        if ctx['pyver'] and int(ctx['pyver'].split('.')[0]) == 3:
+    if ctx["base_packages"]:
+        if not ctx["odoo_ver"]:
             deps_list = package_from_list(
                 deps_list,
                 "python",
-                PIP3_BASE_PACKAGES,
+                PIP_BASE_PACKAGES,
                 with_version=ctx["with_version"],
                 odoo_ver=ctx["odoo_ver"],
                 pyver=ctx["pyver"],
             )
-        if ctx["odoo_ver"]:
-            odoo_majver = int(ctx["odoo_ver"].split(".")[0])
-            if odoo_majver >= 10:
+            if ctx['pyver'] and int(ctx['pyver'].split('.')[0]) == 3:
                 deps_list = package_from_list(
                     deps_list,
                     "python",
-                    ["lessc"],
+                    PIP3_BASE_PACKAGES,
                     with_version=ctx["with_version"],
                     odoo_ver=ctx["odoo_ver"],
                     pyver=ctx["pyver"],
                 )
-        deps_list = package_from_list(
-            deps_list,
-            "bin",
-            BIN_BASE_PACKAGES,
-            with_version=ctx["with_version"],
-            odoo_ver=ctx["odoo_ver"],
-            pyver=ctx["pyver"],
-        )
-    if ctx["secure_pkgs"] and not ctx["base_pkgs"]:
-        deps_list = package_from_list(
-            deps_list,
-            "python",
-            PIP_SECURE_PACKAGES,
-            with_version=ctx["with_version"],
-            odoo_ver=ctx["odoo_ver"],
-            pyver=ctx["pyver"],
-        )
-    if ctx["test_pkgs"]:
-        if ctx['pyver'] and int(ctx['pyver'].split('.')[0]) == 3:
+        else:
             deps_list = package_from_list(
                 deps_list,
                 "python",
-                PIP3_TEST_PACKAGES,
+                PIP_ODOO_BASE_PACKAGES,
+                with_version=ctx["with_version"],
+                odoo_ver=ctx["odoo_ver"],
+                pyver=ctx["pyver"],
+            )
+            # odoo_major = int(ctx["odoo_ver"].split(".")[0])
+            # if odoo_major >= 10:
+            #     deps_list = package_from_list(
+            #         deps_list,
+            #         "python",
+            #         ["lessc"],
+            #         with_version=ctx["with_version"],
+            #         odoo_ver=ctx["odoo_ver"],
+            #         pyver=ctx["pyver"],
+            #     )
+            deps_list = package_from_list(
+                deps_list,
+                "bin",
+                BIN_BASE_PACKAGES,
+                with_version=ctx["with_version"],
+                odoo_ver=ctx["odoo_ver"],
+                pyver=ctx["pyver"],
+            )
+    if ctx["test_packages"]:
+        if ctx['pyver'] and int(ctx['pyver'].split('.')[0]) == 2:
+            deps_list = package_from_list(
+                deps_list,
+                "python",
+                PIP2_TEST_PACKAGES,
                 with_version=ctx["with_version"],
                 odoo_ver=ctx["odoo_ver"],
                 pyver=ctx["pyver"],
             )
         else:
             deps_list = package_from_list(
                 deps_list,
                 "python",
-                PIP_TEST_PACKAGES,
+                PIP3_TEST_PACKAGES,
                 with_version=ctx["with_version"],
                 odoo_ver=ctx["odoo_ver"],
                 pyver=ctx["pyver"],
             )
         deps_list = package_from_list(
             deps_list,
             "bin",
             BIN_TEST_PACKAGES,
             with_version=ctx["with_version"],
             odoo_ver=ctx["odoo_ver"],
             pyver=ctx["pyver"],
         )
-    if ctx["rpc_pkgs"]:
-        if ctx["odoo_ver"] and ctx["odoo_ver"].startswith("2"):
+    if ctx["rpc_packages"]:
+        if ctx["odoo_ver"] and int(ctx["odoo_ver"].split(".")[0]) <= 8:
             deps_list = package_from_list(
                 deps_list,
                 "python",
-                RPC_PACKAGES2,
+                RPC2_PACKAGES,
                 with_version=ctx["with_version"],
                 odoo_ver=ctx["odoo_ver"],
                 pyver=ctx["pyver"],
             )
         else:
             deps_list = package_from_list(
                 deps_list,
                 "python",
-                RPC_PACKAGES3,
+                RPC3_PACKAGES,
                 with_version=ctx["with_version"],
                 odoo_ver=ctx["odoo_ver"],
                 pyver=ctx["pyver"],
             )
 
     deps_list["python"] = sorted(
         deps_list["python1"] + deps_list["python2"], key=lambda s: s.lower())
+    deps_list["bin"] = sorted(
+        deps_list["bin1"] + deps_list["bin2"], key=lambda s: s.lower())
+    if ctx["exclude_devel"]:
+        for item in (PIP_SECURE_PACKAGES
+                     + PIP2_TEST_PACKAGES
+                     + PIP3_TEST_PACKAGES
+                     + BIN_TEST_PACKAGES
+                     + RPC2_PACKAGES
+                     + RPC3_PACKAGES):
+            rm_list = []
+            for ii, dep_pkg in enumerate(deps_list["python"]):
+                if deps_list["python"][ii].startswith(item):
+                    rm_list.append(ii)
+            while len(rm_list):
+                ii = rm_list.pop()
+                del deps_list["python"][ii]
+            for ii, dep_pkg in enumerate(deps_list["bin"]):
+                if deps_list["bin"][ii].startswith(item):
+                    rm_list.append(ii)
+            while len(rm_list):
+                ii = rm_list.pop()
+                del deps_list["bin"][ii]
     for ii, dep_pkg in enumerate(deps_list["python"]):
         if ">" in dep_pkg or "<" in dep_pkg or " " in dep_pkg:
             deps_list["python"][ii] = "'%s'" % dep_pkg
-    deps_list["bin"] = sorted(
-        deps_list["bin1"] + deps_list["bin2"], key=lambda s: s.lower())
     for ii, dep_pkg in enumerate(deps_list["bin"]):
         if ">" in dep_pkg or "<" in dep_pkg or " " in dep_pkg:
             deps_list["bin"][ii] = "'%s'" % dep_pkg
     for item in DEPS:
         if "python" in DEPS[item]:
             if isinstance(DEPS[item]["python"], (tuple, list)):
                 for itm in DEPS[item]["python"]:
```

### Comparing `python_plus-2.0.6/python_plus/scripts/main.py` & `python_plus-2.0.7/python_plus/scripts/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# template 20
+# template 21
 """
 Python supplemental features
 ----------------------------
 
 python_plus adds various features to python 2 and python 3 programs.
 It is designed to be used as integration of pypi future to help to port your code
 from Python 2 to Python 3 and still have it run on Python 2.
@@ -20,15 +20,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
@@ -104,20 +104,28 @@
                             else:
                                 fd.write(help_text)
                         if verbose:
                             print("$ gzip -c %s > %s" % (full_fn, tgt_fn))
                         continue
                     if lib_path:
                         tgt_fn = os.path.join(lib_path, base)
-                        try:
-                            shutil.copy(full_fn, tgt_fn)
-                            if verbose:
-                                print("$ cp %s %s" % (full_fn, tgt_fn))
-                        except shutil.SameFileError:
-                            pass
+                        if sys.version_info[0] == 3:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except shutil.SameFileError:
+                                pass
+                        else:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except BaseException:
+                                pass
                     # TODO> compatibility mode
                     tgt_fn = os.path.join(bin_path, base)
                     if os.path.isfile(tgt_fn):
                         os.unlink(tgt_fn)
                     if not os.path.exists(tgt_fn):
                         if verbose:
                             print("$ ln -s %s %s" % (full_fn, tgt_fn))
```

### Comparing `python_plus-2.0.6/python_plus/scripts/setup.info` & `python_plus-2.0.7/python_plus/scripts/setup.info`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 It is designed to be used as integration of pypi future to help to port your code from Python 2 to Python 3 and still have it run on Python 2.
 
 
 list_requirements.py: list environment requirements
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 This command is an internal command of python-plus but may be used as own command.
-list_requirements.py dispays the pypi and binaries packages needed to create a virtual environment.
+list_requirements.py displays the pypi and binaries packages needed to create a virtual environment.
 It is specially designed to show Odoo requirements.
 Passing Odoo path it reads requirements.txt files in path and setup directories of OCA repositories.
 
 vem: virtual environment manager
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 This command is an interactive tool with some nice features to manage standard virtual environment.
@@ -157,15 +157,15 @@
         'Documentation': 'https://zeroincombenze-tools.readthedocs.io',
         'Source': 'https://github.com/zeroincombenze/tools',
     },
     url='https://zeroincombenze-tools.readthedocs.io',
     author='Antonio Maria Vigliotti',
     author_email='antoniomaria.vigliotti@gmail.com',
     license='Affero GPL',
-    install_requires=['z0lib'],
+    install_requires=['configparser', 'future', 'z0lib'],
     packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
     package_data={'': ['scripts/setup.info', 'scripts/vem.sh', './vem.man']},
     entry_points={
         'console_scripts': [
             'python-plus-info = python_plus.scripts.main:main',
             'vem = python_plus.scripts.vem:main',
             "list_requirements.py = python_plus.scripts.list_requirements:main",
```

### Comparing `python_plus-2.0.6/python_plus/scripts/vem.py` & `python_plus-2.0.7/python_plus/scripts/vem.py`

 * *Files identical despite different names*

### Comparing `python_plus-2.0.6/python_plus/scripts/vem.sh` & `python_plus-2.0.7/python_plus/scripts/vem.sh`

 * *Files 5% similar despite different names*

```diff
@@ -34,35 +34,33 @@
     Z0LIBDIR=$(readlink -e $d)
     break
   fi
 done
 [[ -z "$Z0LIBDIR" ]] && echo "Library file z0librc not found in <$PYPATH>!" && exit 72
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "Z0LIBDIR=$Z0LIBDIR"
 
-# DIST_CONF=$(findpkg ".z0tools.conf" "$PYPATH")
-# TCONF="$HOME/.z0tools.conf"
 CFG_init "ALL"
 link_cfg_def
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.6
+__version__=2.0.7
 
 declare -A PY3_PKGS
-NEEDING_PKGS="future clodoo configparser os0 z0lib"
-DEV_PKGS="click flake8 pycodestyle pylint"
-SUP_PKGS="future python-plus"
-SECURE_PKGS="urllib3[secure] cryptography pyOpenSSL idna certifi asn1crypto pyasn1"
+NEEDING_PKGS="configparser future python_plus z0lib"
+# DEVEL_PKGS="click flake8 pycodestyle pylint"
+# SUP_PKGS="future python-plus"
 EI_PKGS="(distribute)"
 BZR_PKGS="(aeroolib)"
-WGET_PKGS="(pychart|python-chart)"
+# WGET_PKGS="(pychart|python-chart)"
+WGET_PKGS="(_FAULT_)"
 GIT_PKGS="(openupgradelib|prestapyt)"
 PYBIN_PKGS="(dateutil|ldap|openid)"
 BIN_PKGS="(wkhtmltopdf|lessc)"
 FLT_PKGS="(jwt|FOO)"
 UNISOLATED_PKGS="(.?-|lxml)"
 ERROR_PKGS=""
 LOCAL_PKGS="(clodoo|odoo_score|os0|python_plus|z0bug_odoo|z0lib|zerobug)"
@@ -117,19 +115,22 @@
     [[ $opt_verbose -ge 3 || ( ! $1 =~ q && $opt_verbose -ne 0 ) ]] && echo "$FLAG deactivate"
     [[ $(type -t deactivate) == "function" ]] && deactivate
     pop_venv
   fi
 }
 
 run_traced() {
+  # run_traced(cmd, verbose)
   local xcmd="$1"
   local sts=0
-  local PMPT=
+  local PMPT="" VERBOSE=$2
+  [[ -z $VERBOSE ]] && VERBOSE=$opt_verbose
   [[ $opt_dry_run -ne 0 ]] && PMPT="> " || PMPT="\$ "
-  [[ $opt_verbose -lt 2 ]] || echo "$PMPT$xcmd"
+  [[ $VERBOSE -ge 2 ]] && echo "$PMPT$xcmd"
+  [[ $VERBOSE -eq -1 ]] && echo -en "${_CS:$_CX:1}" && echo -en "\b" && ((_CX=_CX+1)) && [[ $_CX -gt 3 ]] && _CX=0
   [[ $opt_dry_run -ne 0 ]] || eval $xcmd
   sts=$?
   return $sts
 }
 
 get_actual_pkg() {
   local pkg=$1
@@ -137,15 +138,14 @@
   [[ $pkg =~ ^(psycopg2).* ]] && pkg="psycopg2-binary>=2.0.0"
   [[ $pkg =~ ^$PYBIN_PKGS([<=>!][0-9.]+)?$ ]] && pkg="python-$pkg"
   [[ $opt_pyver =~ ^3 && $pkg =~ ^${!PY3_PKGS[*]}$ ]] && pkg=${PY3_PKGS[$pkg]}
   echo $pkg
 }
 
 get_local_version() {
-  # grep "version" ./setup.py|awk -F= '{print $2}'|tr -d "'"|tr -d ","
   python ./setup.py --version
 }
 
 get_pkg_wo_version() {
   pkg=$(echo "$1"|grep --color=never -Eo '[^!<=>\\[]*'|head -n1)
   echo $pkg
 }
@@ -191,33 +191,36 @@
     d=$(find $V \( -type f -executable -o -name "*.py" \)|tr "\n" " ")
     for f in $d; do
       grep -Eq "^#\!.*/bin.*python[23]?$" $f &>/dev/null && run_traced "sed -E \"s|^#\!.*/bin.*python[23]?|#\!$PYTHON|\" -i $f" && chmod +x $f
     done
 }
 
 get_req_list() {
-# get_req_list(req_file type [debug|all|base|dev|oe|cur])
+# get_req_list(req_file type [all|base|cur|dev|oe|sec|debug])
     local cmd fn mime tt wh x
     fn="$1"
     tt="$2"
     [[ -z $3 ]] && wh="all" || wh="$3"
 
     cmd="$LIST_REQ"
-    [[ -n $tt ]] && cmd="$cmd -qt $tt -BP" || cmd="$cmd -qt python -BP"
+    [[ -n $tt ]] && cmd="$cmd -qt $tt -P" || cmd="$cmd -qt python -P"
+    [[ $wh =~ "sec" ]] && cmd="${cmd}S"
     [[ $opt_dev -ne 0 && $wh =~ (all|dev) ]] && cmd="${cmd}TR"
+    [[ $wh =~ (all|base|oe) ]] && cmd="${cmd}B"
+    [[ ! $wh =~ "base" && $wh =~ "oe" ]] && cmd="${cmd}X"
     [[ $wh =~ "cur" ]] && cmd="${cmd}C"
     [[ -n "$opt_pyver" ]] && cmd="$cmd -y$opt_pyver"
-    [[ -n "$opt_oever" && $wh =~ (all|oe) ]] && cmd="$cmd -b$opt_oever"
-    [[ -n "$opt_oepath" && $wh =~ (all|oe) ]] && cmd="$cmd -p$opt_oepath"
+    [[ -n "$opt_oever" ]] && cmd="$cmd -b$opt_oever"
+    [[ $wh =~ "oe" && -n "$opt_oepath" ]] && cmd="$cmd -p$opt_oepath"
     x="$opt_deps"
     [[ -d $HOME/OCA ]] && x="$x,${HOME}/OCA"
     [[ -d $HOME/maintainer-tools ]] && x="$x,${HOME}/maintainer-tools"
     [[ -d $HOME/maintainer-quality-tools ]] && x="$x,${HOME}/maintainer-quality-tools"
     [[ -n $x && $x =~ ^, ]] && x="${x:1}"
-    [[ -n $x  && $wh =~ (all|oe) ]] && cmd="$cmd -d${x}"
+    [[ -n $x  && $wh =~ "oe" ]] && cmd="$cmd -d${x}"
     [[ -n $fn ]] && cmd="$cmd -m $fn"
     [[ $wh =~ debug ]] && echo $cmd -qs "" || $cmd -qs" "
 }
 
 bin_install() {
   # bin_install(pkg)
   [[ $opt_verbose -gt 2 ]] && echo ">>> bin_install($*)"
@@ -280,24 +283,26 @@
     x="${pkgs//+/.}"
     [[ -z $XPKGS_RE ]] && XPKGS_RE="$x" || XPKGS_RE="$XPKGS_RE|$x"
   fi
 }
 
 bin_install_1() {
   # bin_install_1()
+  echo -en "\e[?25l"
   [[ $opt_verbose -gt 2 ]] && echo ">>> bin_install_1($*)"
   local pkg
   local binreq bin_re
   [[ -n "$opt_bins" ]] && binreq="${opt_bins//,/ }"
   if [[ -n "$opt_bins" ]]; then
-    [[ $opt_verbose -gt 0 ]] && echo -e "\e[1m.Analyzing $opt_bins\e[0m"
+    [[ $opt_verbose -gt 0 ]] && echo -e "(1) Analyzing \e[36m$opt_bins\e[0m"
     for pkg in $binreq; do
       bin_install $pkg
     done
   fi
+  echo -en "\e[?25h"
 }
 
 pip_install_wget() {
 # pip_install_wget(fn)
     local d="" pfn="$1" x
     pfn="$1"
     [[ $pfn == "python-chart" ]] && d="https://files.pythonhosted.org/packages/22/bf/f37ecd52d9f6ce81d4372956dc52c792de527abfadbf8393dd25deb5c90b/Python-Chart-1.39.tar.gz"
@@ -320,24 +325,29 @@
     [[ -z "$d" ]] && echo "Unknown URL for $pfn" && return
     run_traced "$PIP install $d"
     [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
 }
 
 pip_install() {
   #pip_install(pkg opts)
-  local pkg d x srcdir pfn popts pypath v tmpdir DISTO  FH
+  local d pfn pkg popts pypath srcdir tmpdir v vpkg x DISTO FH
   [[ $1 =~ ^[\'\"] ]] && pkg="${1:1: -1}" || pkg="$1"
   [[ $opt_verbose -gt 1 ]] && echo -e "  \e[32mpip install \"$1\" $2\e[0m"
   [[ -n $opt_FH ]] && FH=$opt_FH || FH=$(xuname -f)
   [[ -n $opt_distro ]] && DISTO=${opt_distro,,} || DISTO=$(xuname -d)
   pypath=$(find $VIRTUAL_ENV/lib -type d -name "python$opt_pyver")
   [[ -n "$pypath" && -d $pypath/site-packages ]] && pypath=$pypath/site-packages || pypath=$(find $(readlink -f $(dirname $(which $PYTHON 2>/dev/null))/../lib) -type d -name site-packages)
   tmpdir=$VIRTUAL_ENV/tmp
   pkg=$(get_actual_pkg "$pkg")
   pfn=$(get_pkg_wo_version "$pkg")
+  x="-qP"
+  [[ -n "$opt_pyver" ]] && x="$x -y$opt_pyver"
+  [[ -n "$opt_oever" ]] && x="$x -b$opt_oever"
+  [[ $pkg =~ / ]] && vpkg="$pkg" || vpkg=$($LIST_REQ $x -j $pkg)
+  [[ $vpkg =~ ^[\'\"] ]] && vpkg="${vpkg:1: -1}"
   [[ $pfn =~ (python-plus|z0bug-odoo) ]] && pfn=${pkg//-/_}
   [[ $pkg =~ "-e " ]] && pkg="${pkg//-e /--editable=}"
   [[ $opt_alone -ne 0 && ! $pkg =~ $UNISOLATED_PKGS ]] && popts="--isolated --disable-pip-version-check --no-python-version-warning --no-cache-dir" || popts="--disable-pip-version-check --no-python-version-warning"
   [[ $PIPVER -gt 18 && ! no-warn-conflicts =~ $popts ]] && popts="$popts --no-warn-conflicts"
   [[ $PIPVER -eq 19 && ! 2020-resolver =~ $popts ]] && popts="$popts --use-feature=2020-resolver"
   [[ $PIPVER -eq 21  && ! in-tree-build =~ $popts  ]] && popts="$popts --use-feature=in-tree-build"
   [[ $opt_pyver =~ ^2 && $(uname -r) =~ ^3 ]] && popts="$popts --trusted-host pypi.org --trusted-host pypi.python.org --trusted-host files.pythonhosted.org"
@@ -347,15 +357,15 @@
     if [[ ! $pfn =~ $BIN_PKGS ]]; then
       srcdir=""
       [[ $opt_debug -eq 2 && -d $SAVED_HOME_DEVEL/../tools/$pfn ]] && srcdir=$(readlink -f $SAVED_HOME_DEVEL/../tools/$pfn)
       if [[ $opt_debug -ge 3 ]]; then
         [[ -d $SAVED_HOME_DEVEL/pypi/$pfn/$pfn ]] && srcdir=$(readlink -f $SAVED_HOME_DEVEL/pypi/$pfn)
       fi
       if [[ $pfn =~ ^(odoo|openerp)$ ]]; then
-        [[ -z $opt_oepath ]] && echo "Missed Odoo version to install (please use -O and -o switches)!" && exit 1
+        [[ -z $opt_oepath ]] && echo "Missed Odoo version to install (please use -o switches)!" && exit 1
         [[ -d $opt_oepath/openerp && -f $opt_oepath/openerp/__init__.py ]] && srcdir=$opt_oepath/openerp
         [[ -d $opt_oepath/odoo && -f $opt_oepath/odoo/__init__.py ]] && srcdir=$opt_oepath/odoo
       fi
       [[ -z $srcdir && $opt_debug -ge 2 && $pfn =~ $LOCAL_PKGS ]] && echo "Invalid or not found source path $srcdir!" && exit 1
       [[ -z $srcdir && $pfn =~ ^(odoo|openerp)$ ]] && echo "Odoo source not found!" && exit 1
     fi
     if [[ $pfn =~ $BIN_PKGS ]]; then
@@ -442,62 +452,85 @@
         else
           echo "Invalid bazar package: file setup.py not found!"
           ERROR_PKGS="$ERROR_PKGS   '$pfn'"
         fi
       fi
     elif [[ $opt_debug -eq 1 ]]; then
       [[ -L $pypath/$pfn ]] && rm -f $pypath/$pfn
-      run_traced "$PIP install $popts --extra-index-url https://testpypi.python.org/pypi \"$pkg\" $2"
+      [[ $opt_verbose -lt 2 ]] && x=-1 || x=""
+      run_traced "$PIP install $popts --extra-index-url https://testpypi.python.org/pypi \"$vpkg\" $2" "$x"
       [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
     else
       [[ -L $pypath/$pfn ]] && rm -f $pypath/$pfn
-      run_traced "$PIP install $popts \"$pkg\" $2"
-      # [[ $? -ne 0 ]] && pip_install_git "$pfn"
+      [[ $opt_verbose -lt 2 ]] && x=-1 || x=""
+      run_traced "$PIP install $popts \"$vpkg\" $2" "$x"
       [[ $? -ne 0 && ! $ERROR_PKGS =~ $pfn ]] && ERROR_PKGS="$ERROR_PKGS   '$pfn'"
     fi
     x="${pkgs//+/.}"
     [[ -z $XPKGS_RE ]] && XPKGS_RE="$x" || XPKGS_RE="$XPKGS_RE|$x"
   fi
 }
 
 pip_install_1() {
   # pip_install_1(popts)
+  echo -en "\e[?25l"
   local pkg popts ll
   [[ $opt_verbose -lt 2 ]] && popts="$1 -q" || popts="$1"
-  ll="$SUP_PKGS $SECURE_PKGS $DEV_PKGS $(get_req_list "" "python" "base")"
-  [[ $opt_verbose -gt 0 ]] && echo -e "\e[1m1 - Analyzing $ll\e[0m (1)"
-  for pkg in $ll; do
-    [[ $opt_verbose -lt 2 ]] && echo -en "."
+  [[ $opt_verbose -gt 0 ]] && echo -e "(2) Analyzing \e[36m$SECURE_PKGS\e[0m"
+  for pkg in $SECURE_PKGS; do
     pip_install "$pkg" "$popts"
   done
-  [[ $opt_verbose -lt 2 ]] && echo -en "\r"
+  if [[ -n $DEVEL_PKGS ]]; then
+    [[ $opt_verbose -gt 0 ]] && echo -e "(3) Analyzing \e[36m$DEVEL_PKGS\e[0m"
+    for pkg in $DEVEL_PKGS; do
+      pip_install "$pkg" "$popts"
+    done
+  elif [[ $opt_verbose -gt 0 ]]; then
+    echo -e "\e[1m(3) No DEVEL packages\e[0m"
+  fi
+  ll=$(get_req_list "" "python" "base")
+  if [[ -n $ll ]]; then
+    [[ $opt_verbose -gt 0 ]] && echo -e "(4) Analyzing \e[36m$ll\e[0m"
+    for pkg in $ll; do
+      pip_install "$pkg" "$popts"
+    done
+  elif [[ $opt_verbose -gt 0 ]]; then
+    echo -e "\e[1m(4) No BASE packages\e[0m"
+  fi
+  echo -en "\e[?25h"
 }
 
 pip_install_2() {
   # pip_install_2(popts)
-  local pkg
-  [[ $opt_verbose -gt 0 ]] && echo -e "\e[1m2 - Analyzing $OEPKGS\e[0m (2)"
+  echo -en "\e[?25l"
+  local pkg popts
+  [[ $opt_verbose -lt 2 ]] && popts="$1 -q" || popts="$1"
+  [[ $opt_verbose -gt 0 ]] && echo -e "(5) Analyzing \e[36m$OEPKGS\e[0m"
   for pkg in $OEPKGS; do
-    pip_install "$pkg" "$1"
+    pip_install "$pkg" "$popts"
   done
+  echo -en "\e[?25h"
 }
 
 pip_install_req() {
   # pip_install_req(popts)
-  local f pfn pkg flist cmd
+  echo -en "\e[?25l"
+  local f pfn pkg flist cmd popts
+  [[ $opt_verbose -lt 2 ]] && popts="$1 -q" || popts="$1"
   for f in ${opt_rfile//,/ }; do
     pfn=$(readlink -f $f)
     [[ -z "$pfn" ]] && echo "File $f not found!" && continue
-    [[ $opt_verbose -gt 0 ]] && echo -e "\e[1m-- Analyzing file $pfn\e[0m"
+    [[ $opt_verbose -gt 0 ]] && echo -e "(6) Analyzing file \e[36m$pfn\e[0m"
     flist=$(get_req_list "$pfn")
     [[ $opt_verbose -gt 2 ]] && echo "<<<$flist>>>$(get_req_list '$pfn' '' 'debug')"
     for pkg in $flist; do
-      pip_install "$pkg" "$1"
+      pip_install "$pkg" "$popts"
     done
   done
+  echo -en "\e[?25h"
 }
 
 pip_uninstall() {
   #pip_uninstall(pkg opts)
   local pkg d x srcdir pfn popts v
   local pypath=$VIRTUAL_ENV/lib/python$opt_pyver/site-packages
   pkg=$(get_pkg_wo_version $(get_actual_pkg $1))
@@ -528,17 +561,17 @@
     fi
     x="${pkgs//+/.}"
     [[ -z $XPKGS_RE ]] && XPKGS_RE="$x" || XPKGS_RE="$XPKGS_RE|$x"
   fi
 }
 
 check_bin_package() {
-  # check_bin_package(pkg)
+  # check_bin_package(pkg, [show])
   local op reqver xreqver sts curver vpkg x
-  local vpkg=$1
+  local vpkg=$1 mode=$2
 
   op=$(echo "$vpkg" | grep --color=never -Eo '[!<=>]*' | head -n1)
   pkg=$(echo "$vpkg" | grep --color=never -Eo '[^!<=>\\[]*' | tr -d "'" | head -n1)
   reqver=$(echo "$vpkg" | grep --color=never -Eo '[^!<=>]*' | tr -d "'" | sed -n '2 p')
   [[ -n "$reqver" ]] && xreqver=$(echo $reqver | grep --color=never -Eo '[0-9]+\.[0-9]+(\.[0-9]+|)' | awk -F. '{print $1*10000 + $2*100 + $3}') || xreqver=0
   sts=0
   curver=$($pkg --version 2>/dev/null | grep --color=never -Eo "[0-9]+\.[0-9]+\.?[0-9]*" | head -n1)
@@ -558,20 +591,34 @@
         if [[ $cmd == "amend" ]]; then
           bin_install "$vpkg"
           [ $? -ne 0 ] && ERROR_PKGS="$ERROR_PKGS   '$pkg'"
         else
           ERROR_PKGS="$ERROR_PKGS   '$pkg'"
         fi
       else
-        printf "Package %-40.40s OK %s\n" "${pkg}${op}${reqver}........................................" "${curver}"
+        if [[ -n $mode && $mode == "show" ]]; then
+          echo "Name: ${pkg}"
+          echo "Version: ${curver}"
+          echo "Summary: binary package"
+          echo "Location: $(which ${pkg})"
+        else
+          printf "Package %-40.40s OK %s\n" "${pkg}${op}${reqver}........................................" "${curver}"
+        fi
       fi
     fi
   else
     if [[ -n "$curver" ]]; then
-      printf "Package %-40.40s OK %s \n" "${pkg}........................................" "${curver}"
+      if [[ -n $mode && $mode == "show" ]]; then
+        echo "Name: ${pkg}"
+        echo "Version: ${curver}"
+        echo "Summary: binary package"
+        echo "Location: $(which ${pkg})"
+      else
+        printf "Package %-40.40s OK %s \n" "${pkg}........................................" "${curver}"
+      fi
     else
       echo "Package $pkg not installed!!!"
       ERROR_PKGS="$ERROR_PKGS   '$pkg'"
     fi
   fi
   if [[ -n "$curver" ]]; then
     x=$(readlink -e $(which $pkg 2>/dev/null) 2>/dev/null)
@@ -581,36 +628,38 @@
       run_traced "ln -s $x $VENV/bin"
     fi
   fi
 }
 
 bin_check_1() {
   # bin_check(cmd VENV)
+  echo -en "\e[?25l"
   local pkg
   local binreq bin_re
   [[ -n "$opt_bins" ]] && binreq="${opt_bins//,/ }"
   [[ -z "$opt_bins" ]] && binreq="${BIN_PKGS//|/ }" && binreq="${binreq:1:-1}"
-  [[ $opt_verbose -gt 0 ]] && echo -e "\e[1m-- Analyzing bin $binreq\e[0m"
+  [[ $opt_verbose -gt 0 ]] && echo -e "(1) Analyzing bin \e[36m$binreq\e[0m"
   for pkg in $binreq; do
     check_bin_package $pkg
   done
+  echo -en "\e[?25h"
 }
 
 check_package() {
   # check_package(pkg cmd)
   local op reqver xreqver sts curver vpkg x
   local vpkg=$(get_actual_pkg $1)
 
   op=$(echo "$vpkg" | grep --color=never -Eo '[!<=>]*' | head -n1)
   pkg=$(echo "$vpkg" | grep --color=never -Eo '[^!<=>\\[]*' | tr -d "'" | head -n1)
   reqver=$(echo "$vpkg" | grep --color=never -Eo '[^!<=>]*' | tr -d "'" | sed -n '2 p')
   [[ -n "$reqver" ]] && xreqver=$(echo $reqver | grep --color=never -Eo '[0-9]+\.[0-9]+(\.[0-9]+|)' | awk -F. '{print $1*10000 + $2*100 + $3}') || xreqver=0
   sts=0
   if [[ $pkg =~ $BIN_PKGS ]]; then
-      check_bin_package "$pkg"
+    check_bin_package "$pkg"
   elif [[ -n "$reqver" ]]; then
     curver=$($PIP show $pkg 2>/dev/null| grep "^[Vv]ersion" | awk -F: '{print $2}' | tr -d ', \r\n\(\)') || curver=
     if [[ -z "$curver" ]]; then
       echo "Package $pkg not installed!!!"
       if [[ $cmd == "amend" ]]; then
         pip_install "$vpkg"
         [ $? -ne 0 ] && ERROR_PKGS="$ERROR_PKGS   '$pkg'"
@@ -629,15 +678,14 @@
         fi
       else
         printf "Package %-40.40s OK %s\n" "${pkg}${op}${reqver}........................................" "${curver}"
       fi
     fi
   else
     curver=$($PIP show $pkg 2>/dev/null| grep "^[Vv]ersion" | awk -F: '{print $2}' | tr -d ', \r\n\(\)') || curver=
-    # eval $PIP show $pkg &>/dev/null
     if [[ -n "$curver" ]]; then
       printf "Package %-40.40s OK %s\n" "${pkg}........................................" "${curver}"
     else
       echo "Package $pkg not installed!!!"
       if [[ $cmd == "amend" ]]; then
         pip_install "$vpkg"
         [ $? -ne 0 ] && ERROR_PKGS="$ERROR_PKGS   '$pkg'"
@@ -650,44 +698,67 @@
     x=$($PIP show $pkg  2>/dev/null| grep "^[Ll]ocation" | awk -F: '{print $2}' | tr -d ', \r\n\(\)')
     [[ -n "$x" && ! $x =~ ^$VENV ]] && echo "Warning: file $x is outside of virtual env"
   fi
 }
 
 pip_check_1() {
   # pip_check_1(cmd)
+  echo -en "\e[?25l"
   local pkg cmd=$1
-  local op reqver xreqver sts curver vpkg
-  [[ $opt_verbose -gt 0 ]] && echo -e "\e[1m1 - Analyzing\e[0m"
-  for vpkg in $SUP_PKGS $SECURE_PKGS $DEV_PKGS; do
-    check_package $vpkg $cmd
+  local ll op reqver xreqver sts curver
+  [[ $opt_verbose -gt 0 ]] && echo -e "(2) Analyzing \e[36m$SECURE_PKGS\e[0m"
+  for pkg in $SECURE_PKGS; do
+    check_package $pkg $cmd
   done
+  if [[ -n $DEVEL_PKGS ]]; then
+    [[ $opt_verbose -gt 0 ]] && echo -e "(3) Analyzing \e[36m$DEVEL_PKGS\e[0m"
+    for pkg in $DEVEL_PKGS; do
+      check_package $pkg $cmd
+    done
+  elif [[ $opt_verbose -gt 0 ]]; then
+    echo -e "\e[1m(3) No DEVEL packages\e[0m"
+  fi
+  ll=$(get_req_list "" "python" "base")
+  if [[ -n $ll ]]; then
+    [[ $opt_verbose -gt 0 ]] && echo -e "(4) Analyzing \e[36m$ll\e[0m"
+    for pkg in $ll; do
+      check_package $pkg $cmd
+    done
+  elif [[ $opt_verbose -gt 0 ]]; then
+    echo -e "\e[1m(4) No BASE packages\e[0m"
+  fi
+  echo -en "\e[?25h"
 }
 
 pip_check_2() {
   # pip_check_2(cmd)
+  echo -en "\e[?25l"
   local pkg cmd=$1
-  [[ $opt_verbose -gt 0 ]] && echo -e "\e[1m2 - Analyzing\e[0m"
-  for vpkg in $OEPKGS; do
-    check_package $vpkg $cmd
+  [[ $opt_verbose -gt 0 ]] && echo -e "(5) Analyzing\e[36m$OEPKGS\e[0m"
+  for pkg in $OEPKGS; do
+    check_package $pkg $cmd
   done
+  echo -en "\e[?25h"
 }
 
 pip_check_req() {
   # pip_check_req(cmd)
+  echo -en "\e[?25l"
   local f pfn pkg cmd=$1 flist cmd
   for f in ${opt_rfile//,/ }; do
     pfn=$(readlink -f $f)
     [[ -z "$pfn" ]] && echo "File $f not found!" && continue
-    [[ $opt_verbose -gt 0 ]] && echo -e "\e[1m-- Analyzing file $pfn\e[0m"
+    [[ $opt_verbose -gt 0 ]] && echo -e "(6) Analyzing file \e[36m$pfn\e[0m"
     flist=$(get_req_list "$pfn")
     [[ $opt_verbose -gt 1 ]] && echo "<<<$flist>>>$(get_req_list '$pfn' '' 'debug')"
     for pkg in $flist; do
       check_package $pkg $cmd
     done
   done
+  echo -en "\e[?25h"
 }
 
 package_debug() {
   # package_debug()
   local pkg pkgdir
   local pkgs="${LOCAL_PKGS//|/ }"
   pkgs="${pkgs:1:-1}"
@@ -701,15 +772,15 @@
     done
   fi
 }
 
 custom_env() {
   # custom_env(VENV pyver)
   [[ $opt_verbose -gt 2 ]] && echo ">>> custom_env($*)"
-  local VIRTUAL_ENV=$1 pyver=$(echo $2|grep --color=never -Eo "[0-9]"|head -n1)
+  local VIRTUAL_ENV=$1 pyver=$(echo $2|grep --color=never -Eo "[23]"|head -n1)
   sed -e 's:VIRTUAL_ENV=.*:VIRTUAL_ENV="\$(dirname \$(dirname \$(readlink -f \$BASH_SOURCE[0])))":g' -i $VIRTUAL_ENV/bin/activate
   if $(grep -q "^export HOME=" $VIRTUAL_ENV/bin/activate); then
     sed -e 's|^export HOME=.*|export HOME="\$VIRTUAL_ENV"|g' -i $VIRTUAL_ENV/bin/activate
   elif $(grep -q "^# export HOME=" $VIRTUAL_ENV/bin/activate); then
     sed -e 's|^# export HOME=.*|# export HOME="\$VIRTUAL_ENV"|g' -i $VIRTUAL_ENV/bin/activate
   else
     sed -r "/deactivate *\(\) *\{/i\READLINK=\$(which greadlink 2>/dev/null) || READLINK=\$(which readlink 2>/dev/null)" -i $VIRTUAL_ENV/bin/activate
@@ -746,42 +817,34 @@
     PIPVER=""
     if [[ -n "$opt_pyver" ]]; then
       PYTHON=$(which python$opt_pyver 2>/dev/null)
       [[ -z "$PYTHON" && $opt_pyver =~ ^3 ]] && PYTHON=python3
       [[ -z "$PYTHON" && $opt_pyver =~ ^2 ]] && PYTHON=python2
       PYTHON=$(which $PYTHON 2>/dev/null)
       [[ -z "$PYTHON" ]] && PYTHON=$(which python 2>/dev/null)
-      opt_pyver=$($PYTHON --version 2>&1 | grep "Python" | grep --color=never -Eo "[0-9]\.[0-9]" | head -n1)
+      opt_pyver=$($PYTHON --version 2>&1 | grep "Python" | grep --color=never -Eo "[23]\.[0-9]" | head -n1)
       PIP=$(which pip$opt_pyver 2>/dev/null)
       [[ -z $PIP ]] && PIP="$PYTHON -m pip"
     else
       PYTHON=$(which python 2>/dev/null)
-      opt_pyver=$($PYTHON --version 2>&1 | grep "Python" | grep --color=never -Eo "[0-9]\.[0-9]" | head -n1)
+      opt_pyver=$($PYTHON --version 2>&1 | grep "Python" | grep --color=never -Eo "[23]\.[0-9]" | head -n1)
       PIP=$(which pip 2>/dev/null)
       [[ -z $PIP ]] && PIP="$PYTHON -m pip"
     fi
-    # [[ -n $PYTHON && ! $LIST_REQ =~ bin/python ]] && LIST_REQ="$PYTHON $LIST_REQ"
 }
 
 find_odoo_path() {
-# find_odoo_path(path opts)
-    local p v x y
-    [[ -n "$1" && -d $1 ]] && p="$1"
-    if [[ -n $p ]]; then
-      x=$(basename $p)
-      [[ $x =~ ^VENV && -d $p/odoo ]] && p="$p/odoo"
-      [[ $x =~ ^venv_odoo && -d $p ]] && p=$(dirname $p)
-    fi
-    [[ -z $p && -n $opt_oepath ]] && p="$opt_oepath"
-    [[ -z $p && -n $opt_oever && -d $HOME/$opt_oever ]] && p="$HOME/$opt_oever"
-    [[ $opt_verbose -gt 2 ]] && echo ">>> find $2 $p -maxdepth 3 -type f -not -path \"*tmp*\" -a -not -path \"*old*\" -not -path \"*/__to_remove/*\" -not -path \"*/lib/*\" -not -path \"*/lib64/*\" -not -path \"*/tests/res/*\" -not -path \"*/include/*\" -not -path \"*/.*/*\" -not -path \"*/node_modules/*\"  ( -name odoo-bin -o -name openerp-server )"
-    for f in $(find $2 $p -maxdepth 3 -type f -not -path "*tmp*" -a -not -path "*old*" -not -path "*/__to_remove/*" -not -path "*/lib/*" -not -path "*/lib64/*" -not -path "*/tests/res/*" -not -path "*/include/*" -not -path "*/.*/*" -not -path "*/node_modules/*" \( -name odoo-bin -o -name openerp-server \) 2>/dev/null|sort); do
-        opt_oepath=$(dirname $f)
-        break
-    done
+# find_odoo_path(venv opts)
+    local p
+    [[ -n "$1" && -d $1 && -f $p/bin/activate  ]] && p="$1" || p="$VIRTUAL_ENV"
+    p=$(find $p -type d -regex ".*/lib/python[23][0-9.]+/site-packages")
+    [[ -z $opt_oepath && -L $p/odoo ]] && opt_oepath=$(dirname $(readlink $p/odoo))
+    [[ -z $opt_oepath && -L $p/openerp ]] && opt_oepath=$(dirname $(readlink $p/openerp))
+    [[ -n $opt_oepath ]] && opt_oepath=$(readlink -f $opt_oepath)
+    [[ ( -d $opt_oepath/odoo && -f $opt_oepath/odoo/__init__.py ) || ( -d $opt_oepath/openerp && -f $opt_oepath/openerp/__init__.py ) ]] || opt_oepath=""
 }
 
 venv_mgr_check_src_path() {
   # venv_mgr_check_src_path(VENV)
   [[ $opt_verbose -gt 2 ]] && echo ">>> venv_mgr_check_src_path($*)"
   local f VENV
   VENV="$1"
@@ -823,21 +886,20 @@
   [[ $PIPVER -gt 18 && ! no-warn-conflicts =~ $popts ]] && popts="$popts --no-warn-conflicts"
   [[ $PIPVER -eq 19 && ! 2020-resolver =~ $popts ]] && popts="$popts --use-feature=2020-resolver"
   [[ $PIPVER -eq 21  && ! in-tree-build =~ $popts  ]] && popts="$popts --use-feature=in-tree-build $popts"
   [[ $opt_pyver =~ ^2 && $(uname -r) =~ ^3 ]] && popts="$popts --trusted-host pypi.org --trusted-host pypi.python.org --trusted-host files.pythonhosted.org"
   [[ $opt_verbose -lt 2 ]] && popts="$popts -q"
   for p in $NEEDING_PKGS; do
     x=${p^^}
-    [[ $opt_debug -ne 0 && $p =~ $LOCAL_PKGS ]] && p2=" --extra-index-url https://testpypi.python.org/pypi" || p2=""
+    # [[ $opt_debug -ne 0 && $p =~ $LOCAL_PKGS ]] && p2=" --extra-index-url https://testpypi.python.org/pypi" || p2=""
     p2=""
-    [[ $opt_verbose -gt 2 && -z "${!x}" ]] && echo ">>> $PIP install $popts$p2 \"$p\""
-    [[ $opt_verbose -lt 2 ]] && echo -en "."
-    [[ -z "${!x}" ]] && $PIP install $popts$p2 "$p"
+    if [[ -z "${!x}" ]]; then
+      [[ $opt_verbose -lt 2 ]] && run_traced "$PIP install $popts$p2 \"$p\"" -1 || run_traced "$PIP install $popts$p2 \"$p\""
+    fi
   done
-  [[ $opt_verbose -lt 2 ]] && echo -en "\r"
   check_4_needing_pkgs
 }
 
 odoo_orm_path() {
     p=$1
     for x in odoo openerp; do
       [[ -d $1/$x ]] && p="$1/$x" && break
@@ -848,17 +910,21 @@
 }
 
 venv_mgr_check_oever() {
   #venv_mgr_check_oever([oe_path] [oe_ver])
   local f p v
   [[ -n $2 ]] && v="$2" || v="$opt_oever"
   [[ -n $1 ]] && p="$1" || p="$opt_oepath"
+  [[ -d $p ]] && p=$(readlink -f $p) && [[ ( -d $p/odoo && -f $p/odoo/__init__.py ) || ( -d $p/openerp && -f $p/openerp/__init__.py ) ]] || p=""
   if [[ -z "$v" && -n "$p" ]]; then
     [[ -d $p/openerp ]] && f="$p/openerp/release.py" || f="$p/odoo/release.py"
     opt_oever=$(grep "^version_info" $f|cut -d= -f2|tr -d "("|tr -d ")"|tr -d " "|awk -F, '{print $1 "." $2}')
+    opt_oepath="$p"
+  elif [[ -n $v ]]; then
+    opt_oever="$v"
   fi
 }
 
 do_venv_mgr_test() {
   # do_venv_mgr_test(VENV)
   [[ $opt_verbose -gt 2 ]] && echo ">>> do_venv_mgr_test($*)"
   local f ssp x VENV
@@ -910,18 +976,18 @@
   fi
   if [[ $cmd =~ (amend) ]]; then
     if grep -q "^ *\[ -x \$f -a ! -d \$f ] " $VENV/bin/activate &>/dev/null; then
       echo "Wrong activation script $VENV/bin/activate"
       sed -Ee "s|^ *\[ -x \\\$f -a ! -d \\\$f ] | [[ -x \$f \&\& ! -d \$f ]] \&\& grep -q \"^#\!.*[ /]python\" \$f \&>/dev/null |" -i $VENV/bin/activate
     fi
   fi
-  BINPKGS=$(get_req_list "" "bin")
-  [[ $opt_verbose -gt 2 ]] && echo "BINPKGS=$BINPKGS #\$(get_req_list '' 'bin' 'debug')"
-  OEPKGS=$(get_req_list "" "python" "oe,cur")
-  [[ $opt_verbose -gt 2 ]] && echo "OEPKGS=$OEPKGS #\$(get_req_list '' 'python' 'debug,oe,cur')"
+  # BINPKGS=$(get_req_list "" "bin")
+  # [[ $opt_verbose -gt 2 ]] && echo "BINPKGS=$BINPKGS #\$(get_req_list '' 'bin' 'debug')"
+  # [[ $opt_force -ne 0 ]] && OEPKGS=$(get_req_list "" "python" "oe,cur") || OEPKGS=$(get_req_list "" "python" "oe")
+  # [[ $opt_verbose -gt 2 ]] && echo "OEPKGS=$OEPKGS #\$(get_req_list '' 'python' 'debug,oe,cur')"
   if [[ $cmd =~ (amend|check|test|inspect) ]]; then
     V=$VENV
   elif [[ "$cmd" == "cp" ]]; then
     do_deactivate "-q"
     if [[ -f $VENV_TGT ]]; then
       # Result by strange bug
       run_traced "rm -f $VENV_TGT"
@@ -964,22 +1030,22 @@
   if [[ ! $cmd =~ (test|inspect) ]]; then
     if [ $opt_dry_run -eq 0 -a -L $V/lib64 ]; then
       rm -f $V/lib64
       ln -s $V/lib $V/lib64
     fi
     [[ ! $cmd =~ (amend|check|cp) ]] && bin_install_1 $VENV
     [[ $cmd =~ (amend|check) ]] && bin_check_1 $VENV
-    x=$($PIP --version|grep --color=never -Eo "python *[23]"|grep --color=never -Eo "[23]")
+    x=$($PIP --version|grep --color=never -Eo "python *[23]"|grep --color=never -Eo "[23]"|head -n1)
     [[ $x == "2" ]] && run_traced "$PIP install \"pip<21.0\" -U" || run_traced "$PIP install pip -U"
     PIPVER=$($PIP --version | grep --color=never -Eo "[0-9]+" | head -n1)
     [[ ! $cmd =~ (amend|check|cp) ]] && pip_install_1 "--upgrade"
     [[ $cmd =~ (amend|check) ]] && pip_check_1 $cmd
-    [[ -n "$opt_oever" && "$cmd" == "amend" ]] && pip_install_2 "--upgrade"
+    # [[ -n "$opt_oever" && "$cmd" == "amend" ]] && pip_install_2 "--upgrade"
     [[ -n "$opt_oever" && $cmd =~ (amend|check) ]] && pip_check_2 $cmd
-    [[ $cmd == "amend" && -n "$opt_rfile" ]] && pip_install_req "--upgrade"
+    # [[ $cmd == "amend" && -n "$opt_rfile" ]] && pip_install_req "--upgrade"
     [[ $cmd =~ (amend|check) && -n "$opt_rfile" ]] && pip_check_req $cmd
     if [[ ! $cmd == "check" && -z "$VENV_STS" ]]; then
       run_traced "sed -i -e 's:VIRTUAL_ENV=.*:VIRTUAL_ENV=\"'$VENV_TGT'\":g' $V/bin/activate"
       if $(grep -q "^# export HOME=" $V/bin/activate); then
         [ $opt_alone -le 1 ] && run_traced "sed -e 's|^# export HOME=.*|# export HOME=\"\$VIRTUAL_ENV\"|g' -i $V/bin/activate"
         [ $opt_alone -gt 1 ] && run_traced "sed -e 's|^# export HOME=.*|export HOME=\"\$VIRTUAL_ENV\"|g' -i $V/bin/activate"
       elif $(grep -q "^export HOME=" $V/bin/activate); then
@@ -1036,24 +1102,22 @@
       ssp=$(grep -E "^include-system-site-packages" $V/pyvenv.cfg|awk -F= '{print $2}'|tr -d " ")
     else
       ssp="false"
     fi
     [[ $ssp != true ]] || cmd="$cmd -s"
     x=$($PIP show odoo 2>/dev/null| grep -E ^Location | awk -F: '{print $2}' | sed -e "s| ||")
     if [[ -n $x ]]; then
-      venv_mgr_check_oever "$x"
       echo "Odoo version: $opt_oever"
-      echo "Odoo path: $(readlink -e $x/odoo)"
+      echo "Odoo path: $opt_oepath"
       cmd="$cmd -O $opt_oever -o $(readlink -e $x/odoo)"
     else
       x=$($PIP show openerp  2>/dev/null| grep -E ^Location | awk -F: '{print $2}' | sed -e "s| ||")
       if [[ -n $x ]]; then
-        venv_mgr_check_oever "$x"
         echo "Odoo version: $opt_oever"
-        echo "Odoo path: $(readlink -e $x/openerp)"
+        echo "Odoo path: $opt_oepath"
         cmd="$cmd -O $opt_oever -o $(readlink -e $x/openerp)"
       fi
     fi
     echo "Internal sys.path: $PATH"
     echo -e "Environment created with command: \e[1m$cmd\e[0m"
     do_deactivate
   fi
@@ -1091,21 +1155,22 @@
           fi
       fi
     fi
   fi
   PYTHON=""
   if [[ -x $opt_pyver ]]; then
     PYTHON=$opt_pyver
-    opt_pyver=$($PYTHON --version 2>&1 | grep "Python" | grep --color=never -Eo "[0-9]\.[0-9]" | head -n1)
+    opt_pyver=$($PYTHON --version 2>&1 | grep "Python" | grep --color=never -Eo "[23]\.[0-9]" | head -n1)
     PIP=$(which pip$opt_pyver 2>/dev/null)
     [[ -z $PIP ]] && PIP="$PYTHON -m pip"
     [[ -n "$PIP" ]] && PIPVER=$($PIP --version | grep --color=never -Eo "[0-9]+" | head -n1)
   else
     set_pybin $opt_pyver "opt_pyver"
   fi
+
   validate_py_oe_vers
   [[ -n "${BASH-}" || -n "${ZSH_VERSION-}" ]] && hash -r 2>/dev/null
   venvexe=$(which virtualenv 2>/dev/null)
   if [[ -n "$venvexe" ]]; then
     v=$(virtualenv --version 2>&1 | grep --color=never -Eo "[0-9]+" | head -n1)
     if [ $v -gt 17 ]; then
       [[ $opt_spkg -ne 0 ]] && p="--system-site-packages"
@@ -1146,39 +1211,34 @@
   venv_mgr_check_src_path "$VENV"
   x=$($PIP --version|grep --color=never -Eo "python *[23]"|grep --color=never -Eo "[23]")
   [[ $x == "2" ]] && run_traced "$PIP install \"pip<21.0\" -Uq" || run_traced "$PIP install pip -Uq"
   PIPVER=$($PIP --version | grep --color=never -Eo "[0-9]+" | head -n1)
   run_traced "$PIP install \"setuptools<58.0\" -Uq"
   [[ $opt_verbose -ne 0 && PRINTED_PIPVER -eq 0 ]] && echo "# $PIP.$PIPVER ..." && PRINTED_PIPVER=1
   check_installed_pkgs
+  pypi_requrements
   pypath=$(find $VENV/lib -type d -name "python$opt_pyver")
   [[ -n "$pypath" && -d $pypath/site-packages ]] && pypath=$pypath/site-packages || pypath=$(find $(readlink -f $(dirname $(which $PYTHON 2>/dev/null))/../lib) -type d -name site-packages)
-  if [[ -n "$opt_oepath" && -n "$opt_oever" ]]; then
-    BINPKGS=$(get_req_list "" "bin")
-    [[ $opt_verbose -gt 2 ]] && echo "BINPKGS=$BINPKGS #$(get_req_list '' 'bin' 'debug')"
-    OEPKGS=$(get_req_list "" "python" "oe")
-    [[ $opt_verbose -gt 2 ]] && echo "OEPKGS=$OEPKGS #$(get_req_list '' 'python' 'debug,oe')"
-    bin_install_1 $VENV
-  fi
   [[ $opt_dry_run -eq 0 ]] && custom_env $VENV $opt_pyver
   pip_install_1
-  [[ -n "$opt_oever" ]] && pip_install_2
+  if [[ -n "$opt_oever" ]]; then
+    bin_install_1 $VENV
+    pip_install_2
+  fi
   [[ -n "$opt_rfile" ]] && pip_install_req
   [[ -n "$opt_oepath" && -d $opt_oepath/openerp ]] && pip_install openerp
   [[ -n "$opt_oepath" && -d $opt_oepath/odoo ]] && pip_install odoo
   do_venv_mgr_test $VENV
 }
 
 do_venv_exec() {
   # do_venv_exec VENV cmd
   local d f mime VENV V sitecustom
   VENV="$1"
-  #do_activate
   run_traced "$2 $3 $4 $5 $6 $7 $8 $9"
-  # do_deactivate
 }
 
 do_venv_pip() {
   # do_venv_pip VENV action pkg
   local d f VENV V popts x
   local SAVED_PATH=$PATH
   local cmd="$2"
@@ -1201,24 +1261,23 @@
     [[ $PIPVER -eq 19 && ! 2020-resolver =~ $popts ]] && popts="$popts --use-feature=2020-resolver"
     [[ $PIPVER -eq 21  && ! in-tree-build =~ $popts  ]] && popts="$popts --use-feature=in-tree-build $popts"
     [[ $opt_pyver =~ ^2 && $(uname -r) =~ ^3 ]] && popts="$popts --trusted-host pypi.org --trusted-host pypi.python.org --trusted-host files.pythonhosted.org"
     [[ $opt_verbose -lt 2 ]] && popts="$popts -q"
     if [[ $cmd =~ (info|show) ]]; then
       pkg=$(get_pkg_wo_version $pkg)
       if [[ $pkg =~ $BIN_PKGS ]]; then
-        check_bin_package "$pkg"
+        check_bin_package "$pkg" "show"
       else
         run_traced "$PIP show $pkg"
         x=$($PIP show $pkg  2>/dev/null| grep -E ^Location | awk -F: '{print $2}' | sed -e "s| ||")
         [[ -n $x ]] && x=$x/$pkg
         [[ -L $x ]] && echo "Actual location is $(readlink -e $x)"
       fi
     fi
     [[ $cmd == "install" ]] && pip_install "$pkg"
-    [[ "$cmd" == "uninstall" ]] && run_traced "$PIP $cmd $pkg"
     [[ $cmd == "update" ]] && pip_install "$pkg" "--upgrade"
   fi
   do_deactivate
   export PATH=$SAVED_PATH
 }
 
 validate_py_oe_vers() {
@@ -1231,54 +1290,71 @@
     if [[ ( $odoo_majver -le 10 && $opt_pyver =~ ^3 ) || ( $odoo_majver -gt 10 && $opt_pyver =~ ^2 ) ]]; then
       echo "Invalid python version $opt_pyver for Odoo $opt_oever!"
       exit 1
     fi
   fi
 }
 
+pypi_requrements() {
+    # pypi_requirements(cur)
+    BINPKGS=$(get_req_list "" "bin")
+    [[ $opt_verbose -gt 2 ]] && echo "BINPKGS=$BINPKGS #$(get_req_list '' '' 'debug,bin')"
+    SECURE_PKGS=$(get_req_list "" "" "sec")
+    [[ $opt_verbose -gt 2 ]] && echo "SECURE_PKGS=$SECURE_PKGS #$(get_req_list '' '' 'debug,sec')"
+    [[ "$opt_bins" == "*" ]] && opt_bins="${BIN_PKGS//|/,}" && opt_bins="${opt_bins:1:-1}"
+    if [[ $opt_dev -eq 0 ]]; then
+      DEVEL_PKGS=""
+    else
+      DEVEL_PKGS=$(get_req_list "" "" "dev")
+      [[ $opt_verbose -gt 2 ]] && echo "DEVEL_PKGS=$DEVEL_PKGS #$(get_req_list '' '' 'debug,dev')"
+    fi
+    [[ -n $1 && $1 -ne 0 ]] && OEPKGS=$(get_req_list "" "python" "oe,cur") || OEPKGS=$(get_req_list "" "python" "oe")
+    [[ $opt_verbose -gt 2 ]] && echo "OEPKGS=$OEPKGS #\$(get_req_list '' 'python' 'debug,oe,cur')"
+}
 
 OPTOPTS=(h        a        B         C      D       d        E          f         F      g       k        I           i         l        n           O         o          p         q           r           s                    t          V           v           y)
 OPTLONG=(help     ""       ""        ""     devel   dep-path distro     force     ""     global  keep     indipendent isolated  lang     dry_run     odoo-ver  odoo-path  python    quiet       requirement system-site-packages travis     version     verbose     yes)
 OPTDEST=(opt_help opt_bins opt_debug opt_cc opt_dev opt_deps opt_distro opt_force opt_FH opt_gbl opt_keep opt_alone   opt_alone opt_lang opt_dry_run opt_oever opt_oepath opt_pyver opt_verbose opt_rfile   opt_spkg             opt_travis opt_version opt_verbose opt_yes)
 OPTACTI=('+'      "="      "+"       1      1       "="      "="        1         "="    1       1        2           1         "="      1           "="       "="        "="       0           "="         1                    1          "*>"        "+"         1)
 OPTDEFL=(1        ""       0         0      0       ""       ""         0         ""     0       0        0           0         ""       0           ""        ""         ""        0           ""          0                    0          ""          -1          0)
 OPTMETA=("help"   "list"   ""        ""     ""      "paths"  "distro"   ""        "name" ""      ""       ""          ""        "iso"    ""          "version" "dir"      "pyver"   ""          "file"      ""                   ""         "version"   "verbose"   "")
 OPTHELP=("this help"
   "bin packages to install (* means wkhtmltopdf,lessc)"
   "use unstable packages: -B testpypi / -BB from ~/tools / -BBB from ~/pypi / -BBBB link to local ~/pypi"
   "clear cache before executing pip command"
   "create v.environment with development packages"
   "odoo dependencies paths (comma separated)"
-  "simulate Linux distro: like Ubuntu20 Centos7 etc (requires -n switch)"
+  "simulate Linux distro: like Ubuntu22 Centos8 etc (requires -n switch)"
   "force v.environment create, if exists or inside another virtual env; amend current packages"
   "simulate Linux family: may be RHEL or Debian (requires -n switch)"
   "install npm packages globally"
   "keep python2 executable as python (deprecated)"
   "run pip in an isolated mode and set home virtual directory"
   "run pip in an isolated mode, ignoring environment variables and user configuration"
-  "set default language"
+  "set default language for environment"
   "do nothing (dry-run)"
   "install pypi required by odoo version (amend or create)"
   "odoo path used to search odoo requirements"
   "python version"
   "silent mode"
   "after created v.environment install from the given requirements file"
   "create v.environment with access to the global site-packages"
   "activate environment for travis test"
   "show version"
   "verbose mode"
   "assume yes")
 OPTARGS=(p3 p4 p5 p6 p7 p8 p9)
-# no-global-site-packages.txt
 parseoptargs "$@"
 if [[ "$opt_version" ]]; then
   echo "$__version__"
   exit $STS_SUCCESS
 fi
 
+_CS="|/-\\"
+_CX=0
 ACTIONS="help amend cp check create exec info inspect install merge mv python shell rm show uninstall update test"
 REXACT="^(${ACTIONS// /|})\$"
 # In old vem version p1 -> action and p2 > venv
 [[ $opt_verbose -gt 3 ]] && set -x
 action=""
 p2=""
 for x in 3 4 5 6; do
@@ -1309,15 +1385,15 @@
 [[ -z "$p8" && -n "$p9" ]] && p8="$p9" && p9=""
 [[ -z "$p7" && -n "$p8" ]] && p7="$p8" && p8=""
 [[ -z "$p6" && -n "$p7" ]] && p6="$p7" && p7=""
 [[ -z "$p5" && -n "$p6" ]] && p5="$p6" && p6=""
 [[ -z "$p4" && -n "$p5" ]] && p4="$p5" && p5=""
 [[ -z "$p3" && -n "$p4" ]] && p3="$p4" && p4=""
 if [[ $opt_help -gt 0 ]]; then
-  print_help "Manage virtual environment\naction may be: $ACTIONS" "(C) 2018-2021 by zeroincombenze(R)\nhttps://zeroincombenze-tools.readthedocs.io/en/latest/pypi_python_plus/rtd_description.html#vem-virtual-environment-manager\nAuthor: antoniomaria.vigliotti@gmail.com"
+  print_help "Manage virtual environment\naction may be: $ACTIONS" "(C) 2018-2023 by zeroincombenze(R)\nhttps://zeroincombenze-tools.readthedocs.io/en/latest/pypi_python_plus/rtd_description.html#vem-virtual-environment-manager\nAuthor: antoniomaria.vigliotti@gmail.com"
   exit $STS_SUCCESS
 fi
 if [[ $action =~ (help|create|python) ]]; then
   # If it is running inside travis test environment
   [[ -z "$opt_pyver" && -n "$TRAVIS_PYTHON_VERSION" ]] && opt_pyver=$TRAVIS_PYTHON_VERSION
 else
   [[ -z "$p2" || ! -f $p2/bin/activate  ]] && echo -e "${RED}Virtual environment not issued! Use $0 <VENV> ...${CLR}" && exit 1
@@ -1344,39 +1420,37 @@
 SAVED_HOME=$HOME
 SAVED_HOME_DEVEL=$HOME_DEVEL
 SAVED_PYTHONPATH=$PYTHONPATH
 PRINTED_PIPVER=0
 [[ $opt_alone -ne 0 ]] && PYTHONPATH=""
 FLAG=">"
 [[ $opt_dry_run -eq 0 ]] && FLAG="\$"
-[[ -f $TDIR/list_requirements.py ]] && LIST_REQ="$TDIR/list_requirements.py" || LIST_REQ=$(whereis list_requirements.py|head -n1|cut -d: -f2|tr -d " ")
+[[ -f $TDIR/list_requirements.py ]] && LIST_REQ="$TDIR/list_requirements.py" || LIST_REQ=""
 [[ -z $LIST_REQ ]] && echo "Command list_requirements.py not found!" && exit 1
 chmod -c +x $LIST_REQ
+# LIST_REQ="python $LIST_REQ"    #debug
 
 if [[ $action == "rm" ]]; then
   [[ $PWD == $(readlink -f $p2) ]] && cd
   rm -fR $p2
   [[ -n "${BASH-}" || -n "${ZSH_VERSION-}" ]] && hash -r 2>/dev/null
   unset PYTHON PIP
   exit 0
-elif [[ ! $action =~ (help|create) ]]; then
+elif [[ $action == "create" ]]; then
+  [[ -n $opt_oepath ]] && opt_oepath=$(readlink -f $opt_oepath) && venv_mgr_check_oever
+elif [[ $action != "help" ]]; then
   do_activate "$p2" "-q"
   venv_mgr_check_src_path "$p2"
-  [[ -z $opt_oepath ]] && find_odoo_path "$p2" "-L" || find_odoo_path "$opt_oepath" "-L"
-  venv_mgr_check_oever
+  [[ -z $opt_oepath ]] && find_odoo_path "$p2"
+  [[ -z $opt_oever ]] && venv_mgr_check_oever
   check_installed_pkgs
   validate_py_oe_vers
+  pypi_requrements "$opt_force"
 fi
-[[ "$opt_bins" == "*" ]] && opt_bins="${BIN_PKGS//|/,}" && opt_bins="${opt_bins:1:-1}"
-if [[ $action =~ (help|create|exec|python|shell) || $opt_dev -eq 0 || -z "$FUTURE" || -z "$CONFIGPARSER" || -z "$Z0LIB" || -z "$OS0" ]]; then
-  [[ $opt_dev -eq 0 ]] && DEV_PKGS=""
-else
-  DEV_PKGS=$(get_req_list "" "" "dev")
-  [[ $opt_verbose -gt 2 ]] && echo "DEV_PKGS=$DEV_PKGS #$(get_req_list '' '' 'debug,dev')"
-fi
+
 if [[ "$action" == "help" ]]; then
   man $(dirname $0)/man/man8/$(basename $0).8.gz
 elif [[ "$action" == "exec" ]]; then
   do_venv_exec "$p2" "$p3" "$p4" "$p5" "$p6" "$p7" "$p8" "$p9"
   do_deactivate "-q"
 elif [[ "$action" == "python" ]]; then
   do_venv_exec "$p2" "python" "$p3" "$p4" "$p5" "$p6" "$p7" "$p8" "$p9"
@@ -1438,10 +1512,15 @@
     echo "$XTAL install $PKGLIST    # pycups"
   fi
   if [[ $ERROR_PKGS =~ shapely ]]; then
     PKGLIST=""
     [[ $FH == "RHEL" ]] && PKGLIST="$PKGLIST geos-devel" || PKGLIST="$PKGLIST libgeos-dev"
     echo "$XTAL install $PKGLIST    # shapely"
   fi
+  if [[ $ERROR_PKGS =~ psycopg2 ]]; then
+    PKGLIST=""
+    [[ $FH == "RHEL" ]] && PKGLIST="$PKGLIST postgresql-devel" || PKGLIST="$PKGLIST libpq-dev"
+    echo "$XTAL install $PKGLIST    # psycopg2-binary / psycopg2"
+  fi
 fi
 unset PYTHON PIP
 exit 0
```

### Comparing `python_plus-2.0.6/python_plus/vem.man` & `python_plus-2.0.7/python_plus/vem.man`

 * *Files identical despite different names*

### Comparing `python_plus-2.0.6/python_plus.egg-info/PKG-INFO` & `python_plus-2.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,26 @@
-Metadata-Version: 2.1
-Name: python-plus
-Version: 2.0.6
-Summary: python useful function
-Home-page: https://zeroincombenze-tools.readthedocs.io
-Author: Antonio Maria Vigliotti
-Author-email: antoniomaria.vigliotti@gmail.com
-License: Affero GPL
-Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Project-URL: Source, https://github.com/zeroincombenze/tools
-Keywords: unit test virtual environment venv
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: System :: System Shells
-
+from setuptools import find_packages, setup
 
+setup(
+    name='python_plus',
+    version='2.0.7',
+    description='python useful function',
+    long_description="""
 Python supplemental features
 ----------------------------
 
 python-plus adds various features to python 2 and python 3 programs.
 It is designed to be used as integration of pypi future to help to port your code from Python 2 to Python 3 and still have it run on Python 2.
 
 
 list_requirements.py: list environment requirements
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 This command is an internal command of python-plus but may be used as own command.
-list_requirements.py dispays the pypi and binaries packages needed to create a virtual environment.
+list_requirements.py displays the pypi and binaries packages needed to create a virtual environment.
 It is specially designed to show Odoo requirements.
 Passing Odoo path it reads requirements.txt files in path and setup directories of OCA repositories.
 
 vem: virtual environment manager
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 This command is an interactive tool with some nice features to manage standard virtual environment.
@@ -152,9 +133,43 @@
 2.0.4 (2022-12-15)
 ~~~~~~~~~~~~~~~~~~
 
 * [IMP] Package version adjustment
 * [IMP] vem: amend show current package version
 * [IMP] vem: no python2 warning in linux kernel 3
 * [FIX] vem: best recognition of python version
-
-
+""",
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'License :: OSI Approved :: GNU Affero General Public License v3',
+        'Operating System :: POSIX',
+        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: System :: System Shells',
+    ],
+    keywords='unit test virtual environment venv',
+    project_urls={
+        'Documentation': 'https://zeroincombenze-tools.readthedocs.io',
+        'Source': 'https://github.com/zeroincombenze/tools',
+    },
+    url='https://zeroincombenze-tools.readthedocs.io',
+    author='Antonio Maria Vigliotti',
+    author_email='antoniomaria.vigliotti@gmail.com',
+    license='Affero GPL',
+    install_requires=['configparser', 'future', 'z0lib'],
+    packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
+    package_data={'': ['scripts/setup.info', 'scripts/vem.sh', './vem.man']},
+    entry_points={
+        'console_scripts': [
+            'python-plus-info = python_plus.scripts.main:main',
+            'vem = python_plus.scripts.vem:main',
+            "list_requirements.py = python_plus.scripts.list_requirements:main",
+        ]
+    },
+    zip_safe=False,
+)
```

### Comparing `python_plus-2.0.6/python_plus.egg-info/SOURCES.txt` & `python_plus-2.0.7/python_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

