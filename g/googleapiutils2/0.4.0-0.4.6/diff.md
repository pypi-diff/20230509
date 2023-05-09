# Comparing `tmp/googleapiutils2-0.4.0.tar.gz` & `tmp/googleapiutils2-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.4.0.tar", max compression
+gzip compressed data, was "googleapiutils2-0.4.6.tar", max compression
```

## Comparing `googleapiutils2-0.4.0.tar` & `googleapiutils2-0.4.6.tar`

### file list

```diff
@@ -1,11 +1,16 @@
--rw-r--r--   0        0        0     1071 2022-12-29 04:17:14.518544 googleapiutils2-0.4.0/LICENSE
--rw-r--r--   0        0        0        0 2022-12-23 19:17:41.312780 googleapiutils2-0.4.0/googleapiutils2/__init__.py
--rw-r--r--   0        0        0        0 2022-12-23 19:17:41.312852 googleapiutils2-0.4.0/googleapiutils2/_types/__init__.py
--rw-r--r--   0        0        0      915 2022-12-23 19:20:08.955432 googleapiutils2-0.4.0/googleapiutils2/_types/geocode.py
--rw-r--r--   0        0        0    14286 2022-12-20 09:27:37.583956 googleapiutils2-0.4.0/googleapiutils2/drive.py
--rw-r--r--   0        0        0     1056 2022-12-23 19:16:33.628602 googleapiutils2-0.4.0/googleapiutils2/geocode.py
--rw-r--r--   0        0        0     8184 2022-12-24 07:52:17.563535 googleapiutils2-0.4.0/googleapiutils2/sheets.py
--rw-r--r--   0        0        0     6059 2022-12-06 15:53:13.125975 googleapiutils2-0.4.0/googleapiutils2/utils.py
--rw-r--r--   0        0        0      575 2022-12-29 22:02:47.385233 googleapiutils2-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 googleapiutils2-0.4.0/setup.py
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 googleapiutils2-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-12-30 01:32:12.340806 googleapiutils2-0.4.6/LICENSE
+-rw-r--r--   0        0        0       96 2023-01-30 06:00:44.616601 googleapiutils2-0.4.6/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-01-15 05:10:18.196566 googleapiutils2-0.4.6/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    14624 2023-05-09 18:49:08.407236 googleapiutils2-0.4.6/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      297 2022-12-30 01:32:12.341593 googleapiutils2-0.4.6/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.4.6/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1049 2022-12-30 01:32:12.342019 googleapiutils2-0.4.6/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.4.6/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      118 2023-01-30 06:00:44.617619 googleapiutils2-0.4.6/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     6494 2023-05-09 18:46:09.012912 googleapiutils2-0.4.6/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    11511 2023-05-09 18:46:09.013129 googleapiutils2-0.4.6/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     4699 2023-05-09 18:46:09.013605 googleapiutils2-0.4.6/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     6822 2023-05-09 17:40:05.660193 googleapiutils2-0.4.6/googleapiutils2/utils.py
+-rw-r--r--   0        0        0      685 2023-05-09 18:46:09.014272 googleapiutils2-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 googleapiutils2-0.4.6/setup.py
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 googleapiutils2-0.4.6/PKG-INFO
```

### Comparing `googleapiutils2-0.4.0/LICENSE` & `googleapiutils2-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.4.0/googleapiutils2/drive.py` & `googleapiutils2-0.4.6/googleapiutils2/drive/drive.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,166 +1,159 @@
 from __future__ import annotations
 
-import os
 from io import BytesIO
 from pathlib import Path
 from typing import *
 
 import googleapiclient
 import googleapiclient.http
 from google.oauth2.credentials import Credentials
 from googleapiclient import discovery
 
