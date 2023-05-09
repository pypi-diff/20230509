# Comparing `tmp/posym-0.5.3.tar.gz` & `tmp/posym-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posym-0.5.3.tar", last modified: Thu Apr 20 12:58:42 2023, max compression
+gzip compressed data, was "posym-0.5.4.tar", last modified: Tue May  9 13:08:38 2023, max compression
```

## Comparing `posym-0.5.3.tar` & `posym-0.5.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:58:42.537954 posym-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 12:58:31.000000 posym-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-04-20 12:58:42.533954 posym-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-04-20 12:58:31.000000 posym-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:58:42.533954 posym-0.5.3/c/
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-04-20 12:58:31.000000 posym-0.5.3/c/integrals.c
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-20 12:58:31.000000 posym-0.5.3/c/permutations.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:58:42.533954 posym-0.5.3/posym/
--rw-r--r--   0 runner    (1001) docker     (123)    28015 2023-04-20 12:58:31.000000 posym-0.5.3/posym/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-20 12:58:31.000000 posym-0.5.3/posym/algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    30004 2023-04-20 12:58:31.000000 posym-0.5.3/posym/basis.py
--rw-r--r--   0 runner    (1001) docker     (123)    28249 2023-04-20 12:58:31.000000 posym-0.5.3/posym/generate_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-04-20 12:58:31.000000 posym-0.5.3/posym/ir_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:58:42.533954 posym-0.5.3/posym/operations/
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-20 12:58:31.000000 posym-0.5.3/posym/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-20 12:58:31.000000 posym-0.5.3/posym/operations/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-20 12:58:31.000000 posym-0.5.3/posym/operations/inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-04-20 12:58:31.000000 posym-0.5.3/posym/operations/irotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-20 12:58:31.000000 posym-0.5.3/posym/operations/reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-20 12:58:31.000000 posym-0.5.3/posym/operations/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-20 12:58:31.000000 posym-0.5.3/posym/pointgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-04-20 12:58:31.000000 posym-0.5.3/posym/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:58:42.533954 posym-0.5.3/posym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-04-20 12:58:42.000000 posym-0.5.3/posym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-20 12:58:42.000000 posym-0.5.3/posym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:58:42.000000 posym-0.5.3/posym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 12:58:42.000000 posym-0.5.3/posym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 12:58:42.000000 posym-0.5.3/posym.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:58:42.537954 posym-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-20 12:58:31.000000 posym-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:08:38.236697 posym-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-09 13:08:29.000000 posym-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-09 13:08:38.236697 posym-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-05-09 13:08:29.000000 posym-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:08:38.236697 posym-0.5.4/c/
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-05-09 13:08:29.000000 posym-0.5.4/c/integrals.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-09 13:08:29.000000 posym-0.5.4/c/permutations.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:08:38.236697 posym-0.5.4/posym/
+-rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-05-09 13:08:29.000000 posym-0.5.4/posym/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-09 13:08:29.000000 posym-0.5.4/posym/algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30004 2023-05-09 13:08:29.000000 posym-0.5.4/posym/basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28249 2023-05-09 13:08:29.000000 posym-0.5.4/posym/generate_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-05-09 13:08:29.000000 posym-0.5.4/posym/ir_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:08:38.236697 posym-0.5.4/posym/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-09 13:08:29.000000 posym-0.5.4/posym/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-09 13:08:29.000000 posym-0.5.4/posym/operations/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-09 13:08:29.000000 posym-0.5.4/posym/operations/inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-09 13:08:29.000000 posym-0.5.4/posym/operations/irotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-09 13:08:29.000000 posym-0.5.4/posym/operations/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-09 13:08:29.000000 posym-0.5.4/posym/operations/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-09 13:08:29.000000 posym-0.5.4/posym/pointgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-05-09 13:08:29.000000 posym-0.5.4/posym/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:08:38.236697 posym-0.5.4/posym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-09 13:08:38.000000 posym-0.5.4/posym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-09 13:08:38.000000 posym-0.5.4/posym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:08:38.000000 posym-0.5.4/posym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 13:08:38.000000 posym-0.5.4/posym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 13:08:38.000000 posym-0.5.4/posym.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:08:38.236697 posym-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-09 13:08:29.000000 posym-0.5.4/setup.py
```

### Comparing `posym-0.5.3/LICENSE` & `posym-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/PKG-INFO` & `posym-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posym
-Version: 0.5.3
+Version: 0.5.4
 Summary: posym module
 Home-page: https://github.com/abelcarreras/posym
 Author: Abel Carreras
 Author-email: abelcarreras83@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `posym-0.5.3/README.md` & `posym-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/c/integrals.c` & `posym-0.5.4/c/integrals.c`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/c/permutations.c` & `posym-0.5.4/c/permutations.c`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/posym/__init__.py` & `posym-0.5.4/posym/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = 'Abel Carreras'
-__version__ = '0.5.3'
+__version__ = '0.5.4'
 
 from posym.tools import list_round
 from posym.pointgroup import PointGroup
 from posym.basis import BasisFunction
 from scipy.spatial.transform import Rotation as R
 from scipy.optimize import minimize, basinhopping
 import numpy as np
@@ -125,22 +125,19 @@
     def __init__(self, group, coordinates, symbols, total_state=None, orientation_angles=None, center=None,
                  fast_optimization=True):
 
         self._setup_structure(coordinates, symbols, group, center, orientation_angles, fast_optimization=fast_optimization)
 
         if total_state is None:
             rotmol = R.from_euler('zyx', self._angles, degrees=True)
-            geom_center = np.average(coordinates, axis=0)
-            centered_coor = np.subtract(coordinates, geom_center)
-
             self._operator_measures = []
             for operation in self._pg.operations:
                 operator_measures = []
                 for op in self._pg.get_sub_operations(operation.label):
-                    overlap = op.get_measure_pos(centered_coor, symbols, orientation=rotmol)
+                    overlap = op.get_measure_pos(self._coordinates, symbols, orientation=rotmol)
                     operator_measures.append(overlap)
 
                 self._operator_measures.append(np.array(operator_measures))
 
             total_state = pd.Series(self._operator_measures, index=self._pg.op_labels)
 
         super().__init__(group, total_state)
@@ -274,17 +271,17 @@
 
     @property
     def center(self):
         return self._center
 
 
 class SymmetryModes(SymmetryMoleculeBase):
-    def __init__(self, group, coordinates, modes, symbols, orientation_angles=None):
+    def __init__(self, group, coordinates, modes, symbols, orientation_angles=None, center=None):
 
-        self._setup_structure(coordinates, symbols, group, None, orientation_angles)
+        self._setup_structure(coordinates, symbols, group, center, orientation_angles)
 
         self._modes = modes
 
         rotmol = R.from_euler('zyx', self._angles, degrees=True)
 
         self._mode_measures = []
         for operation in self._pg.operations:
@@ -308,15 +305,15 @@
         for m in range(len(self._mode_measures[0].T)):
             reshaped_modes_measures.append([k[:, m] for k in self._mode_measures])
 
         self._mode_measures = reshaped_modes_measures
 
         total_state = pd.Series(mode_measures_total, index=self._pg.op_labels)
 
-        super().__init__(group, self._coordinates, self._symbols, total_state, self._angles, [0,0,0])
+        super().__init__(group, self._coordinates, self._symbols, total_state, self._angles, [0, 0, 0])
 
     def get_state_mode(self, n):
         return SymmetryBase(group=self._group, rep=pd.Series(self._mode_measures[n],
                                                              index=self._pg.op_labels))
 
 
 class SymmetryModesFull(SymmetryMoleculeBase):
@@ -342,15 +339,15 @@
                 mode_measures.append(measure_xyz * measure_atom)
 
             mode_measures = np.array(mode_measures)
             self._mode_measures.append(mode_measures)
 
         self._mode_measures = np.array(self._mode_measures, dtype=object).flatten() - trans_rots
         total_state = pd.Series(self._mode_measures, index=self._pg.op_labels)
-        super().__init__(group, self._coordinates, self._symbols, total_state, self._angles, [0,0,0])
+        super().__init__(group, self._coordinates, self._symbols, total_state, self._angles, [0, 0, 0])
 
 
 class SymmetryFunction(SymmetryMoleculeBase):
     def __init__(self, group, function, orientation_angles=None, center=None):
 
         symbols, coordinates = function.get_environment_centers()
 
@@ -369,23 +366,23 @@
             for op in self._pg.get_sub_operations(operation.label):
                 overlap = op.get_overlap_func(self._function, self._function, orientation=rotmol)
                 operator_measures.append(overlap/self._self_similarity)
 
             self._operator_measures.append(np.array(operator_measures))
 
         total_state = pd.Series(self._operator_measures, index=self._pg.op_labels)
-        super().__init__(group, self._coordinates, self._symbols, total_state, self._angles, [0,0,0])
+        super().__init__(group, self._coordinates, self._symbols, total_state, self._angles, [0, 0, 0])
 
     @property
     def self_similarity(self):
         return self._self_similarity
 
 
 class SymmetryWaveFunction(SymmetryMoleculeBase):
-    def __init__(self, group, alpha_orbitals, beta_orbitals, center=None, orientation_angles=None):
+    def __init__(self, group, alpha_orbitals, beta_orbitals, orientation_angles=None, center=None):
 
         # generate copy to not modify original orbitals
         alpha_orbitals = [f.copy() for f in alpha_orbitals]
         beta_orbitals = [f.copy() for f in beta_orbitals]
 
         function = BasisFunction([], [])
         for f in alpha_orbitals:
@@ -460,17 +457,15 @@
 
             operator_overlaps_beta = get_overlaps(beta_orbitals)
             total_state = pd.Series(operator_overlaps_beta, index=self._pg.op_labels)
             super().__init__(group, self._coordinates, self._symbols, total_state, self._angles, [0, 0, 0])
 
 
 class SymmetryWaveFunctionCI(SymmetryMoleculeBase):
-    def __init__(self, group, orbitals,
-                 configurations,
-                 center=None, orientation_angles=None):
+    def __init__(self, group, orbitals, configurations, orientation_angles=None, center=None):
 
         # generate copy to not modify original orbitals
         orbitals = [f.copy() for f in orbitals]
 
         function = BasisFunction([], [])
         for f in orbitals:
             function = function + f
```

