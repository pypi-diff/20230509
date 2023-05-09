# Comparing `tmp/driveup-0.3.0.tar.gz` & `tmp/driveup-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "driveup-0.3.0.tar", last modified: Fri May  5 14:12:31 2023, max compression
+gzip compressed data, was "driveup-0.4.0.tar", last modified: Tue May  9 12:36:56 2023, max compression
```

## Comparing `driveup-0.3.0.tar` & `driveup-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:12:31.782610 driveup-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:12:31.778610 driveup-0.3.0/Driveup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:12:20.000000 driveup-0.3.0/Driveup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-05 14:12:20.000000 driveup-0.3.0/Driveup/drive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:12:31.778610 driveup-0.3.0/Driveup/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:12:20.000000 driveup-0.3.0/Driveup/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-05 14:12:20.000000 driveup-0.3.0/Driveup/features/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 14:12:20.000000 driveup-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 14:12:31.782610 driveup-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 14:12:20.000000 driveup-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:12:31.782610 driveup-0.3.0/driveup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 14:12:31.000000 driveup-0.3.0/driveup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-05 14:12:31.000000 driveup-0.3.0/driveup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:12:31.000000 driveup-0.3.0/driveup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 14:12:31.000000 driveup-0.3.0/driveup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 14:12:31.000000 driveup-0.3.0/driveup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:12:31.782610 driveup-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-05 14:12:20.000000 driveup-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:36:56.903078 driveup-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:36:56.903078 driveup-0.4.0/Driveup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:36:40.000000 driveup-0.4.0/Driveup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-09 12:36:40.000000 driveup-0.4.0/Driveup/drive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:36:56.903078 driveup-0.4.0/Driveup/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:36:40.000000 driveup-0.4.0/Driveup/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-09 12:36:40.000000 driveup-0.4.0/Driveup/features/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 12:36:40.000000 driveup-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-09 12:36:56.903078 driveup-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 12:36:40.000000 driveup-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:36:56.903078 driveup-0.4.0/driveup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-09 12:36:56.000000 driveup-0.4.0/driveup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-09 12:36:56.000000 driveup-0.4.0/driveup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 12:36:56.000000 driveup-0.4.0/driveup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-09 12:36:56.000000 driveup-0.4.0/driveup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 12:36:56.000000 driveup-0.4.0/driveup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 12:36:56.903078 driveup-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-09 12:36:40.000000 driveup-0.4.0/setup.py
```

### Comparing `driveup-0.3.0/Driveup/drive.py` & `driveup-0.4.0/Driveup/drive.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from googleapiclient.discovery import build
 from googleapiclient.http import MediaFileUpload
 import os
 import re
 
 class Drive:
     def __init__(self,creds):
-        self.service = build('drive', 'v3', credentials=creds)
+        self.mode = creds['type']
+        self.service = build('drive', 'v3', credentials=creds['creds'])
     
     def upload(self,file_path,folder_id,file_title=None,file_id=None,update=True,convert=False,url=True):
 
         if url == True:
             folder_id = self.url_to_id(folder_id)
 
         if file_title == None:
@@ -22,37 +23,54 @@
         media = MediaFileUpload(file_path, resumable=True)
 
         # possible refactor
         if update == True:
             file_metadata = self.get_update(file_title,file_id,folder_id,drive_service)
                 
         if file_metadata == None: # Doesn't exist in the folder already or update=False
-            file_metadata = {'name': file_title,'parents': [folder_id]}
+            if self.mode == 'client':
+                file_metadata = {'name': file_title,'parents': [folder_id]}
+            else:
+                file_metadata = {'name': file_title,'parents': folder_id}
 
             if convert == True:
                 file_metadata = self.convert(file_metadata,self.get_file_extension(file_path))
 
-            gfile = drive_service.files().create(body=file_metadata, media_body=media, fields='id')
+            gfile = drive_service.files().create(body=file_metadata, media_body=media, fields='id').execute()
         else:
             file_id = file_metadata['id']
             void_metadata = {}
-            gfile = drive_service.files().update(fileId=file_id, body=void_metadata, media_body=media)
+            gfile = drive_service.files().update(fileId=file_id, body=void_metadata, media_body=media).execute()
 
-        gfile.execute()
+        if self.mode == 'service':
+                old_parents = gfile.get('parents')
+                file_id = gfile.get('id')
+
+                drive_service.files().update(fileId=file_id,removeParents=old_parents,addParents=folder_id).execute()
 
     # returns metadata for the file (whether it exists or not)
     def get_update(self,name,file_id,folder_id,service):
-        if file_id != None: # use specified id
-                file_metadata = {'id':file_id,'name': name,'parents': [folder_id]} # Change name: doesn't work
-        else: # obtain id for duplicated file (file with same name) and overwrite
-            file_id = self.find_duplicate(self.list_files(folder_id,service),name)
-            if file_id != None: # duplicate found
-                file_metadata = {'id':file_id,'name': name,'parents': [folder_id]}
-            else: # duplicate not found
-                file_metadata = None
+        if self.mode == 'client':
+            if file_id != None: # use specified id
+                    file_metadata = {'id':file_id,'name': name,'parents': [folder_id]} # Change name: doesn't work
+            else: # obtain id for duplicated file (file with same name) and overwrite
+                file_id = self.find_duplicate(self.list_files(folder_id,service),name)
+                if file_id != None: # duplicate found
+                    file_metadata = {'id':file_id,'name': name,'parents': [folder_id]}
+                else: # duplicate not found
+                    file_metadata = None
+        else:
+            if file_id != None: # use specified id
+                    file_metadata = {'id':file_id,'name': name,'parents': folder_id} # Change name: doesn't work
+            else: # obtain id for duplicated file (file with same name) and overwrite
+                file_id = self.find_duplicate(self.list_files(folder_id,service),name)
+                if file_id != None: # duplicate found
+                    file_metadata = {'id':file_id,'name': name,'parents': folder_id}
+                else: # duplicate not found
+                    file_metadata = None
 
         return file_metadata
             
     def get_filename(self,path):
         name = os.path.basename(path)
         name = os.path.splitext(name)[0]
 
@@ -76,15 +94,15 @@
         file_id = None
         for file in list:
             if file['name'] == name:
                 file_id = file['id']
         
         return file_id
     
-    def upload_folder(self,local_folder_path,folder_id,update=True,subfolder=True,subfolder_name=None,subfolder_id=None,recursive=True,convert=True,url=True):
+    def upload_folder(self,local_folder_path,folder_id,update=True,subfolder=True,subfolder_name=None,subfolder_id=None,recursive=True,convert=False,url=True):
 
         if url == True:
             folder_id = self.url_to_id(folder_id)
 
         files_list = os.listdir(local_folder_path)
 
         if subfolder == True:
```

### Comparing `driveup-0.3.0/LICENSE` & `driveup-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `driveup-0.3.0/setup.py` & `driveup-0.4.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 
 # ...
 
 setup(
     long_description=README_DESCRIPTION,
     long_description_content_type="text/markdown",
     name='driveup',
-    version='0.3.0',
+    version='0.4.0',
     author='Raúl M.R.',
     author_email="raul.martin4bc@gmail.com",
     license="MIT",
-    description='Python package for uploading files and folders to Google Drive',
+    description='Python package for uploading files and folders to Google Drive.',
     packages=find_packages(include=["Driveup","Driveup.features"]),
     install_requires=[
-        'pandas',
-        'pydrive',
+        'google-api-python-client',
+        'google-auth-httplib2',
+        'google-auth-oauthlib',
     ],
 )
```