-from .utils import (
+from ..utils import (
     FilePath,
     GoogleMimeTypes,
     download_large_file,
     parse_file_id,
     q_escape,
 )
+from .misc import DEFAULT_DOWNLOAD_CONVERSION_MAP, DOWNLOAD_LIMIT, VERSION
 
 if TYPE_CHECKING:
     from googleapiclient._apis.drive.v3.resources import (
         DriveList,
         DriveResource,
         File,
         FileList,
         Permission,
         PermissionList,
     )
 
-    from .utils import FileId
-
-
-DEFAULT_DOWNLOAD_CONVERSION_MAP = {
-    GoogleMimeTypes.sheets: (GoogleMimeTypes.xlsx, ".xlsx"),
-    GoogleMimeTypes.docs: (GoogleMimeTypes.doc, ".docx"),
-    GoogleMimeTypes.slides: (GoogleMimeTypes.pdf, ".pdf"),
-}
-
-DOWNLOAD_LIMIT = 4e6
-
-VERSION = "v3"
-
 
 class Drive:
     def __init__(self, creds: Credentials):
         self.creds = creds
         self.service: DriveResource = discovery.build(
             "drive", VERSION, credentials=self.creds
         )
         self.files: DriveResource.FilesResource = self.service.files()
 
-    def get(self, file_id: FileId, fields: str = "*", **kwargs: Any) -> File:
+    def get(self, file_id: str, fields: str = "*", **kwargs: Any) -> File:
+        """Get a file by its ID."""
         file_id = parse_file_id(file_id)
         return self.files.get(fileId=file_id, fields=fields, **kwargs).execute()
 
+    def _download(self, file_id: str, out_filepath: Path, mime_type: GoogleMimeTypes):
+        request = self.files.export_media(fileId=file_id, mimeType=mime_type.value)
+        with out_filepath.open("wb") as out_file:
+            downloader = googleapiclient.http.MediaIoBaseDownload(out_file, request)
+            done = False
+            while done is False:
+                status, done = downloader.next_chunk()
+        return out_filepath
+
+    def _download_nested_filepath(
+        self,
+        out_filepath: FilePath,
+        file_id: str,
+    ) -> None:
+        """Internal usage function. Download a folder given by "out_filepath" and its contents recursively.
+
+        Args:
+            out_filepath (FilePath): The path to the folder to download to.
+            file_id (str): The ID of the folder to download.
+        """
+        for file in self.list_children(file_id):
+            t_name, t_file_id, t_mime_type = (
+                file["name"],
+                file["id"],
+                GoogleMimeTypes(file["mimeType"]),
+            )
+            t_out_filepath = out_filepath.joinpath(t_name)
+
+            if t_mime_type == GoogleMimeTypes.folder:
+                self._download_nested_filepath(
+                    out_filepath=t_out_filepath, file_id=t_file_id
+                )
+            else:
+                self.download(
+                    out_filepath=t_out_filepath,
+                    file_id=t_file_id,
+                    mime_type=t_mime_type,
+                    recursive=True,
+                )
+        return out_filepath
+
     def download(
         self,
         out_filepath: FilePath,
-        file_id: FileId,
+        file_id: str,
         mime_type: GoogleMimeTypes,
         recursive: bool = False,
         conversion_map: dict[
             GoogleMimeTypes, tuple[GoogleMimeTypes, str]
         ] = DEFAULT_DOWNLOAD_CONVERSION_MAP,
     ) -> Path:
         file_id = parse_file_id(file_id)
         out_filepath = Path(out_filepath)
 
         if recursive and mime_type == GoogleMimeTypes.folder:
-            for file in self.list_children(file_id):
-                t_name, t_id, t_mime_type = (
-                    file["name"],
-                    file["id"],
-                    GoogleMimeTypes(file["mimeType"]),
-                )
-
-                t_path = out_filepath.joinpath(t_name)
-
-                self.download(
-                    out_filepath=t_path,
-                    file_id=t_id,
-                    mime_type=t_mime_type,
-                    recursive=recursive,
-                )
-        else:
-            mime_type, ext = conversion_map.get(mime_type, (mime_type, ""))
-            out_filepath = out_filepath.with_suffix(ext)
+            return self._download_nested_filepath(out_filepath, file_id)
 
-            request = self.files.export_media(fileId=file_id, mimeType=mime_type.value)
+        mime_type, ext = conversion_map.get(mime_type, (mime_type, ""))
+        out_filepath = out_filepath.with_suffix(ext)
+        out_filepath.parent.mkdir(parents=True, exist_ok=True)
 
-            out_filepath.parent.mkdir(parents=True, exist_ok=True)
+        file = self.get(file_id=file_id)
 
-            file = self.get(file_id=file_id)
-
-            if float(file["size"]) >= DOWNLOAD_LIMIT:
-                link = file["exportLinks"].get(mime_type.value, "")
-                download_large_file(url=link, filepath=out_filepath)
-            else:
-                with out_filepath.open("wb") as out_file:
-                    downloader = googleapiclient.http.MediaIoBaseDownload(
-                        out_file, request
-                    )
-                    done = False
-                    while done is False:
-                        status, done = downloader.next_chunk()
-
-        return out_filepath
+        if float(file["size"]) >= DOWNLOAD_LIMIT:
+            link = file["exportLinks"].get(mime_type.value, "")
+            return download_large_file(url=link, filepath=out_filepath)
+        else:
+            return self._download(file_id, out_filepath, mime_type)
 
     @staticmethod
     def _upload_file_body(
         name: str,
-        parents: List[FileId] | None = None,
+        parents: List[str] | None = None,
         body: File | None = None,
         **kwargs: Any,
     ) -> dict[str, File | Any]:
         body = body if body is not None else {}
-        kwargs = {
-            "body": {
-                "name": name,
-                **body,
-                **kwargs,
-            }
-        }
+        body = {"name": name, **body, **kwargs}
+        kwargs = {"body": body}
 
         if parents is not None:
             kwargs["body"].setdefault("parents", parents)
 
         return kwargs
 
     def copy(
         self,
-        file_id: FileId,
+        file_id: str,
         to_filename: str,
         to_folder_id: str,
         body: File | None = None,
         **kwargs: Any,
-    ) -> File | None:
-        # TODO! Check if this and update returns valid File object.
-
+    ) -> File:
         file_id = parse_file_id(file_id)
         to_folder_id = parse_file_id(to_folder_id)
 
         kwargs = {
             "fileId": file_id,
             **self._upload_file_body(
                 name=to_filename, parents=[to_folder_id], body=body
             ),
             **kwargs,
         }
