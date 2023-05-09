# Comparing `tmp/axdd-person-client-1.1.5.tar.gz` & `tmp/axdd-person-client-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axdd-person-client-1.1.5.tar", last modified: Thu May  4 19:27:47 2023, max compression
+gzip compressed data, was "axdd-person-client-1.1.6.tar", last modified: Tue May  9 20:54:51 2023, max compression
```

## Comparing `axdd-person-client-1.1.5.tar` & `axdd-person-client-1.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.083322 axdd-person-client-1.1.5/axdd_person_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-04 19:27:46.000000 axdd-person-client-1.1.5/axdd_person_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-04 19:27:47.000000 axdd-person-client-1.1.5/axdd_person_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 19:27:46.000000 axdd-person-client-1.1.5/axdd_person_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-04 19:27:46.000000 axdd-person-client-1.1.5/axdd_person_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-04 19:27:46.000000 axdd-person-client-1.1.5/axdd_person_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.083322 axdd-person-client-1.1.5/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/uw_person_client/
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/uw_person_client/clients/
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25868 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/clients/core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/clients/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3549 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/uw_person_client/databases/
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/databases/postgres.py
--rw-r--r--   0 runner    (1001) docker     (122)     5858 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/databases/uwpds.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:47.087322 axdd-person-client-1.1.5/uw_person_client/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (122)    34221 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/tests/test_core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-05-04 19:27:36.000000 axdd-person-client-1.1.5/uw_person_client/tests/test_mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.849752 axdd-person-client-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-09 20:54:51.849752 axdd-person-client-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.845752 axdd-person-client-1.1.6/axdd_person_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-09 20:54:51.000000 axdd-person-client-1.1.6/axdd_person_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-09 20:54:51.000000 axdd-person-client-1.1.6/axdd_person_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 20:54:51.000000 axdd-person-client-1.1.6/axdd_person_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-09 20:54:51.000000 axdd-person-client-1.1.6/axdd_person_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-09 20:54:51.000000 axdd-person-client-1.1.6/axdd_person_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.845752 axdd-person-client-1.1.6/conf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 20:54:51.849752 axdd-person-client-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.845752 axdd-person-client-1.1.6/uw_person_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.845752 axdd-person-client-1.1.6/uw_person_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27350 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/clients/core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/clients/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3588 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.849752 axdd-person-client-1.1.6/uw_person_client/databases/
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/databases/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6038 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/databases/uwpds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:51.849752 axdd-person-client-1.1.6/uw_person_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35548 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/tests/test_core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-05-09 20:54:40.000000 axdd-person-client-1.1.6/uw_person_client/tests/test_mock_client.py
```

### Comparing `axdd-person-client-1.1.5/LICENSE` & `axdd-person-client-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.5/PKG-INFO` & `axdd-person-client-1.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.5
+Version: 1.1.6
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.5/README.md` & `axdd-person-client-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.5/axdd_person_client.egg-info/PKG-INFO` & `axdd-person-client-1.1.6/axdd_person_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.5
+Version: 1.1.6
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.5/axdd_person_client.egg-info/SOURCES.txt` & `axdd-person-client-1.1.6/axdd_person_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.5/conf/settings.py` & `axdd-person-client-1.1.6/conf/settings.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.5/setup.py` & `axdd-person-client-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.5/uw_person_client/clients/__init__.py` & `axdd-person-client-1.1.6/uw_person_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.5/uw_person_client/clients/core_client.py` & `axdd-person-client-1.1.6/uw_person_client/clients/core_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sqlalchemy.orm.exc import NoResultFound
 from uw_person_client.clients import AbstractUWPersonClient
 from uw_person_client.databases.uwpds import UWPDS
 from uw_person_client.exceptions import (
     PersonNotFoundException, AdviserNotFoundException)
 from uw_person_client.components import (
     Person, Student, Employee, Transcript, Major, Sport, Adviser, Term,
-    Transfer, Hold)
+    Transfer, Hold, Degree)
 
 
 class UWPersonClient(AbstractUWPersonClient):
 
     """
     Public methods
     """
@@ -125,15 +125,16 @@
                     include_student=True,
                     include_student_transcripts=True,
                     include_student_transfers=True,
                     include_student_sports=True,
                     include_student_advisers=True,
                     include_student_majors=True,
                     include_student_pending_majors=True,
-                    include_student_holds=True):
+                    include_student_holds=True,
+                    include_student_degrees=True):
         person = Person()
         person.uwnetid = sqla_person.uwnetid
         person.uwregid = sqla_person.uwregid
         person.prior_uwnetids = sqla_person.prior_uwnetids
         person.prior_uwregids = sqla_person.prior_uwregids
         person.pronouns = sqla_person.pronouns
         person.full_name = sqla_person.full_name
