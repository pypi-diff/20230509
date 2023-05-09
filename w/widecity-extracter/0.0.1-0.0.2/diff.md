# Comparing `tmp/widecity-extracter-0.0.1.tar.gz` & `tmp/widecity-extracter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widecity-extracter-0.0.1.tar", last modified: Tue May  9 02:34:04 2023, max compression
+gzip compressed data, was "widecity-extracter-0.0.2.tar", last modified: Tue May  9 02:55:15 2023, max compression
```

## Comparing `widecity-extracter-0.0.1.tar` & `widecity-extracter-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 02:34:04.631336 widecity-extracter-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-05-09 02:23:18.000000 widecity-extracter-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      543 2023-05-09 02:34:04.631336 widecity-extracter-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      103 2023-05-09 02:33:37.000000 widecity-extracter-0.0.1/README.txt
--rw-rw-rw-   0        0        0      108 2023-05-09 02:29:53.000000 widecity-extracter-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      684 2023-05-09 02:34:04.634486 widecity-extracter-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 02:34:04.573717 widecity-extracter-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 02:34:04.597017 widecity-extracter-0.0.1/src/widecity_extracter/
--rw-rw-rw-   0        0        0        0 2023-05-09 02:24:59.000000 widecity-extracter-0.0.1/src/widecity_extracter/__init__.py
--rw-rw-rw-   0        0        0      875 2023-05-09 02:14:33.000000 widecity-extracter-0.0.1/src/widecity_extracter/text_extracter.py
-drwxrwxrwx   0        0        0        0 2023-05-09 02:34:04.629317 widecity-extracter-0.0.1/src/widecity_extracter.egg-info/
--rw-rw-rw-   0        0        0      543 2023-05-09 02:34:04.000000 widecity-extracter-0.0.1/src/widecity_extracter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-05-09 02:34:04.000000 widecity-extracter-0.0.1/src/widecity_extracter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 02:34:04.000000 widecity-extracter-0.0.1/src/widecity_extracter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-09 02:34:04.000000 widecity-extracter-0.0.1/src/widecity_extracter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 02:55:15.397395 widecity-extracter-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-05-09 02:23:18.000000 widecity-extracter-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      543 2023-05-09 02:55:15.397395 widecity-extracter-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2023-05-09 02:33:37.000000 widecity-extracter-0.0.2/README.txt
+-rw-rw-rw-   0        0        0      108 2023-05-09 02:29:53.000000 widecity-extracter-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      684 2023-05-09 02:55:15.400397 widecity-extracter-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 02:55:15.360032 widecity-extracter-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 02:55:15.377204 widecity-extracter-0.0.2/src/widecity_extracter/
+-rw-rw-rw-   0        0        0        0 2023-05-09 02:24:59.000000 widecity-extracter-0.0.2/src/widecity_extracter/__init__.py
+-rw-rw-rw-   0        0        0     1034 2023-05-09 02:54:31.000000 widecity-extracter-0.0.2/src/widecity_extracter/text_extracter.py
+drwxrwxrwx   0        0        0        0 2023-05-09 02:55:15.395387 widecity-extracter-0.0.2/src/widecity_extracter.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-05-09 02:55:15.000000 widecity-extracter-0.0.2/src/widecity_extracter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-05-09 02:55:15.000000 widecity-extracter-0.0.2/src/widecity_extracter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 02:55:15.000000 widecity-extracter-0.0.2/src/widecity_extracter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-09 02:55:15.000000 widecity-extracter-0.0.2/src/widecity_extracter.egg-info/top_level.txt
```

### Comparing `widecity-extracter-0.0.1/PKG-INFO` & `widecity-extracter-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widecity-extracter
-Version: 0.0.1
+Version: 0.0.2
 Summary: a simple package to extract text from  bills.
 Home-page: https://github.com/pypa/sampleproject
 Author: amal benny
 Author-email: widecity.official@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `widecity-extracter-0.0.1/setup.cfg` & `widecity-extracter-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6964 6563 6974 792d 6578 7472   = widecity-extr
 00000020: 6163 7465 720d 0a76 6572 7369 6f6e 203d  acter..version =
-00000030: 2030 2e30 2e31 0d0a 6175 7468 6f72 203d   0.0.1..author =
+00000030: 2030 2e30 2e32 0d0a 6175 7468 6f72 203d   0.0.2..author =
 00000040: 2061 6d61 6c20 6265 6e6e 790d 0a61 7574   amal benny..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 7769 6465  hor_email = wide
 00000060: 6369 7479 2e6f 6666 6963 6961 6c40 676d  city.official@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2061 2073 696d 706c 6520  tion = a simple 
 00000090: 7061 636b 6167 6520 746f 2065 7874 7261  package to extra
 000000a0: 6374 2074 6578 7420 6672 6f6d 2020 6269  ct text from  bi
```

### Comparing `widecity-extracter-0.0.1/src/widecity_extracter/text_extracter.py` & `widecity-extracter-0.0.2/src/widecity_extracter/text_extracter.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,33 @@
 # Defining paths to tesseract.exe
 # and the image we would be using
 path_to_tesseract = r"teract\tesseract.exe"
 
 def extract_text(image,requirement):
     image_path = image
     img = Image.open(image_path)
-    pytesseract.tesseract_cmd = path_to_tesseract
+    try:
+        pytesseract.tesseract_cmd = path_to_tesseract
+    except:
+        return 'pytesseract not found'
     text = pytesseract.image_to_string(img)
     text = str(text).capitalize()
     try:
         if text.index(requirement):
             return True
     except:
         return False
 
 
 def getmybills(folder_path,requirement):
     result= []
     for image in os.listdir(folder_path):
         found = extract_text(folder_path+'/'+image,requirement)
-        if found:
+        if found == 'pytesseract not found':
+            return 'pytesseract not found'
+        elif found:
             result.append(image)
             shutil.copy(folder_path+'/'+image,'results')
     return result
 
 
 print(getmybills('bills','total'))
```

### Comparing `widecity-extracter-0.0.1/src/widecity_extracter.egg-info/PKG-INFO` & `widecity-extracter-0.0.2/src/widecity_extracter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widecity-extracter
-Version: 0.0.1
+Version: 0.0.2
 Summary: a simple package to extract text from  bills.
 Home-page: https://github.com/pypa/sampleproject
 Author: amal benny
 Author-email: widecity.official@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