-
-        try:
-            return self.files.copy(**kwargs).execute()
-        except:
-            return None
+        return self.files.copy(**kwargs).execute()
 
     def update(
         self,
-        file_id: FileId,
+        file_id: str,
         filepath: FilePath,
         body: File | None = None,
         **kwargs: Any,
     ) -> File:
         file_id = parse_file_id(file_id)
         body = body if body is not None else {}
 
@@ -187,15 +180,14 @@
     def _list(
         list_func: Callable[[str | None], FileList | PermissionList]
     ) -> Iterable[FileList | PermissionList]:
         page_token = None
         while True:
             response = list_func(page_token)
             yield response
-
             if (page_token := response.get("nextPageToken", None)) is None:
                 break
 
     def list(
         self,
         query: str,
         fields: str = "*",
@@ -213,27 +205,25 @@
             pageToken=x,
             fields=self._list_fields(fields),
             orderBy=order_by,
             **kwargs,
         ).execute()
 
         for response in self._list(list_func):
-            for file in response.get("files", []):
-                yield file
+            yield from response.get("files", [])
 
     def list_children(
-        self, parent_id: FileId, fields: str = "*", **kwargs: Any
+        self, parent_id: str, fields: str = "*", **kwargs: Any
     ) -> Iterable[File]:
         parent_id = parse_file_id(parent_id)
-
         return self.list(
             query=f"{q_escape(parent_id)} in parents", fields=fields, **kwargs
         )
 
-    def _query_children(self, name: str, parents: List[FileId], q: str | None = None):
+    def _query_children(self, name: str, parents: List[str], q: str | None = None):
         filename = Path(name)
 
         parents_list = " or ".join(
             (f"{q_escape(parent)} in parents" for parent in parents)
         )
         names_list = " or ".join(
             (
@@ -241,142 +231,137 @@
                 f"name = {q_escape(filename.stem)}",
             )
         )
 
         queries = [parents_list, names_list, "trashed = false"]
         if q is not None:
             queries.append(q)
-
         query = " and ".join((f"({i})" for i in queries))
-
         return self.list(query=query)
 
     def _update_if_exists(
         self,
         name: str,
         filepath: FilePath,
-        parents: List[FileId] | None = None,
+        parents: List[str] | None = None,
         team_drives: bool = True,
     ) -> File | None:
-
         if parents is None:
             return None
-
-        files = self._query_children(name=name, parents=parents)
-
-        for file in files:
+        for file in self._query_children(name=name, parents=parents):
             return self.update(file["id"], filepath, supportsAllDrives=team_drives)
