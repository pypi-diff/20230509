# Comparing `tmp/yo-1.0.0.tar.gz` & `tmp/yo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yo-1.0.0.tar", last modified: Tue Apr 18 19:38:46 2023, max compression
+gzip compressed data, was "yo-1.0.1.tar", last modified: Tue May  9 18:33:19 2023, max compression
```

## Comparing `yo-1.0.0.tar` & `yo-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-04-18 19:38:46.940616 yo-1.0.0/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1848 2023-04-17 22:02:18.000000 yo-1.0.0/LICENSE.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3193 2023-04-18 19:38:46.940616 yo-1.0.0/PKG-INFO
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2598 2023-04-18 15:34:57.000000 yo-1.0.0/README.md
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   156525 2023-03-01 19:22:05.000000 yo-1.0.0/THIRD_PARTY_LICENSES.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      307 2023-04-18 19:38:46.940616 yo-1.0.0/setup.cfg
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3435 2023-04-18 19:36:34.000000 yo-1.0.0/setup.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-04-18 19:38:46.936616 yo-1.0.0/tests/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7971 2023-03-01 19:22:05.000000 yo-1.0.0/tests/test_api.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7350 2023-03-21 16:43:28.000000 yo-1.0.0/tests/test_cmds.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-04-18 19:38:46.936616 yo-1.0.0/yo/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        0 2023-01-25 21:25:24.000000 yo-1.0.0/yo/__init__.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1998 2023-03-01 19:22:05.000000 yo-1.0.0/yo/__main__.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)    67592 2023-03-23 20:42:24.000000 yo-1.0.0/yo/api.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-04-18 19:38:46.936616 yo-1.0.0/yo/data/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8092 2023-03-21 20:11:11.000000 yo-1.0.0/yo/data/sample.yo.ini
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-04-18 19:38:46.940616 yo-1.0.0/yo/data/yo-tasks/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2396 2023-03-01 19:22:05.000000 yo-1.0.0/yo/data/yo-tasks/drgn
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1956 2023-03-01 19:22:05.000000 yo-1.0.0/yo/data/yo-tasks/ocid
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2032 2023-03-01 19:22:05.000000 yo-1.0.0/yo/data/yo-tasks/test-deps
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       23 2023-01-25 21:25:24.000000 yo-1.0.0/yo/data/yo-tasks/test-existing-task
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1957 2023-03-01 19:22:05.000000 yo-1.0.0/yo/data/yo-tasks/test-run-many
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2008 2023-03-01 19:22:05.000000 yo-1.0.0/yo/data/yo-tasks/test-task
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1277 2023-03-23 17:58:33.000000 yo-1.0.0/yo/data/yo_tasklib.sh
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   107708 2023-03-23 19:04:59.000000 yo-1.0.0/yo/main.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     5886 2023-03-02 23:11:21.000000 yo-1.0.0/yo/oci.py
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8366 2023-03-23 18:16:50.000000 yo-1.0.0/yo/util.py
-drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-04-18 19:38:46.936616 yo-1.0.0/yo.egg-info/
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3193 2023-04-18 19:38:46.000000 yo-1.0.0/yo.egg-info/PKG-INFO
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      541 2023-04-18 19:38:46.000000 yo-1.0.0/yo.egg-info/SOURCES.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        1 2023-04-18 19:38:46.000000 yo-1.0.0/yo.egg-info/dependency_links.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       37 2023-04-18 19:38:46.000000 yo-1.0.0/yo.egg-info/entry_points.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       64 2023-04-18 19:38:46.000000 yo-1.0.0/yo.egg-info/requires.txt
--rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        3 2023-04-18 19:38:46.000000 yo-1.0.0/yo.egg-info/top_level.txt
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-05-09 18:33:19.289710 yo-1.0.1/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1848 2023-04-17 22:02:18.000000 yo-1.0.1/LICENSE.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-05-09 18:33:19.289710 yo-1.0.1/PKG-INFO
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2532 2023-05-09 18:31:11.000000 yo-1.0.1/README.md
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   156525 2023-03-01 19:22:05.000000 yo-1.0.1/THIRD_PARTY_LICENSES.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      307 2023-05-09 18:33:19.289710 yo-1.0.1/setup.cfg
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3427 2023-05-09 18:31:11.000000 yo-1.0.1/setup.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-05-09 18:33:19.285710 yo-1.0.1/tests/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7971 2023-03-01 19:22:05.000000 yo-1.0.1/tests/test_api.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     7350 2023-03-21 16:43:28.000000 yo-1.0.1/tests/test_cmds.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-05-09 18:33:19.285710 yo-1.0.1/yo/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        0 2023-01-25 21:25:24.000000 yo-1.0.1/yo/__init__.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1998 2023-03-01 19:22:05.000000 yo-1.0.1/yo/__main__.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)    67592 2023-03-23 20:42:24.000000 yo-1.0.1/yo/api.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-05-09 18:33:19.285710 yo-1.0.1/yo/data/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8092 2023-03-21 20:11:11.000000 yo-1.0.1/yo/data/sample.yo.ini
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-05-09 18:33:19.289710 yo-1.0.1/yo/data/yo-tasks/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2396 2023-03-01 19:22:05.000000 yo-1.0.1/yo/data/yo-tasks/drgn
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1956 2023-03-01 19:22:05.000000 yo-1.0.1/yo/data/yo-tasks/ocid
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2032 2023-03-01 19:22:05.000000 yo-1.0.1/yo/data/yo-tasks/test-deps
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       23 2023-01-25 21:25:24.000000 yo-1.0.1/yo/data/yo-tasks/test-existing-task
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1957 2023-03-01 19:22:05.000000 yo-1.0.1/yo/data/yo-tasks/test-run-many
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     2008 2023-03-01 19:22:05.000000 yo-1.0.1/yo/data/yo-tasks/test-task
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     1277 2023-03-23 17:58:33.000000 yo-1.0.1/yo/data/yo_tasklib.sh
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)   107744 2023-05-09 18:31:11.000000 yo-1.0.1/yo/main.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     5886 2023-03-02 23:11:21.000000 yo-1.0.1/yo/oci.py
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     8366 2023-03-23 18:16:50.000000 yo-1.0.1/yo/util.py
+drwxrwxr-x   0 stepbren  (1000) stepbren  (1000)        0 2023-05-09 18:33:19.285710 yo-1.0.1/yo.egg-info/
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)     3099 2023-05-09 18:33:19.000000 yo-1.0.1/yo.egg-info/PKG-INFO
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)      541 2023-05-09 18:33:19.000000 yo-1.0.1/yo.egg-info/SOURCES.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        1 2023-05-09 18:33:19.000000 yo-1.0.1/yo.egg-info/dependency_links.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       36 2023-05-09 18:33:19.000000 yo-1.0.1/yo.egg-info/entry_points.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)       64 2023-05-09 18:33:19.000000 yo-1.0.1/yo.egg-info/requires.txt
+-rw-rw-r--   0 stepbren  (1000) stepbren  (1000)        3 2023-05-09 18:33:19.000000 yo-1.0.1/yo.egg-info/top_level.txt
```

### Comparing `yo-1.0.0/LICENSE.txt` & `yo-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/PKG-INFO` & `yo-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: yo
-Version: 1.0.0
+Version: 1.0.1
 Summary: A fast and simple CLI client for managing OCI instances
