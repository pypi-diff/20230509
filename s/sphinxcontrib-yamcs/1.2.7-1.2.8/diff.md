# Comparing `tmp/sphinxcontrib-yamcs-1.2.7.tar.gz` & `tmp/sphinxcontrib-yamcs-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-yamcs-1.2.7.tar", last modified: Sun Mar 19 20:28:09 2023, max compression
+gzip compressed data, was "sphinxcontrib-yamcs-1.2.8.tar", last modified: Tue May  9 09:14:40 2023, max compression
```

## Comparing `sphinxcontrib-yamcs-1.2.7.tar` & `sphinxcontrib-yamcs-1.2.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-19 20:28:09.044778 sphinxcontrib-yamcs-1.2.7/
--rw-r--r--   0 fdi        (503) staff       (20)     1316 2022-04-08 07:01:59.000000 sphinxcontrib-yamcs-1.2.7/LICENSE
--rw-r--r--   0 fdi        (503) staff       (20)      419 2023-03-19 20:28:09.044619 sphinxcontrib-yamcs-1.2.7/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)     1102 2022-04-08 07:01:59.000000 sphinxcontrib-yamcs-1.2.7/README.rst
--rw-r--r--   0 fdi        (503) staff       (20)       38 2023-03-19 20:28:09.044833 sphinxcontrib-yamcs-1.2.7/setup.cfg
--rw-r--r--   0 fdi        (503) staff       (20)      747 2023-03-19 20:26:35.000000 sphinxcontrib-yamcs-1.2.7/setup.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-19 20:28:09.021506 sphinxcontrib-yamcs-1.2.7/src/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-19 20:28:09.024376 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/
--rw-r--r--   0 fdi        (503) staff       (20)      339 2022-04-08 07:02:01.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/__init__.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-19 20:28:09.027637 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/
--rw-r--r--   0 fdi        (503) staff       (20)     3348 2023-01-31 13:24:38.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     6479 2023-03-19 20:26:00.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/autogen.py
--rw-r--r--   0 fdi        (503) staff       (20)      609 2022-04-08 07:02:01.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/color.py
--rw-r--r--   0 fdi        (503) staff       (20)      487 2022-04-08 07:02:01.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/javadoc.py
--rw-r--r--   0 fdi        (503) staff       (20)      859 2022-04-08 07:02:01.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/lexers.py
--rw-r--r--   0 fdi        (503) staff       (20)     2198 2022-04-08 07:02:01.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/opi.py
--rw-r--r--   0 fdi        (503) staff       (20)     5512 2022-06-15 21:26:21.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/options.py
--rw-r--r--   0 fdi        (503) staff       (20)     8479 2022-11-01 20:36:39.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/proto.py
--rw-r--r--   0 fdi        (503) staff       (20)    13295 2022-11-08 21:02:27.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/protoparse.py
--rw-r--r--   0 fdi        (503) staff       (20)     2216 2023-03-19 19:37:13.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/templates.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-19 20:28:09.044308 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib_yamcs.egg-info/
--rw-r--r--   0 fdi        (503) staff       (20)      419 2023-03-19 20:28:08.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib_yamcs.egg-info/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)      740 2023-03-19 20:28:08.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib_yamcs.egg-info/SOURCES.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2023-03-19 20:28:08.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib_yamcs.egg-info/dependency_links.txt
--rw-r--r--   0 fdi        (503) staff       (20)       14 2023-03-19 20:28:08.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib_yamcs.egg-info/namespace_packages.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2022-04-08 07:02:01.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib_yamcs.egg-info/not-zip-safe
--rw-r--r--   0 fdi        (503) staff       (20)       34 2023-03-19 20:28:08.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib_yamcs.egg-info/requires.txt
--rw-r--r--   0 fdi        (503) staff       (20)       14 2023-03-19 20:28:08.000000 sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib_yamcs.egg-info/top_level.txt
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-09 09:14:40.680186 sphinxcontrib-yamcs-1.2.8/
+-rw-r--r--   0 fdi        (503) staff       (20)     1316 2022-04-08 07:01:59.000000 sphinxcontrib-yamcs-1.2.8/LICENSE
+-rw-r--r--   0 fdi        (503) staff       (20)      419 2023-05-09 09:14:40.679974 sphinxcontrib-yamcs-1.2.8/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)     1102 2022-04-08 07:01:59.000000 sphinxcontrib-yamcs-1.2.8/README.rst
+-rw-r--r--   0 fdi        (503) staff       (20)       38 2023-05-09 09:14:40.680243 sphinxcontrib-yamcs-1.2.8/setup.cfg
+-rw-r--r--   0 fdi        (503) staff       (20)      747 2023-05-09 09:12:25.000000 sphinxcontrib-yamcs-1.2.8/setup.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-09 09:14:40.634648 sphinxcontrib-yamcs-1.2.8/src/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-09 09:14:40.637398 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/
+-rw-r--r--   0 fdi        (503) staff       (20)      339 2022-04-08 07:02:01.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/__init__.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-09 09:14:40.640875 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/
+-rw-r--r--   0 fdi        (503) staff       (20)     3348 2023-01-31 13:24:38.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6479 2023-03-19 20:26:00.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/autogen.py
+-rw-r--r--   0 fdi        (503) staff       (20)      609 2022-04-08 07:02:01.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/color.py
+-rw-r--r--   0 fdi        (503) staff       (20)      499 2023-05-09 08:32:57.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/javadoc.py
+-rw-r--r--   0 fdi        (503) staff       (20)      859 2022-04-08 07:02:01.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/lexers.py
+-rw-r--r--   0 fdi        (503) staff       (20)     2198 2022-04-08 07:02:01.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/opi.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6028 2023-05-09 08:44:23.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/options.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8479 2022-11-01 20:36:39.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/proto.py
+-rw-r--r--   0 fdi        (503) staff       (20)    13295 2022-11-08 21:02:27.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/protoparse.py
+-rw-r--r--   0 fdi        (503) staff       (20)     2216 2023-03-19 19:37:13.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/templates.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-09 09:14:40.679638 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib_yamcs.egg-info/
+-rw-r--r--   0 fdi        (503) staff       (20)      419 2023-05-09 09:14:40.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib_yamcs.egg-info/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)      740 2023-05-09 09:14:40.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib_yamcs.egg-info/SOURCES.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2023-05-09 09:14:40.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib_yamcs.egg-info/dependency_links.txt
+-rw-r--r--   0 fdi        (503) staff       (20)       14 2023-05-09 09:14:40.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib_yamcs.egg-info/namespace_packages.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2022-04-08 07:02:01.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib_yamcs.egg-info/not-zip-safe
+-rw-r--r--   0 fdi        (503) staff       (20)       34 2023-05-09 09:14:40.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib_yamcs.egg-info/requires.txt
+-rw-r--r--   0 fdi        (503) staff       (20)       14 2023-05-09 09:14:40.000000 sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib_yamcs.egg-info/top_level.txt
```

### Comparing `sphinxcontrib-yamcs-1.2.7/LICENSE` & `sphinxcontrib-yamcs-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-yamcs-1.2.7/README.rst` & `sphinxcontrib-yamcs-1.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-yamcs-1.2.7/setup.py` & `sphinxcontrib-yamcs-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 import setuptools
 
 setuptools.setup(
     name="sphinxcontrib-yamcs",
-    version="1.2.7",
+    version="1.2.8",
     license="BSD",
     description="Sphinx extensions for use within the Yamcs project.",
     author="Space Applications Services",
     author_email="yamcs@spaceapplications.com",
     url="https://github.com/yamcs/sphinxcontrib-yamcs",
     packages=setuptools.find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/__init__.py` & `sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/autogen.py` & `sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/autogen.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/color.py` & `sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/color.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/lexers.py` & `sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/lexers.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/opi.py` & `sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/opi.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/options.py` & `sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,31 @@
     temp_node.document = state.document
     nested_parse_with_titles(state, unprocessed, temp_node)
     return [node for node in temp_node.children]
 
 
 class OptionsDirective(SphinxDirective):
     required_arguments = 1
+    option_spec = {"scope": str}
 
     def run(self):
+        conf_key = "options"
+        if "scope" in self.options:
+            if self.options["scope"] == "global":
+                conf_key = "options"
+            if self.options["scope"] == "instance":
+                conf_key = "instanceOptions"
+            else:
+                raise Exception(f"Unexpected scope {conf_key}")
+
         result = []
         yaml_file = self.arguments[0]
         with open(yaml_file) as f:
             descriptor = yaml.load(f, Loader=yaml.FullLoader)
-            options = descriptor["options"].items()
+            options = descriptor[conf_key].items()
             head = []
             tail = []
             self.generate_nodes(options, head=head, tail=tail)
             result += head + tail
         return result
 
     def generate_nodes(self, options, head, tail):
@@ -62,17 +72,19 @@
 
             definition_nodes = []
 
             if option.get("hidden", False):
                 continue
 
             if deprecated:
-                node = nodes.Text("Deprecated: " + option["deprecationMessage"])
+                para_nodes = [nodes.Text("Deprecated.")]
+                para_nodes += produce_nodes(self.state, option["deprecationMessage"])
+                # node = nodes.Text("Deprecated: " + option["deprecationMessage"])
                 definition_nodes.append(
-                    nodes.warning("", nodes.paragraph("", "", node))
+                    nodes.warning("", nodes.paragraph("", "", *para_nodes))
                 )
 
             if "description" in option:
                 for idx, para in enumerate(option["description"]):
                     para_nodes = []
                     if idx == 0 and option.get("required", False):
                         para_nodes.append(nodes.strong("", "Required."))
```

### Comparing `sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/proto.py` & `sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/proto.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/protoparse.py` & `sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/protoparse.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib/yamcs/templates.py` & `sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib/yamcs/templates.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-yamcs-1.2.7/src/sphinxcontrib_yamcs.egg-info/SOURCES.txt` & `sphinxcontrib-yamcs-1.2.8/src/sphinxcontrib_yamcs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

