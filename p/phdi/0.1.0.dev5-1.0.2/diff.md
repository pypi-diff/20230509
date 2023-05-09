# Comparing `tmp/phdi-0.1.0.dev5.tar.gz` & `tmp/phdi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdi-0.1.0.dev5.tar", max compression
+gzip compressed data, was "phdi-1.0.2.tar", max compression
```

## Comparing `phdi-0.1.0.dev5.tar` & `phdi-1.0.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     7048 2023-05-05 20:21:47.950468 phdi-0.1.0.dev5/LICENSE.md
--rw-r--r--   0        0        0    11787 2023-05-05 20:21:47.950468 phdi-0.1.0.dev5/README.md
--rw-r--r--   0        0        0       27 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/__init__.py
--rw-r--r--   0        0        0      223 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/cloud/README.md
--rw-r--r--   0        0        0        0 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/cloud/__init__.py
--rw-r--r--   0        0        0     8647 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/cloud/azure.py
--rw-r--r--   0        0        0     2516 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/cloud/core.py
--rw-r--r--   0        0        0     6055 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/cloud/gcp.py
--rw-r--r--   0        0        0      163 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/containers/README.md
--rw-r--r--   0        0        0        0 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/containers/__init__.py
--rw-r--r--   0        0        0     2198 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/containers/base_service.py
--rw-r--r--   0        0        0        0 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/__init__.py
--rw-r--r--   0        0        0      292 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/cloud/README.md
--rw-r--r--   0        0        0      119 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/cloud/__init__.py
--rw-r--r--   0        0        0     2111 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/cloud/azure.py
--rw-r--r--   0        0        0      311 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/conversion/README.md
--rw-r--r--   0        0        0       89 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/conversion/__init__.py
--rw-r--r--   0        0        0     8026 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/conversion/convert.py
--rw-r--r--   0        0        0      808 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/geospatial/README.md
--rw-r--r--   0        0        0      294 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/geospatial/__init__.py
--rw-r--r--   0        0        0     3494 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/geospatial/census.py
--rw-r--r--   0        0        0     4521 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/geospatial/core.py
--rw-r--r--   0        0        0     3587 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/geospatial/smarty.py
--rw-r--r--   0        0        0      890 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/harmonization/README.md
--rw-r--r--   0        0        0      335 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/harmonization/__init__.py
--rw-r--r--   0        0        0    11809 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/harmonization/standardization.py
--rw-r--r--   0        0        0      179 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/linkage/__init__.py
--rw-r--r--   0        0        0     3591 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/linkage/link.py
--rw-r--r--   0        0        0      412 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/tabulation/README.md
--rw-r--r--   0        0        0      367 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/tabulation/__init__.py
--rw-r--r--   0        0        0    27459 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/tabulation/tables.py
--rw-r--r--   0        0        0      397 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/transport/README.md
--rw-r--r--   0        0        0      327 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/transport/__init__.py
--rw-r--r--   0        0        0     7383 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/transport/export.py
--rw-r--r--   0        0        0     6822 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/transport/http.py
--rw-r--r--   0        0        0     7005 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/utils.py
--rw-r--r--   0        0        0      881 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/geospatial/README.md
--rw-r--r--   0        0        0      291 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/geospatial/__init__.py
--rw-r--r--   0        0        0     9294 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/geospatial/census.py
--rw-r--r--   0        0        0     2697 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/geospatial/core.py
--rw-r--r--   0        0        0     5911 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/geospatial/smarty.py
--rw-r--r--   0        0        0     1027 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/README.md
--rw-r--r--   0        0        0      869 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/__init__.py
--rw-r--r--   0        0        0    28162 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/double_metaphone.py
--rw-r--r--   0        0        0    10909 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/hl7.py
--rw-r--r--   0        0        0    36359 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/phdi_nicknames.csv
--rw-r--r--   0        0        0    11999 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/standardization.py
--rw-r--r--   0        0        0     1952 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/utils.py
--rw-r--r--   0        0        0      255 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/README.md
--rw-r--r--   0        0        0     1869 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/__init__.py
--rw-r--r--   0        0        0     1948 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/algorithms.py
--rw-r--r--   0        0        0     2288 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/core.py
--rw-r--r--   0        0        0    56924 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/link.py
--rw-r--r--   0        0        0    10976 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/postgres.py
--rw-r--r--   0        0        0     2667 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/seed.py
--rw-r--r--   0        0        0      399 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/tables.ddl
--rw-r--r--   0        0        0      225 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/tabulation/README.md
--rw-r--r--   0        0        0      134 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/tabulation/__init__.py
--rw-r--r--   0        0        0    11839 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/tabulation/tables.py
--rw-r--r--   0        0        0     2881 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/tabulation/validation_schema.json
--rw-r--r--   0        0        0      225 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/transport/README.md
--rw-r--r--   0        0        0       81 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/transport/__init__.py
--rw-r--r--   0        0        0     2334 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/transport/http.py
--rw-r--r--   0        0        0     1244 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/validation/__init__.py
--rw-r--r--   0        0        0     6260 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/validation/validation.py
--rw-r--r--   0        0        0    17870 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/validation/xml_utils.py
--rw-r--r--   0        0        0     1438 2023-05-05 20:21:48.422473 phdi-0.1.0.dev5/pyproject.toml
--rw-r--r--   0        0        0    13594 1970-01-01 00:00:00.000000 phdi-0.1.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-05-09 16:54:17.546780 phdi-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0    11787 2023-05-09 16:54:17.546780 phdi-1.0.2/README.md
+-rw-r--r--   0        0        0       27 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/cloud/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/cloud/__init__.py
+-rw-r--r--   0        0        0     8647 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/cloud/azure.py
+-rw-r--r--   0        0        0     2516 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/cloud/core.py
+-rw-r--r--   0        0        0     6055 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/cloud/gcp.py
+-rw-r--r--   0        0        0      163 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/containers/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/containers/__init__.py
+-rw-r--r--   0        0        0     2760 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/containers/base_service.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/__init__.py
+-rw-r--r--   0        0        0      292 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/cloud/README.md
+-rw-r--r--   0        0        0      119 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/cloud/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/cloud/azure.py
+-rw-r--r--   0        0        0      311 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/conversion/README.md
+-rw-r--r--   0        0        0       89 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/conversion/__init__.py
+-rw-r--r--   0        0        0     8026 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/conversion/convert.py
+-rw-r--r--   0        0        0      808 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/geospatial/README.md
+-rw-r--r--   0        0        0      294 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/geospatial/__init__.py
+-rw-r--r--   0        0        0     3494 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/geospatial/census.py
+-rw-r--r--   0        0        0     4521 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/geospatial/core.py
+-rw-r--r--   0        0        0     3587 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/geospatial/smarty.py
+-rw-r--r--   0        0        0      890 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/harmonization/README.md
+-rw-r--r--   0        0        0      335 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/harmonization/__init__.py
+-rw-r--r--   0        0        0    11809 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/harmonization/standardization.py
+-rw-r--r--   0        0        0      179 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/linkage/__init__.py
+-rw-r--r--   0        0        0     3591 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/linkage/link.py
+-rw-r--r--   0        0        0      412 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/tabulation/README.md
+-rw-r--r--   0        0        0      367 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/tabulation/__init__.py
+-rw-r--r--   0        0        0    27459 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/tabulation/tables.py
+-rw-r--r--   0        0        0      397 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/transport/README.md
+-rw-r--r--   0        0        0      327 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/transport/__init__.py
+-rw-r--r--   0        0        0     7383 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/transport/export.py
+-rw-r--r--   0        0        0     6822 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/transport/http.py
+-rw-r--r--   0        0        0     7005 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/fhir/utils.py
+-rw-r--r--   0        0        0      881 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/geospatial/README.md
+-rw-r--r--   0        0        0      291 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/geospatial/__init__.py
+-rw-r--r--   0        0        0     9294 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/geospatial/census.py
+-rw-r--r--   0        0        0     2697 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/geospatial/core.py
+-rw-r--r--   0        0        0     5911 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/geospatial/smarty.py
+-rw-r--r--   0        0        0     1027 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/README.md
+-rw-r--r--   0        0        0      869 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/__init__.py
+-rw-r--r--   0        0        0    28162 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/double_metaphone.py
+-rw-r--r--   0        0        0    10909 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/hl7.py
+-rw-r--r--   0        0        0    36359 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/phdi_nicknames.csv
+-rw-r--r--   0        0        0    11999 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/standardization.py
+-rw-r--r--   0        0        0     1952 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/harmonization/utils.py
+-rw-r--r--   0        0        0      255 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/README.md
+-rw-r--r--   0        0        0     1869 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/__init__.py
+-rw-r--r--   0        0        0     1948 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/algorithms.py
+-rw-r--r--   0        0        0     2288 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/core.py
+-rw-r--r--   0        0        0    56924 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/link.py
+-rw-r--r--   0        0        0    10976 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/postgres.py
+-rw-r--r--   0        0        0     2667 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/seed.py
+-rw-r--r--   0        0        0      399 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/linkage/tables.ddl
+-rw-r--r--   0        0        0      225 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/tabulation/README.md
+-rw-r--r--   0        0        0      134 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/tabulation/__init__.py
+-rw-r--r--   0        0        0    11839 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/tabulation/tables.py
+-rw-r--r--   0        0        0     2881 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/tabulation/validation_schema.json
+-rw-r--r--   0        0        0      225 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/transport/README.md
+-rw-r--r--   0        0        0       81 2023-05-09 16:54:18.026780 phdi-1.0.2/phdi/transport/__init__.py
+-rw-r--r--   0        0        0     2334 2023-05-09 16:54:18.030780 phdi-1.0.2/phdi/transport/http.py
+-rw-r--r--   0        0        0     1244 2023-05-09 16:54:18.030780 phdi-1.0.2/phdi/validation/__init__.py
+-rw-r--r--   0        0        0     6260 2023-05-09 16:54:18.030780 phdi-1.0.2/phdi/validation/validation.py
+-rw-r--r--   0        0        0    17870 2023-05-09 16:54:18.030780 phdi-1.0.2/phdi/validation/xml_utils.py
+-rw-r--r--   0        0        0     1820 2023-05-09 16:54:18.038780 phdi-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    13589 1970-01-01 00:00:00.000000 phdi-1.0.2/PKG-INFO
```

### Comparing `phdi-0.1.0.dev5/LICENSE.md` & `phdi-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/README.md` & `phdi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/cloud/azure.py` & `phdi-1.0.2/phdi/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/cloud/core.py` & `phdi-1.0.2/phdi/cloud/core.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/cloud/gcp.py` & `phdi-1.0.2/phdi/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/containers/base_service.py` & `phdi-1.0.2/phdi/containers/base_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,62 @@
 from fastapi import FastAPI
 from pathlib import Path