-        else:
-            return None
+        return None
 
     def _create_nested_folders(
-        self, filepath: Path, parents: List[FileId] | None, update: bool = True
-    ) -> None:
-        def create_or_get_if_exists(name: str, parents: List[FileId]):
+        self, filepath: Path, parents: List[str], update: bool = True
+    ) -> List[str]:
+        def create_or_get_if_exists(name: str, parents: List[str]):
             folders = self._query_children(
                 name=name,
                 parents=parents,
-                q=f"mimeType = '{GoogleMimeTypes.folder.value}'",
+                q=f"mimeType='{GoogleMimeTypes.folder.value}'",
             )
-
             if update and (folder := next(folders, None)) is not None:
                 return folder
-            else:
-                return self.files.create(
-                    **self._upload_file_body(
-                        name=dirname,
-                        parents=parents,
-                        mimeType=GoogleMimeTypes.folder.value,
-                    )
-                ).execute()
+
+            return self.files.create(
+                **self._upload_file_body(
+                    name=dirname,
+                    parents=parents,
+                    mimeType=GoogleMimeTypes.folder.value,
+                )
+            ).execute()
 
         for dirname in filepath.parts[:-1]:
             folder = create_or_get_if_exists(dirname, parents)
             parents = [folder["id"]]
 
         return parents
 
     def create(
         self,
         filepath: FilePath,
-        mime_type: GoogleMimeTypes | None = None,
-        parents: List[FileId] | None = None,
+        mime_type: GoogleMimeTypes,
+        parents: List[str] | None = None,
         create_folders: bool = False,
         update: bool = False,
         fields: str = "*",
         **kwargs: Any,
     ) -> File:
         filepath = Path(filepath)
-        parents = parse_file_id(parents)
+        parents = list(map(parse_file_id, parents)) if parents is not None else []
 
         if create_folders:
             parents = self._create_nested_folders(
                 filepath=filepath, parents=parents, update=update
             )
-
         if (
             update
             and (file := next(self._query_children(filepath.name, parents), None))
             is not None
         ):
             return file
 
-        if mime_type is not None:
-            kwargs = {
-                **self._upload_file_body(
-                    name=filepath.name, parents=parents, mimeType=mime_type.value
-                ),
-                **kwargs,
-            }
-            file = self.files.create(**kwargs).execute()
+        kwargs = {
+            **self._upload_file_body(
+                name=filepath.name, parents=parents, mimeType=mime_type.value
+            ),
+            **kwargs,
+            "fields": fields,
+        }
+        file = self.files.create(**kwargs).execute()
+        return file
 
-            return self.get(file_id=file["id"], fields=fields)
+    def delete(self, file_id: str, **kwargs: Any):
+        return self.files.delete(fileId=file_id, **kwargs).execute()
 
     def _upload(
         self,
         uploader: Callable,
         name: str,
         filepath: FilePath,
         mime_type: GoogleMimeTypes | None = None,
-        parents: List[FileId] | None = None,
+        parents: List[str] | None = None,
         body: File | None = None,
         update: bool = True,
-        fields: str = "*",
         **kwargs,
     ) -> File:
         filepath = Path(filepath)
-        parents = parse_file_id(parents)
-
+        parents = list(map(parse_file_id, parents)) if parents is not None else []
         if (
             update
             and (file := self._update_if_exists(name, filepath, parents)) is not None
         ):
             return file
 
         kwargs = {
             **self._upload_file_body(
                 name=name, parents=parents, body=body, mimeType=mime_type.value
             ),
             **kwargs,
         }
-
         kwargs["media_body"] = uploader()
         return self.files.create(**kwargs).execute()
 
     def upload_file(
         self,
         filepath: FilePath,
         name: str | None = None,
         mime_type: GoogleMimeTypes | None = None,
-        parents: List[FileId] | None = None,
+        parents: List[str] | None = None,
         body: File | None = None,
         update: bool = True,
         **kwargs: Any,
     ) -> File:
         filepath = Path(filepath)
