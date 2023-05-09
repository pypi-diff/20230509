# Comparing `tmp/simpful-2.8.0.tar.gz` & `tmp/simpful-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpful-2.8.0.tar", last modified: Wed Sep  7 15:54:49 2022, max compression
+gzip compressed data, was "simpful-2.9.0.tar", last modified: Mon Nov 21 11:12:13 2022, max compression
```

## Comparing `simpful-2.8.0.tar` & `simpful-2.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 15:54:49.013186 simpful-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-09-07 15:54:39.000000 simpful-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-09-07 15:54:49.013186 simpful-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4076 2022-09-07 15:54:39.000000 simpful-2.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-07 15:54:49.013186 simpful-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-09-07 15:54:39.000000 simpful-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 15:54:49.009186 simpful-2.8.0/simpful/
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-09-07 15:54:39.000000 simpful-2.8.0/simpful/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-09-07 15:54:39.000000 simpful-2.8.0/simpful/fuzzy_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (121)    20237 2022-09-07 15:54:39.000000 simpful-2.8.0/simpful/fuzzy_sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     7434 2022-09-07 15:54:39.000000 simpful-2.8.0/simpful/rule_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)    36079 2022-09-07 15:54:39.000000 simpful-2.8.0/simpful/simpful.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 15:54:49.013186 simpful-2.8.0/simpful.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-09-07 15:54:49.000000 simpful-2.8.0/simpful.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-09-07 15:54:49.000000 simpful-2.8.0/simpful.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-07 15:54:49.000000 simpful-2.8.0/simpful.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-09-07 15:54:49.000000 simpful-2.8.0/simpful.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-07 15:54:49.000000 simpful-2.8.0/simpful.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 11:12:13.948556 simpful-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-11-21 11:11:59.000000 simpful-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-11-21 11:12:13.948556 simpful-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4076 2022-11-21 11:11:59.000000 simpful-2.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-21 11:12:13.948556 simpful-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2022-11-21 11:11:59.000000 simpful-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 11:12:13.948556 simpful-2.9.0/simpful/
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2022-11-21 11:11:59.000000 simpful-2.9.0/simpful/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-11-21 11:11:59.000000 simpful-2.9.0/simpful/fuzzy_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20237 2022-11-21 11:11:59.000000 simpful-2.9.0/simpful/fuzzy_sets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7503 2022-11-21 11:11:59.000000 simpful-2.9.0/simpful/rule_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37906 2022-11-21 11:11:59.000000 simpful-2.9.0/simpful/simpful.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 11:12:13.948556 simpful-2.9.0/simpful.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-11-21 11:12:13.000000 simpful-2.9.0/simpful.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-21 11:12:13.000000 simpful-2.9.0/simpful.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 11:12:13.000000 simpful-2.9.0/simpful.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-21 11:12:13.000000 simpful-2.9.0/simpful.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-21 11:12:13.000000 simpful-2.9.0/simpful.egg-info/top_level.txt
```

### Comparing `simpful-2.8.0/LICENSE` & `simpful-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simpful-2.8.0/PKG-INFO` & `simpful-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpful
-Version: 2.8.0
+Version: 2.9.0
 Summary: A user-friendly Python library for fuzzy logic
 Home-page: https://github.com/aresio/simpful
 Author: Marco S. Nobile
 Author-email: marco.nobile@unive.it
 License: LICENSE.txt
 Keywords: fuzzy logic,sugeno,mamdani,reasoner,python,modeling
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `simpful-2.8.0/README.md` & `simpful-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `simpful-2.8.0/setup.py` & `simpful-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'simpful',
   packages = ['simpful'], # this must be the same as the name above
