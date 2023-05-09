# Comparing `tmp/express-pascal-voc-tools-0.0.1.tar.gz` & `tmp/express-pascal-voc-tools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express-pascal-voc-tools-0.0.1.tar", last modified: Tue May  9 11:19:18 2023, max compression
+gzip compressed data, was "express-pascal-voc-tools-0.1.0.tar", last modified: Tue May  9 17:38:45 2023, max compression
```

## Comparing `express-pascal-voc-tools-0.0.1.tar` & `express-pascal-voc-tools-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 11:19:18.045763 express-pascal-voc-tools-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      703 2023-05-09 11:19:18.037435 express-pascal-voc-tools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-09 11:17:56.000000 express-pascal-voc-tools-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 11:19:17.972515 express-pascal-voc-tools-0.0.1/express_pascal_voc_tools.egg-info/
--rw-rw-rw-   0        0        0      703 2023-05-09 11:19:16.000000 express-pascal-voc-tools-0.0.1/express_pascal_voc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-05-09 11:19:17.000000 express-pascal-voc-tools-0.0.1/express_pascal_voc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 11:19:16.000000 express-pascal-voc-tools-0.0.1/express_pascal_voc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-09 11:19:16.000000 express-pascal-voc-tools-0.0.1/express_pascal_voc_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-09 11:19:16.000000 express-pascal-voc-tools-0.0.1/express_pascal_voc_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 11:19:18.046752 express-pascal-voc-tools-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-05-09 11:19:06.000000 express-pascal-voc-tools-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:19:18.029445 express-pascal-voc-tools-0.0.1/voc_tools/
--rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.0.1/voc_tools/__init__.py
--rw-rw-rw-   0        0        0     1538 2023-05-09 10:46:50.000000 express-pascal-voc-tools-0.0.1/voc_tools/annotation.py
--rw-rw-rw-   0        0        0     1216 2023-05-09 10:39:05.000000 express-pascal-voc-tools-0.0.1/voc_tools/reader.py
--rw-rw-rw-   0        0        0        0 2023-05-09 10:19:19.000000 express-pascal-voc-tools-0.0.1/voc_tools/visulizer.py
--rw-rw-rw-   0        0        0        0 2023-05-09 10:11:39.000000 express-pascal-voc-tools-0.0.1/voc_tools/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:38:45.007046 express-pascal-voc-tools-0.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      798 2023-05-09 17:38:45.001040 express-pascal-voc-tools-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-05-09 11:26:47.000000 express-pascal-voc-tools-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 17:38:44.903297 express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/
+-rw-rw-rw-   0        0        0      798 2023-05-09 17:38:43.000000 express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-09 17:38:44.000000 express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 17:38:43.000000 express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-09 17:38:43.000000 express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-09 17:38:43.000000 express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 17:38:45.008341 express-pascal-voc-tools-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-05-09 12:11:51.000000 express-pascal-voc-tools-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:38:44.967205 express-pascal-voc-tools-0.1.0/voc_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.1.0/voc_tools/__init__.py
+-rw-rw-rw-   0        0        0     2051 2023-05-09 13:23:59.000000 express-pascal-voc-tools-0.1.0/voc_tools/annotation.py
+-rw-rw-rw-   0        0        0     2318 2023-05-09 17:37:01.000000 express-pascal-voc-tools-0.1.0/voc_tools/reader.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:38:44.987774 express-pascal-voc-tools-0.1.0/voc_tools/unittest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.1.0/voc_tools/unittest/__init__.py
+-rw-rw-rw-   0        0        0     1289 2023-05-09 13:54:53.000000 express-pascal-voc-tools-0.1.0/voc_tools/unittest/reader_test.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 10:19:19.000000 express-pascal-voc-tools-0.1.0/voc_tools/visulizer.py
+-rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.1.0/voc_tools/writer.py
```

### Comparing `express-pascal-voc-tools-0.0.1/LICENSE` & `express-pascal-voc-tools-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.0.1/PKG-INFO` & `express-pascal-voc-tools-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.0.1
+Version: 0.1.0
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Express Pascal Voc Tools
  A tool for creating, reading and visualizing Pascal VOC annotations
 
