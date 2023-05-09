# Comparing `tmp/MatAn-0.1.5.2.1-py3-none-any.whl.zip` & `tmp/MatAn-0.1.5.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 19807 bytes, number of entries: 8
--rw-r--r--  2.0 unx    17003 b- defN 23-Apr-20 21:22 matan/__init__.py
--rw-r--r--  2.0 unx      107 b- defN 23-Apr-18 08:30 misc/__init__.py
--rw-r--r--  2.0 unx     2491 b- defN 23-Apr-20 21:21 properties/__init__.py
--rw-r--r--  2.0 unx    34670 b- defN 23-Apr-20 21:28 MatAn-0.1.5.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3931 b- defN 23-Apr-20 21:28 MatAn-0.1.5.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 21:28 MatAn-0.1.5.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-20 21:28 MatAn-0.1.5.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 23-Apr-20 21:28 MatAn-0.1.5.2.1.dist-info/RECORD
-8 files, 58939 bytes uncompressed, 18729 bytes compressed:  68.2%
+Zip file size: 21024 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    15734 b- defN 23-May-08 17:43 matan/__init__.py
+-rw-r--r--  2.0 unx     4803 b- defN 23-May-08 17:43 matan/files.py
+-rw-r--r--  2.0 unx      155 b- defN 23-May-06 21:05 misc/__init__.py
+-rw-r--r--  2.0 unx     2771 b- defN 23-May-08 18:03 properties/__init__.py
+-rw-r--r--  2.0 unx    34670 b- defN 23-May-09 15:15 MatAn-0.1.5.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3931 b- defN 23-May-09 15:15 MatAn-0.1.5.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-09 15:15 MatAn-0.1.5.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-May-09 15:15 MatAn-0.1.5.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      694 b- defN 23-May-09 15:15 MatAn-0.1.5.2.2.dist-info/RECORD
+9 files, 62872 bytes uncompressed, 19842 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: matan/__init__.py
 Comment: 
 
+Filename: matan/files.py
+Comment: 
+
 Filename: misc/__init__.py
 Comment: 
 
 Filename: properties/__init__.py
 Comment: 
 
-Filename: MatAn-0.1.5.2.1.dist-info/LICENSE
+Filename: MatAn-0.1.5.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: MatAn-0.1.5.2.1.dist-info/METADATA
+Filename: MatAn-0.1.5.2.2.dist-info/METADATA
 Comment: 
 
-Filename: MatAn-0.1.5.2.1.dist-info/WHEEL
+Filename: MatAn-0.1.5.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: MatAn-0.1.5.2.1.dist-info/top_level.txt
+Filename: MatAn-0.1.5.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: MatAn-0.1.5.2.1.dist-info/RECORD
+Filename: MatAn-0.1.5.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matan/__init__.py