-Home-page: https://github.com/oracle-samples/yo
+Home-page: https://github.com/oracle/yo
 Author: Oracle
 Author-email: stephen.s.brennan@oracle.com
 License: UPL
 Keywords: oci client
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Universal Permissive License (UPL)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: THIRD_PARTY_LICENSES.txt
@@ -36,24 +35,19 @@
 
 ## Installation
 
 A minimum of Python 3.6 is required in order to use Yo.
 
 **Via Pip:**
 
-Yo is not currently available on the Python Package Index. Check back soon!
+    pip install yo oci-cli
 
-**From Source:**
-
-Clone the repository, and then install with:
-
-    python setup.py install
-
-After installation, you'll need to configure Yo to work with your OCI tenancy.
-Please see the [documentation][] for detailed instructions.
+This will install the standard OCI CLI alongside Yo, which can be useful as
+well.  After installation, you'll need to configure Yo to work with your OCI
+tenancy.  Please see the [documentation][] for detailed instructions.
 
 ## Documentation
 
 The [documentation][] contains information on the configuration file, as well as
 a listing of sub-commands and features offered.
 
 ## Examples
@@ -94,12 +88,10 @@
 ## License
 
 Copyright (c) 2023 Oracle and/or its affiliates.
 
 Released under the Universal Permissive License v1.0 as shown at
 https://oss.oracle.com/licenses/upl/.
 
