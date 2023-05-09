# Comparing `tmp/html_msg-1.0.4.tar.gz` & `tmp/html_msg-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_msg-1.0.4.tar", last modified: Tue May  9 18:15:56 2023, max compression
+gzip compressed data, was "html_msg-1.0.5.tar", last modified: Tue May  9 19:31:34 2023, max compression
```

## Comparing `html_msg-1.0.4.tar` & `html_msg-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 18:15:56.915755 html_msg-1.0.4/
--rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     2521 2023-05-09 18:15:56.915755 html_msg-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2020 2023-05-09 18:11:58.000000 html_msg-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 18:15:56.894811 html_msg-1.0.4/html_msg/
--rw-rw-rw-   0        0        0      115 2023-05-09 18:14:42.000000 html_msg-1.0.4/html_msg/__init__.py
--rw-rw-rw-   0        0        0    12111 2023-05-09 17:31:43.000000 html_msg-1.0.4/html_msg/html_message.py
--rw-rw-rw-   0        0        0    14906 2023-05-09 18:14:07.000000 html_msg-1.0.4/html_msg/html_table.py
-drwxrwxrwx   0        0        0        0 2023-05-09 18:15:56.914758 html_msg-1.0.4/html_msg.egg-info/
--rw-rw-rw-   0        0        0     2521 2023-05-09 18:15:56.000000 html_msg-1.0.4/html_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-09 18:15:56.000000 html_msg-1.0.4/html_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 18:15:56.000000 html_msg-1.0.4/html_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-09 18:15:56.000000 html_msg-1.0.4/html_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-09 18:15:56.000000 html_msg-1.0.4/html_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 18:15:56.915755 html_msg-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      796 2023-05-09 18:15:38.000000 html_msg-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:31:34.591179 html_msg-1.0.5/
+-rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     3935 2023-05-09 19:31:34.591179 html_msg-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 19:31:34.577205 html_msg-1.0.5/html_msg/
+-rw-rw-rw-   0        0        0      115 2023-05-09 18:14:42.000000 html_msg-1.0.5/html_msg/__init__.py
+-rw-rw-rw-   0        0        0    12111 2023-05-09 17:31:43.000000 html_msg-1.0.5/html_msg/html_message.py
+-rw-rw-rw-   0        0        0    14517 2023-05-09 19:00:47.000000 html_msg-1.0.5/html_msg/html_table.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:31:34.590372 html_msg-1.0.5/html_msg.egg-info/
+-rw-rw-rw-   0        0        0     3935 2023-05-09 19:31:34.000000 html_msg-1.0.5/html_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-09 19:31:34.000000 html_msg-1.0.5/html_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 19:31:34.000000 html_msg-1.0.5/html_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-09 19:31:34.000000 html_msg-1.0.5/html_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 19:31:34.000000 html_msg-1.0.5/html_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 19:31:34.591179 html_msg-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-05-09 19:30:38.000000 html_msg-1.0.5/setup.py
```

### Comparing `html_msg-1.0.4/LICENSE.txt` & `html_msg-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.4/PKG-INFO` & `html_msg-1.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,134 @@
-Metadata-Version: 2.1
-Name: html_msg
-Version: 1.0.4
-Summary: This tool allows to create HTML message via simple methods,      without the need to write HTML code manually.
-Home-page: https://github.com/
-Download-URL: https://pypi.org/project/
-Author: Sirakan Bagdasarian
-Author-email: bsirak@bk.ru
-License: MIT
-Keywords: HTML,Message
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# What is it?
-
-**html_msg** is a Python package that provides functionality to build up HTML messages via simple methods, without need to write HTML code manually.
-
-# Main Features
-
-Here are a few of the things that **html_msg** does well:
-
-* Easy adding of plain text into message
-* Creation of tables and adding them into message
-* Easy formating of text and tables via CSS properties
-* Rendering and displaying of HTML message in IPython notebook
-
-# Where to get it
-
-```
-# PyPI
-pip install html-msg
-```
-
-# Documentation
-
-## Getting started
-
-
-Import main classes from the package. 
-
-```
-from html_msg import HTMLMessage, HTMLTable
-```
-
-## Message creation
-
-Now let's create a message and add there some text.
-
-```
-# Create an instance of HTMLMessage
-message = HTMLMessage()
-
-# add line of text into message
-message.insert_text('Hello, Dears!')
-
-# add another line of text, but on new line this time
-message.insert_text('Here are the latest news...', new_line=True)
-
-# in order to add an empty line, pass an empty string to the method 'insert_text'
-message.insert_text('', new_line=True)
-
-# and let's add another line of text, but this time it should be bold
-bold_text_style = {'font-weight':'bold'}
-message.insert_text('Must be this line of text is important!', new_line=True, style_dict=bold_text_style)
-```
-
-In order to see, what we created, use the method 'display'. 
-Please note, that this method uses IPython functionality. 
-
-```
-message.display()
-```
-
-The result should look like this:
-  
-Hello, Dears!  
-Here are the latest news...  
-  
-**Must be this line of text is important!**
-
-## Transformation to HTML code
-
-Now, we can transform this message to HTML code in order to send it.  
-Please note, that this library does not provide functionality to send messages.  
-One should use other libraries for that. 
-
-```
-# the method 'to_string' returns HTML code in string formart. 
-# One can pass it to abstract email sender, which will send it to the recepient.
-html_code = message.to_string()
-```
-
-
-```python
-
-```
-
-
+# What is it?
+
+**html_msg** is a Python package that provides functionality to build up HTML messages via simple methods, without the need to write HTML code manually.
+
+# Main Features
+
+Here are a few of the things that **html_msg** does well:
+
+* Easy adding of plain text into message
+* Creation of tables and adding them into message
+* Easy formating of text and tables via CSS properties
+* Rendering and displaying of HTML message in IPython notebook
+
+# Where to get it
+
+```
+# PyPI
+pip install html-msg
+```
+
+# Documentation
+
+## Getting started
+
+
+Import main classes from the package. 
+
+```
+from html_msg import HTMLMessage, HTMLTable
+```
+
+## Message creation
+
+Now let's create a message and add there some text.
+
+```
+# Create an instance of HTMLMessage
+message = HTMLMessage()
+
+# add line of text into message
+message.insert_text('Hello, Dears!')
+
+# add another line of text, but on new line this time
+message.insert_text('Here are the latest news...', new_line=True)
+
+# in order to add an empty line, pass an empty string to the method 'insert_text'
+message.insert_text('', new_line=True)
+
+# and let's add another line of text, but this time it should be bold
+bold_text_style = {'font-weight':'bold'}
+message.insert_text('Must be this line of text is important!', 
+                    new_line=True, 
+                    style_dict=bold_text_style)
+```
+
+In order to see, what we created, use the method 'display'. 
+Please note, that this method uses IPython functionality. 
+
+```
+message.display()
+```
+
+The result should look like this:
+  
+Hello, Dears!  
+Here are the latest news...  
+  
+**Must be this line of text is important!**
+
+## Table creation
+
+Let's create a table and fill it with some data
+
+```
+# create list that contains table headers
+table_headers = ['Item', 'Price', 'quantity']
+
+# rows are represented as list of lists. Every list is a row. 
+initial_rows = [ 
+    ['Apple', 10, 245], 
+    ['Orange', 25, 199] 
+]
+
+# create an instance of HTMLTable, pass arguments that were defined above
+table = HTMLTable(rows=initial_rows, headers=table_headers)
+```
+
+We can add rows whenever we want to:
+
+```
+# in order to add a row to the table, use method 'add_row'
+table.add_row(['Pear', 19, 387])
+```
+
+Or change headers, if necessary:
+
+```
+table.set_headers(['Goods', 'Net price', 'Amount'])
+```
+
+There are several design presets that you can apply to the table, in order to see them, use method 'show_table_design_presets'
+
+```
+table.show_table_design_presets()
+```
+
+By default, preset 'Basic' is used, but you can apply any design you like better via the method 'apply_design_preset'
+
+```
+table.apply_design_preset('Grey')
+```
+
+In order to insert the table into the message, you first need to transform the table into HTML code  
+and then insert this HTML into the message body.
+
+```
+# transforming table into html code, which is contained in string format
+table_html = table.to_string()
+
+# inserting table into message body
+message.insert_html(table_html)
+```
+
+## Transformation to HTML code
+
+Now, we can transform this message to HTML code in order to send it.  
+Please note that this library does not provide functionality to send messages.  
+One should use other libraries for that. 
+
+```
+# the method 'to_string' returns HTML code in string formart. 
+# One can pass it to abstract email sender, which will send it to the recepient.
+html_code = message.to_string()
+```
```

### Comparing `html_msg-1.0.4/html_msg/html_message.py` & `html_msg-1.0.5/html_msg/html_message.py`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.4/html_msg/html_table.py` & `html_msg-1.0.5/html_msg/html_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 class HTMLTable:
     
     presets = {
-         "Simple": {
+        "Basic": {
         
-            "table_style": "border: none; padding: 5pt 5pt 5pt;",
-            "header_style": "border: none; padding: 5pt 5pt 5pt; font-weight: bold;",
+            "table_style": "border: 1px solid; border-collapse: collapse; padding: 5pt 5pt 5pt;",
+            "header_style": "border: 1px solid; border-collapse: collapse; padding: 5pt 5pt 5pt; font-weight: bold; text-align: center;",
         },
-            "Fancy":{
+            
+        "Tile":{
             
             "table_style": "border: solid #E0E0E0 1.0pt; border-radius: 10px; padding: 10pt 10pt 10pt; background-color: #F8F8F8;",
             "header_style": "border: solid #E0E0E0 1.0pt; border-radius: 10px; padding: 10pt 10pt 10pt; background-color: #F8F8F8; font-weight: bold;",
         },
-        "Modern": {
-            
-            "table_style": "border-collapse: collapse; padding: 5pt 5pt 5pt; font-family: Arial, sans-serif;",
-            "header_style": "border: solid #E0E0E0 1.0pt; border-collapse: collapse; padding: 5pt 5pt 5pt; background-color: #F8F8F8; font-weight: bold; font-family: Arial, sans-serif;",
-        },
-        "Modern2":
+        
+        "Modern":
         {
             "table_style": "border-top: solid #E0E0E0 1.0pt; border-left: none; border-bottom: solid #E0E0E0 1.0pt; border-right: none; padding: 3.75pt 3.75pt 3.75pt; color: #1B5198; text-align: left;",
             "header_style": "border-top: none; border-left: none; border-bottom: solid #E0E0E0 1.0pt; border-right: none; padding: 3.75pt 3.75pt 3.75pt; text-align: center; color: #6C8999"
         },
-        'Grey':{
+        
+        "Grey":{
             "table_style": "border: 1.5px solid #000000;text-align: center;border-collapse: collapse; padding: 5pt 5pt 5pt;color: black;",
             "header_style": "border: 1.5px solid #000000;text-align: center;border-collapse: collapse;background: linear-gradient(to bottom, #dbdbdb 0%, #d3d3d3 66%, #CFCFCF 100%);border-bottom: 1.5px solid #000000;color: black;padding: 10pt 10pt 10pt;margin-left: auto;margin-right: auto;"
         },
         
     }
     
     def __init__(self, rows=None, headers=None):
@@ -36,17 +34,17 @@
             self.rows = rows
         
         self.headers = headers
         self.cell_color_map = {}
         self.cell_style_map = {}
         self.font_family = 'Arial'
         self.font_size = '12px'
-        self.font_color = '#1B5198'
-        self.table_style = self.presets["True Modern"]["table_style"]
-        self.header_style = self.presets["True Modern"]["header_style"]
+        self.font_color = 'black'
+        self.table_style = self.presets["Basic"]["table_style"]
+        self.header_style = self.presets["Basic"]["header_style"]
         self.html_table  = ''
     
     def __update_table(self):
         self.html_table = f'<table style="font-family: {self.font_family}; font-size: {self.font_size}; color: {self.font_color}; {self.table_style}">\n'
         self.__update_headers()
         self.__update_rows()
         self.html_table += '</table>'
@@ -333,15 +331,15 @@
         self.set_headers(df_headers)
         df_rows = df.values.tolist()
         for row in df_rows:
             self.add_row(row)
         
 
     def create_html_hyperlink(self, link, text):
-        # возможно нужно создать класс Formatter, который будет отвечать за такие штуки. 
+        
         '''
         Create an HTML hyperlink with the given link text and URL.
         This method might be used with the method "add_row" in order to insert link into the table.  
 
         Args:
             link_text (str): The text to be displayed as the hyperlink.
             url (str): The URL that the hyperlink should point to.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `html_msg-1.0.4/html_msg.egg-info/PKG-INFO` & `html_msg-1.0.5/html_msg.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: html-msg