@@ -156,14 +157,15 @@
                     include_student_transcripts=include_student_transcripts,
                     include_student_transfers=include_student_transfers,
                     include_student_sports=include_student_sports,
                     include_student_advisers=include_student_advisers,
                     include_student_majors=include_student_majors,
                     include_student_pending_majors=include_student_pending_majors,  # noqa
                     include_student_holds=include_student_holds,
+                    include_student_degrees=include_student_degrees,
                 )
             except NoResultFound:
                 pass
 
         if include_employee:
             try:
                 sqla_employee = self.DB.session.query(self.DB.Employee).filter(
@@ -177,15 +179,16 @@
     def _map_student(self, sqla_student,
                      include_student_transcripts=True,
                      include_student_transfers=True,
                      include_student_sports=True,
                      include_student_advisers=True,
                      include_student_majors=True,
                      include_student_pending_majors=True,
-                     include_student_holds=True):
+                     include_student_holds=True,
+                     include_student_degrees=True):
         student = Student()
 
         student.system_key = sqla_student.system_key
         student.student_number = sqla_student.student_number
         student.application_status_code = sqla_student.application_status_code
         student.application_status_desc = sqla_student.application_status_desc
         student.application_type_code = sqla_student.application_type_code
@@ -371,14 +374,21 @@
         if include_student_holds:
             # map holds
             student.holds = []
             for hold in sqla_student.student_hold:
                 hold = self._map_hold(hold)
                 student.holds.append(hold)
 
+        if include_student_degrees:
+            # map degrees
+            student.degrees = []
+            for degree in sqla_student.student_degree:
+                degree = self._map_degree(degree)
+                student.degrees.append(degree)
+
         return student
 
     def _map_employee(self, sqla_employee):
         employee = Employee()
         employee.employee_number = sqla_employee.employee_number
         employee.employee_affiliation_state = \
             sqla_employee.employee_affiliation_state
@@ -522,12 +532,31 @@
         hold.hold_office = sqla_hold.hold_office
         hold.hold_office_desc = sqla_hold.hold_office_desc
         hold.hold_reason = sqla_hold.hold_reason
         hold.hold_type = sqla_hold.hold_type
         hold.hold_type_desc = Hold.TYPE_DESCRIPTIONS.get(sqla_hold.hold_type)
         return hold
 
+    def _map_degree(self, sqla_degree):
+        degree = Degree()
+        degree.degree_term = self._map_term(sqla_degree.degree_term)
+        degree.campus_code = sqla_degree.campus_code
+        degree.degree_abbr_code = sqla_degree.degree_abbr_code
+        degree.degree_pathway_num = sqla_degree.degree_pathway_num
+        degree.degree_level_code = sqla_degree.degree_level_code
+        degree.degree_level_desc = sqla_degree.degree_level_desc
+        degree.degree_type_code = sqla_degree.degree_type_code
+        degree.degree_level_type_desc = sqla_degree.degree_level_type_desc
+        degree.degree_desc = sqla_degree.degree_desc
+        degree.degree_uw_credits = sqla_degree.degree_uw_credits
+        degree.degree_transfer_credits = sqla_degree.degree_transfer_credits
+        degree.degree_extension_credits = sqla_degree.degree_extension_credits
+        degree.degree_gpa = sqla_degree.degree_gpa
+        degree.fin_org_key = sqla_degree.fin_org_key
+        degree.primary_fin_org_key = sqla_degree.primary_fin_org_key
+        return degree
+
     def _map_term(self, sqla_term):
         term = Term()
         term.year = sqla_term.year
         term.quarter = sqla_term.quarter
         return term
```

### Comparing `axdd-person-client-1.1.5/uw_person_client/clients/mock_client.py` & `axdd-person-client-1.1.6/uw_person_client/clients/mock_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.5/uw_person_client/components.py` & `axdd-person-client-1.1.6/uw_person_client/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,18 @@
     TYPE_DESCRIPTIONS = {
         1: "REGISTRATION HOLD",
         2: "TRANSCRIPT HOLD",
         3: "REGISTRATION AND TRANSCRIPT HOLD"
     }
 
 
+class Degree(AbstractBase):
+    pass
+
+
 class Major(AbstractBase):
     pass
 
 
 class Sport(AbstractBase):
     pass
