# Comparing `tmp/docassemble.MassAppealsCourt-0.1.0.tar.gz` & `tmp/docassemble.MassAppealsCourt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.MassAppealsCourt-0.1.0.tar", last modified: Fri Jun  3 19:57:01 2022, max compression
+gzip compressed data, was "docassemble.MassAppealsCourt-0.2.1.tar", last modified: Tue May  9 14:46:04 2023, max compression
```

## Comparing `docassemble.MassAppealsCourt-0.1.0.tar` & `docassemble.MassAppealsCourt-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:57:01.947116 docassemble.MassAppealsCourt-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-06-03 19:56:45.000000 docassemble.MassAppealsCourt-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-03 19:56:45.000000 docassemble.MassAppealsCourt-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-06-03 19:57:01.947116 docassemble.MassAppealsCourt-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-06-03 19:56:45.000000 docassemble.MassAppealsCourt-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:57:01.947116 docassemble.MassAppealsCourt-0.1.0/docassemble/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:57:01.947116 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-03 19:56:45.000000 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:57:01.943116 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:57:01.947116 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/data/questions/
--rw-r--r--   0 runner    (1001) docker     (121)     9655 2022-06-03 19:56:45.000000 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/data/questions/appeals-basic-questions.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:57:01.947116 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/data/sources/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-06-03 19:56:45.000000 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/data/sources/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:57:01.947116 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/data/static/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-03 19:56:45.000000 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/data/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:57:01.947116 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/data/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-06-03 19:56:45.000000 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/data/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    12092 2022-06-03 19:56:45.000000 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/data/templates/appeals_cover_sheet.docx
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-06-03 19:56:45.000000 docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/ma_appeals_specific_logic.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-06-03 19:56:45.000000 docassemble.MassAppealsCourt-0.1.0/docassemble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:57:01.947116 docassemble.MassAppealsCourt-0.1.0/docassemble.MassAppealsCourt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-06-03 19:57:01.000000 docassemble.MassAppealsCourt-0.1.0/docassemble.MassAppealsCourt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-06-03 19:57:01.000000 docassemble.MassAppealsCourt-0.1.0/docassemble.MassAppealsCourt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 19:57:01.000000 docassemble.MassAppealsCourt-0.1.0/docassemble.MassAppealsCourt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-03 19:57:01.000000 docassemble.MassAppealsCourt-0.1.0/docassemble.MassAppealsCourt.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 19:56:59.000000 docassemble.MassAppealsCourt-0.1.0/docassemble.MassAppealsCourt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-03 19:57:01.000000 docassemble.MassAppealsCourt-0.1.0/docassemble.MassAppealsCourt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-03 19:57:01.000000 docassemble.MassAppealsCourt-0.1.0/docassemble.MassAppealsCourt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-03 19:57:01.947116 docassemble.MassAppealsCourt-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-06-03 19:56:45.000000 docassemble.MassAppealsCourt-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:46:04.063219 docassemble.MassAppealsCourt-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      402 2023-05-09 14:46:04.063219 docassemble.MassAppealsCourt-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:46:04.059219 docassemble.MassAppealsCourt-0.2.1/docassemble/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:46:04.059219 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:46:04.059219 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:46:04.059219 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/questions/
+-rw-r--r--   0 runner    (1001) docker     (122)     8251 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/questions/appeals-basic-questions.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2217 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/questions/efiling.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:46:04.063219 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/sources/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:46:04.063219 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:46:04.063219 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    12092 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/templates/appeals_cover_sheet.docx
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/ma_appeals_specific_logic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/docassemble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:46:04.059219 docassemble.MassAppealsCourt-0.2.1/docassemble.MassAppealsCourt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      402 2023-05-09 14:46:04.000000 docassemble.MassAppealsCourt-0.2.1/docassemble.MassAppealsCourt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      896 2023-05-09 14:46:04.000000 docassemble.MassAppealsCourt-0.2.1/docassemble.MassAppealsCourt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 14:46:04.000000 docassemble.MassAppealsCourt-0.2.1/docassemble.MassAppealsCourt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-09 14:46:04.000000 docassemble.MassAppealsCourt-0.2.1/docassemble.MassAppealsCourt.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 14:46:03.000000 docassemble.MassAppealsCourt-0.2.1/docassemble.MassAppealsCourt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-09 14:46:04.000000 docassemble.MassAppealsCourt-0.2.1/docassemble.MassAppealsCourt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-09 14:46:04.000000 docassemble.MassAppealsCourt-0.2.1/docassemble.MassAppealsCourt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-09 14:46:04.063219 docassemble.MassAppealsCourt-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-05-09 14:45:55.000000 docassemble.MassAppealsCourt-0.2.1/setup.py
```

### Comparing `docassemble.MassAppealsCourt-0.1.0/LICENSE` & `docassemble.MassAppealsCourt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/data/questions/appeals-basic-questions.yml` & `docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/questions/appeals-basic-questions.yml`

 * *Files 14% similar despite different names*

```diff
@@ -84,63 +84,23 @@
   If you do not hear from the court in 1 business day, call the Appeals Court 
   Clerk's Office:  
   617-921-4443 
   Monday-Friday  
   8:30am - 4:30pm
   
   % else:
