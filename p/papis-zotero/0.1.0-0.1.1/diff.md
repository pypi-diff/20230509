# Comparing `tmp/papis-zotero-0.1.0.linux-x86_64.tar.gz` & `tmp/papis-zotero-0.1.1.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/gallo/software/papis/papis-zotero/dist/papis-zotero-0.1.0.linux-x86_64.tar", last modified: Mon Oct 21 09:56:58 2019, max compression
+gzip compressed data, was "papis-zotero-0.1.1.linux-x86_64.tar", last modified: Tue May  9 20:09:28 2023, max compression
```

## Comparing `papis-zotero-0.1.0.linux-x86_64.tar` & `papis-zotero-0.1.1.linux-x86_64.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:56:58.000000 ./
-drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:56:58.000000 ./usr/
-drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:56:58.000000 ./usr/local/
-drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:56:58.000000 ./usr/local/lib/
-drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/
-drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/
-drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero/
--rw-r--r--   0 gallo     (1000) gallo     (1000)     2021 2019-10-21 09:56:29.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero/__init__.py
--rw-r--r--   0 gallo     (1000) gallo     (1000)     8325 2019-04-05 01:02:46.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero/server.py
--rw-r--r--   0 gallo     (1000) gallo     (1000)     8682 2019-10-20 19:25:36.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero/sql.py
--rw-r--r--   0 gallo     (1000) gallo     (1000)     2200 2019-10-21 09:56:29.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero/bibtex.py
--rw-r--r--   0 gallo     (1000) gallo     (1000)      230 2019-04-05 01:02:46.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero/utils.py
-drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero/__pycache__/
--rw-r--r--   0 gallo     (1000) gallo     (1000)     2202 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 gallo     (1000) gallo     (1000)      461 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero/__pycache__/utils.cpython-35.pyc
--rw-r--r--   0 gallo     (1000) gallo     (1000)     7455 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero/__pycache__/server.cpython-35.pyc
--rw-r--r--   0 gallo     (1000) gallo     (1000)     6914 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero/__pycache__/sql.cpython-35.pyc
--rw-r--r--   0 gallo     (1000) gallo     (1000)     1825 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero/__pycache__/bibtex.cpython-35.pyc
-drwxr-xr-x   0 gallo     (1000) gallo     (1000)        0 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero-0.1.0-py3.5.egg-info/
--rw-r--r--   0 gallo     (1000) gallo     (1000)      350 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero-0.1.0-py3.5.egg-info/SOURCES.txt
--rw-r--r--   0 gallo     (1000) gallo     (1000)        1 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero-0.1.0-py3.5.egg-info/dependency_links.txt
--rw-r--r--   0 gallo     (1000) gallo     (1000)       13 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero-0.1.0-py3.5.egg-info/top_level.txt
--rw-r--r--   0 gallo     (1000) gallo     (1000)     2494 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero-0.1.0-py3.5.egg-info/PKG-INFO
--rw-r--r--   0 gallo     (1000) gallo     (1000)       13 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero-0.1.0-py3.5.egg-info/requires.txt
--rw-r--r--   0 gallo     (1000) gallo     (1000)       44 2019-10-21 09:56:58.000000 ./usr/local/lib/python3.5/dist-packages/papis_zotero-0.1.0-py3.5.egg-info/entry_points.txt
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.367884 ./
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.367884 ./home/
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.368884 ./home/gallo/
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.368884 ./home/gallo/software/
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.368884 ./home/gallo/software/papis/
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.368884 ./home/gallo/software/papis/env/
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.368884 ./home/gallo/software/papis/env/lib/
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.368884 ./home/gallo/software/papis/env/lib/python3.10/
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.490883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.371884 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/
+-rw-r--r--   0 gallo     (1000) users      (100)     2214 2023-05-09 19:52:11.000000 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__init__.py
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.375884 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__pycache__/
+-rw-r--r--   0 gallo     (1000) users      (100)     2129 2023-05-09 20:09:28.373885 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 gallo     (1000) users      (100)     1731 2023-05-09 20:09:28.371884 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__pycache__/bibtex.cpython-310.pyc
+-rw-r--r--   0 gallo     (1000) users      (100)     6999 2023-05-09 20:09:28.373885 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__pycache__/server.cpython-310.pyc
+-rw-r--r--   0 gallo     (1000) users      (100)     7043 2023-05-09 20:09:28.375884 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__pycache__/sql.cpython-310.pyc
+-rw-r--r--   0 gallo     (1000) users      (100)      484 2023-05-09 20:09:28.374884 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 gallo     (1000) users      (100)     2215 2023-05-09 20:06:28.000000 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/bibtex.py
+-rw-r--r--   0 gallo     (1000) users      (100)     7952 2023-05-09 20:05:33.000000 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/server.py
+-rw-r--r--   0 gallo     (1000) users      (100)     9385 2023-05-09 20:04:40.000000 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/sql.py
+-rw-r--r--   0 gallo     (1000) users      (100)      230 2023-05-09 19:34:06.000000 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/utils.py
+drwxr-xr-x   0 gallo     (1000) users      (100)        0 2023-05-09 20:09:28.491883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/
+-rw-r--r--   0 gallo     (1000) users      (100)     4912 2023-05-09 20:09:28.457883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/PKG-INFO
+-rw-r--r--   0 gallo     (1000) users      (100)      350 2023-05-09 20:09:28.490883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/SOURCES.txt
+-rw-r--r--   0 gallo     (1000) users      (100)        1 2023-05-09 20:09:28.458883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/dependency_links.txt
+-rw-r--r--   0 gallo     (1000) users      (100)       43 2023-05-09 20:09:28.458883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/entry_points.txt
+-rw-r--r--   0 gallo     (1000) users      (100)       12 2023-05-09 20:09:28.458883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/requires.txt
+-rw-r--r--   0 gallo     (1000) users      (100)       13 2023-05-09 20:09:28.458883 ./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero-0.1.1-py3.10.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `./usr/local/lib/python3.5/dist-packages/papis_zotero/__init__.py` & `./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,75 @@
 import click
 import os
-import papis.api
 
 import logging
 import http.server
 import papis_zotero.server
 
 
-@click.group('zotero')
-@click.help_option('-h', '--help')
+@click.group("zotero")
+@click.help_option("-h", "--help")
 def main():
     """
     Zotero interface for papis
     """
-    logger = logging.getLogger("papis:zotero")
+    pass
 
 
-@main.command('serve')
-@click.help_option('-h', '--help')
-@click.option(
-    "--port",
-    help="Port to listen to",
-    default=papis_zotero.server.zotero_port,
-    type=int
-)
-@click.option(
-    "--address",
-    help="Address to bind",
-    default="localhost"
-)
+@main.command("serve")
+@click.help_option("-h", "--help")
+@click.option("--port",
+              help="Port to listen to",
+              default=papis_zotero.server.zotero_port,
+              type=int)
+@click.option("--address", help="Address to bind", default="localhost")
 def serve(address, port):
     """Start a zotero-connector server"""
     global logger
+    logging.warning("The zotero-connector server is experimental,"
+                    " please report bugs and improvements.")
     server_address = (address, port)
-    httpd = http.server.HTTPServer(
-        server_address,
-        papis_zotero.server.PapisRequestHandler
-    )
+    httpd = http.server.HTTPServer(server_address,
+                                   papis_zotero.server.PapisRequestHandler)
     httpd.serve_forever()
 
 
-@main.command('import')
-@click.help_option('-h', '--help')
-@click.option(
-    '-f', '--from-bibtex', 'from_bibtex',
-    help='Import zotero library from a bibtex dump, the files fields in '
-         'the bibtex files should point to valid paths',
-    default=None,
-    type=click.Path(exists=True)
-)
+@main.command("import")
+@click.help_option("-h", "--help")
 @click.option(
-    '-s', '--from-sql', 'from_sql',
-    help='Path to the FOLDER where the "zotero.sqlite" file resides',
+    "-f",
+    "--from-bibtex",
+    "from_bibtex",
+    help="Import zotero library from a bibtex dump, the files fields in "
+    "the bibtex files should point to valid paths",
     default=None,
-    type=click.Path(exists=True)
-)
-@click.option(
-    '-o', '--outfolder',
-    help='Folder to save the imported library',
-    type=str,
-    required=True
-)
-@click.option(
-    '--link',
-    help='Wether to link the pdf files or copy them',
-    default=None
-)
+    type=click.Path(exists=True))
+@click.option("-s",
+              "--from-sql",
+              "--from-sql-folder",
+              "from_sql",
+              help="Path to the FOLDER where the 'zotero.sqlite' file resides",
+              default=None,
+              type=click.Path(exists=True))
+@click.option("-o",
+              "--outfolder",
+              help="Folder to save the imported library",
+              type=str,
+              required=True)
+@click.option("--link",
+              help="Wether to link the pdf files or copy them",
+              default=None)
 def do_importer(from_bibtex, from_sql, outfolder, link):
     """Import zotero libraries into papis libraries
     """
     import papis_zotero.bibtex
     import papis_zotero.sql
     if not os.path.exists(outfolder):
         os.makedirs(outfolder)
     if from_bibtex is not None:
-        papis_zotero.bibtex.add_from_bibtex(
-            from_bibtex, outfolder, link
-        )
+        papis_zotero.bibtex.add_from_bibtex(from_bibtex, outfolder, link)
     elif from_sql is not None:
-        papis_zotero.sql.add_from_sql(
-            from_sql, outfolder
-        )
+        papis_zotero.sql.add_from_sql(from_sql, outfolder)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `./usr/local/lib/python3.5/dist-packages/papis_zotero/server.py` & `./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -120,22 +120,17 @@
 
     def log_message(self, fmt, *args):
         global logger
         logger.info(fmt % args)
         return
 
     def set_zotero_headers(self):