-Version: 1.0.4
+Version: 1.0.5
 Summary: This tool allows to create HTML message via simple methods,      without the need to write HTML code manually.
 Home-page: https://github.com/
 Download-URL: https://pypi.org/project/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
 Keywords: HTML,Message
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # What is it?
 
-**html_msg** is a Python package that provides functionality to build up HTML messages via simple methods, without need to write HTML code manually.
+**html_msg** is a Python package that provides functionality to build up HTML messages via simple methods, without the need to write HTML code manually.
 
 # Main Features
 
 Here are a few of the things that **html_msg** does well:
 
 * Easy adding of plain text into message
 * Creation of tables and adding them into message
@@ -57,15 +57,17 @@
 message.insert_text('Here are the latest news...', new_line=True)
 
 # in order to add an empty line, pass an empty string to the method 'insert_text'
 message.insert_text('', new_line=True)
 
 # and let's add another line of text, but this time it should be bold
 bold_text_style = {'font-weight':'bold'}
-message.insert_text('Must be this line of text is important!', new_line=True, style_dict=bold_text_style)
+message.insert_text('Must be this line of text is important!', 
+                    new_line=True, 
+                    style_dict=bold_text_style)
 ```
 
 In order to see, what we created, use the method 'display'. 
 Please note, that this method uses IPython functionality. 
 
 ```
 message.display()
