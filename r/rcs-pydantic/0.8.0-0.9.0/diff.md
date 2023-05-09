# Comparing `tmp/rcs_pydantic-0.8.0.tar.gz` & `tmp/rcs_pydantic-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcs_pydantic-0.8.0.tar", max compression
+gzip compressed data, was "rcs_pydantic-0.9.0.tar", max compression
```

## Comparing `rcs_pydantic-0.8.0.tar` & `rcs_pydantic-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1076 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/LICENSE
--rw-r--r--   0        0        0     6172 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/README.md
--rw-r--r--   0        0        0     1287 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1462 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/rcs_pydantic/__init__.py
--rw-r--r--   0        0        0     5037 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/rcs_pydantic/enums.py
--rw-r--r--   0        0        0    45689 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/rcs_pydantic/errors.py
--rw-r--r--   0        0        0      713 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/rcs_pydantic/exceptions.py
--rw-r--r--   0        0        0     3954 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/rcs_pydantic/main.py
--rw-r--r--   0        0        0    20259 2023-04-21 00:20:57.361608 rcs_pydantic-0.8.0/rcs_pydantic/scheme.py
--rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 rcs_pydantic-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-09 05:24:34.300335 rcs_pydantic-0.9.0/LICENSE
+-rw-r--r--   0        0        0     6172 2023-05-09 05:24:34.300335 rcs_pydantic-0.9.0/README.md
+-rw-r--r--   0        0        0     1287 2023-05-09 05:24:34.300335 rcs_pydantic-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1462 2023-05-09 05:24:34.300335 rcs_pydantic-0.9.0/rcs_pydantic/__init__.py
+-rw-r--r--   0        0        0     5037 2023-05-09 05:24:34.300335 rcs_pydantic-0.9.0/rcs_pydantic/enums.py
+-rw-r--r--   0        0        0    45689 2023-05-09 05:24:34.300335 rcs_pydantic-0.9.0/rcs_pydantic/errors.py
+-rw-r--r--   0        0        0      713 2023-05-09 05:24:34.300335 rcs_pydantic-0.9.0/rcs_pydantic/exceptions.py
+-rw-r--r--   0        0        0     4260 2023-05-09 05:24:34.300335 rcs_pydantic-0.9.0/rcs_pydantic/main.py
+-rw-r--r--   0        0        0    20259 2023-05-09 05:24:34.300335 rcs_pydantic-0.9.0/rcs_pydantic/scheme.py
+-rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 rcs_pydantic-0.9.0/PKG-INFO
```

### Comparing `rcs_pydantic-0.8.0/LICENSE` & `rcs_pydantic-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.8.0/README.md` & `rcs_pydantic-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.8.0/pyproject.toml` & `rcs_pydantic-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rcs-pydantic"
-version = "0.8.0"
+version = "0.9.0"
 description = ""
 authors = ["xncbf <xncbf12@gmail.com>"]
 keywords = ["pydantic", "rcs", "fastapi"]
 homepage = "https://github.com/xncbf/rcs-pydantic"
 repository = "https://github.com/xncbf/rcs-pydantic"
 license = "MIT"
 readme = "README.md"
```

### Comparing `rcs_pydantic-0.8.0/rcs_pydantic/__init__.py` & `rcs_pydantic-0.9.0/rcs_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.8.0/rcs_pydantic/enums.py` & `rcs_pydantic-0.9.0/rcs_pydantic/enums.py`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.8.0/rcs_pydantic/errors.py` & `rcs_pydantic-0.9.0/rcs_pydantic/errors.py`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.8.0/rcs_pydantic/exceptions.py` & `rcs_pydantic-0.9.0/rcs_pydantic/exceptions.py`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.8.0/rcs_pydantic/main.py` & `rcs_pydantic-0.9.0/rcs_pydantic/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,28 +18,32 @@
             scheme.RcsSMSCarouselBody,
             scheme.RcsLMSCarouselBody,
             scheme.RcsMMSCarouselBody,
             scheme.RcsCHATCarouselBody,
             dict,
         ],
         agency_id: Optional[str] = None,
+        agency_key: Optional[str] = None,
+        brand_key: Optional[str] = None,
         message_base_id: Union[enums.MessageEnum, enums.RCSMessageEnum] = enums.MessageEnum.SMS,
         service_type: enums.ServiceTypeEnum = enums.ServiceTypeEnum.SMS,
         expiry_option: Optional[enums.ExpiryOptionEnum] = None,
         header: enums.HeaderEnum = enums.HeaderEnum.NOT_ADVERTISE,
         footer: Optional[str] = None,
         cdr_id: Optional[str] = None,
         copy_allowed: Optional[bool] = None,
         buttons: Optional[list] = None,
         chips: Optional[list] = None,
         legacy: Optional[scheme.LegacyInfo] = None,
         message_group_id: Optional[str] = None,
     ):
         self.message_info = message_info
         self.agency_id = agency_id
+        self.agency_key = agency_key
+        self.brand_key = brand_key
         self.message_base_id = message_base_id
         self.service_type = service_type
         self.expiry_option = expiry_option
         self.header = header
         self.footer = footer
         self.cdr_id = cdr_id
         self.copy_allowed = copy_allowed
@@ -91,14 +95,18 @@
             messagebaseId=self.message_base_id,
             serviceType=self.service_type,
             header=self.header,
             body=self.body,
         )
         if self.agency_id:
             rcs_info.agencyId = self.agency_id
+        if self.agency_key:
+            rcs_info.agencyKey = self.agency_key
+        if self.brand_key:
+            rcs_info.brandKey = self.brand_key
         if self.expiry_option:
             rcs_info.expiryOption = self.expiry_option
         if self.service_type == enums.ServiceTypeEnum.CHAT:
             rcs_info.expiryOption = enums.ExpiryOptionEnum.AFTER_SETTING_TIMES
         if self.footer:
             rcs_info.footer = self.footer
         if self.cdr_id:
```

### Comparing `rcs_pydantic-0.8.0/rcs_pydantic/scheme.py` & `rcs_pydantic-0.9.0/rcs_pydantic/scheme.py`

 * *Files identical despite different names*

### Comparing `rcs_pydantic-0.8.0/PKG-INFO` & `rcs_pydantic-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcs-pydantic
-Version: 0.8.0
+Version: 0.9.0
 Summary: 
 Home-page: https://github.com/xncbf/rcs-pydantic
 License: MIT
 Keywords: pydantic,rcs,fastapi
 Author: xncbf
 Author-email: xncbf12@gmail.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rcs-pydantic Version: 0.8.0 Summary: Home-page:
+Metadata-Version: 2.1 Name: rcs-pydantic Version: 0.9.0 Summary: Home-page:
 https://github.com/xncbf/rcs-pydantic License: MIT Keywords:
 pydantic,rcs,fastapi Author: xncbf Author-email: xncbf12@gmail.com Requires-
 Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