+        mime_type = (
+            mime_type
+            if mime_type is not None
+            else GoogleMimeTypes[filepath.suffix.lstrip(".")]
+        )
 
         def uploader():
             return googleapiclient.http.MediaFileUpload(str(filepath), resumable=True)
 
         return self._upload(
             uploader=uploader,
             name=name if name is not None else filepath.name,
@@ -388,16 +373,16 @@
             **kwargs,
         )
 
     def upload_data(
         self,
         data: bytes,
         name: str,
-        mime_type: GoogleMimeTypes | None = None,
-        parents: List[FileId] | None = None,
+        mime_type: GoogleMimeTypes,
+        parents: List[str] | None = None,
         body: File | None = None,
         update: bool = True,
         **kwargs: Any,
     ) -> File:
         with BytesIO(data) as tio:
 
             def uploader():
@@ -411,53 +396,49 @@
                 parents=parents,
                 body=body,
                 update=update,
                 **kwargs,
             )
 
     def permissions_get(
-        self, file_id: FileId, permission_id: str, **kwargs: Any
+        self, file_id: str, permission_id: str, **kwargs: Any
     ) -> Permission:
         file_id = parse_file_id(file_id)
-
         return (
             self.service.permissions()
             .get(fileId=file_id, permissionId=permission_id, **kwargs)
             .execute()
         )
 
     def permissions_list(
-        self, file_id: FileId, fields: str = "*", **kwargs: Any
+        self, file_id: str, fields: str = "*", **kwargs: Any
     ) -> Iterable[Permission]:
         file_id = parse_file_id(file_id)
-
         list_func = (
             lambda x: self.service.permissions()
             .list(
                 fileId=file_id, pageToken=x, fields=self._list_fields(fields), **kwargs
             )
             .execute()
         )
-
         for response in self._list(list_func):
-            for file in response.get("permissions", []):
-                yield file
+            yield from response.get("permissions", [])
 
     def _permission_update_if_exists(
-        self, file_id: FileId, user_permission: Permission
+        self, file_id: str, user_permission: Permission
     ) -> Permission | None:
         for p in self.permissions_list(file_id):
             if p["emailAddress"].strip().lower() == user_permission["emailAddress"]:
                 return p
         else:
             return None
 
     def permissions_create(
         self,
-        file_id: FileId,
+        file_id: str,
         email_address: str,
         permission: Permission | None = None,
         sendNotificationEmail: bool = True,
         update: bool = False,
         **kwargs: Any,
     ) -> Permission:
         file_id = parse_file_id(file_id)
@@ -486,15 +467,14 @@
                 fields="*",
                 sendNotificationEmail=sendNotificationEmail,
                 **kwargs,
             )
             .execute()
         )
 
-    def permissions_delete(self, file_id: FileId, permission_id: str, **kwargs: Any):
+    def permissions_delete(self, file_id: str, permission_id: str, **kwargs: Any):
         file_id = parse_file_id(file_id)
-
         return (
             self.service.permissions()
             .delete(fileId=file_id, permissionId=permission_id, **kwargs)
             .execute()
         )
```

### Comparing `googleapiutils2-0.4.0/googleapiutils2/geocode.py` & `googleapiutils2-0.4.6/googleapiutils2/geocode/geocode.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import *
 
 import requests
 from requests.exceptions import JSONDecodeError
 
-from ._types.geocode import *
-from .utils import update_url_params
+from ..utils import update_url_params
+from .misc import *
 
 
 class Geocode:
     URL = "https://maps.googleapis.com/maps/api/geocode/json"
 
     def __init__(self, api_key: str):
         self.api_key = api_key
@@ -24,14 +24,16 @@
                 return None
         else:
             return None
 
     def geocode(self, address: str):
         url = update_url_params(Geocode.URL, {"address": address, "key": self.api_key})
         r = requests.get(url)
+
         return self._return_if_200(r)
 
     def reverse_geocode(self, lat: float, long: float):
         latlng = f"{lat},{long}"
         url = update_url_params(Geocode.URL, {"latlng": latlng, "key": self.api_key})
         r = requests.get(url)
+
         return self._return_if_200(r)
```

### Comparing `googleapiutils2-0.4.0/googleapiutils2/utils.py` & `googleapiutils2-0.4.6/googleapiutils2/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import json
 import pickle
 import urllib.parse
+from collections import defaultdict
 from enum import Enum
 from functools import cache
 from pathlib import Path
 from typing import *
 
 import googleapiclient.http
 import requests
@@ -18,61 +19,77 @@
 FilePath = str | Path
 
 
 if TYPE_CHECKING:
     from googleapiclient._apis.drive.v3.resources import File
     from googleapiclient._apis.sheets.v4.resources import Spreadsheet
 