```

### Comparing `axdd-person-client-1.1.5/uw_person_client/databases/__init__.py` & `axdd-person-client-1.1.6/uw_person_client/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.5/uw_person_client/databases/postgres.py` & `axdd-person-client-1.1.6/uw_person_client/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.5/uw_person_client/databases/uwpds.py` & `axdd-person-client-1.1.6/uw_person_client/databases/uwpds.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         self.Major = UWPDS.Base.classes.major
         self.Sport = UWPDS.Base.classes.sport
         self.StudentToSport = UWPDS.Base.classes.student_to_sport
         self.StudentToAdviser = UWPDS.Base.classes.student_to_adviser
         self.Transcript = UWPDS.Base.classes.transcript
         self.Transfer = UWPDS.Base.classes.transfer
         self.Hold = UWPDS.Base.classes.student_hold
+        self.Degree = UWPDS.Base.classes.degree
         self.Term = UWPDS.Base.classes.term
 
     def initialize_relationships(self):
         student_to_sport = Table(
             'student_to_sport',
             UWPDS.Base.metadata,
             autoload=True,
@@ -91,14 +92,17 @@
                              viewonly=True)
             transcript = relationship(
                 "Transcript", back_populates="student", uselist=True,
                 viewonly=True)
             transfer = relationship(
                 "transfer", back_populates="student", uselist=True,
                 viewonly=True)
+            degree = relationship(
+                "degree", back_populates="student", uselist=True,
+                viewonly=True)
             student_hold = relationship(
                 "student_hold", back_populates="student", uselist=True,
                 order_by="student_hold.seq", viewonly=True)
             academic_term_id = Column(
                 'academic_term_id', ForeignKey('term.id', ondelete="CASCADE"))
             academic_term = \
                 relationship("term", foreign_keys=[academic_term_id],
```

### Comparing `axdd-person-client-1.1.5/uw_person_client/tests/test_core_client.py` & `axdd-person-client-1.1.6/uw_person_client/tests/test_core_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from unittest import TestCase
 from unittest.mock import patch, MagicMock
 from uw_person_client.exceptions import (
     AdviserNotFoundException, PersonNotFoundException)
 from uw_person_client.clients.core_client import UWPersonClient
 from uw_person_client.components import (
     Adviser, Employee, Major, Person, Sport, Student, Term, Transcript,
-    Transfer, Hold)
+    Transfer, Hold, Degree)
 from sqlalchemy.orm.exc import NoResultFound
 
 
 class UWPersonClientTest(TestCase):
 
     @patch('uw_person_client.clients.core_client.UWPDS')
     def get_mock_person_client(self, mock_uwpds):
@@ -688,14 +688,43 @@
         mock_dict = self._mock_to_dict(mock_hold)
         hold = client._map_hold(mock_hold)
 
         # assertions
         self.assertIsInstance(hold, Hold)
         self.assertDictContainsSubset(mock_dict, hold.to_dict())
 
+    @patch('uw_person_client.clients.core_client.UWPersonClient._map_term')
+    def test_map_degree(self, mock_map_term):
+        client = self.get_mock_person_client()
+        mock_degree = MagicMock()
+        mock_degree.degree_term = MagicMock()
+        mock_degree.campus_code = MagicMock()
+        mock_degree.degree_abbr_code = MagicMock()
+        mock_degree.degree_pathway_num = MagicMock()
+        mock_degree.degree_level_code = MagicMock()
+        mock_degree.degree_level_desc = MagicMock()
+        mock_degree.degree_type_code = MagicMock()
+        mock_degree.degree_level_type_desc = MagicMock()
+        mock_degree.degree_desc = MagicMock()
+        mock_degree.degree_uw_credits = MagicMock()
+        mock_degree.degree_transfer_credits = MagicMock()
+        mock_degree.degree_extension_credits = MagicMock()
+        mock_degree.degree_gpa = MagicMock()
+        mock_degree.fin_org_key = MagicMock()
+        mock_degree.primary_fin_org_key = MagicMock()
+
+        mock_dict = self._mock_to_dict(mock_degree)
+        degree = client._map_degree(mock_degree)
+
+        # assertions
+        self.assertIsInstance(degree, Degree)
+        self.assertEqual(mock_map_term.return_value, degree.degree_term)
+        del mock_dict['degree_term']
+        self.assertDictContainsSubset(mock_dict, degree.to_dict())
+
     def test_map_term(self):
         client = self.get_mock_person_client()
         mock_term = MagicMock()
         mock_term.year = MagicMock()
         mock_term.quarter = MagicMock()
 
         mock_dict = self._mock_to_dict(mock_term)
```

### Comparing `axdd-person-client-1.1.5/uw_person_client/tests/test_mock_client.py` & `axdd-person-client-1.1.6/uw_person_client/tests/test_mock_client.py`

 * *Files identical despite different names*