-  version = '2.8.0',
+  version = '2.9.0',
   description = 'A user-friendly Python library for fuzzy logic',
   author = 'Marco S. Nobile',
   author_email = 'marco.nobile@unive.it',
   url = 'https://github.com/aresio/simpful', # use the URL to the github repo
   keywords = ['fuzzy logic', 'sugeno', 'mamdani', 'reasoner', 'python', 'modeling'], # arbitrary keywords
   license='LICENSE.txt',
   install_requires=[
```

### Comparing `simpful-2.8.0/simpful/fuzzy_aggregation.py` & `simpful-2.9.0/simpful/fuzzy_aggregation.py`

 * *Files identical despite different names*

### Comparing `simpful-2.8.0/simpful/fuzzy_sets.py` & `simpful-2.9.0/simpful/fuzzy_sets.py`

 * *Files identical despite different names*

### Comparing `simpful-2.8.0/simpful/rule_parsing.py` & `simpful-2.9.0/simpful/rule_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 class Functional(object):
 
     def __init__(self, fun, A, B, operators=None):
         self._A = A
         self._B = B
 
         if fun=="NOT":
-            if B == "": raise Exception("OMG")
-        elif A == "": raise Exception("OMG")
+            if B == "": raise Exception("Second operand missing")
+        elif A == "": raise Exception("First operand missing")
 
         if operators is None:
             self._fun = fun
         else:
             if "AND_PRODUCT" in operators: 
                 if fun=="AND":
                     self._fun = "AND_p"
@@ -67,14 +67,15 @@
         
     def __repr__(self):
         return "f.(" + str(self._A) + " " + self._fun + " " + str(self._B) + ")"
 
 
 # basic definitions of 
 def OR(x,y): return max(x, y)
+def OR_p(x,y): return x+y-(x*y)
 def AND(x,y): return min(x, y)
 def AND_p(x,y): return x*y
 def NOT(x): return 1.-x
 
 
 def preparse(STRINGA):
     # extract the antecedent
```

### Comparing `simpful-2.8.0/simpful/simpful.py` & `simpful-2.9.0/simpful/simpful.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .rule_parsing import recursive_parse, preparse, postparse
 from numpy import array, linspace, geomspace, log10, finfo, float64
 from scipy.interpolate import interp1d
 from copy import deepcopy
 from collections import defaultdict, OrderedDict
 import re
 import string
+from math import prod
 try:
     from matplotlib.pyplot import plot, show, title, subplots, legend
     matplotlib = True
 except ImportError:
     matplotlib = False
 try:
     import seaborn as sns
@@ -38,16 +39,15 @@
             concept: a string providing a brief description of the concept represented by the linguistic variable (optional).
             universe_of_discourse: a list of two elements, specifying min and max of the universe of discourse. Optional, but it must be specified to exploit plotting facilities.
     """
 
     def __init__(self, FS_list=[], concept=None, universe_of_discourse=None):
         
         if FS_list==[]:
-            print("ERROR: please specify at least one fuzzy set")
-            exit(-2)
+            raise Exception("ERROR: please specify at least one fuzzy set")
         self._universe_of_discourse = universe_of_discourse
         self._FSlist = FS_list
         self._concept = concept
 
 
     def get_values(self, v):
         result = {}
@@ -481,14 +481,17 @@
             
             for (ant, res) in zip(antecedent, results):
                 outname = res[0]
                 outterm = res[1]
                 weight = float(res[2])
                 crisp = True
 
+                if verbose: 
+                    print(" ** Rule composition:", ant, "->", res, ", output variable: '%s'" % outname, "with term: '%s'" % outterm)            
+
                 if outname==output:
                     if outterm not in list_crisp_values:
                         crisp = False
                         if outterm not in list_output_funs:
                             raise Exception("ERROR: one rule calculates an output named '"
                                 + outterm
                                 + "', but I cannot find it among the output terms.\n"
@@ -532,56 +535,53 @@
                 if ignore_errors:
                     print("WARNING: cannot perform Sugeno inference for variable '%s'. The variable appears only as antecedent in the rules or an arithmetic error occurred." % output)
                 else:
                     raise Exception("ERROR: cannot perform Sugeno inference for variable '%s'. The variable appears only as antecedent in the rules or an arithmetic error occurred." % output)
         
         return final_result
 
-
     def mediate_Mamdani(self, 
         outputs, 
         antecedent, 
         results, 
         ignore_errors=False, 
         ignore_warnings=False, 
         verbose=False, 
         subdivisions=1000,
-        aggregation_function=max,
-        ):
+        aggregation_function=max):
 
         final_result = {}
 
         for output in outputs:
-
             if verbose:
                 print(" * Processing output for variable '%s'" %  output)
                 print("   whose universe of discourse is:", self._lvs[output].get_universe_of_discourse())
                 print("   contains the following fuzzy sets:", self._lvs[output]._FSlist )
             cuts_list = defaultdict(list)
 
             x0, x1 = self._lvs[output].get_universe_of_discourse()
 
             for (ant, res) in zip(antecedent, results):
-
                 outname = res[0]
                 outterm = res[1]
+                weight = float(res[2])
 
                 if verbose: 
                     print(" ** Rule composition:", ant, "->", res, ", output variable: '%s'" % outname, "with term: '%s'" % outterm)            
 
                 if outname==output:
-
                     try:
-                        value = ant.evaluate(self) 
+                        value = ant.evaluate(self)
                     except RuntimeError: 
                         raise Exception("ERROR: one rule could not be evaluated\n"
                         + " --- PROBLEMATIC RULE:\n"
                         + "IF " + str(ant) + " THEN " + str(res) + "\n")
 
-                    cuts_list[outterm].append(value)
+                    #degree of satisfaction of the rule is multiplied by rule weight
+                    cuts_list[outterm].append(value*weight)
 
             values = []
             weightedvalues = []
             integration_points = linspace(x0, x1, subdivisions)
 
             convenience_dict = {}
             for k in cuts_list.keys():
@@ -668,21 +668,22 @@
             cost_terms = [t for t in terms if t in self._constants]
             for name in cost_terms:
                 result[name] = self._variables[name]
         
         return result
 
 
-    def Mamdani_inference(self, terms=None, subdivisions=1000, ignore_errors=False, ignore_warnings=False, verbose=False, aggregation_function=max):
+    def Mamdani_inference(self, terms=None, subdivisions=1000, aggregation_function=max, ignore_errors=False, ignore_warnings=False, verbose=False):
         """
         Performs Mamdani fuzzy inference.
 
         Args:
-            terms: list of the names of the variables on which inference must be performed. If empty, all variables appearing in the consequent of a fuzzy rule are inferred.
-            subdivisions: the number of integration steps to be performed (default: 1000).
+            terms: list of the names of the variables on which inference must be performed.If empty, all variables appearing in the consequent of a fuzzy rule are inferred.
+            subdivisions: the number of integration steps to be performed for calculating fuzzy set area (default: 1000).
+            aggregation_function: pointer to function used to aggregate fuzzy sets during Mamdani inference, default is max. Use Python sum function, or simpful's probor function for sum and probabilistic OR, respectively.
             ignore_errors: True/False, toggles the raising of errors during the inference.
             ignore_warnings: True/False, toggles the raising of warnings during the inference.
             verbose: True/False, toggles verbose mode.
 
         Returns:
             a dictionary, containing as keys the variables' names and as values their numerical inferred values.
         """
@@ -697,14 +698,20 @@
             # get rid of duplicates in terms to infer
             terms = list(set(terms))
             for t in terms:
                 if t not in set([rule[1][0] for rule in self._rules]):
                     raise Exception("ERROR: Variable "+t+" does not appear in any consequent.")
 
         array_rules = array(self._rules, dtype=object)
+        # cheking if the rule base is weighted, if not add dummy weights
+        for n, cons in enumerate(array_rules.T[1]):
+            if len(cons)<3:
+                cons = cons + ("1.0",)
+                array_rules.T[1][n] = cons
+        
         if len(self._constants)==0:
             result = self.mediate_Mamdani(terms, array_rules.T[0], array_rules.T[1], ignore_errors=ignore_errors, ignore_warnings=ignore_warnings, verbose=verbose, subdivisions=subdivisions, aggregation_function=aggregation_function)
         else:
             #remove constant variables from list of variables to infer
             ncost_terms = [t for t in terms if t not in self._constants]
             result = self.mediate_Mamdani(ncost_terms, array_rules.T[0], array_rules.T[1], ignore_errors=ignore_errors, ignore_warnings=ignore_warnings, verbose=verbose, subdivisions=subdivisions, aggregation_function=aggregation_function)
             #add values of constant variables
@@ -715,21 +722,22 @@
         return result
 
 
     def probabilistic_inference(self, terms=None, ignore_errors=False, ignore_warnings=False, verbose=False):
         raise NotImplementedError()
 
 
-    def inference(self, terms=None, subdivisions=1000, ignore_errors=False, ignore_warnings=False, verbose=False, aggregation_function=max):
+    def inference(self, terms=None, subdivisions=1000, aggregation_function=max, ignore_errors=False, ignore_warnings=False, verbose=False):
         """
         Performs the fuzzy inference, trying to automatically choose the correct inference engine.
 
         Args:
             terms: list of the names of the variables on which inference must be performed. If empty, all variables appearing in the consequent of a fuzzy rule are inferred.
-            subdivisions: set the number of integration steps to be performed by Mamdani inference (default: 1000).
+            subdivisions: the number of integration steps to be performed for calculating fuzzy set area (default: 1000).
+            aggregation_function: pointer to function used to aggregate fuzzy sets during Mamdani inference, default is max. Use Python sum function, or simpful's probor function for sum and probabilistic OR, respectively.
             ignore_errors: True/False, toggles the raising of errors during the inference.
             ignore_warnings: True/False, toggles the raising of warnings during the inference.
             verbose: True/False, toggles verbose mode.
 
         Returns:
             a dictionary, containing as keys the variables' names and as values their numerical inferred values.
         """ 
@@ -826,9 +834,39 @@
         memberships = []
         for variable, fuzzyset in list_variables.items():
             value = self._variables[variable]
             result = self._lvs[variable].get_values(value)[fuzzyset]
             memberships.append(result)
         return function(memberships)
 
+# useful pre-implemented functions for aggregation or implication during fuzzy inference
+def prod(m_list):
+    """
+        Performs aggregation of membership values using the product operation.
+
+        Args:
+            m_list: list of membership values to aggregate.
+
+        Returns:
+            the aggregated membership value.
+    """ 
+    return prod(m_list)
+
+def probor(m_list):
+    """
+        Performs aggregation of membership values using the probabilistic OR operation.
+
+        Args:
+            m_list: list of membership values to aggregate.
+
+        Returns:
+            the aggregated membership value.
+    """
+    res = m_list[0]
+    if len(m_list) == 1:
+        return m_list[0]
+    for i in range(1, len(m_list)):
+        res = res + m_list[i] - res * m_list[i]
+    return res
+
 if __name__ == '__main__':
-    pass
+    pass
```

### Comparing `simpful-2.8.0/simpful.egg-info/PKG-INFO` & `simpful-2.9.0/simpful.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpful
-Version: 2.8.0
+Version: 2.9.0
 Summary: A user-friendly Python library for fuzzy logic
 Home-page: https://github.com/aresio/simpful
 Author: Marco S. Nobile
 Author-email: marco.nobile@unive.it
 License: LICENSE.txt
 Keywords: fuzzy logic,sugeno,mamdani,reasoner,python,modeling
 Classifier: Programming Language :: Python :: 3.7
```