-    FileId = str | File | Spreadsheet
-
-GEOCODE_URL = "https://maps.googleapis.com/maps/api/geocode/json"
 
 SCOPES = [
     "https://www.googleapis.com/auth/spreadsheets",
     "https://www.googleapis.com/auth/drive.file",
     "https://www.googleapis.com/auth/drive",
 ]
 
 
 TOKEN_PATH = "auth/token.pickle"
 CONFIG_PATH = "auth/credentials.json"
 
 
 class GoogleMimeTypes(Enum):
+    audio = "application/vnd.google-apps.audio"
+    docs = "application/vnd.google-apps.document"
+    drive_sdk = "application/vnd.google-apps.drive-sdk"
+    drawing = "application/vnd.google-apps.drawing"
+    file = "application/vnd.google-apps.file"
+    folder = "application/vnd.google-apps.folder"
+    form = "application/vnd.google-apps.form"
+    fusiontable = "application/vnd.google-apps.fusiontable"
+    jam = "application/vnd.google-apps.jam"
+    map = "application/vnd.google-apps.map"
+    photo = "application/vnd.google-apps.photo"
+    slides = "application/vnd.google-apps.presentation"
+    script = "application/vnd.google-apps.script"
+    shortcut = "application/vnd.google-apps.shortcut"
+    site = "application/vnd.google-apps.site"
+    sheets = "application/vnd.google-apps.spreadsheet"
+    unknown = "application/vnd.google-apps.unknown"
+    video = "application/vnd.google-apps.video"
+
     xls = "application/vnd.ms-excel"
     xlsx = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
-    xml = "text/xml"
     ods = "application/vnd.oasis.opendocument.spreadsheet"
-    csv = "text/plain"
-    tmpl = "text/plain"
-    pdf = "application/pdf"
-    php = "application/x-httpd-php"
+    csv = "text/csv"
+
     jpg = "image/jpeg"
     png = "image/png"
+    svg = "image/svg+xml"
     gif = "image/gif"
     bmp = "image/bmp"
+
     txt = "text/plain"
+    html = "text/html"
+    htm = "text/html"
+    xml = "text/xml"
+    tmpl = "text/plain"
+
     doc = "application/msword"
+    pdf = "application/pdf"
     js = "text/js"
     swf = "application/x-shockwave-flash"
     mp3 = "audio/mpeg"
     zip = "application/zip"
     rar = "application/rar"
     tar = "application/tar"
     arj = "application/arj"
     cab = "application/cab"
-    html = "text/html"
-    htm = "text/html"
-    default = "application/octet-stream"
-
-    folder = "application/vnd.google-apps.folder"
+    php = "application/x-httpd-php"
+    json = "application/vnd.google-apps.script+json"
 
-    docs = "application/vnd.google-apps.document"
-    sheets = "application/vnd.google-apps.spreadsheet"
-    slides = "application/vnd.google-apps.presentation"
+    default = "application/octet-stream"
 
 
 def url_components(url: str) -> dict[str, List[str]]:
     return urllib.parse.parse_qs(urllib.parse.urlparse(url).query)
 
 
 def update_url_params(url: str, params: dict) -> str:
@@ -129,14 +146,29 @@
         return creds
     else:
         return service_account.Credentials.from_service_account_info(
             client_config, scopes=scopes
         )
 
 