```diff
@@ -1,17 +1,13 @@
-import sys, os
-sys.path.insert(0, os.path.join(os.getcwd(), "src"))
-
 import numpy as np
 import matplotlib.pyplot as plt
-
-import glob
 from typing import Union
-import properties
-# from sklearn.linear_model import LinearRegression
+
+from .. import properties
+
 
 
 """
 TODO:
 Create  abstract class for properties like tensile strength, tensile modulus, etc, with pass, so using diffrent norms and materials will be easier
 Move calculation of real values into method of engineering values
 Add decorators
@@ -19,122 +15,90 @@
 SOURCES:
 
 https://professorkazarinoff.github.io/Engineering-Materials-Programming/07-Mechanical-Properties/mechanical-properties-from-stress-strain-curves.html
 
 
 """
 
-"""c
-    class to menage files
-    methods are types of techniques used to manufacture material
-    """
-
-class files:
-    def __init__(self,path, extension:str, methods=None):
-        """This class can manage the files as well as it's parameters
-
-        This class helps managing he files, find their names/paths, extract the method of manufacturing or other
-        parameters
-
-        Parameters
-        ----------
-        path : str
-            This variable is used to put path to your files
-        extension : str
-            Extention is the extention of your files. If your file is .csv put csv in there, be aware and do not put the dot before your extention
-        methods : str
-            Descripe the technique of manufacturing there, or find it using find_method in that class
-
-        Examples
-        --------
-        FIXME: Add docs.
-
-        """
-
-        if extension.startswith("."):
-            extension=extension[1:]
-        
-        self.files=glob.glob(os.path.join(path, f"*.{extension}"))
-        
-        try:
-            splitted = [os.path.split(file)[1] for file in self.files if any(method in file for method in methods)] #split to extract names
-            self.paths = [file for file in self.files if any(method in file for method in methods)]
-        except TypeError:
-            splitted = [os.path.split(file)[1] for file in self.files]
-            self.paths = [file for file in self.files]
-        self.names = [name.split("_")[0] for name  in splitted]
-        self.methods = [self.find_method(name) for name in self.names ] #thats for 
-    def find_method(self,path, delimiter='-'):
-        """Find the technique how the material was created
-
-        Find the method how the material was created, what methods were used to modify it, etc. To do so it is using
-        first letters of filename, so for extruded parts you can use EXT, for annealed extruded parts you can use aEXT
-        etc.
-
-        Parameters
-        ----------
-        path : str
-            path for your file
-        delimiter : str
-            what sign you wanna use to finish your method string. By default it is -
-
-        Examples
-        --------
-        FIXME: Add docs.
-
-        """
-
-        method = path.split(delimiter)[0]
-        return method
 
 class sample:
     """
     Class to menage material, material properities, converting to engineerin stress etc.
     """
     def __init__(self,name: str,
                  thickness:float = None,
                  width:float = None,
                  elongation_array: Union[list, np.array] =None,
                  force_array: Union[list, np.array] =None,
                  stress_array: Union[list, np.array] =None,
                  strain_array: Union[list, np.array] =None,
+                 manufactured_method=None,
+                 comments=None,
                  force_units: str="N",
                  lenght_units: str="mm"):
 
         self.name=name
         self.thickness, self.width= thickness,width
         self.eng_values=engineering_values(name=name,
                                            force_units=force_units,
                                            lenght_units=lenght_units,
                                            thickness=thickness,
                                            width=width
                                            )
-        self.real_values=real_values_class(name=name,
-                                           thickness=thickness,
-                                           width=width,
-                                           force_units=force_units,
-                                           lenght_units=lenght_units,)
-        
+        self.force_units, self.lenght_units=force_units,lenght_units
         if stress_array is None and strain_array is None:
             if elongation_array is None and force_array is None:
                 raise ValueError("None of elongation/force or stress/strain arrays are defined!")
             elif thickness is None:
                 raise ValueError("Thickness is not defined!")
             elif width is None:
                 raise ValueError(" Width is not defined!")
             else:
+                self.elongation_array=elongation_array
+                self.force_array=force_array
                 self.eng_values.calculate(thickness=self.thickness,
                                           width=self.width,
                                           elongation_array=elongation_array,
                                           force_array=force_array)
-                self.real_values.calculate(self.eng_values.stress,
-                                           self.eng_values.strain)
+
         else:
             self.eng_values.set(stress_array, strain_array)
 
+    def calculate_real_values(self):
+        self.real_values=real_values_class(name=self.name,
+                                           thickness=self.thickness,
+                                           width=self.width,
+                                           force_units=self.force_units,
+                                            lenght_units=self.lenght_units
+                                               )
+        self.real_values.calculate(self.eng_values.stress,
+                                           self.eng_values.strain)            
+    def plot(self, show=False):
+            """Method for plotting the results
+
+            This method can be used to plot your engineering stress-strain curve. If you wanna show it instantly use
+            parameter show as True
+
+            Parameters
+            ----------
+            show : bool
+                It it equal to matplotlib.pyplot function show
+
+            Examples
+            --------
+            FIXME: Add docs.
+
+            """
+            plt.plot(self.elongation_array,self.force_array, label=self.name)
+            plt.title(self.name)
+            plt.ylabel(f"Force [{self.force_units}]")
+            plt.xlabel(f"Strain [{self.lenght_units}]")
+            plt.legend()
+            if show:
+                plt.show()        
 
 
                 
         
     def composition_from_name(delimiter: str, percent_sign="p"):
         """
         TODODO baby shark
@@ -250,15 +214,16 @@
                 
                 strength = properties.strenght(strain,stress)
                 self.value=strength.value
                 self.strain=strength.strain
 
         class calculate_yield_strength:
             def __init__(self, stress: np.array, strain: np.array):
-                """Yield strenght  is according to ISO-527-1 strain increase without stress increase. 
+                """
+                Yield strenght  is according to ISO-527-1 strain increase without stress increase. 
 
                 Parameters
                 ----------
                 stress : np.array
                     stress numpy array
                 strain : np.array
                     strain numpy array
@@ -277,15 +242,15 @@
             def __init__(self,stress, strain):
                 at_break=properties.at_break(stress, strain)
                 self.stress=at_break.stress
                 self.strain=at_break.strain
 
 
         def calculate_tensile_modulus(self,
-                                    plot=True,
+                                    plot=False,
                                     r2=True,
                                     output=True,
                                     lower_limit=0.05,
                                     upper_limit=0.25
                                     ):
             """            Tensile, or Young's modulus is the slope of strain/stress curve, between strains equals to 0.05 and 0.25 percent according to DIN ISO 527-1
```

## misc/__init__.py

```diff
@@ -1,3 +1,6 @@
 from math import log10, floor
 def round_sig(x, sig=2):
-   return round(x, sig-int(floor(log10(abs(x))))-1)
+   try:
+      return round(x, sig-int(floor(log10(abs(x))))-1)
+   except ValueError:
+      return x
```