+# Getting Started
+
+## Install
+`pip install express-pascal-voc-tools`
+
+## VOC Reading
+
+
 # Collaborate
 GitHub: [https://github.com/Redcof/pascal_voc_tools.git](https://github.com/Redcof/pascal_voc_tools.git)
```

### Comparing `express-pascal-voc-tools-0.0.1/express_pascal_voc_tools.egg-info/PKG-INFO` & `express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.0.1
+Version: 0.1.0
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Express Pascal Voc Tools
  A tool for creating, reading and visualizing Pascal VOC annotations
 
+# Getting Started
+
+## Install
+`pip install express-pascal-voc-tools`
+
+## VOC Reading
+
+
 # Collaborate
 GitHub: [https://github.com/Redcof/pascal_voc_tools.git](https://github.com/Redcof/pascal_voc_tools.git)
```

### Comparing `express-pascal-voc-tools-0.0.1/setup.py` & `express-pascal-voc-tools-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,10 +18,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=['lxml'],
     version_config=True,
-    version="0.0.1"
+    version="0.1.0"
     # setup_requires=["setuptools-git-versioning"]
 )
```

### Comparing `express-pascal-voc-tools-0.0.1/voc_tools/reader.py` & `express-pascal-voc-tools-0.1.0/voc_tools/reader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,73 @@
 import os
 import pathlib
 import xml.etree.ElementTree as ET
 from voc_tools.annotation import Annotation
 
 
-def from_xml(xml_file: str):
+def from_file(file: str):
+    """
+    Generate a list of Annotation objects for a given image or xml of a PASCAL VOC dataset
+    """
+    if file.endswith(".xml"):
+        return from_xml(file)
+    else:
+        return from_image(file)
+
+
+def from_image(image_file: str):
+    """
+    Generate a list of Annotation objects for a given image of a PASCAL VOC dataset
+    """
+    image_file = pathlib.Path(image_file)
+    parent_path = image_file.parents[1] / "Annotations"
+    file_name = image_file.name.replace(".jpeg", ".xml")
+    xml_file = str(parent_path / file_name)
+    return from_xml(xml_file)
+
+
+def from_xml(xml_file: str, empty_placeholder="NULL"):
     """
     Generate a list of Annotation objects from a given VOC XML file
     """
     tree = ET.parse(xml_file)
     root = tree.getroot()
 
-    list_with_all_boxes = []
+    no_threat = True
 
     filename = root.find('filename').text
     for boxes in root.iter('object'):
+        no_threat = False
         class_ = boxes.find("name").text
         ymin = int(boxes.find("bndbox/ymin").text)
         xmin = int(boxes.find("bndbox/xmin").text)
         ymax = int(boxes.find("bndbox/ymax").text)
         xmax = int(boxes.find("bndbox/xmax").text)
         cx = (xmin + xmax) / 2
         cy = (ymin + ymax) / 2
 
         single_annotation = Annotation(filename, xmin, ymin, xmax, ymax, cx, cy, class_)
         yield single_annotation
+    if no_threat:
+        yield Annotation(filename, 0, 0, 0, 0, 0, 0, empty_placeholder)
 
 
-def from_directory(dir_path: str):
+def list_dir(dir_path: str, images=False, fullpath=True):
     """
-    Generate a list of Annotation object per file form a given directory
+    Generate a list of XML files form a given PASCAL VOC directory
     """
     dir_path = pathlib.Path(dir_path)
-    annotations_dir = dir_path / "Annotations"
+    annotations_dir = dir_path / ("JPEGImages" if images else "Annotations")
     for xml_file in os.listdir(str(annotations_dir)):
-        for annotation in from_xml(str(annotations_dir / xml_file)):
+        if fullpath:
+            yield str(annotations_dir / xml_file)
+        else:
+            yield (annotations_dir / xml_file).name
+
+
+def from_dir(dir_path: str):
+    """
+    Generate a list of Annotation object per file form a given PASCAL VOC directory
+    """
+    for xml_file in list_dir(dir_path):
+        for annotation in from_xml(xml_file):
             yield annotation
```