+def download_large_file(
+    url: str, filepath: FilePath, chunk_size=googleapiclient.http.DEFAULT_CHUNK_SIZE
+) -> Path:
+    filepath = Path(filepath)
+
+    with requests.get(url, stream=True) as r:
+        r.raise_for_status()
+
+        with open(filepath, "wb") as f:
+            for chunk in r.iter_content(chunk_size=chunk_size):
+                f.write(chunk)
+
+    return filepath
+
+
 def get_id_from_url(url: str) -> str:
     url_obj = urllib.parse.urlparse(url)
     path = url_obj.path
     paths = path.split("/")
 
     get_adjacent = (
         lambda x: paths[t_ix]
@@ -152,71 +184,58 @@
         comps = url_components(url)
         if (ids := comps.get("id")) is not None:
             return ids[0]
         else:
             raise ValueError(f"Could not parse file URL of {url}")
 
 
-def download_large_file(
-    url: str, filepath: FilePath, chunk_size=googleapiclient.http.DEFAULT_CHUNK_SIZE
-):
-    filepath = Path(filepath)
-
-    with requests.get(url, stream=True) as r:
-        r.raise_for_status()
-
-        with open(filepath, "wb") as f:
-            for chunk in r.iter_content(chunk_size=chunk_size):
-                f.write(chunk)
-
-
+@cache
 def parse_file_id(
-    file_id: FileId | Iterable[FileId] | None,
-) -> str | Iterable[str] | None:
-    def obj_to_id(file: str | File | Spreadsheet):
-        if isinstance(file, str):
-            return file
-        elif isinstance(file, dict):
-            return file.get("id", file.get("spreadsheetId"))
-        else:
-            return None
-
-    @cache
+    file_id: str,
+) -> str:
     def parse(file_id: str) -> str:
-        if file_id.find("http") != -1:
+        if "http" in file_id:
             return get_id_from_url(file_id)
         else:
             return file_id
 
-    def inner(file_id: FileId) -> str:
-        if (id := obj_to_id(file_id)) is not None:
-            return parse(id)
-        else:
-            return None
+    def obj_to_id(file: str) -> str:
+        if isinstance(file, str):
+            return file
+        elif isinstance(file, dict):
+            return file.get("id", file.get("spreadsheetId", None))
 
-    if isinstance(file_id, str):
-        return inner(file_id)
-    elif isinstance(file_id, Iterable):
-        return list(map(inner, file_id))
+    if (id := obj_to_id(file_id)) is not None:
+        return parse(id)
     else:
-        return None
+        return file_id
 
 
 def to_base(x: str | int, base: int, from_base: int = 10) -> list[int]:
     if isinstance(x, str):
         x = int(x, base=from_base)
 
     y = []
-    while x != 0:
+    while True:
         y.append(x % base)
-        x //= base
+        if (x := (x // base) - 1) < 0:
+            break
 
     return y[::-1]
 
 
+def nested_defaultdict(existing: dict | Any | None = None, **kwargs: Any):
+    if existing is None:
+        existing = {}
+    elif not isinstance(existing, dict):
+        return existing
+    existing = {key: nested_defaultdict(val) for key, val in existing.items()}
+    return defaultdict(nested_defaultdict, existing, **kwargs)
+
+
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 def take_annotation_from(
     this: Callable[P, Optional[T]]
 ) -> Callable[[Callable], Callable[P, Optional[T]]]:
```

### Comparing `googleapiutils2-0.4.0/setup.py` & `googleapiutils2-0.4.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['googleapiutils2', 'googleapiutils2._types']
+['googleapiutils2',
+ 'googleapiutils2.drive',
+ 'googleapiutils2.geocode',
+ 'googleapiutils2.sheets']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['google-api-python-client-stubs>=1.11.0,<2.0.0',
+['cachetools>=5.2.1,<6.0.0',
+ 'google-api-python-client-stubs>=1.11.0,<2.0.0',
  'google-api-python-client>=2.47.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.1,<0.6.0',
- 'pandas>=1.4.3,<2.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'types-requests>=2.28.9,<3.0.0']
+ 'pandas>=1.5.3,<2.0.0',
+ 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'googleapiutils2',
-    'version': '0.4.0',
-    'description': '',
+    'version': '0.4.6',
+    'description': "Simple and convenient wrapper for Google's Python API.",
     'long_description': 'None',
     'author': 'Mike Babb',
     'author_email': 'mike7400@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `googleapiutils2-0.4.0/PKG-INFO` & `googleapiutils2-0.4.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.4.0
-Summary: 
+Version: 0.4.6
+Summary: Simple and convenient wrapper for Google's Python API.
 Author: Mike Babb
 Author-email: mike7400@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cachetools (>=5.2.1,<6.0.0)
 Requires-Dist: google-api-python-client (>=2.47.0,<3.0.0)
 Requires-Dist: google-api-python-client-stubs (>=1.11.0,<2.0.0)
 Requires-Dist: google-auth-httplib2 (>=0.1.0,<0.2.0)
 Requires-Dist: google-auth-oauthlib (>=0.5.1,<0.6.0)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: types-requests (>=2.28.9,<3.0.0)
```