### Comparing `posym-0.5.3/posym/algebra.py` & `posym-0.5.4/posym/algebra.py`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/posym/basis.py` & `posym-0.5.4/posym/basis.py`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/posym/generate_tables.py` & `posym-0.5.4/posym/generate_tables.py`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/posym/ir_tables.py` & `posym-0.5.4/posym/ir_tables.py`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/posym/operations/__init__.py` & `posym-0.5.4/posym/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/posym/operations/identity.py` & `posym-0.5.4/posym/operations/identity.py`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/posym/operations/inversion.py` & `posym-0.5.4/posym/operations/inversion.py`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/posym/operations/irotation.py` & `posym-0.5.4/posym/operations/irotation.py`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/posym/operations/reflection.py` & `posym-0.5.4/posym/operations/reflection.py`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/posym/operations/rotation.py` & `posym-0.5.4/posym/operations/rotation.py`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/posym/pointgroup.py` & `posym-0.5.4/posym/pointgroup.py`

 * *Files identical despite different names*

### Comparing `posym-0.5.3/posym/tools.py` & `posym-0.5.4/posym/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,20 +75,27 @@
     orbital = BasisFunction([], [])
     for mo_coeff, basis in zip(mo_coefficients, basis_set):
         orbital += mo_coeff * basis
 
     return orbital
 
 
