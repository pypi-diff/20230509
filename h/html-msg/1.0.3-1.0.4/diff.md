# Comparing `tmp/html_msg-1.0.3.tar.gz` & `tmp/html_msg-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_msg-1.0.3.tar", last modified: Mon May  8 17:21:43 2023, max compression
+gzip compressed data, was "html_msg-1.0.4.tar", last modified: Tue May  9 18:15:56 2023, max compression
```

## Comparing `html_msg-1.0.3.tar` & `html_msg-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 17:21:43.011905 html_msg-1.0.3/
--rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      405 2023-05-08 17:21:43.011905 html_msg-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-05-08 15:29:13.000000 html_msg-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 17:21:43.001932 html_msg-1.0.3/html_msg/
--rw-rw-rw-   0        0        0      115 2023-05-08 17:15:04.000000 html_msg-1.0.3/html_msg/__init__.py
--rw-rw-rw-   0        0        0    12353 2023-05-06 11:56:05.000000 html_msg-1.0.3/html_msg/html_message.py
--rw-rw-rw-   0        0        0    14922 2023-05-06 11:55:20.000000 html_msg-1.0.3/html_msg/html_table.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:21:43.010908 html_msg-1.0.3/html_msg.egg-info/
--rw-rw-rw-   0        0        0      405 2023-05-08 17:21:42.000000 html_msg-1.0.3/html_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-08 17:21:42.000000 html_msg-1.0.3/html_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 17:21:42.000000 html_msg-1.0.3/html_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 17:21:42.000000 html_msg-1.0.3/html_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 17:21:42.000000 html_msg-1.0.3/html_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 17:21:43.011905 html_msg-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      779 2023-05-08 17:21:21.000000 html_msg-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:15:56.915755 html_msg-1.0.4/
+-rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2521 2023-05-09 18:15:56.915755 html_msg-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2020 2023-05-09 18:11:58.000000 html_msg-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 18:15:56.894811 html_msg-1.0.4/html_msg/
+-rw-rw-rw-   0        0        0      115 2023-05-09 18:14:42.000000 html_msg-1.0.4/html_msg/__init__.py
+-rw-rw-rw-   0        0        0    12111 2023-05-09 17:31:43.000000 html_msg-1.0.4/html_msg/html_message.py
+-rw-rw-rw-   0        0        0    14906 2023-05-09 18:14:07.000000 html_msg-1.0.4/html_msg/html_table.py
+drwxrwxrwx   0        0        0        0 2023-05-09 18:15:56.914758 html_msg-1.0.4/html_msg.egg-info/
+-rw-rw-rw-   0        0        0     2521 2023-05-09 18:15:56.000000 html_msg-1.0.4/html_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-09 18:15:56.000000 html_msg-1.0.4/html_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 18:15:56.000000 html_msg-1.0.4/html_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-09 18:15:56.000000 html_msg-1.0.4/html_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 18:15:56.000000 html_msg-1.0.4/html_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 18:15:56.915755 html_msg-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-05-09 18:15:38.000000 html_msg-1.0.4/setup.py
```

### Comparing `html_msg-1.0.3/LICENSE.txt` & `html_msg-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.3/html_msg/html_message.py` & `html_msg-1.0.4/html_msg/html_message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# add method 'show_design_tips'
 # How to center table: add to header style this two attributes - margin-left: auto; margin-right: auto;
-# надо добавить метод info, который будет возвращать...хз что, инфу про каждый метод? Надо глянуть у Ромы как это реализовано.
 # сделать 2 красивых пресета
 
 class HTMLMessage:
     def __init__(self, body=""):
         self.body = body
         self.html = ""
 
@@ -53,23 +51,23 @@
         '''
         
         self.html = ""
         self.__add_header()
         self.__add_body()
         self.__add_footer()
 
-    def add_html(self, html_code):
+    def insert_html(self, html_code):
         
         '''
-        Add HTML code to the message body.
+        Inserts HTML code into the message body.
         Args:
             html_code (str): The HTML code to be added to the message body.
         Example:
             msg = HTMLMessage()
