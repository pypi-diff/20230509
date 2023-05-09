# Comparing `tmp/ntdsdotsqlite-0.9.2.tar.gz` & `tmp/ntdsdotsqlite-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntdsdotsqlite-0.9.2.tar", max compression
+gzip compressed data, was "ntdsdotsqlite-0.9.3.tar", max compression
```

## Comparing `ntdsdotsqlite-0.9.2.tar` & `ntdsdotsqlite-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0        0 2023-04-24 19:34:15.811658 ntdsdotsqlite-0.9.2/ntdsdotsqlite/__init__.py
--rw-r--r--   0        0        0      854 2023-05-08 16:23:21.892529 ntdsdotsqlite-0.9.2/ntdsdotsqlite/__main__.py
--rw-r--r--   0        0        0     4778 2023-05-08 15:39:42.476407 ntdsdotsqlite-0.9.2/ntdsdotsqlite/accounts.py
--rw-r--r--   0        0        0     1454 2023-05-08 09:43:59.572323 ntdsdotsqlite-0.9.2/ntdsdotsqlite/containers.py
--rw-r--r--   0        0        0     4145 2023-05-06 15:44:55.688794 ntdsdotsqlite-0.9.2/ntdsdotsqlite/decrypt.py
--rw-r--r--   0        0        0     3089 2023-05-08 21:09:08.053917 ntdsdotsqlite-0.9.2/ntdsdotsqlite/domain.py
--rw-r--r--   0        0        0      905 2023-05-08 13:52:27.251046 ntdsdotsqlite-0.9.2/ntdsdotsqlite/groups.py
--rw-r--r--   0        0        0      320 2023-05-08 21:09:14.178994 ntdsdotsqlite-0.9.2/ntdsdotsqlite/links.py
--rw-r--r--   0        0        0     2726 2023-05-08 15:41:39.616697 ntdsdotsqlite-0.9.2/ntdsdotsqlite/model.sql
--rw-r--r--   0        0        0     4630 2023-05-08 16:07:39.897658 ntdsdotsqlite-0.9.2/ntdsdotsqlite/ntdsdotsqlite.py
--rw-r--r--   0        0        0     1595 2023-05-08 09:44:10.802061 ntdsdotsqlite-0.9.2/ntdsdotsqlite/orga_units.py
--rw-r--r--   0        0        0    26997 2023-05-08 21:10:10.754799 ntdsdotsqlite-0.9.2/ntdsdotsqlite/secretsdump.py
--rw-r--r--   0        0        0     5678 2023-05-08 21:13:24.935764 ntdsdotsqlite-0.9.2/ntdsdotsqlite/utils.py
--rw-r--r--   0        0        0      695 2023-05-08 21:14:52.804604 ntdsdotsqlite-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2005 2023-05-08 16:12:51.277756 ntdsdotsqlite-0.9.2/README.md
--rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 ntdsdotsqlite-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-24 19:34:15.811658 ntdsdotsqlite-0.9.3/ntdsdotsqlite/__init__.py
+-rw-r--r--   0        0        0      854 2023-05-08 16:23:21.892529 ntdsdotsqlite-0.9.3/ntdsdotsqlite/__main__.py
+-rw-r--r--   0        0        0     4795 2023-05-09 17:02:10.560346 ntdsdotsqlite-0.9.3/ntdsdotsqlite/accounts.py
+-rw-r--r--   0        0        0    92828 2023-05-09 17:52:11.090901 ntdsdotsqlite-0.9.3/ntdsdotsqlite/column_names.py
+-rw-r--r--   0        0        0     1454 2023-05-08 09:43:59.572323 ntdsdotsqlite-0.9.3/ntdsdotsqlite/containers.py
+-rw-r--r--   0        0        0     4145 2023-05-06 15:44:55.688794 ntdsdotsqlite-0.9.3/ntdsdotsqlite/decrypt.py
+-rw-r--r--   0        0        0     3089 2023-05-08 21:09:08.053917 ntdsdotsqlite-0.9.3/ntdsdotsqlite/domain.py
+-rw-r--r--   0        0        0      905 2023-05-08 13:52:27.251046 ntdsdotsqlite-0.9.3/ntdsdotsqlite/groups.py
+-rw-r--r--   0        0        0      320 2023-05-08 21:09:14.178994 ntdsdotsqlite-0.9.3/ntdsdotsqlite/links.py
+-rw-r--r--   0        0        0     2726 2023-05-08 15:41:39.616697 ntdsdotsqlite-0.9.3/ntdsdotsqlite/model.sql
+-rw-r--r--   0        0        0     4597 2023-05-09 17:49:54.425809 ntdsdotsqlite-0.9.3/ntdsdotsqlite/ntdsdotsqlite.py
+-rw-r--r--   0        0        0     1595 2023-05-08 09:44:10.802061 ntdsdotsqlite-0.9.3/ntdsdotsqlite/orga_units.py
+-rw-r--r--   0        0        0    26997 2023-05-08 21:10:10.754799 ntdsdotsqlite-0.9.3/ntdsdotsqlite/secretsdump.py
+-rw-r--r--   0        0        0     3938 2023-05-09 17:50:14.137338 ntdsdotsqlite-0.9.3/ntdsdotsqlite/utils.py
+-rw-r--r--   0        0        0      695 2023-05-09 17:53:31.468357 ntdsdotsqlite-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2005 2023-05-08 16:12:51.277756 ntdsdotsqlite-0.9.3/README.md
+-rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 ntdsdotsqlite-0.9.3/PKG-INFO
```

### Comparing `ntdsdotsqlite-0.9.2/ntdsdotsqlite/__main__.py` & `ntdsdotsqlite-0.9.3/ntdsdotsqlite/__main__.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.2/ntdsdotsqlite/accounts.py` & `ntdsdotsqlite-0.9.3/ntdsdotsqlite/accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,26 @@
         datatable.records()
     )
     for a in accounts:
         lastLogonTimestamp = a.get(ese_db.column_names["lastLogonTimestamp"])
         pwdlastset = a.get(ese_db.column_names["pwdLastSet"])
         if pwdlastset:
             pwdlastset = hundredns_to_datetime(pwdlastset)