@@ -74,25 +76,74 @@
 The result should look like this:
   
 Hello, Dears!  
 Here are the latest news...  
   
 **Must be this line of text is important!**
 
+## Table creation
+
+Let's create a table and fill it with some data
+
+```
+# create list that contains table headers
+table_headers = ['Item', 'Price', 'quantity']
+
+# rows are represented as list of lists. Every list is a row. 
+initial_rows = [ 
+    ['Apple', 10, 245], 
+    ['Orange', 25, 199] 
+]
+
+# create an instance of HTMLTable, pass arguments that were defined above
+table = HTMLTable(rows=initial_rows, headers=table_headers)
+```
+
+We can add rows whenever we want to:
+
+```
+# in order to add a row to the table, use method 'add_row'
+table.add_row(['Pear', 19, 387])
+```
+
+Or change headers, if necessary:
+
+```
+table.set_headers(['Goods', 'Net price', 'Amount'])
+```
+
+There are several design presets that you can apply to the table, in order to see them, use method 'show_table_design_presets'
+
+```
+table.show_table_design_presets()
+```
+
+By default, preset 'Basic' is used, but you can apply any design you like better via the method 'apply_design_preset'
+
+```
+table.apply_design_preset('Grey')
+```
+
+In order to insert the table into the message, you first need to transform the table into HTML code  
+and then insert this HTML into the message body.
+
+```
+# transforming table into html code, which is contained in string format
+table_html = table.to_string()
+
+# inserting table into message body
+message.insert_html(table_html)
+```
+
 ## Transformation to HTML code
 
 Now, we can transform this message to HTML code in order to send it.  
-Please note, that this library does not provide functionality to send messages.  
+Please note that this library does not provide functionality to send messages.  
 One should use other libraries for that. 
 
 ```
 # the method 'to_string' returns HTML code in string formart. 
 # One can pass it to abstract email sender, which will send it to the recepient.
 html_code = message.to_string()
 ```
 
 
-```python
-
-```
-
-
```

### Comparing `html_msg-1.0.4/setup.py` & `html_msg-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 
 setup_args = dict(
     name='html_msg',
-    version='1.0.4',
+    version='1.0.5',
     description='This tool allows to create HTML message via simple methods, \
      without the need to write HTML code manually.',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     license='MIT',
     packages=find_packages(),
     author='Sirakan Bagdasarian',
```