-[documentation]: https://oracle-samples.github.io/yo/
+[documentation]: https://oracle.github.io/yo/
 [contributing]: ./CONTRIBUTING.md
 [security]: ./SECURITY.md
-
-
```

### Comparing `yo-1.0.0/README.md` & `yo-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,24 +18,19 @@
 
 ## Installation
 
 A minimum of Python 3.6 is required in order to use Yo.
 
 **Via Pip:**
 
-Yo is not currently available on the Python Package Index. Check back soon!
+    pip install yo oci-cli
 
-**From Source:**
-
-Clone the repository, and then install with:
-
-    python setup.py install
-
-After installation, you'll need to configure Yo to work with your OCI tenancy.
-Please see the [documentation][] for detailed instructions.
+This will install the standard OCI CLI alongside Yo, which can be useful as
+well.  After installation, you'll need to configure Yo to work with your OCI
+tenancy.  Please see the [documentation][] for detailed instructions.
 
 ## Documentation
 
 The [documentation][] contains information on the configuration file, as well as
 a listing of sub-commands and features offered.
 
 ## Examples
@@ -76,10 +71,10 @@
 ## License
 
 Copyright (c) 2023 Oracle and/or its affiliates.
 
 Released under the Universal Permissive License v1.0 as shown at
 https://oss.oracle.com/licenses/upl/.
 
-[documentation]: https://oracle-samples.github.io/yo/
+[documentation]: https://oracle.github.io/yo/
 [contributing]: ./CONTRIBUTING.md
 [security]: ./SECURITY.md
```

### Comparing `yo-1.0.0/THIRD_PARTY_LICENSES.txt` & `yo-1.0.1/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/setup.py` & `yo-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from setuptools import find_packages
 from setuptools import setup
 
 long_description = open("README.md").read()
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 setup(
     name="yo",
     version=VERSION,
     description="A fast and simple CLI client for managing OCI instances",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -54,15 +54,15 @@
         # writing.
         "oci>=2.85.0",
         "subc>=0.7.0",
         "setuptools",
         "argcomplete",
         "dataclasses",
     ],