-            msg.add_html("<h1>Hello, World!</h1>")
+            msg.insert_html("<h1>Hello, World!</h1>")
         '''
         
         self.body += html_code
         self.__update_message()
 
     def insert_text(self, text, new_line=False, style_dict={}):
         
@@ -232,15 +230,16 @@
         <h1>vertical-align:</h1> The vertical alignment of the text can be specified as a keyword (e.g. "baseline", "middle", "top", "bottom").
         <p style="vertical-align: top;">{'vertical-align': 'top'}</p>
         <p style="vertical-align: bottom;">{'vertical-align': 'bottom'}</p>
         
         <h1>text-shadow:</h1> The shadow effect of the text can be specified as a series of values, including the horizontal and vertical offsets (in pixels or other units), the blur radius, and the color of the shadow (e.g. "2px 2px 2px #000000").
         <p style="text-shadow: 1px 1px 1px #ff0000;">{'text-shadow': '1px 1px 1px #ff0000'}</p>
         <p style="text-shadow: 3px 3px 5px rgba(0, 0, 0, 0.5);">{'text-shadow': '3px 3px 5px rgba(0, 0, 0, 0.5)'}</p>        
-                '''
+        
+        '''
         
         msg_display(msg_HTML(html_tips))
     
     def to_string(self):
         
         '''
         Converts the HTML message to a string. This method should be used to assign html code in string format to a variable,
```

### Comparing `html_msg-1.0.3/html_msg/html_table.py` & `html_msg-1.0.4/html_msg/html_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 class HTMLTable:
     
     presets = {
-         "Minimalistic": {
+         "Simple": {
         
             "table_style": "border: none; padding: 5pt 5pt 5pt;",
             "header_style": "border: none; padding: 5pt 5pt 5pt; font-weight: bold;",
         },
             "Fancy":{
             
             "table_style": "border: solid #E0E0E0 1.0pt; border-radius: 10px; padding: 10pt 10pt 10pt; background-color: #F8F8F8;",
             "header_style": "border: solid #E0E0E0 1.0pt; border-radius: 10px; padding: 10pt 10pt 10pt; background-color: #F8F8F8; font-weight: bold;",
         },
         "Modern": {
             
             "table_style": "border-collapse: collapse; padding: 5pt 5pt 5pt; font-family: Arial, sans-serif;",
             "header_style": "border: solid #E0E0E0 1.0pt; border-collapse: collapse; padding: 5pt 5pt 5pt; background-color: #F8F8F8; font-weight: bold; font-family: Arial, sans-serif;",
         },
-        "True Modern":
+        "Modern2":
         {
             "table_style": "border-top: solid #E0E0E0 1.0pt; border-left: none; border-bottom: solid #E0E0E0 1.0pt; border-right: none; padding: 3.75pt 3.75pt 3.75pt; color: #1B5198; text-align: left;",
             "header_style": "border-top: none; border-left: none; border-bottom: solid #E0E0E0 1.0pt; border-right: none; padding: 3.75pt 3.75pt 3.75pt; text-align: center; color: #6C8999"
         },
-        'Grey Table':{
+        'Grey':{
             "table_style": "border: 1.5px solid #000000;text-align: center;border-collapse: collapse; padding: 5pt 5pt 5pt;color: black;",
             "header_style": "border: 1.5px solid #000000;text-align: center;border-collapse: collapse;background: linear-gradient(to bottom, #dbdbdb 0%, #d3d3d3 66%, #CFCFCF 100%);border-bottom: 1.5px solid #000000;color: black;padding: 10pt 10pt 10pt;margin-left: auto;margin-right: auto;"
         },
         
     }
     
     def __init__(self, rows=None, headers=None):
```

### Comparing `html_msg-1.0.3/setup.py` & `html_msg-1.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 
 setup_args = dict(
     name='html_msg',
-    version='1.0.3',
+    version='1.0.4',
     description='This tool allows to create HTML message via simple methods, \
-        even if you dont now HTML',
+     without the need to write HTML code manually.',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     license='MIT',
     packages=find_packages(),
     author='Sirakan Bagdasarian',
     author_email='bsirak@bk.ru',
     keywords=['HTML', 'Message'],
```