+from enum import Enum
 from importlib import metadata
 
 
+# create a class with the DIBBs default Creative Commons Zero v1.0 and
+# MIT license to be used by the BaseService class
+class LicenseType(Enum):
+    CreativeCommonsZero = {
+        "name": "Creative Commons Zero v1.0 Universal",
+        "url": "https://creativecommons.org/publicdomain/zero/1.0/",
+    }
+    MIT = {"name": "The MIT License", "url": "https://mit-license.org/"}
+
+
 class BaseService:
     """
     Base class for all DIBBs services. This class provides a FastAPI instance with DIBBs
     metadata and optionally a health check endpoint.
     """
 
+    LICENSE_INFO = LicenseType.CreativeCommonsZero
+    DIBBS_CONTACT = {
+        "name": "CDC Public Health Data Infrastructure",
+        "url": "https://cdcgov.github.io/phdi-site/",
+        "email": "dmibuildingblocks@cdc.gov",
+    }
+
     def __init__(
         self,
         service_name: str,
         description_path: str,
         include_health_check_endpoint: bool = True,
+        license_info: LicenseType = LICENSE_INFO,
     ):
         """
         Initialize a BaseService instance.
 
         :param service_name: The name of the service.
         :param description_path: The path to a markdown file containing a description of
             the service.
         :param include_health_check_endpoint: If True, the standard DIBBs health check
             endpoint will be added.
+        :param license_info: If empty, the standard DIBBs Creative Commons Zero v1.0
+            Universal license will be used. The other available option is to use the
+            MIT license.
         """
         description = Path(description_path).read_text(encoding="utf-8")
         self.include_health_check_endpoint = include_health_check_endpoint
         self.app = FastAPI(
             title=service_name,
             version=metadata.version("phdi"),
-            contact={
-                "name": "CDC Public Health Data Infrastructure",
-                "url": "https://cdcgov.github.io/phdi-site/",
-                "email": "dmibuildingblocks@cdc.gov",
-            },
-            license_info={
-                "name": "Creative Commons Zero v1.0 Universal",
-                "url": "https://creativecommons.org/publicdomain/zero/1.0/",
-            },
+            contact=self.DIBBS_CONTACT,
+            license_info=license_info,
             description=description,
         )
 
     def add_health_check_endpoint(self):
         @self.app.get("/")
         async def health_check() -> dict:
             """
```

### Comparing `phdi-0.1.0.dev5/phdi/fhir/cloud/azure.py` & `phdi-1.0.2/phdi/fhir/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/fhir/conversion/convert.py` & `phdi-1.0.2/phdi/fhir/conversion/convert.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/fhir/geospatial/README.md` & `phdi-1.0.2/phdi/fhir/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/fhir/geospatial/census.py` & `phdi-1.0.2/phdi/fhir/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/fhir/geospatial/core.py` & `phdi-1.0.2/phdi/fhir/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/fhir/geospatial/smarty.py` & `phdi-1.0.2/phdi/fhir/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/fhir/harmonization/README.md` & `phdi-1.0.2/phdi/fhir/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/fhir/harmonization/standardization.py` & `phdi-1.0.2/phdi/fhir/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/fhir/linkage/link.py` & `phdi-1.0.2/phdi/fhir/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/fhir/tabulation/tables.py` & `phdi-1.0.2/phdi/fhir/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/fhir/transport/export.py` & `phdi-1.0.2/phdi/fhir/transport/export.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/fhir/transport/http.py` & `phdi-1.0.2/phdi/fhir/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/fhir/utils.py` & `phdi-1.0.2/phdi/fhir/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/geospatial/README.md` & `phdi-1.0.2/phdi/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/geospatial/census.py` & `phdi-1.0.2/phdi/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/geospatial/core.py` & `phdi-1.0.2/phdi/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/geospatial/smarty.py` & `phdi-1.0.2/phdi/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/harmonization/README.md` & `phdi-1.0.2/phdi/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/harmonization/__init__.py` & `phdi-1.0.2/phdi/harmonization/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/harmonization/double_metaphone.py` & `phdi-1.0.2/phdi/harmonization/double_metaphone.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/harmonization/hl7.py` & `phdi-1.0.2/phdi/harmonization/hl7.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/harmonization/phdi_nicknames.csv` & `phdi-1.0.2/phdi/harmonization/phdi_nicknames.csv`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/harmonization/standardization.py` & `phdi-1.0.2/phdi/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/harmonization/utils.py` & `phdi-1.0.2/phdi/harmonization/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/linkage/__init__.py` & `phdi-1.0.2/phdi/linkage/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/linkage/algorithms.py` & `phdi-1.0.2/phdi/linkage/algorithms.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/linkage/core.py` & `phdi-1.0.2/phdi/linkage/core.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/linkage/link.py` & `phdi-1.0.2/phdi/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/linkage/postgres.py` & `phdi-1.0.2/phdi/linkage/postgres.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/linkage/seed.py` & `phdi-1.0.2/phdi/linkage/seed.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/tabulation/tables.py` & `phdi-1.0.2/phdi/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/tabulation/validation_schema.json` & `phdi-1.0.2/phdi/tabulation/validation_schema.json`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/transport/http.py` & `phdi-1.0.2/phdi/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/validation/__init__.py` & `phdi-1.0.2/phdi/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/validation/validation.py` & `phdi-1.0.2/phdi/validation/validation.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/phdi/validation/xml_utils.py` & `phdi-1.0.2/phdi/validation/xml_utils.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev5/pyproject.toml` & `phdi-1.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "phdi"
-version = "v0.1.0.dev5"
+version = "v1.0.2"
 description = "Public health data infrastructure Building Blocks is a library to help public health departments work with their data"
-authors = ["Kenneth Chow <kenneth@skylight.digital>", "Brandon Mader <brandon@skylight.digital>", "Spencer Kathol <spencer@skylight.digital>"]
+authors = ["Kenneth Chow <kenneth@skylight.digital>", "Brandon Mader <brandon@skylight.digital>", "Spencer Kathol <spencer@skylight.digital>", "Nick Clyde <nclyde@skylight.digital", "Dan Paseltiner <dan@skylight.digital>", "Brady Fausett <brady@skylight.digital>", "Marcelle Goggins <marcelle@skylight.digital", "Nick Bristow <nick@skylight.digital>", "Bryan Britten <bryan@skylight.digital>", "Emma Stephenson <emma@skylight.digital>" , "Gordon Farrell <gordon@skylight.digital>", "Robert Mitchell <rmitchell@skylight.digital>"]
 homepage = "https://github.com/CDCgov/phdi"
 repository = "https://github.com/CDCgov/phdi"
 documentation = "https://cdcgov.github.io/phdi"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `phdi-0.1.0.dev5/PKG-INFO` & `phdi-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdi
-Version: 0.1.0.dev5
+Version: 1.0.2
 Summary: Public health data infrastructure Building Blocks is a library to help public health departments work with their data
 Home-page: https://github.com/CDCgov/phdi
 Author: Kenneth Chow
 Author-email: kenneth@skylight.digital
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