-    url="https://github.com/oracle-samples/yo",
+    url="https://github.com/oracle/yo",
     author="Oracle",
     author_email="stephen.s.brennan@oracle.com",
     license="UPL",
     packages=find_packages(include=["yo", "yo.*"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Universal Permissive License (UPL)",
```

### Comparing `yo-1.0.0/tests/test_api.py` & `yo-1.0.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/tests/test_cmds.py` & `yo-1.0.1/tests/test_cmds.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/yo/__main__.py` & `yo-1.0.1/yo/__main__.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/yo/api.py` & `yo-1.0.1/yo/api.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/yo/data/sample.yo.ini` & `yo-1.0.1/yo/data/sample.yo.ini`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/yo/data/yo-tasks/drgn` & `yo-1.0.1/yo/data/yo-tasks/drgn`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/yo/data/yo-tasks/ocid` & `yo-1.0.1/yo/data/yo-tasks/ocid`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/yo/data/yo-tasks/test-deps` & `yo-1.0.1/yo/data/yo-tasks/test-deps`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/yo/data/yo-tasks/test-run-many` & `yo-1.0.1/yo/data/yo-tasks/test-run-many`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/yo/data/yo-tasks/test-task` & `yo-1.0.1/yo/data/yo-tasks/test-task`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/yo/data/yo_tasklib.sh` & `yo-1.0.1/yo/data/yo_tasklib.sh`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/yo/main.py` & `yo-1.0.1/yo/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,19 +143,23 @@
     "-oLogLevel=ERROR",
     # The following two options are mostly useful for long-running serial
     # console connections. But they certainly don't harm things when you're
     # keeping SSH open for a while.
     "-oServerAliveInterval=60",
     "-oTCPKeepAlive=yes",
 ]
+SSH_CONSOLE_OPTIONS = [
+    "-oHostKeyAlgorithms +ssh-rsa",
+    "-oPubkeyAcceptedAlgorithms +ssh-rsa",
+]
 SSH_MINIMUM_TIME = 4
 
 # TODO: update with an external link
-REPOSITORY_URL = "https://github.com/oracle-samples/yo"
-DOCUMENTATION_URL = "https://oracle-samples.github.io/yo/"
+REPOSITORY_URL = "https://github.com/oracle/yo"
+DOCUMENTATION_URL = "https://oracle.github.io/yo/"
 INITIAL_CONFIG_LINK = REPOSITORY_URL
 
 warned_about_SSH_timeout = False
 
 PYVER = sys.version_info[:2]
 
 
@@ -1315,33 +1319,33 @@
         processed_args = []
         target = None
 
         for val in args:
             if val == "ssh":
                 continue  # strip the ssh command from the args
             elif identity is not None and "ProxyCommand" in val:
-                # We need to insert the "-i" for identity into the SSH proxy
-                # command. However, we shouldn't modify the rest of the
-                # arguments, because we really don't want to mess it up.
+                insert_args = f" -i {identity}"
+                for arg in SSH_CONSOLE_OPTIONS:
+                    insert_args += " " + shlex.quote(arg)
                 ssh_ix = val.index("ssh") + 3
-                val = val[:ssh_ix] + f" -i {identity}" + val[ssh_ix:]
+                val = val[:ssh_ix] + insert_args + val[ssh_ix:]
                 processed_args.append(val)
             elif inst.id in val:
                 target = val  # identify the target of the SSH
             else:
                 processed_args.append(val)  # pass all other args
 
         if target is None:
             self.c.con.print(args)
             raise YoExc(
                 "Could not understand OCI's console SSH string. This is a "
                 "yo bug, please report it on Github."
             )
 
-        cmd = ssh_cmd(self.c, target, processed_args)
+        cmd = ssh_cmd(self.c, target, SSH_CONSOLE_OPTIONS, processed_args)
 
         self.c.con.print("About to execute:")
         self.c.con.print(cmd)
         self.c.con.print(
             "[bold red]This connection will stay open for a long time.\n"
             "To exit a running SSH connection, use the escape sequence: "
             "<Return>~.\n"
```

### Comparing `yo-1.0.0/yo/oci.py` & `yo-1.0.1/yo/oci.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/yo/util.py` & `yo-1.0.1/yo/util.py`

 * *Files identical despite different names*

### Comparing `yo-1.0.0/yo.egg-info/PKG-INFO` & `yo-1.0.1/yo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: yo
-Version: 1.0.0
+Version: 1.0.1
 Summary: A fast and simple CLI client for managing OCI instances
-Home-page: https://github.com/oracle-samples/yo
+Home-page: https://github.com/oracle/yo
 Author: Oracle
 Author-email: stephen.s.brennan@oracle.com
 License: UPL
 Keywords: oci client
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Universal Permissive License (UPL)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: THIRD_PARTY_LICENSES.txt
@@ -36,24 +35,19 @@
 
 ## Installation
 
 A minimum of Python 3.6 is required in order to use Yo.
 
 **Via Pip:**
 
-Yo is not currently available on the Python Package Index. Check back soon!
+    pip install yo oci-cli
 
-**From Source:**
-
-Clone the repository, and then install with:
-
-    python setup.py install
-
-After installation, you'll need to configure Yo to work with your OCI tenancy.
-Please see the [documentation][] for detailed instructions.
+This will install the standard OCI CLI alongside Yo, which can be useful as
+well.  After installation, you'll need to configure Yo to work with your OCI
+tenancy.  Please see the [documentation][] for detailed instructions.
 
 ## Documentation
 
 The [documentation][] contains information on the configuration file, as well as
 a listing of sub-commands and features offered.
 
 ## Examples
@@ -94,12 +88,10 @@
 ## License
 
 Copyright (c) 2023 Oracle and/or its affiliates.
 
 Released under the Universal Permissive License v1.0 as shown at
 https://oss.oracle.com/licenses/upl/.
 
-[documentation]: https://oracle-samples.github.io/yo/
+[documentation]: https://oracle.github.io/yo/
 [contributing]: ./CONTRIBUTING.md
 [security]: ./SECURITY.md
-
-
```

### Comparing `yo-1.0.0/yo.egg-info/SOURCES.txt` & `yo-1.0.1/yo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