-        else:
-            pwdlastset = None
         if lastLogonTimestamp:
             lastLogonTimestamp = hundredns_to_datetime(lastLogonTimestamp)
         admincount = a.get(ese_db.column_names["adminCount"])
         if admincount is None:
             admincount = 0
         spn = a.get(ese_db.column_names["servicePrincipalName"])
         accountExpires = a.get(ese_db.column_names["accountExpires"])
-        if accountExpires == 0 or accountExpires == 0x7FFFFFFFFFFFFFFF:
-            accountExpires = 0
-        else:
-            accountExpires = hundredns_to_datetime(accountExpires)
+        if accountExpires:
+            if accountExpires and accountExpires == 0 or accountExpires == 0x7FFFFFFFFFFFFFFF:
+                accountExpires = 0
+            else:
+                accountExpires = hundredns_to_datetime(accountExpires)
         uac = a.get(ese_db.column_names["userAccountControl"])
         account = {
             "id": a.get("DNT_col"), "description": a.get(ese_db.column_names["description"]),
             "UAC": uac,
             "SID": raw_to_sid(a.get(ese_db.column_names["objectSid"])),
             "samaccountname": a.get(ese_db.column_names["sAMAccountName"]),
             # unix epoch or NULL if password never set
```

### Comparing `ntdsdotsqlite-0.9.2/ntdsdotsqlite/containers.py` & `ntdsdotsqlite-0.9.3/ntdsdotsqlite/containers.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.2/ntdsdotsqlite/decrypt.py` & `ntdsdotsqlite-0.9.3/ntdsdotsqlite/decrypt.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.2/ntdsdotsqlite/domain.py` & `ntdsdotsqlite-0.9.3/ntdsdotsqlite/domain.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.2/ntdsdotsqlite/groups.py` & `ntdsdotsqlite-0.9.3/ntdsdotsqlite/groups.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.2/ntdsdotsqlite/model.sql` & `ntdsdotsqlite-0.9.3/ntdsdotsqlite/model.sql`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.2/ntdsdotsqlite/ntdsdotsqlite.py` & `ntdsdotsqlite-0.9.3/ntdsdotsqlite/ntdsdotsqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ntdsdotsqlite.utils import get_ESE_column_names, create_database
 from ntdsdotsqlite.containers import containers_generator
 from ntdsdotsqlite.accounts import account_generator
+from ntdsdotsqlite.column_names import column_names
 from ntdsdotsqlite.domain import get_domain_objects
-from ntdsdotsqlite.groups import group_generator
 from ntdsdotsqlite.orga_units import ou_generator
 from ntdsdotsqlite.decrypt import decrypt_sqlite
+from ntdsdotsqlite.groups import group_generator
+from ntdsdotsqlite.utils import create_database
 from ntdsdotsqlite.links import compute_links
 from dissect.esedb import EseDB
 import sqlite3
 import json
 
 
 def run(ese_path, outpath, system_path):
     create_database(outpath)
     sqlite_db = sqlite3.connect(outpath)
     ese_db = EseDB(open(ese_path, "rb"))
     cursor = sqlite_db.cursor()
     # Getting column names
-    number_rows, column_names = get_ESE_column_names(ese_path)
     ese_db.column_names = column_names
     # Compute links
     print("Retrieving and storing links information ...")
     link_relations = compute_links(ese_db)
     # Get the domain
     print("Retrieving the domain object ...")
     domain = get_domain_objects(ese_db)
```

### Comparing `ntdsdotsqlite-0.9.2/ntdsdotsqlite/orga_units.py` & `ntdsdotsqlite-0.9.3/ntdsdotsqlite/orga_units.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.2/ntdsdotsqlite/secretsdump.py` & `ntdsdotsqlite-0.9.3/ntdsdotsqlite/secretsdump.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.2/ntdsdotsqlite/utils.py` & `ntdsdotsqlite-0.9.3/ntdsdotsqlite/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from datetime import datetime, timedelta
-from dissect.esedb import EseDB
 from enum import IntFlag
 from pathlib import Path
 import binascii
 import sqlite3
-import re
 
 
 # transforms a guid from raw hex byte returned by dissect to a correct GUID string
 def raw_to_guid(raw):
     p1 = raw[:4][::-1].hex()
     p2 = raw[4:6][::-1].hex()
     p3 = raw[6:8][::-1].hex()
@@ -30,52 +28,14 @@
 
 
 # Translates microsoft duration/datetime format (intervals of 100ns) to python datetime object
 def hundredns_to_datetime(ns):
     return timedelta(seconds=ns / 10000000) + datetime(1601, 1, 1)
 
 
-# Function to get attribute names from the ESE database. Gets real column names
-# like "sAMAccountName" from attribute IDs like "ATTc131102". Way easier to work
-# with !
-# returns a 2-tuple of :
-# (n, keys):
-# with n beeing the number of rows in the datatable table, and
-# keys the dictionary associating attribute ids and keys names:
-#    {"ATTc131102": "AttributeID",  "ATTm13": "Description", ...}
-def get_ESE_column_names(db_path):
-    # from https://github.com/xmco/ntds_extract/tree/main/Part-2-La-Datatable
-    def find_complete_record_name(complete_record_names, partial_record_name):
-        for record_name in complete_record_names:
-            if str(partial_record_name) == ''.join(re.findall(r'\d+', record_name)):
-                return record_name
-
-    with open(db_path, "rb") as fh:
-        db = EseDB(fh)
-        datatable_col_names = []
-        output = {}
-        attributeID = 'ATTc131102'
-        lDAPDisplayName = 'ATTm131532'
-        datatable = db.table("datatable")
-        msysobjects = db.table("MSysObjects")
-        for record in msysobjects.records():  # Look for attribute ID (column) in the datatable
-            if record.Name.startswith('ATT'):
-                datatable_col_names.append(record.Name)
-        n = 0
-        # Then, look the LDAP value corresponding to the attribute ID
-        for record in datatable.records():
-            n += 1
-            complete_record_name = find_complete_record_name(
-                datatable_col_names, record.get(attributeID)
-            )
-            if complete_record_name:
-                output[record.get(lDAPDisplayName)] = complete_record_name
-        return n, output
-
-
 # Writes an initial sqlite database, with the chosen sql representation of an NTDS db.
 def create_database(sqlite_path):
     # overwrite database if already existing
     f = open(sqlite_path, "w")
     f.close()
     db = sqlite3.connect(sqlite_path)
     script = open(Path(__file__).parent / "model.sql", "r").read()
```

### Comparing `ntdsdotsqlite-0.9.2/pyproject.toml` & `ntdsdotsqlite-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ntdsdotsqlite"
-version = "0.9.2"
+version = "0.9.3"
 description = "A small utility to get an SQLite  database from an NTDS.DIT file."
 authors = ["Virgile Jarry <virgile@mailbox.org>"]
 readme = "README.md"
 license = "Beerware"
 homepage = "https://github.com/almandin/ntdsdotsqlite"
 repository = "https://github.com/almandin/ntdsdotsqlite"
 documentation = "https://github.com/almandin/ntdsdotsqlite/README.md"
```

### Comparing `ntdsdotsqlite-0.9.2/README.md` & `ntdsdotsqlite-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.2/PKG-INFO` & `ntdsdotsqlite-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntdsdotsqlite
-Version: 0.9.2
+Version: 0.9.3
 Summary: A small utility to get an SQLite  database from an NTDS.DIT file.
 Home-page: https://github.com/almandin/ntdsdotsqlite
 License: Beerware
 Author: Virgile Jarry
 Author-email: virgile@mailbox.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