-        self.send_header(
-            "X-Zotero-Version",
-            zotero_version
-        )
-        self.send_header(
-            "X-Zotero-Connector-API-Version",
-            connector_api_version
-        )
+        self.send_header("X-Zotero-Version", zotero_version)
+        self.send_header("X-Zotero-Connector-API-Version",
+                         connector_api_version)
         self.end_headers()
 
     def read_input(self):
         length = int(self.headers['content-length'])
         return self.rfile.read(length)
 
     def pong(self, POST=True):
@@ -160,94 +155,79 @@
             </html>
             '''
         else:  # POST
             logger.debug("POST request")
             self.send_response(200)
             self.send_header("Content-Type", "application/json")
             self.set_zotero_headers()
-            response = json.dumps(
-                {
-                    "prefs": {
-                        "automaticSnapshots": True
-                    }
-                }
-            )
+            response = json.dumps({"prefs": {"automaticSnapshots": True}})
 
         self.wfile.write(bytes(response, "utf8"))
 
     def papis_collection(self):
         self.send_response(200)
         self.send_header("Content-Type", "application/json")
         self.set_zotero_headers()
         papis_library = papis.api.get_lib_name()
-        response = json.dumps(
-            {
-                "libraryID": 1,
-                "libraryName": papis_library,
-                # I'm not aware of a read-only papis mode
-                "libraryEditable": True,
-                # collection-level parameters
-                "editable": True,
-                # collection-level
-                "id": None,
-                # collection if collection, else library
-                "name": papis_library
-            }
-        )
+        response = json.dumps({
+            "libraryID": 1,
+            "libraryName": papis_library,
+            # I'm not aware of a read-only papis mode
+            "libraryEditable": True,
+            # collection-level parameters
+            "editable": True,
+            # collection-level
+            "id": None,
+            # collection if collection, else library
+            "name": papis_library
+        })
         self.wfile.write(bytes(response, "utf8"))
 
     def add(self):
         logger.info("Adding paper from zotero connector")
         rawinput = self.read_input()
         data = json.loads(rawinput.decode('utf8'))
 
         for item in data['items']:
             files = []
             if item.get('attachments') and len(item.get('attachments')) > 0:
                 for attachment in item.get('attachments'):
                     mime = str(attachment.get('mimeType'))
-                    logger.info(
-                        "Checking attachment (mime {0})".format(mime)
-                    )
+                    logger.info("Checking attachment (mime {0})".format(mime))
                     if re.match(r'.*pdf.*', mime):
                         url = attachment.get('url')
                         logger.info("Downloading pdf '{0}'".format(url))
                         try:
                             pdfbuffer = urllib.request.urlopen(url).read()
                         except urllib.error.HTTPError:
                             logger.error(
                                 'Error downloading pdf, probably you do not'
-                                'have the rights for the journal.'
-                            )
+                                'have the rights for the journal.')
                             continue
 
                         pdfpath = tempfile.mktemp(suffix='.pdf')
                         logger.info("Saving pdf in '{0}'".format(pdfpath))
 
                         with open(pdfpath, 'wb+') as fd:
                             fd.write(pdfbuffer)
 
                         if papis_zotero.utils.is_pdf(pdfpath):
                             files.append(pdfpath)
                         else:
                             logger.error(
                                 'File retrieved does not appear to be a pdf'
-                                'So no file will be saved...'
-                            )
+                                'So no file will be saved...')
             else:
                 logger.warning("Document has no attachments")
 
             papis_item = zotero_data_to_papis_data(item)
             if len(files) == 0:
                 logger.warning('Not adding any attachments...')
             logger.info("Adding paper")
-            papis.commands.add.run(
-                files,
-                data=papis_item
-            )
+            papis.commands.add.run(files, data=papis_item)
 
         self.send_response(201)  # Created
         self.set_zotero_headers()
         # return the JSON data back
         self.wfile.write(rawinput)
 
     def snapshot(self):
```

### Comparing `./usr/local/lib/python3.5/dist-packages/papis_zotero/sql.py` & `./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/sql.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,28 +12,40 @@
 
 # zotero item types to be excluded.
 # "attachment" are automatically excluded and will be treated as "files"
 excludedTypes = ["note"]
 
 # dictionary of zotero attachments mime types to be included
 # mapped onto their respective extension to be used in papis
-includedAttachments = {"application/pdf": "pdf"}
+includedAttachments = {
+    "application/vnd.ms-htmlhelp": "chm",
+    "image/vnd.djvu": "djvu",
+    "application/msword": "doc",
+    "application/vnd.openxmlformats-officedocument.wordprocessingml.document":
+    "docx",
+    "application/epub+zip": "epub",
+    "application/octet-stream": "fb2",
+    "application/x-mobipocket-ebook": "mobi",
+    "application/pdf": "pdf",
+    "text/rtf": "rtf",
+    "application/zip": "zip"
+}
 
 # dictionary translating from zotero to papis type names
 translatedTypes = {"journalArticle": "article"}
 
 # dictionary translating from zotero to papis field names
 translatedFields = {"DOI": "doi"}
 
 # seperator between multiple tags
 tagDelimiter = ","
 
 # if no attachment is found, give info.yaml as content file
 # set to None if no file should be given in that case
-defaultFile = "info.yaml"
+defaultFile = None
 
 
 def getTuple(elements):
     """
     Concatenate given strings to SQL tuple of strings
     """
     elementsTuple = "("
@@ -84,37 +96,35 @@
       creatorTypes.creatorTypeID = itemCreators.creatorTypeID AND
       creators.creatorID = itemCreators.creatorID
     ORDER BY
       creatorTypes.creatorType,
       itemCreators.orderIndex
     """
     creatorCursor = connection.cursor()
-    creatorCursor.execute(
-        itemCreatorQuery.format(itemID=itemId)
-    )
+    creatorCursor.execute(itemCreatorQuery.format(itemID=itemId))
     creators = {}  # type: ignore
 
     for creatorRow in creatorCursor:
         creatorName = creatorRow[0]
         creatorNameList = creatorName + "_list"
         givenName = creatorRow[1]
         surname = creatorRow[2]
 
         currentCreators = creators.get(creatorName, "")
         if currentCreators != "":
             currentCreators += " and "
-        currentCreators += "{surname}, {givenName}".format(
-          givenName=givenName, surname=surname
-        )
+        currentCreators += "{surname}, {givenName}".format(givenName=givenName,
+                                                           surname=surname)
         creators[creatorName] = currentCreators
 
         currentCreatorsList = creators.get(creatorNameList, [])
-        currentCreatorsList.append(
-            {"given_name": givenName, "surname": surname}
-        )
+        currentCreatorsList.append({
+            "given_name": givenName,
+            "surname": surname
+        })
         creators[creatorNameList] = currentCreatorsList
 
     return creators
 
 
 def getFiles(connection, itemId, itemKey):
     global inputPath
@@ -130,37 +140,33 @@
       itemAttachments.parentItemID = {itemID} AND
       itemAttachments.contentType IN {mimeTypes} AND
       items.itemID = itemAttachments.itemID
     """
     mimeTypes = getTuple(includedAttachments.keys())
     attachmentCursor = connection.cursor()
     attachmentCursor.execute(
-        itemAttachmentQuery.format(itemID=itemId, mimeTypes=mimeTypes)
-    )
+        itemAttachmentQuery.format(itemID=itemId, mimeTypes=mimeTypes))
     files = []
     for attachmentRow in attachmentCursor:
         key = attachmentRow[0]
         path = attachmentRow[1]
         mime = attachmentRow[2]
-        extension = includedAttachments[mime]
+        # extension = includedAttachments[mime]
         try:
             # NOTE: a single file is assumed in the attachment's folder
             # to avoid using path, which may contain invalid characters
             importPath = glob.glob(inputPath + "/storage/" + key + "/*.*")[0]
-            localPath = os.path.join(
-                outputPath, itemKey, key + "." + extension
-            )
+            extension = os.path.splitext(importPath)[1]
+            localPath = os.path.join(outputPath, itemKey,
+                                     key + "." + extension)
             shutil.copyfile(importPath, localPath)
             files.append(key + "." + extension)
         except:
-            print(
-              "failed to export attachment {key}: {path} ({mime})".format(
-                key=key, path=path, mime=mime
-              )
-            )
+            print("failed to export attachment {key}: {path} ({mime})".format(
+                key=key, path=path, mime=mime))
             pass
 
     if files == [] and defaultFile:
         files.append(defaultFile)
     return {"files": files}
 
 
@@ -202,17 +208,17 @@
     collections = []
     for collectionRow in collectionCursor:
         collections.append(collectionRow[0])
 
     return {"project": collections}
 
 
-
 ###############################################################################
 
+
 def add_from_sql(input_path, output_path):
     """
 
     :param input_path: path to zotero SQLite database "zoter.sqlite" and
         "storage" to be imported
     :param output_path: path where all items will be exported to created if not
         existing
@@ -245,15 +251,18 @@
     for row in cursor:
         itemsCount = row[0]
 
     itemsQuery = """
       SELECT
         item.itemID,
         itemType.typeName,
-        key
+        key,
+        dateAdded,
+        dateModified,
+        clientDateModified
       FROM
         items item,
         itemTypes itemType
       WHERE
         itemType.itemTypeID = item.itemTypeID AND
         itemType.typeName NOT IN {excludedTypeTuple}
       ORDER BY
@@ -263,19 +272,19 @@
     cursor.execute(itemsQuery.format(excludedTypeTuple=excludedTypeTuple))
     currentItem = 0
     for row in cursor:
         currentItem += 1
         itemId = row[0]
         itemType = translatedTypes.get(row[1], row[1])
         itemKey = row[2]
-        logger.info(
-            "exporting item {currentItem}/{itemsCount}: {key}".format(
-                currentItem=currentItem, itemsCount=itemsCount, key=itemKey
-            )
-        )
+        dateAdded = row[3]
+        dateModified = row[4]
+        clientDateModified = row[5]
+        logger.info("exporting item {currentItem}/{itemsCount}: {key}".format(
+            currentItem=currentItem, itemsCount=itemsCount, key=itemKey))
 
         path = os.path.join(outputPath, itemKey)
         if not os.path.exists(path):
             os.makedirs(path)
 
         # Get mendeley keys
         fields = getFields(connection, itemId)
@@ -283,15 +292,21 @@
         ref = itemKey
         if extra:
             # try to convert
             matches = re.search(r'.*Citation Key: (\w+)', extra)
             if matches:
                 ref = matches.group(1)
         logger.info("exporting under ref %s" % ref)
-        item = {"ref": ref, "type": itemType}
+        item = {
+            "ref": ref,
+            "type": itemType,
+            "created": dateAdded,
+            "modified": dateModified,
+            "modified.client": clientDateModified
+        }
         item.update(fields)
         item.update(getCreators(connection, itemId))
         item.update(getTags(connection, itemId))
         item.update(getCollections(connection, itemId))
         item.update(getFiles(connection, itemId, itemKey))
 
         item.update({"ref": ref})
```

### Comparing `./usr/local/lib/python3.5/dist-packages/papis_zotero/bibtex.py` & `./home/gallo/software/papis/env/lib/python3.10/site-packages/papis_zotero/bibtex.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import papis.utils
 import logging
 import tqdm
 import colorama
 
 logger = logging.getLogger('zotero:bibtex')
 
-
 info_template = """{c.Back.BLACK}
 {c.Fore.RED}||
 {c.Fore.RED}||{c.Fore.YELLOW}    ref: {c.Fore.GREEN}{ref}
 {c.Fore.RED}||{c.Fore.YELLOW} author: {c.Fore.GREEN}{author}
 {c.Fore.RED}||{c.Fore.YELLOW}  title: {c.Fore.GREEN}{title}
 {c.Fore.RED}||{c.Style.RESET_ALL}
 """
@@ -38,35 +37,32 @@
 
             if 'author' not in entry.keys():
                 entry['tags'] = 'Unkown'
 
             if 'ref' in entry.keys():
                 entry['ref'] = entry['ref'].replace('?', '')
 
-            print(info_template.format(
-                c=colorama,
-                author=entry.get('author'),
-                title=entry.get('title'),
-                ref=entry.get('ref'),
-            ))
+            print(
+                info_template.format(
+                    c=colorama,
+                    author=entry.get('author'),
+                    title=entry.get('title'),
+                    ref=entry.get('ref'),
+                ))
 
             pdf_file = None
             if 'file' in entry.keys():
                 pdf_file = entry.get('file').split(':')[1]
                 pdf_file = os.path.join(os.path.dirname(bib_file), pdf_file)
                 logger.info('\tINFO: File field detected (%s)' % pdf_file)
                 if not os.path.exists(pdf_file):
-                    logger.warning(
-                        colorama.Back.YELLOW + colorama.Fore.BLACK +
-                        ('Path (%s)' % pdf_file ) +
-                        colorama.Back.RED +
-                        ' not found! Ignoring it' +
-                        colorama.Style.RESET_ALL
-                    )
+                    logger.warning(colorama.Back.YELLOW + colorama.Fore.BLACK +
+                                   ('Path (%s)' % pdf_file) +
+                                   colorama.Back.RED +
+                                   ' not found! Ignoring it' +
+                                   colorama.Style.RESET_ALL)
                     del entry['file']
                     pdf_file = None
 
-            papis_add(
-                [pdf_file] if pdf_file is not None else [],
-                data=entry,
-                link=link
-            )
+            papis_add([pdf_file] if pdf_file is not None else [],
+                      data=entry,
+                      link=link)
```