## properties/__init__.py

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-import misc
+from .. import misc
 
 """
 According to ISO 527-1: https://cdn.standards.iteh.ai/samples/75824/61c480ef4bf0494aa6966bd4c2244c2e/ISO-527-1-2019.pdf
 """
 class tensile_modulus:
     def __init__(self,
                  stress,
@@ -40,15 +40,15 @@
         
 class strenght:
     def __init__(self, stress, strain):
         self.value=misc.round_sig(self.find_local_maximum(stress), sig=3)
         self.strain=misc.round_sig(strain[self.idx])
     def find_local_maximum(self, stress):
         for i in range(1, len(stress)-1):
-            if stress[i-1] < stress[i] > stress[i+1]:
+            if stress[i-1] < stress[i] > stress[i+1] and stress[i]>1:
                 self.idx=i
                 return  stress[i]
 
         print("Local maximum not found, gives max value")
         self.idx=np.where(stress==np.max(stress))[0][0]
         val = np.max(stress)
         return val
@@ -56,12 +56,19 @@
 
 class yield_strenght:
     def __init__(self,stress, strain):
         self.value=misc.round_sig(stress[self.find_idx(stress,strain)], sig=3)
         self.strain=misc.round_sig(strain[self.find_idx(stress,strain)])
     def find_idx(self, stress,strain):
         for i in range(1, len(strain)):
+            print(i, stress[i] , 'huju')
             if strain[i] > strain[i-1] and stress[i] <= stress[i-1]:
-                return  i
+                if stress[i]>1:
+                    print(stress[i])
+                    return i
+                else:
+                    print("kurwo", i , stress[i], len(stress))
+                    continue
+                    # exit()
```

## Comparing `MatAn-0.1.5.2.1.dist-info/LICENSE` & `MatAn-0.1.5.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `MatAn-0.1.5.2.1.dist-info/METADATA` & `MatAn-0.1.5.2.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MatAn
-Version: 0.1.5.2.1
+Version: 0.1.5.2.2
 Summary: Material analysis package to plot or extract properties like tensile modulus etc. 
 Home-page: https://codeberg.org/309631/matan
 Author: Igor Cudnik
 Author-email: igor.cudnik@student.put.poznan.pl
 License: GPLv3
 Keywords: material analysis,ISO 527,ISO 527-1,polymers analysis
 Classifier: Development Status :: 3 - Alpha
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib
 Requires-Dist: numpy
+Requires-Dist: matplotlib
 
 **This package is still under development. Be aware of often updates!**
 # MaTan
 
 Shortcut comes from **Mat**erial **An**analysis - ultimately is should contains modules allowing user to calculate metals and polymers properties from tensile, HDT (polymers) and DSC tests, as well as the others. There are few similar  packages in PyPI, but none of them I found good to me, so I wrote new one. 
 
 For now it includes:
```

## Comparing `MatAn-0.1.5.2.1.dist-info/RECORD` & `MatAn-0.1.5.2.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-matan/__init__.py,sha256=goYle_tEy1F32RmFhGsxQDEeltgCDig2xcrFcLSBSEk,17003
-misc/__init__.py,sha256=S4SweLuIAeWI1arT-Lwzy4ifxc8Ettq7RvbJVuLIFnc,107
-properties/__init__.py,sha256=f7_2HBg31bxVpAJc81oY_918a7Mh8jmzVi8pOB8K97U,2491
-MatAn-0.1.5.2.1.dist-info/LICENSE,sha256=tqi_Y64slbCqJW7ndGgNe9GPIfRX2nVGb3YQs7FqzE4,34670
-MatAn-0.1.5.2.1.dist-info/METADATA,sha256=0gFF1c4mZaj8sIX20_x3ru2rGginPY_VKkblu3RdeLQ,3931
-MatAn-0.1.5.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-MatAn-0.1.5.2.1.dist-info/top_level.txt,sha256=w-JKsP40rv98l3aspw7sJg6CBr_vifDhX3EyG_RP9Xs,22
-MatAn-0.1.5.2.1.dist-info/RECORD,,
+matan/__init__.py,sha256=j76IcIwhsbOsDRpaAHpbCBl6NdPdE-UhuomVCK2XBOg,15734
+matan/files.py,sha256=GMwuWl48tXjYRz87je9IenQ7JwLj9zORngCFHKFR9Qs,4803
+misc/__init__.py,sha256=8ugPfV78VbnSfz7-_SEH40R-khE687Qlpua62La9OGw,155
+properties/__init__.py,sha256=ss6fsDd7MbEaro0rIPl2wsqJuZOnuBS2OAwEBh9oNuc,2771
+MatAn-0.1.5.2.2.dist-info/LICENSE,sha256=tqi_Y64slbCqJW7ndGgNe9GPIfRX2nVGb3YQs7FqzE4,34670
+MatAn-0.1.5.2.2.dist-info/METADATA,sha256=poEo0RMDzpaq3BxjPbCzwNLwgRxd_l1YkXmWJNsdAxE,3931
+MatAn-0.1.5.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+MatAn-0.1.5.2.2.dist-info/top_level.txt,sha256=w-JKsP40rv98l3aspw7sJg6CBr_vifDhX3EyG_RP9Xs,22
+MatAn-0.1.5.2.2.dist-info/RECORD,,
```