-  Something went wrong delivering your form to the ${courts[0]}.  
-  Try again later or call the Appeals Court Clerk's Office:  
+  Something went wrong delivering your form to the ${courts[0]}.
+  Try again later or call the Appeals Court Clerk's Office:
   617-921-4443 
   Monday-Friday  
   8:30am - 4:30pm
   % endif
 continue button field: email_status
 continue button label: Back to download screen
 ---
-id: appeals user address
-question: |
-  What is your address?
-subquestion: |
-  List the address where you want the court to mail papers to you.
-fields:
-  - Email address: users[0].email    
-    datatype: email
-    required: False
-  - Street address: users[0].address.address
-    address autocomplete: True
-  - Unit: users[0].address.unit
-    required: False
-  - City: users[0].address.city
-  - State: users[0].address.state
-    code: states_list()
-  - Zip: users[0].address.zip 
----
-id: contact information
-question: |
-  Contact information
-subquestion: |
-  Provide at least one other way for the court to reach you. 
-fields:
-  - Mobile number: users[0].mobile_number
-    required: False
-  - Other phone number: users[0].phone_number
-    required: False
-  - Other ways to reach you: users[0].other_contact_method
-    input type: area
-    required: False
-    help: |
-      If you do not have a phone number or email the court can use, provide specific contact instructions. For example, use a friend's phone number.
-      But the friend must be someone you can rely on to tell you the court is trying to reach you.
-validation code: |
-  if (not showifdef('users[0].phone_number')) and \
-      (not showifdef('users[0].mobile_number')) and \
-      (not showifdef('users[0].other_contact_method')):
-    validation_error(word("You need to provide at least one other contact method."))
----
 code: |
   all_final_forms_combined = al_final_form_to_file.as_pdf(key='final')
 ---
 need:
   - comments_to_clerk
   - package_version_number
 id: ready to email
@@ -214,27 +174,28 @@
 id: Appeals send to court
 comment: |
   Send to court code--tweaked slightly for MAC
 need:
   - email_to_court_template
   - court_email
   - should_cc_user
+  - al_final_form_to_file
 code: |
   if will_send_to_real_court():
     email_to_use = court_email
   else:
     email_to_use = dev_email_to_use
   
   if task_not_yet_performed('send email'):
     log("Court email is ".format(court_email))
     email_success = False
     if should_cc_user:
       log('Sending email to {} and ccing {} for {}'.format(email_to_use, cc_email, str(users)))
       email_success = send_email(to=email_to_use, template=email_to_court_template, task='send email', 
-                                 cc=cc_email, attachments=al_final_form_to_file.as_pdf_list(key='final')) # True # until we're ready to turn this on
+                                 cc=cc_email, attachments=al_final_form_to_file.as_pdf_list(key='final'))
     else:
       log('Sending email to {} and no cc for {}'.format(email_to_use, str(users)))
       email_success = send_email(to=email_to_use, template=email_to_court_template, task='send email', 
                                  attachments=al_final_form_to_file.as_pdf_list(key='final'))
     mark_task_as_performed('send email')
   sent_email_to_court = True
 ---
```

### Comparing `docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/data/templates/appeals_cover_sheet.docx` & `docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/data/templates/appeals_cover_sheet.docx`

 * *Files identical despite different names*

### Comparing `docassemble.MassAppealsCourt-0.1.0/docassemble/MassAppealsCourt/ma_appeals_specific_logic.py` & `docassemble.MassAppealsCourt-0.2.1/docassemble/MassAppealsCourt/ma_appeals_specific_logic.py`

 * *Files identical despite different names*

### Comparing `docassemble.MassAppealsCourt-0.1.0/docassemble.MassAppealsCourt.egg-info/SOURCES.txt` & `docassemble.MassAppealsCourt-0.2.1/docassemble.MassAppealsCourt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,11 +10,12 @@
 docassemble.MassAppealsCourt.egg-info/namespace_packages.txt
 docassemble.MassAppealsCourt.egg-info/not-zip-safe
 docassemble.MassAppealsCourt.egg-info/requires.txt
 docassemble.MassAppealsCourt.egg-info/top_level.txt
 docassemble/MassAppealsCourt/__init__.py
 docassemble/MassAppealsCourt/ma_appeals_specific_logic.py
 docassemble/MassAppealsCourt/data/questions/appeals-basic-questions.yml
+docassemble/MassAppealsCourt/data/questions/efiling.yml
 docassemble/MassAppealsCourt/data/sources/README.md
 docassemble/MassAppealsCourt/data/static/README.md
 docassemble/MassAppealsCourt/data/templates/README.md
 docassemble/MassAppealsCourt/data/templates/appeals_cover_sheet.docx
```

### Comparing `docassemble.MassAppealsCourt-0.1.0/setup.py` & `docassemble.MassAppealsCourt-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.MassAppealsCourt',
-      version='0.1.0',
+      version='0.2.1',
       description=('A docassemble extension.'),
       long_description='# docassemble.MassAppealsCourt\r\n\r\nA docassemble extension.\r\n\r\n## Author\r\n\r\nSystem Administrator, admin@admin.com\r\n\r\n',
       long_description_content_type='text/markdown',
       author='System Administrator',
       author_email='admin@admin.com',
       license='The MIT License (MIT)',
       url='https://docassemble.org',
```

