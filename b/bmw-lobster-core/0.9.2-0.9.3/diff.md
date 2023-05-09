# Comparing `tmp/bmw-lobster-core-0.9.2.tar.gz` & `tmp/bmw-lobster-core-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-core-0.9.2.tar", last modified: Mon May  8 15:06:38 2023, max compression
+gzip compressed data, was "bmw-lobster-core-0.9.3.tar", last modified: Tue May  9 09:58:19 2023, max compression
```

## Comparing `bmw-lobster-core-0.9.2.tar` & `bmw-lobster-core-0.9.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.505486 bmw-lobster-core-0.9.2/
--rw-r--r--   0 florian   (1000) florian   (1000)     2692 2023-05-08 15:06:38.505486 bmw-lobster-core-0.9.2/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1733 2023-05-08 15:03:18.000000 bmw-lobster-core-0.9.2/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.497486 bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2692 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      679 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      240 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.501486 bmw-lobster-core-0.9.2/lobster/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.501486 bmw-lobster-core-0.9.2/lobster/config/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/config/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4160 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/config/lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9086 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/config/parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2500 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1243 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/exceptions.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.501486 bmw-lobster-core-0.9.2/lobster/html/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/html/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2682 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/html/assets.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9667 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/html/htmldoc.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4401 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/io.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11204 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/items.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7161 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/location.py
--rw-r--r--   0 florian   (1000) florian   (1000)     8157 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/report.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.497486 bmw-lobster-core-0.9.2/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.501486 bmw-lobster-core-0.9.2/lobster/tools/core/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/tools/core/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     1917 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/tools/core/ci_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)    15949 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/tools/core/html_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     3707 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/tools/core/online_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     1817 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/tools/core/report.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1025 2023-05-08 15:06:38.000000 bmw-lobster-core-0.9.2/lobster/version.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-08 15:06:38.505486 bmw-lobster-core-0.9.2/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2513 2023-05-08 15:03:18.000000 bmw-lobster-core-0.9.2/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.812659 bmw-lobster-core-0.9.3/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2692 2023-05-09 09:58:19.812659 bmw-lobster-core-0.9.3/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1733 2023-05-08 15:03:18.000000 bmw-lobster-core-0.9.3/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.808659 bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2692 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      679 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      240 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.808659 bmw-lobster-core-0.9.3/lobster/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.808659 bmw-lobster-core-0.9.3/lobster/config/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/config/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4160 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/config/lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9086 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/config/parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2500 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1243 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/exceptions.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.808659 bmw-lobster-core-0.9.3/lobster/html/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/html/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2682 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/html/assets.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9667 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/html/htmldoc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4401 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/io.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11204 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/items.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7161 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/location.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     8157 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/report.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.804659 bmw-lobster-core-0.9.3/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.812659 bmw-lobster-core-0.9.3/lobster/tools/core/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/tools/core/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     1917 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/tools/core/ci_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)    15949 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/tools/core/html_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     3707 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/tools/core/online_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     1817 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/tools/core/report.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1025 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/version.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-09 09:58:19.812659 bmw-lobster-core-0.9.3/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2513 2023-05-08 15:03:18.000000 bmw-lobster-core-0.9.3/setup.py
```

### Comparing `bmw-lobster-core-0.9.2/PKG-INFO` & `bmw-lobster-core-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-core
-Version: 0.9.2
+Version: 0.9.3
 Summary: Lightweight Open BMW Software Tracability Evidence Report
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-core-0.9.2/README.md` & `bmw-lobster-core-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/PKG-INFO` & `bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-core
-Version: 0.9.2
+Version: 0.9.3
 Summary: Lightweight Open BMW Software Tracability Evidence Report
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-core-0.9.2/bmw_lobster_core.egg-info/SOURCES.txt` & `bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/config/lexer.py` & `bmw-lobster-core-0.9.3/lobster/config/lexer.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/config/parser.py` & `bmw-lobster-core-0.9.3/lobster/config/parser.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/errors.py` & `bmw-lobster-core-0.9.3/lobster/errors.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/exceptions.py` & `bmw-lobster-core-0.9.3/lobster/exceptions.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/html/assets.py` & `bmw-lobster-core-0.9.3/lobster/html/assets.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/html/htmldoc.py` & `bmw-lobster-core-0.9.3/lobster/html/htmldoc.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/io.py` & `bmw-lobster-core-0.9.3/lobster/io.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/items.py` & `bmw-lobster-core-0.9.3/lobster/items.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/location.py` & `bmw-lobster-core-0.9.3/lobster/location.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/report.py` & `bmw-lobster-core-0.9.3/lobster/report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/tools/core/ci_report.py` & `bmw-lobster-core-0.9.3/lobster/tools/core/ci_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/tools/core/html_report.py` & `bmw-lobster-core-0.9.3/lobster/tools/core/html_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/tools/core/online_report.py` & `bmw-lobster-core-0.9.3/lobster/tools/core/online_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/tools/core/report.py` & `bmw-lobster-core-0.9.3/lobster/tools/core/report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.2/lobster/version.py` & `bmw-lobster-core-0.9.3/lobster/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public
 # License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-VERSION_TUPLE = (0, 9, 2)
+VERSION_TUPLE = (0, 9, 3)
 VERSION_SUFFIX = ""
 
 LOBSTER_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
     ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "LOBSTER %s" % LOBSTER_VERSION
```

### Comparing `bmw-lobster-core-0.9.2/setup.py` & `bmw-lobster-core-0.9.3/setup.py`

 * *Files identical despite different names*