-def get_basis_set(coordinates, basis_set, use_angstrom=True):
+def get_basis_set(coordinates, basis, use_angstrom=True):
+    """
+    get list of basis functions (basis_set) from pyQchem formatted basis dictionary
+    :param coordinates: list/array of atom positions
+    :param basis: pyQchem basis dictionary
+    :param use_angstrom: if True, coordinates are provided in angstrom else Bohr
+    :return: list of BasisFunction objects
+    """
     if use_angstrom:
         coordinates = np.array(coordinates)*1.8897259886  # convert from Angstrom to bohr
 
     basis_list = []
-    for iatom, atom in enumerate(basis_set['atoms']):
+    for iatom, atom in enumerate(basis['atoms']):
         for shell in atom['shells']:
             if shell['shell_type'] == 's':
                 primitives = []
                 for exponent in shell['p_exponents']:
                     primitives.append(PrimitiveGaussian(alpha=exponent))
 
                 basis_list.append(BasisFunction(primitives, shell['con_coefficients'],
```

### Comparing `posym-0.5.3/posym.egg-info/PKG-INFO` & `posym-0.5.4/posym.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posym
-Version: 0.5.3
+Version: 0.5.4
 Summary: posym module
 Home-page: https://github.com/abelcarreras/posym
 Author: Abel Carreras
 Author-email: abelcarreras83@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `posym-0.5.3/setup.py` & `posym-0.5.4/setup.py`

 * *Files identical despite different names*

