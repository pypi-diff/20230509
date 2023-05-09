# Comparing `tmp/fsst-0.8.0.tar.gz` & `tmp/fsst-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsst-0.8.0.tar", last modified: Tue Apr 18 10:27:03 2023, max compression
+gzip compressed data, was "fsst-0.8.1.tar", last modified: Tue May  9 19:41:43 2023, max compression
```

## Comparing `fsst-0.8.0.tar` & `fsst-0.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-18 10:27:03.930779 fsst-0.8.0/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-04-18 10:27:03.930779 fsst-0.8.0/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.0/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-18 10:27:03.930779 fsst-0.8.0/fsst.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-04-18 10:27:03.000000 fsst-0.8.0/fsst.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-04-18 10:27:03.000000 fsst-0.8.0/fsst.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-04-18 10:27:03.000000 fsst-0.8.0/fsst.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-04-18 10:27:03.000000 fsst-0.8.0/fsst.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.0/fsst.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       80 2023-04-18 10:27:03.000000 fsst-0.8.0/fsst.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-04-18 10:27:03.000000 fsst-0.8.0/fsst.egg-info/top_level.txt
--rwxrwxr-x   0 rob       (1000) rob       (1000)   109707 2023-04-18 10:25:13.000000 fsst-0.8.0/fsst.py
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-04-18 10:27:03.930779 fsst-0.8.0/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)     1162 2023-04-18 10:26:12.000000 fsst-0.8.0/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 19:41:43.267390 fsst-0.8.1/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 19:41:43.267390 fsst-0.8.1/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.1/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 19:41:43.267390 fsst-0.8.1/fsst.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 19:41:42.000000 fsst-0.8.1/fsst.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-09 19:41:43.000000 fsst-0.8.1/fsst.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-09 19:41:42.000000 fsst-0.8.1/fsst.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-09 19:41:42.000000 fsst-0.8.1/fsst.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.1/fsst.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       80 2023-05-09 19:41:43.000000 fsst-0.8.1/fsst.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-09 19:41:43.000000 fsst-0.8.1/fsst.egg-info/top_level.txt
+-rwxrwxr-x   0 rob       (1000) rob       (1000)   116353 2023-05-09 19:40:45.000000 fsst-0.8.1/fsst.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-09 19:41:43.267390 fsst-0.8.1/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1162 2023-05-09 19:40:12.000000 fsst-0.8.1/setup.py
```

### Comparing `fsst-0.8.0/PKG-INFO` & `fsst-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.0
+Version: 0.8.1
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.0/README.md` & `fsst-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `fsst-0.8.0/fsst.egg-info/PKG-INFO` & `fsst-0.8.1/fsst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.0
+Version: 0.8.1
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.0/fsst.py` & `fsst-0.8.1/fsst.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import argparse
 import json
 import time
 import asyncio
 import itertools
 import importlib.util
 import requests
-VERSION = "0.8.0"
+VERSION = "0.8.1"
 CRYPTO_OK = True
 DOCKER_OK = True
 try:
     import aioflureedb
 except ModuleNotFoundError:
     print("WARNING: - aioflureedb python lib not found.")
     CRYPTO_OK = False
@@ -104,14 +104,81 @@
                "33b7299d3ebe5590aba6618f2369911faf98fb0853a85d6d4cdeae0a951fae9e"],
     "auth30": ["TfC9jrDs1PbXJtY5iJQCGSszs88xFBgZyKW",
                "09e65ff02f2e78379d753681ae37ca3964e72ec97765eb63e6b0b10533d34d26"],
     "auth31": ["Tf8JAdpa3MASMLdWtcTvayHKdWBngZcWW88",
                "7881f421654c8ca1ff085b57a5ce8cd230894a30c66432e19c68f6a96d22add9"]
 }
 
+def wait_for_flureedb_to_terminate():
+    """In a multi run, wait for flureedb to terminate between runs"""
+    found = True
+    print("Waiting fof FlureeDB to terminate")
+    while found: # pylint: disable=while-used
+        found = False
+        for procdir in [os.path.join("/proc",x) for x in os.listdir("/proc") if x.isnumeric()]:
+            cmdpath = os.path.join(procdir,"cmdline")
+            try:
+                with open(cmdpath,"rb") as cmdfil:
+                    data = cmdfil.read()
+                    if b"-Dfdb." in data:
+                        found = True
+            except: # pylint: disable=bare-except
+                pass
+        if found:
+            print("- waiting")
+            time.sleep(5)
+        else:
+            print("-terminated")
+
+class Hooks:
+    """Helper class for running hooks between runs"""
+    def __init__(self):
+        self.hookmodule = None
+        self.hook = None
+        is_ok = False
+        hookmodpath = os.path.join("hooks", "hooks.py")
+        if os.path.exists(hookmodpath):
+            try:
+                hookspec = importlib.util.spec_from_file_location("hooks", hookmodpath)
+                self.hookmodule= importlib.util.module_from_spec(hookspec)
+                hookspec.loader.exec_module(self.hookmodule)
+                is_ok = True
+            except: # pylint: disable=bare-except
+                print("Problem imorting hooks: ", hookmodpath)
+                self.hookmodule = None
+            if is_ok:
+                self.hooks = getattr(self.hooksmodule, "Hooks", None)
+                if self.hooks is None:
+                    print("ERROR: No Hooks in hooks file")
+                    is_ok = False
+            if is_ok:
+                for method in ("before", "between", "after"):
+                    if getattr(self.hook, method, None) is None:
+                        print("ERROR: missing hook: ", method)
+                        is_ok = False
+            if not is_ok:
+                self.hook = None
+                self.hookmodule = None
+        else:
+            print("WARNING: No hooks file found: ", hookmodpath)
+
+    def before(self):
+        """Before hook"""
+        if self.hook:
+            self.hook.before()
+
+    def between(self):
+        """In between hook"""
+        if self.hook:
+            self.hook.between()
+
+    def after(self):
+        """After hook"""
+        if self.hook:
+            self.hook.after()
 
 class FlushFile:
     """Helper class for file like objects to always flush on write"""
     def __init__(self, file_descriptor):
         """Constructor
          Parameters
          ----------
@@ -960,15 +1027,15 @@
                                     print("     ERROR : Exception in prepare of test no",
                                           test_index)
                                     raise ex
                                 if isinstance(is_ok, bool):
                                     if not is_ok:
                                         raise RuntimeError("The prepare failed for test at index "
                                                            + str(test_index))
-                                elif not is_ok[0]:
+                                elif not is_ok[0]: # pylint: disable=confusing-consecutive-elif
                                     raise RuntimeError("The prepare_user failed for test at index " +
                                                        str(test_index) + " : " + str(is_ok[1]))
                             for subtest in current_test["sub_tests"]:
                                 subtest_name = subtest[0]
                                 should_succeed = subtest[1]
                                 warn_only = subtest[2]
                                 methods = []
@@ -1124,15 +1191,16 @@
             # Run all test scenarios.
             for scenario in testscenarios:
                 await run_test_scenario(database, subdir, fluree_parts, fdb, scenario)
             print(" -", len(testscenarios), "tests completed")
 
 
 async def fluree_main(notest, network, host, port, output, createkey,
-                      target, fluree_parts, verboseerrors, api="apimap", stages="ALL"):
+                      target, fluree_parts, verboseerrors, api="apimap", stages="ALL",
+                      runs=1, hooks=False, fluree_process=None, verbosefluree=False):
     # pylint: disable=too-many-branches, too-many-statements, fixme
     # TODO: We may want to dismantle this function and refactor. Below is a remnant
     #       of the 0.1 version of fsst that didn't yet use subcommands.
     """The tools main function
 
     Parameters
     ----------
@@ -1151,15 +1219,15 @@
     target:
         The build target name to use.
     fluree_parts: string
         Fluree build sources top dir directory path
     verboseerrors: boolean
         Add extra error strings to rules if undefined.
     """
-    # pylint: disable=too-many-locals,too-many-arguments
+    # pylint: disable=too-many-locals,too-many-arguments, too-many-nested-blocks
     maxblock = [expand_operation({
         "_id": "_fn$lastblock",
         "name": "lastBlock",
         "doc": "Get the number of the last known block on the ledger",
         "code_from_query": {
             "select": "?maxBlock",
             "where": [
@@ -1172,15 +1240,15 @@
     allstages = False
     teststages = set()
     if stages == "ALL":
         allstages = True
     else:
         teststages = set(stages.split(","))
     print("DEBUG:", allstages, list(teststages))
-    try:
+    try: # pylint: disable=too-many-try-statements
         expanded = []
         expanded.append(maxblock)
         # Build.json contains the different build targets and lists their components.
         # Fetch the specified target from this file.
         try:
             with open(os.path.join(fluree_parts, "build.json")) as buildfile:
                 build = json.load(buildfile)
@@ -1189,300 +1257,314 @@
                 else:
                     print("ERROR: No target '" + target + "' in build.json")
                     sys.exit(2)
         except FileNotFoundError:
             print("ERROR: No build.json in", fluree_parts, "dir.")
             print("       Use --dir option to specify alternative build dir")
             return
-        maxstage = 0
-        # Outer loop for finding out where and how far to run the inner loop.
-        # pylint: disable=too-many-nested-blocks
-        testcount = 0
-        for subdir in build:
-            if output or notest:
-                # If output or notest, we dont run any tests, we just fill the expanded list
-                #  with expanded transactions.
-                main = os.path.join(fluree_parts, subdir, "main.json")
-                noexpand = os.path.join(fluree_parts, subdir + ".json")
-                if os.path.isfile(noexpand):
-                    with open(noexpand) as nefile:
-                        nelist = json.load(nefile)
-                    for transaction in nelist:
-                        out_transaction = []
-                        for operation in transaction:
-                            if (verboseerrors and "_id" in operation and "id" in operation
-                                    and operation["_id"].startswith("_rule")
-                                    and "errorMessage" not in operation):
-                                print("Adding verbose error for", operation["id"])
-                                operation["errorMessage"] = "Verbose Errors: " + operation["id"]
-                            out_transaction.append(operation)
-                        expanded.append(out_transaction)
+        hooks = Hooks()
+        hooks.before()
+        for run in range(0, runs):
+            if run > 1 and fluree_process is not None:
+                fluree_process.terminate()
+                wait_for_flureedb_to_terminate()
+                hooks.between()
+                command = ["/bin/bash", "/usr/src/fsst/fluree_start.sh", "-Dfdb-api-port=8090"]
+                if not verbosefluree:
+                    # pylint: disable=consider-using-with
+                    fluree_process = subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
                 else:
-                    with open(main) as mainfile:
-                        mainlist = json.load(mainfile)
-                    for entry in mainlist:
-                        expanded.append(expand_transaction(entry,
-                                                           subdir,
-                                                           fluree_parts,
-                                                           verboseerrors))
-            else:
-                # Otherwise, if notest is false and the stage has a test.json,
-                #  we run our inner loop for testing
-                testfile = os.path.join(fluree_parts, subdir, "test.json")
-                if os.path.isfile(testfile) and not notest and (allstages or subdir in teststages):
-                    testcount += 1
-                    # Make up a database name for our test, using network and stage name.
-                    database = network + "/" + subdir
-                    database = "-".join(database.lower().split("_"))
-                    expanded2 = []
-                    expanded2.append(maxblock)
-                    print("- Database:", database)
-                    print(" - collecting transactions from build subdirs")
-                    # Run the test with transactions from all stages up to this one.
-                    print("Going through first", maxstage+1, "stages")
-                    for subdir2 in build[:maxstage+1]:
-                        print("  -", subdir2)
-                        main = os.path.join(fluree_parts, subdir2, "main.json")
-                        noexpand = os.path.join(fluree_parts, subdir2 + ".json")
-                        if os.path.isfile(noexpand):
-                            with open(noexpand) as nefile:
-                                nelist = json.load(nefile)
-                            for transaction in nelist:
-                                transaction_out = []
-                                for operation in transaction:
-                                    if (verboseerrors and "_id" in operation and "id" in operation
-                                            and operation["_id"].startswith("_rule")
-                                            and "errorMessage" not in operation):
-                                        print("       + Adding verbose error for", operation["id"])
-                                        operation["errorMessage"] = "Verbose Errors: " + \
-                                                                    operation["id"]
-                                    transaction_out.append(operation)
-                                expanded2.append(transaction_out)
-                        else:
-                            with open(main) as mainfile:
-                                mainlist = json.load(mainfile)
-                            for entry in mainlist:
-                                expanded2.append(expand_transaction(entry,
-                                                                    subdir2,
-                                                                    fluree_parts,
-                                                                    verboseerrors))
-                    # Run all test scenarios for this stage
-                    if allstages or build[maxstage] in teststages:
-                        print("Running smartfunction_test")
-                        await smartfunction_test(host,
-                                                 port,
-                                                 database,
-                                                 createkey,
-                                                 build[maxstage],
-                                                 expanded2,
-                                                 fluree_parts)
+                    # pylint: disable=consider-using-with
+                    fluree_process = subprocess.Popen(command)
+            maxstage = 0
+            # Outer loop for finding out where and how far to run the inner loop.
+            # pylint: disable=too-many-nested-blocks
+            testcount = 0
+            for subdir in build:
+                if output or notest:
+                    # If output or notest, we dont run any tests, we just fill the expanded list
+                    #  with expanded transactions.
+                    main = os.path.join(fluree_parts, subdir, "main.json")
+                    noexpand = os.path.join(fluree_parts, subdir + ".json")
+                    if os.path.isfile(noexpand):
+                        with open(noexpand) as nefile:
+                            nelist = json.load(nefile)
+                        for transaction in nelist:
+                            out_transaction = []
+                            for operation in transaction:
+                                if (verboseerrors and "_id" in operation and "id" in operation
+                                        and operation["_id"].startswith("_rule")
+                                        and "errorMessage" not in operation):
+                                    print("Adding verbose error for", operation["id"])
+                                    operation["errorMessage"] = "Verbose Errors: " + operation["id"]
+                                out_transaction.append(operation)
+                            expanded.append(out_transaction)
                     else:
-                        print("Skipping tests for", build[maxstage])
-                # If notest is false and the stage has a domain.json,
-                #  we run domain-API tests
-                testfile = os.path.join(fluree_parts, subdir, "domain.json")
-                if os.path.isfile(testfile) and not notest and (allstages or subdir in teststages):
-                    expanded2 = []
-                    expanded2.append(maxblock)
-                    # Make up a database name for our test, using network and stage name.
-                    database = network + "/api_" + subdir
-                    database = "-".join(database.lower().split("_"))
-                    print("- Database:", database)
-                    print(" - collecting transactions from build subdirs")
-                    # Run the test with transactions from all stages up to this one.
-                    print("Going through first", maxstage+1, "stages")
-                    for subdir2 in build[:maxstage+1]:
-                        print("  -", subdir2)
-                        main = os.path.join(fluree_parts, subdir2, "main.json")
-                        noexpand = os.path.join(fluree_parts, subdir2 + ".json")
-                        if os.path.isfile(noexpand):
-                            with open(noexpand) as nefile:
-                                nelist = json.load(nefile)
-                            for transaction in nelist:
-                                transaction_out = []
-                                for operation in transaction:
-                                    if (verboseerrors and "_id" in operation and "id" in operation
-                                            and operation["_id"].startswith("_rule")
-                                            and "errorMessage" not in operation):
-                                        print("       + Adding verbose error for", operation["id"])
-                                        operation["errorMessage"] = "Verbose Errors: " + \
-                                                                    operation["id"]
-                                    transaction_out.append(operation)
-                                expanded2.append(transaction_out)
+                        with open(main) as mainfile:
+                            mainlist = json.load(mainfile)
+                        for entry in mainlist:
+                            expanded.append(expand_transaction(entry,
+                                                               subdir,
+                                                               fluree_parts,
+                                                               verboseerrors))
+                else:
+                    # Otherwise, if notest is false and the stage has a test.json,
+                    #  we run our inner loop for testing
+                    testfile = os.path.join(fluree_parts, subdir, "test.json")
+                    if os.path.isfile(testfile) and not notest and (allstages or subdir in teststages):
+                        testcount += 1
+                        # Make up a database name for our test, using network and stage name.
+                        database = network + "/" + subdir
+                        database = "-".join(database.lower().split("_"))
+                        expanded2 = []
+                        expanded2.append(maxblock)
+                        print("- Database:", database)
+                        print(" - collecting transactions from build subdirs")
+                        # Run the test with transactions from all stages up to this one.
+                        print("Going through first", maxstage+1, "stages")
+                        for subdir2 in build[:maxstage+1]:
+                            print("  -", subdir2)
+                            main = os.path.join(fluree_parts, subdir2, "main.json")
+                            noexpand = os.path.join(fluree_parts, subdir2 + ".json")
+                            if os.path.isfile(noexpand):
+                                with open(noexpand) as nefile:
+                                    nelist = json.load(nefile)
+                                for transaction in nelist:
+                                    transaction_out = []
+                                    for operation in transaction:
+                                        if (verboseerrors and "_id" in operation and "id" in operation
+                                                and operation["_id"].startswith("_rule")
+                                                and "errorMessage" not in operation):
+                                            print("       + Adding verbose error for", operation["id"])
+                                            operation["errorMessage"] = "Verbose Errors: " + \
+                                                                        operation["id"]
+                                        transaction_out.append(operation)
+                                    expanded2.append(transaction_out)
+                            else:
+                                with open(main) as mainfile:
+                                    mainlist = json.load(mainfile)
+                                for entry in mainlist:
+                                    expanded2.append(expand_transaction(entry,
+                                                                        subdir2,
+                                                                        fluree_parts,
+                                                                        verboseerrors))
+                        # Run all test scenarios for this stage
+                        if allstages or build[maxstage] in teststages:
+                            print("Running smartfunction_test")
+                            await smartfunction_test(host,
+                                                     port,
+                                                     database,
+                                                     createkey,
+                                                     build[maxstage],
+                                                     expanded2,
+                                                     fluree_parts)
                         else:
-                            with open(main) as mainfile:
-                                mainlist = json.load(mainfile)
-                            for entry in mainlist:
-                                expanded2.append(expand_transaction(entry,
-                                                                    subdir2,
-                                                                    fluree_parts,
-                                                                    verboseerrors))
-                    with open(testfile) as testfil:
-                        testsets = json.load(testfil)
-                    if (os.path.isdir(api) and
-                            os.path.isdir(os.path.join(api, "fsst")) and
-                            os.path.isdir(os.path.join(api, "roles")) and
-                            os.path.isdir(os.path.join(api, "fsst", "tests"))):
-                        apimap_modules = {}
-                        for modname in [fil[:-3] for fil in os.listdir(os.path.join(api,
-                                                                                    "fsst",
-                                                                                    "tests")) if
-                                        fil[-3:] == ".py"]:
-                            modpath = os.path.join(api, "fsst", "tests", modname + ".py")
-                            spec = importlib.util.spec_from_file_location(modname, modpath)
-                            apimap_modules[modname] = importlib.util.module_from_spec(spec)
-                            spec.loader.exec_module(apimap_modules[modname])
-                            if getattr(apimap_modules[modname], 'DomainApiTest', None) is None:
-                                del apimap_modules[modname]
+                            print("Skipping tests for", build[maxstage])
+                    # If notest is false and the stage has a domain.json,
+                    #  we run domain-API tests
+                    testfile = os.path.join(fluree_parts, subdir, "domain.json")
+                    if os.path.isfile(testfile) and not notest and (allstages or subdir in teststages):
+                        expanded2 = []
+                        expanded2.append(maxblock)
+                        # Make up a database name for our test, using network and stage name.
+                        database = network + "/api_" + subdir
+                        database = "-".join(database.lower().split("_"))
+                        print("- Database:", database)
+                        print(" - collecting transactions from build subdirs")
+                        # Run the test with transactions from all stages up to this one.
+                        print("Going through first", maxstage+1, "stages")
+                        for subdir2 in build[:maxstage+1]:
+                            print("  -", subdir2)
+                            main = os.path.join(fluree_parts, subdir2, "main.json")
+                            noexpand = os.path.join(fluree_parts, subdir2 + ".json")
+                            if os.path.isfile(noexpand):
+                                with open(noexpand) as nefile:
+                                    nelist = json.load(nefile)
+                                for transaction in nelist:
+                                    transaction_out = []
+                                    for operation in transaction:
+                                        if (verboseerrors and "_id" in operation and "id" in operation
+                                                and operation["_id"].startswith("_rule")
+                                                and "errorMessage" not in operation):
+                                            print("       + Adding verbose error for", operation["id"])
+                                            operation["errorMessage"] = "Verbose Errors: " + \
+                                                                        operation["id"]
+                                        transaction_out.append(operation)
+                                    expanded2.append(transaction_out)
                             else:
-                                print("NOTICE: Loaded Domain-API testing module", modname)
-                        full_coverage = {}
-                        for role in [fil[:-5] for fil in os.listdir(os.path.join(api, "roles")) if
-                                     fil[-5:] == ".json"]:
-                            full_coverage[role] = set()
-                            with open(os.path.join(api, "roles", role + ".json")) as rolefile:
-                                role_data = json.load(rolefile)
-                            for key in role_data.keys():
-                                for val in role_data[key]:
-                                    full_coverage[role].add(val)
-                        test_list = []
-                        for test in testsets:
-                            if "api_role" in test:
-                                role = test["api_role"]
-                                test_name = role
-                                if "test" in test:
-                                    test_name = test["test"]
-                                if role in full_coverage:
-                                    role_all = full_coverage[role]
-                                    auth = "$auth00"
-                                    auth_prepare = "$auth31"
-                                    if "auth" in test:
-                                        auth = test["auth"]
-                                    if "auth_prepare" in test:
-                                        auth_prepare = test["auth_prepare"]
-                                    if auth[0] != "$":
+                                with open(main) as mainfile:
+                                    mainlist = json.load(mainfile)
+                                for entry in mainlist:
+                                    expanded2.append(expand_transaction(entry,
+                                                                        subdir2,
+                                                                        fluree_parts,
+                                                                        verboseerrors))
+                        with open(testfile) as testfil:
+                            testsets = json.load(testfil)
+                        if (os.path.isdir(api) and
+                                os.path.isdir(os.path.join(api, "fsst")) and
+                                os.path.isdir(os.path.join(api, "roles")) and
+                                os.path.isdir(os.path.join(api, "fsst", "tests"))):
+                            apimap_modules = {}
+                            for modname in [fil[:-3] for fil in os.listdir(os.path.join(api,
+                                                                                        "fsst",
+                                                                                        "tests")) if
+                                            fil[-3:] == ".py"]:
+                                modpath = os.path.join(api, "fsst", "tests", modname + ".py")
+                                spec = importlib.util.spec_from_file_location(modname, modpath)
+                                apimap_modules[modname] = importlib.util.module_from_spec(spec)
+                                spec.loader.exec_module(apimap_modules[modname])
+                                if getattr(apimap_modules[modname], 'DomainApiTest', None) is None:
+                                    del apimap_modules[modname]
+                                else:
+                                    print("NOTICE: Loaded Domain-API testing module", modname)
+                            full_coverage = {}
+                            for role in [fil[:-5] for fil in os.listdir(os.path.join(api, "roles")) if
+                                         fil[-5:] == ".json"]:
+                                full_coverage[role] = set()
+                                with open(os.path.join(api, "roles", role + ".json")) as rolefile:
+                                    role_data = json.load(rolefile)
+                                for key in role_data.keys():
+                                    for val in role_data[key]:
+                                        full_coverage[role].add(val)
+                            test_list = []
+                            for test in testsets:
+                                if "api_role" in test:
+                                    role = test["api_role"]
+                                    test_name = role
+                                    if "test" in test:
+                                        test_name = test["test"]
+                                    if role in full_coverage:
+                                        role_all = full_coverage[role]
                                         auth = "$auth00"
-                                    if auth_prepare[0] != "$":
                                         auth_prepare = "$auth31"
-                                    if auth[1:] in AUTHMAP:
-                                        auth_info = AUTHMAP[auth[1:]]
-                                        user = auth[1:]
-                                    else:
-                                        auth_info = AUTHMAP["auth00"]
-                                        user = "auth00"
-                                    if auth_prepare[1:] in AUTHMAP:
-                                        auth_info_prepare = AUTHMAP[auth_prepare[1:]]
-                                        user_prepare = auth_prepare[1:]
-                                    else:
-                                        auth_info_prepare = AUTHMAP["auth31"]
-                                        user_prepare = "auth31"
-                                    if "user" in test:
-                                        user = test["user"]
-                                    if "user_prepare" in test:
-                                        user_prepare = test["user_prepare"]
-                                    auth_roles = set()
-                                    auth_roles_prepare = set()
-                                    if "auth_roles" in test:
-                                        auth_roles = set(test["auth_roles"])
-                                    if "auth_roles_prepare" in test:
-                                        auth_roles_prepare = set(test["auth_roles_prepare"])
-                                    else:
-                                        auth_roles_prepare = auth_roles
-                                    user_roles = set()
-                                    user_roles_prepare = set()
-                                    if "user_roles" in test:
-                                        user_roles = set(test["user_roles"])
-                                    if "user_roles_prepare" in test:
-                                        user_roles_prepare = set(test["user_roles_prepare"])
-                                    else:
-                                        user_roles_prepare = user_roles
-                                    minimal_coverage = 100.0
-                                    if "minimal_coverage" in test:
-                                        minimal_coverage = float(test["minimal_coverage"])
-                                    should_succeed = True
-                                    if "should_succeed" in test:
-                                        should_succeed = bool(test["should_succeed"])
-                                    should_succeed_exceptions = set()
-                                    if "should_succeed_exceptions" in test:
-                                        should_succeed_exceptions = set(
-                                            test["should_succeed_exceptions"])
-                                    warn_only = False
-                                    if "warn_only" in test:
-                                        warn_only = bool(test["warn_only"])
-                                    warn_only_exceptions = set()
-                                    if "warn_only_exceptions" in test:
-                                        warn_only_exceptions = set(test["warn_only_exceptions"])
-                                    skip = set()
-                                    if "skip" in test:
-                                        skip = set(test["skip"])
-                                    run_scenarios = True
-                                    if "scenarios" in test and not test["scenarios"]:
-                                        run_scenarios = False
-                                    doc = "No doc for test"
-                                    if "doc" in test:
-                                        doc = test["doc"]
-                                    role_used = set()
-                                    for key in role_all:
-                                        if key not in skip:
-                                            role_used.add(key)
-                                    should_succeed_map = {}
-                                    warn_only_map = {}
-                                    for key in role_used:
-                                        if key in should_succeed_exceptions:
-                                            should_succeed_map[key] = not should_succeed
+                                        if "auth" in test:
+                                            auth = test["auth"]
+                                        if "auth_prepare" in test:
+                                            auth_prepare = test["auth_prepare"]
+                                        if auth[0] != "$":
+                                            auth = "$auth00"
+                                        if auth_prepare[0] != "$":
+                                            auth_prepare = "$auth31"
+                                        if auth[1:] in AUTHMAP:
+                                            auth_info = AUTHMAP[auth[1:]]
+                                            user = auth[1:]
                                         else:
-                                            should_succeed_map[key] = should_succeed
-                                        if key in warn_only_exceptions:
-                                            warn_only_map[key] = not warn_only
+                                            auth_info = AUTHMAP["auth00"]
+                                            user = "auth00"
+                                        if auth_prepare[1:] in AUTHMAP:
+                                            auth_info_prepare = AUTHMAP[auth_prepare[1:]]
+                                            user_prepare = auth_prepare[1:]
                                         else:
-                                            warn_only_map[key] = warn_only
-                                    minimal_succeed_count = int((minimal_coverage + 0.01) *
-                                                                len(should_succeed_map.keys()) /
-                                                                100)
-                                    test_obj = {}
-                                    test_obj["role"] = role
-                                    test_obj["test"] = test_name
-                                    test_obj["addr"] = auth_info[0]
-                                    test_obj["key"] = auth_info[1]
-                                    test_obj["addr_prepare"] = auth_info_prepare[0]
-                                    test_obj["key_prepare"] = auth_info_prepare[1]
-                                    test_obj["auth_roles"] = list(auth_roles)
-                                    test_obj["auth_roles_prepare"] = list(auth_roles_prepare)
-                                    test_obj["user"] = user
-                                    test_obj["user_prepare"] = user_prepare
-                                    test_obj["user_roles"] = list(user_roles)
-                                    test_obj["user_roles_prepare"] = list(user_roles_prepare)
-                                    test_obj["sub_tests"] = []
-                                    test_obj["run_scenarios"] = run_scenarios
-                                    test_obj["doc"] = doc
-                                    for key, val in should_succeed_map.items():
-                                        test_obj["sub_tests"].append([key,
-                                                                      val,
-                                                                      warn_only_map[key]])
-                                    test_obj["coverage"] = minimal_succeed_count
-                                    test_list.append(test_obj)
+                                            auth_info_prepare = AUTHMAP["auth31"]
+                                            user_prepare = "auth31"
+                                        if "user" in test:
+                                            user = test["user"]
+                                        if "user_prepare" in test:
+                                            user_prepare = test["user_prepare"]
+                                        auth_roles = set()
+                                        auth_roles_prepare = set()
+                                        if "auth_roles" in test:
+                                            auth_roles = set(test["auth_roles"])
+                                        if "auth_roles_prepare" in test:
+                                            auth_roles_prepare = set(test["auth_roles_prepare"])
+                                        else:
+                                            auth_roles_prepare = auth_roles
+                                        user_roles = set()
+                                        user_roles_prepare = set()
+                                        if "user_roles" in test:
+                                            user_roles = set(test["user_roles"])
+                                        if "user_roles_prepare" in test:
+                                            user_roles_prepare = set(test["user_roles_prepare"])
+                                        else:
+                                            user_roles_prepare = user_roles
+                                        minimal_coverage = 100.0
+                                        if "minimal_coverage" in test:
+                                            minimal_coverage = float(test["minimal_coverage"])
+                                        should_succeed = True
+                                        if "should_succeed" in test:
+                                            should_succeed = bool(test["should_succeed"])
+                                        should_succeed_exceptions = set()
+                                        if "should_succeed_exceptions" in test:
+                                            should_succeed_exceptions = set(
+                                                test["should_succeed_exceptions"])
+                                        warn_only = False
+                                        if "warn_only" in test:
+                                            warn_only = bool(test["warn_only"])
+                                        warn_only_exceptions = set()
+                                        if "warn_only_exceptions" in test:
+                                            warn_only_exceptions = set(test["warn_only_exceptions"])
+                                        skip = set()
+                                        if "skip" in test:
+                                            skip = set(test["skip"])
+                                        run_scenarios = True
+                                        if "scenarios" in test and not test["scenarios"]:
+                                            run_scenarios = False
+                                        doc = "No doc for test"
+                                        if "doc" in test:
+                                            doc = test["doc"]
+                                        role_used = set()
+                                        for key in role_all:
+                                            if key not in skip:
+                                                role_used.add(key)
+                                        should_succeed_map = {}
+                                        warn_only_map = {}
+                                        for key in role_used:
+                                            if key in should_succeed_exceptions:
+                                                should_succeed_map[key] = not should_succeed
+                                            else:
+                                                should_succeed_map[key] = should_succeed
+                                            if key in warn_only_exceptions:
+                                                warn_only_map[key] = not warn_only
+                                            else:
+                                                warn_only_map[key] = warn_only
+                                        minimal_succeed_count = int((minimal_coverage + 0.01) *
+                                                                    len(should_succeed_map.keys()) /
+                                                                    100)
+                                        test_obj = {}
+                                        test_obj["role"] = role
+                                        test_obj["test"] = test_name
+                                        test_obj["addr"] = auth_info[0]
+                                        test_obj["key"] = auth_info[1]
+                                        test_obj["addr_prepare"] = auth_info_prepare[0]
+                                        test_obj["key_prepare"] = auth_info_prepare[1]
+                                        test_obj["auth_roles"] = list(auth_roles)
+                                        test_obj["auth_roles_prepare"] = list(auth_roles_prepare)
+                                        test_obj["user"] = user
+                                        test_obj["user_prepare"] = user_prepare
+                                        test_obj["user_roles"] = list(user_roles)
+                                        test_obj["user_roles_prepare"] = list(user_roles_prepare)
+                                        test_obj["sub_tests"] = []
+                                        test_obj["run_scenarios"] = run_scenarios
+                                        test_obj["doc"] = doc
+                                        for key, val in should_succeed_map.items():
+                                            test_obj["sub_tests"].append([key,
+                                                                          val,
+                                                                          warn_only_map[key]])
+                                        test_obj["coverage"] = minimal_succeed_count
+                                        test_list.append(test_obj)
+                                    else:
+                                        print("WARNING: role", role, " defined in",
+                                              testfile, "not defined in", os.path.join(api, "roles"))
                                 else:
-                                    print("WARNING: role", role, " defined in",
-                                          testfile, "not defined in", os.path.join(api, "roles"))
-                            else:
-                                print("WARNING: test in", testfile,
-                                      "without api_role, skipping tests")
-                        await domainapi_test(host,
-                                             port,
-                                             database,
-                                             createkey,
-                                             test_list,
-                                             expanded2,
-                                             api,
-                                             apimap_modules)
-                    else:
-                        print("WARNING: Skipping apimap tests because apimap dir is missing or",
-                              "incomplete:", api)
-
-            maxstage += 1
+                                    print("WARNING: test in", testfile,
+                                          "without api_role, skipping tests")
+                            await domainapi_test(host,
+                                                 port,
+                                                 database,
+                                                 createkey,
+                                                 test_list,
+                                                 expanded2,
+                                                 api,
+                                                 apimap_modules)
+                        else:
+                            print("WARNING: Skipping apimap tests because apimap dir is missing or",
+                                  "incomplete:", api)
+                maxstage += 1
+        hooks.after()
         if output:
             # Write the expanded transaction list for all stages combined to a single artifact.
             with open(output, "w") as opf:
                 opf.write(json.dumps(expanded, indent=4))
         elif notest:
             # If no output but notest specified, fill the database with the expanded tranactions
             # list.
@@ -1510,37 +1592,37 @@
 
 
 def get_container_info(container):
     """Get host port and create key from docker"""
     hostport = None
     createkey = None
     if ("HostConfig" in container.attrs and "PortBindings" in container.attrs["HostConfig"]):
-        for portoption in ["8090/tcp", "8090/tcp"]:
+        for portoption in ("8090/tcp", "8090/tcp"):
             if portoption in container.attrs["HostConfig"]["PortBindings"]:
                 for binding in container.attrs["HostConfig"]["PortBindings"][portoption]:
                     if "HostPort" in binding:
                         hostport = binding["HostPort"]
     command_result = container.exec_run("cat default-private-key.txt")
     if command_result.exit_code == 0: # pylint: disable=compare-to-zero
         createkey = command_result.output.decode()
     return hostport, createkey
 
 
 def get_from_docker(tag):
     """Retreive the host port and the createkey from a running fsst docker image"""
     client = docker.from_env()
     container = get_running_docker(client, tag)
-    if not container:
+    if not container: # pylint: disable=consider-using-assignment-expr
         print("ERROR: Running docker with tag", tag, "not found")
         sys.exit(1)
     hostport, createkey = get_container_info(container)
     return hostport, createkey
 
 
-def run_in_docker(tag, command, directory, daemonize, expose, api="apimap", debug=False):
+def run_in_docker(tag, command, directory, daemonize, expose, api="apimap", debug=False, hooks=False):
     """Run a given command in a new docker container"""
     # pylint: disable=too-many-locals, too-many-statements, too-many-branches, too-many-arguments
     print("COMMAND:", command)
     match = None
     lookfor = "pibara/fsst:" + tag
     print("IMAGE:", lookfor)
     client = docker.from_env()
@@ -1562,14 +1644,19 @@
         sys.exit(1)
     mounts = [docker.types.Mount("/usr/src/fsst/fluree_parts",
                                  workdir, read_only=True, type="bind")]
     apidir = os.path.join(os.getcwd(), api)
     if os.path.isdir(apidir):
         mounts.append(docker.types.Mount("/usr/src/fsst/apimap",
                                          apidir, read_only=True, type="bind"))
+    if hooks:
+        hooksdir = os.path.join(os.getcwd(), "hooks")
+        if os.path.isdir(hooksdir):
+            mounts.append(docker.types.Mount("/usr/src/fsst/hooks",
+                                             hooksdir, read_only=True, type="bind"))
     ports = {}
     name = "fsst-guestcommand-" + tag
     if expose or daemonize:
         if tag == "stable":
             ports["8090/tcp"] = 8090
         else:
             ports["8090/tcp"] = 8090
@@ -1607,48 +1694,49 @@
 
 async def get_createkey_and_port(createkey, keyfile, dockerfind,
                                  port, startfluree, verbosefluree):
     """Get the create-key and fluree port using the relevant commandline info"""
     # pylint: disable=too-many-arguments
     if startfluree:
         rval = None
+        process = None
         command = ["/bin/bash", "/usr/src/fsst/fluree_start.sh", "-Dfdb-api-port=8090"]
         if not verbosefluree:
             # pylint: disable=consider-using-with
-            subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+            process = subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         else:
             # pylint: disable=consider-using-with
-            subprocess.Popen(command)
+            process = subprocess.Popen(command)
         times = 0
         while not rval: # pylint: disable=while-used
             try:
                 with open("./default-private-key.txt") as kfile:
                     rval = kfile.read()
             except FileNotFoundError:
                 print("# waiting for default-private-key.txt to appear")
             await asyncio.sleep(6)
             times += 1
             if times > 40:
                 print("ERROR: Taking too long for default-private-key.txt to apear in docker")
                 print("       container after starting FlureeDB")
                 sys.exit(1)
         print("Started FlureeDB and got createkey from newly created keyfile")
-        return rval, port
+        return rval, port, process
     if createkey:
         print("Using --createkey and --port values", )
-        return createkey, port
+        return createkey, port, None
     if keyfile:
         print("Using --keyfile and --port values")
         with open(keyfile) as kfil:
             createkey = kfil.read().replace("\r", "").replace("\n", "")
-            return createkey, port
+            return createkey, port, None
     if dockerfind:
         print("Fetching createkey and port from running image:", dockerfind)
         hostport, createkey = get_from_docker(dockerfind)
-        return createkey, hostport
+        return createkey, hostport, None
     print("ERROR: No way specfied to find default signing key for FlureeDB")
     print("       Use one of the following command line options:")
     print("")
     print("         --createkey")
     print("         --keyfile")
     print("         --dockerfind")
     sys.exit(1)
@@ -1704,26 +1792,29 @@
                               verboseerrors=verboseerrors)
     if not is_ok:
         sys.exit(1)
     return
 
 
 async def dockertest_main(directory, target, verboseerrors,
-                          network, tag, verbosefluree, linger, api, stages, debug):
+                          network, tag, verbosefluree, linger, api, stages, debug,
+                          runs, hooks):
     """Main function for the dockertest subcommand"""
     # pylint: disable=too-many-arguments
-    cmd = "fsst guesttest --target " + target + " --network " + network
+    cmd = "fsst guesttest --target " + target + " --network " + network + " --runs " + runs
     if verboseerrors:
         cmd += " --verboseerrors"
     if verbosefluree:
         cmd += " --verbosefluree"
     if linger:
         cmd += " --linger"
+    if hooks:
+        cmd += " --hooks"
     cmd += " --stages " + stages
-    return run_in_docker(tag, cmd, directory, False, linger, api=api, debug=debug)
+    return run_in_docker(tag, cmd, directory, False, linger, api=api, debug=debug, hooks=hooks)
 
 
 async def dockerstart_main(tag):
     """Main function for the dockerstart subcommand"""
     imagename = "pibara/fsst:" + tag
     fluree_command = "/bin/bash /usr/src/fsst/fluree_start.sh  -Dfdb-api-port=8090"
     ports = {}
@@ -1743,15 +1834,15 @@
 
 
 async def dockerstop_main(tag):
     """Main function for the dockerstop subcommand"""
     lookfor = "pibara/fsst:" + tag
     client = docker.from_env()
     container = get_running_docker(client, tag)
-    if container:
+    if container: # pylint: disable=consider-using-assignment-expr
         container.stop()
         print("Stopping", lookfor)
     else:
         print("ERROR: no running instance of", lookfor, "found")
 
 
 async def versioncheck_main(tag):
@@ -1813,28 +1904,34 @@
     if verboseerrors:
         cmd += " --verboseerrors"
     if verbosefluree or not daemonize:
         cmd += " --verbosefluree"
     return run_in_docker(tag, cmd, directory, daemonize, True, debug=debug)
 
 
-async def guesttest_main(target, verboseerrors, network, linger, createkey, stages):
+async def guesttest_main(target, verboseerrors, network, linger, createkey, stages,
+                         runs, hooks, fluree_process, verbosefluree=False):
     """Main function for the guesttest subcommand"""
     # pylint: disable=too-many-arguments
     prt = 8090
     is_ok = await fluree_main(notest=False,
                               network=network,
                               host="localhost",
                               port=prt,
                               output=None,
                               createkey=createkey,
                               target=target,
                               fluree_parts="fluree_parts",
                               verboseerrors=verboseerrors,
-                              stages=stages)
+                              stages=stages,
+                              runs=int(runs),
+                              hooks=hooks,
+                              fluree_process=fluree_process,
+                              verbosefluree=verbosefluree
+                              )
     if linger:
         print("LINGER == True")
         count = 0
         while True: # pylint: disable=while-used
             await asyncio.sleep(30)
             count += 1
             print('LINGER', count, flush=True)
@@ -1895,15 +1992,15 @@
     return
 
 
 async def dockerparams_main(tag):
     """Main function for the dockerparams subcommand"""
     client = docker.from_env()
     container = get_running_docker(client, tag)
-    if container is None:
+    if container is None: # pylint: disable=consider-using-assignment-expr
         print("ERROR, running container not found for tag =", tag)
         return
     echo = container.exec_run("cat default-private-key.txt")
     createkey = None
     port = None
     if echo.exit_code == 0: # pylint: disable=compare-to-zero
         createkey = echo.output.decode()
@@ -2027,20 +2124,20 @@
                                     name in desired["transactions"] or
                                     subdir == "roles" and
                                     name in desired["roles"]):
                                 with open(filepath) as infil:
                                     obj[subdir][name] = json.load(infil)
                                     if subdir == "query" and name not in obj["xform"]:
                                         obj["xform"][name] = "$"
-                        elif (subdir in {"query", "multi"} and
+                        elif (subdir in {"query", "multi"} and # pylint: disable=confusing-consecutive-elif
                               ext.lower() == "xform" and
                               name in desired["queries"]):
                             with open(filepath) as infil:
                                 obj["xform"][name] = infil.read()
-                elif (os.path.isdir(filepath) and
+                elif (os.path.isdir(filepath) and # pylint: disable=confusing-consecutive-elif
                       subdir == "transaction" and
                       filename in desired["transactions"]):
                     subsubdir = os.path.join(fulldir, filename)
                     for subfilename in os.listdir(subsubdir):
                         subfilepath = os.path.join(subsubdir, subfilename)
                         if os.path.isfile(subfilepath):
                             name2, _ = subfilename.split(".")
@@ -2099,15 +2196,17 @@
         "output": "Output JSON file",
         "input": "Input JSON file",
         "db": "Name for the new database to deploy to.",
         "js": "Output a JavaScript module file instead of a JSON file",
         "roles": "Comma seperated list of roles to include in the domain-API artifact",
         "force": "Overwrite output file if it already exists",
         "stages": "Comma seperrated list of stages to run tests for. If none specified, then all tests will be run.",
-        "debug": "Run aioflureedb in debug mode"
+        "debug": "Run aioflureedb in debug mode",
+        "hooks": "Invoke custom hooks when running",
+        "runs": "For special test cases, run flureedb a number of times over"
     }
     # pylint: enable=line-too-long
     defaults = {
         "dir": "fluree_parts",
         "api": "apimap",
         "target": "default",
         "verboseerrors": False,
@@ -2121,15 +2220,17 @@
         "linger": False,
         "tag": "stable",
         "verbosefluree": False,
         "daemonize": False,
         "roles": "ALL",
         "force": False,
         "stages": "ALL",
-        "debug": False
+        "debug": False,
+        "hooks": False,
+        "runs": "1"
     }
     argsmap = {
         "artifact": {"output", "dir", "target", "verboseerrors"},
         "test": {
             "dir",
             "api",
             "target",
@@ -2158,27 +2259,48 @@
                        "target",
                        "verboseerrors",
                        "network",
                        "linger",
                        "tag",
                        "verbosefluree",
                        "stages",
-                       "debug"},
-        "dockerdeploy": {"db", "dir", "target", "verboseerrors", "tag", "daemonize", "debug"},
+                       "debug",
+                       "runs",
+                       "hooks"},
+        "dockerdeploy": {"db",
+                         "dir",
+                         "target",
+                         "verboseerrors",
+                         "tag",
+                         "daemonize",
+                         "debug"},
         "dockerparams": {"tag"},
-        "artifactdeploy": {"input:db", "host", "port", "createkey", "keyfile", "dockerfind"},
+        "artifactdeploy": {"input",
+                           "db",
+                           "host",
+                           "port",
+                           "createkey",
+                           "keyfile",
+                           "dockerfind"},
         "guesttest": {"target",
                       "verboseerrors",
                       "network",
                       "keyfile",
                       "linger",
                       "verbosefluree",
                       "api",
-                      "stages"},
-        "guestdeploy": {"db", "target", "verboseerrors", "keyfile", "linger", "verbosefluree"},
+                      "stages",
+                      "runs",
+                      "hooks"},
+        "guestdeploy": {"db",
+                        "target",
+                        "verboseerrors",
+                        "keyfile",
+                        "linger",
+                        "verbosefluree"},
         "versioncheck": {"tag"},
         "dockerstart": {"tag"},
         "dockerstop": {"tag"},
         "version": {},
         "apiartifact": {"js", "api", "roles", "force", "output"}
     }
     if CRYPTO_OK:
@@ -2245,15 +2367,17 @@
             "input",
             "db",
             "daemonize",
             "js",
             "roles",
             "force",
             "stages",
-            "debug"
+            "debug",
+            "runs",
+            "hooks"
         }
         for sc_arg in sc_args:
             for subarg in sc_arg.split(":"):
                 sa_help = helps[subarg]
                 if subarg in defaults:
                     sa_default = defaults[subarg]
                     if sa_default is not None and not sa_default:
@@ -2273,17 +2397,18 @@
     if not vars(args):
         print("Please supply commandline agruments. Use --help for info")
         sys.exit(1)
     if args.subcommand == "artifact":
         return await artifact_main(args.output, args.dir, args.target, args.verboseerrors)
     createkey = args.createkey
     port = args.port
+    fluree_process = None
     if args.subcommand in {"test", "deploy", "guesttest", "guestdeploy", "artifactdeploy"}:
         startfluree = bool(args.subcommand in {"guesttest", "guestdeploy"})
-        createkey, port = await get_createkey_and_port(args.createkey,
+        createkey, port, fluree_process = await get_createkey_and_port(args.createkey,
                                                        args.keyfile,
                                                        args.dockerfind,
                                                        args.port,
                                                        startfluree,
                                                        args.verbosefluree)
     if args.subcommand == "test":
         await test_main(args.dir,
@@ -2308,15 +2433,17 @@
                               args.verboseerrors,
                               args.network,
                               args.tag,
                               args.verbosefluree,
                               args.linger,
                               args.api,
                               args.stages,
-                              args.debug)
+                              args.debug,
+                              args.runs,
+                              args.hooks)
     elif args.subcommand == "dockerdeploy":
         await dockerdeploy_main(args.dir,
                                 args.target,
                                 args.verboseerrors,
                                 args.db,
                                 args.tag,
                                 args.verbosefluree,
@@ -2324,17 +2451,23 @@
                                 args.debug)
     elif args.subcommand == "guesttest":
         await guesttest_main(args.target,
                              args.verboseerrors,
                              args.network,
                              args.linger,
                              createkey,
-                             args.stages)
+                             args.stages,
+                             args.runs,
+                             args.hooks,
+                             fluree_process,
+                             verbosefluree=args.verbosefluree)
     elif args.subcommand == "guestdeploy":
-        await guestdeploy_main(args.target, args.verboseerrors, args.db, createkey)
+        await guestdeploy_main(args.target,
+                               args.verboseerrors,
+                               args.db, createkey)
     elif args.subcommand == "artifactdeploy":
         await artifactdeploy_main(args.input, args.db, args.host, port, createkey)
     elif args.subcommand == "dockerparams":
         await dockerparams_main(args.tag)
     elif args.subcommand == "version":
         print("FSST VERSION:", VERSION)
     elif args.subcommand == "versioncheck":
```

### Comparing `fsst-0.8.0/setup.py` & `fsst-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='fsst',
-    version="0.8.0",
+    version="0.8.1",
     description="Fluree Schema Scenario Tool",
     long_description="Testing tool for schema and smart function unit tests for FlureeDB",
     author='Rob Meijer',
     author_email='pibara@gmail.com',
     url='https://github.com/pibara/fluree-schema-scenario-tool',
     license='BSD',
     py_modules=['fsst'],
```

