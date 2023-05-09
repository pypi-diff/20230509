# Comparing `tmp/rad-tools-0.5.9.tar.gz` & `tmp/rad-tools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.5.9.tar", last modified: Fri Mar  3 15:58:13 2023, max compression
+gzip compressed data, was "rad-tools-0.6.0.tar", last modified: Tue May  9 00:29:06 2023, max compression
```

## Comparing `rad-tools-0.5.9.tar` & `rad-tools-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,48 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.609304 rad-tools-0.5.9/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.5.9/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1230 2023-03-03 15:58:13.608927 rad-tools-0.5.9/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      545 2022-11-15 22:40:46.000000 rad-tools-0.5.9/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.584511 rad-tools-0.5.9/rad_tools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       60 2023-03-03 15:56:31.000000 rad-tools-0.5.9/rad_tools/__init__.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.593174 rad-tools-0.5.9/rad_tools/exchange/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      196 2023-02-23 16:19:10.000000 rad-tools-0.5.9/rad_tools/exchange/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7583 2023-02-24 16:56:38.000000 rad-tools-0.5.9/rad_tools/exchange/bond.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    27284 2023-02-24 17:23:45.000000 rad-tools-0.5.9/rad_tools/exchange/model.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1171 2022-12-15 15:38:31.000000 rad-tools-0.5.9/rad_tools/exchange/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.595674 rad-tools-0.5.9/rad_tools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      149 2023-01-18 13:16:00.000000 rad-tools-0.5.9/rad_tools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1928 2022-12-15 15:43:18.000000 rad-tools-0.5.9/rad_tools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3944 2023-02-24 16:56:38.000000 rad-tools-0.5.9/rad_tools/io/tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.598597 rad-tools-0.5.9/rad_tools/kpoints/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      600 2023-02-23 16:19:10.000000 rad-tools-0.5.9/rad_tools/kpoints/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    29021 2023-02-23 16:19:10.000000 rad-tools-0.5.9/rad_tools/kpoints/high_symmetry_point.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3775 2023-02-23 16:19:10.000000 rad-tools-0.5.9/rad_tools/kpoints/kpoints.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1357 2022-12-15 17:25:30.000000 rad-tools-0.5.9/rad_tools/map.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     6817 2023-02-24 16:56:38.000000 rad-tools-0.5.9/rad_tools/routines.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.601355 rad-tools-0.5.9/rad_tools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      266 2023-02-24 16:56:38.000000 rad-tools-0.5.9/rad_tools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    38005 2023-03-03 15:47:48.000000 rad-tools-0.5.9/rad_tools/score/rad_dos_plotter_core.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5097 2023-03-03 13:21:07.000000 rad-tools-0.5.9/rad_tools/score/rad_make_template_core.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5474 2023-03-03 13:20:04.000000 rad-tools-0.5.9/rad_tools/score/tb2j_extractor_core.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    10167 2023-03-03 13:16:39.000000 rad-tools-0.5.9/rad_tools/score/tb2j_plotter_core.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.588383 rad-tools-0.5.9/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1230 2023-03-03 15:58:13.000000 rad-tools-0.5.9/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      927 2023-03-03 15:58:13.000000 rad-tools-0.5.9/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-03-03 15:58:13.000000 rad-tools-0.5.9/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       17 2023-03-03 15:58:13.000000 rad-tools-0.5.9/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       10 2023-03-03 15:58:13.000000 rad-tools-0.5.9/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.607980 rad-tools-0.5.9/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3167 2023-02-23 16:19:10.000000 rad-tools-0.5.9/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5014 2023-03-03 14:19:40.000000 rad-tools-0.5.9/scripts/identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3051 2023-02-23 16:19:10.000000 rad-tools-0.5.9/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      207 2023-03-03 00:32:48.000000 rad-tools-0.5.9/scripts/rad-dos-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      209 2023-02-24 16:56:38.000000 rad-tools-0.5.9/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      206 2023-02-24 16:56:38.000000 rad-tools-0.5.9/scripts/tb2j-extractor.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      204 2023-02-24 16:56:38.000000 rad-tools-0.5.9/scripts/tb2j-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-03-03 15:58:13.609394 rad-tools-0.5.9/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1369 2023-02-23 16:19:10.000000 rad-tools-0.5.9/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-09 00:29:06.049432 rad-tools-0.6.0/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.6.0/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2840 2023-05-09 00:29:06.048835 rad-tools-0.6.0/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2123 2023-05-09 00:12:40.000000 rad-tools-0.6.0/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-09 00:29:05.959755 rad-tools-0.6.0/rad_tools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      613 2023-05-09 00:15:00.000000 rad-tools-0.6.0/rad_tools/__init__.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-09 00:29:05.974783 rad-tools-0.6.0/rad_tools/dos/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/dos/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    21740 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/dos/dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    22059 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/dos/pdos.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-09 00:29:05.980888 rad-tools-0.6.0/rad_tools/exchange/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/exchange/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7428 2023-05-07 21:38:27.000000 rad-tools-0.6.0/rad_tools/exchange/bond.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    27641 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/exchange/model.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1196 2023-03-30 12:48:24.000000 rad-tools-0.6.0/rad_tools/exchange/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-09 00:29:05.985855 rad-tools-0.6.0/rad_tools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      549 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1956 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4042 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/io/tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-09 00:29:05.988981 rad-tools-0.6.0/rad_tools/kpoints/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      616 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/kpoints/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    30577 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/kpoints/high_symmetry_point.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3626 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/kpoints/kpoints.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-03-30 12:48:24.000000 rad-tools-0.6.0/rad_tools/map.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     6315 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/routines.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-09 00:29:05.996356 rad-tools-0.6.0/rad_tools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1584 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4511 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/score/extract_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4054 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/score/identify_wannier_centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4758 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/score/make_template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    13305 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/score/plot_dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9921 2023-05-09 00:12:40.000000 rad-tools-0.6.0/rad_tools/score/plot_tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-09 00:29:05.971291 rad-tools-0.6.0/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2840 2023-05-09 00:29:05.000000 rad-tools-0.6.0/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1008 2023-05-09 00:29:05.000000 rad-tools-0.6.0/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-05-09 00:29:05.000000 rad-tools-0.6.0/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       22 2023-05-09 00:29:05.000000 rad-tools-0.6.0/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       10 2023-05-09 00:29:05.000000 rad-tools-0.6.0/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-05-09 00:29:06.039860 rad-tools-0.6.0/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.6.0/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.6.0/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      292 2023-05-09 00:12:40.000000 rad-tools-0.6.0/scripts/rad-extract-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      304 2023-05-09 00:12:40.000000 rad-tools-0.6.0/scripts/rad-identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      293 2023-05-09 00:12:40.000000 rad-tools-0.6.0/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      288 2023-05-09 00:12:40.000000 rad-tools-0.6.0/scripts/rad-plot-dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      289 2023-05-09 00:12:40.000000 rad-tools-0.6.0/scripts/rad-plot-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-05-09 00:29:06.049565 rad-tools-0.6.0/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1400 2023-05-09 00:12:40.000000 rad-tools-0.6.0/setup.py
```

### Comparing `rad-tools-0.5.9/LICENSE.txt` & `rad-tools-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.9/rad_tools/exchange/bond.py` & `rad-tools-0.6.0/rad_tools/exchange/bond.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,60 +7,56 @@
 import numpy as np
 
 
 class Bond:
     r"""
     Exchange bond.
 
-    If ``matrix`` is specified then ``iso``, ``aniso`` and ``dmi`` are 
-    ignored and derived from ``matrix``. If ``matrix`` is not specified 
-    then it is derived from ``iso``, ``aniso`` and ``dmi``. 
+    If ``matrix`` is specified then ``iso``, ``aniso`` and ``dmi`` are
+    ignored and derived from ``matrix``. If ``matrix`` is not specified
+    then it is derived from ``iso``, ``aniso`` and ``dmi``.
     If nothing is provided exchange matrix is set to zero matrix.
 
     Parameters
     ----------
     iso : int or float, default None
         Value of isotropic exchange parameter.
     aniso : 3 x 3 array, None
         3 x 3 matrix of symmetric anisotropic exchange.
     dmi : 1 x 3 array, None
         Dzyaroshinsky-Moria interaction vector :math:`(D_x, D_y, D_z)`.
     matrix : 3 x 3 array, None
-        Exchange matrix. 
+        Exchange matrix.
 
     Attributes
     ----------
     matrix : 3 x 3 array of floats
-        Exchange matrix. 
+        Exchange matrix.
 
         .. code-block:: python
 
             [[J_xx, J_xy, J_xz],
              [J_yx, J_yy, J_yz],
              [J_zx, J_zy, J_zz]]
 
     symm_matrix : 3 x 3 array of floats
     asymm_matrix : 3 x 3 array of floats
     iso : float
     iso_matrix : 3 x 3 array of floats
     aniso : 3 x 3 array of floats
-    aniso_diagonal : 1 x 3 array of floats 
-    aniso_diagonal_matrix : 3 x 3 array of floats 
+    aniso_diagonal : 1 x 3 array of floats
+    aniso_diagonal_matrix : 3 x 3 array of floats
     dmi : 1 x 3 array of floats
     dmi_matrix : 3 x 3 array of floats
     dmi_module : float
     """
 
-    def __init__(self,
-                 matrix=None,
-                 iso=None,
-                 aniso=None,
-                 dmi=None) -> None:
+    def __init__(self, matrix=None, iso=None, aniso=None, dmi=None) -> None:
         self._matrix = np.zeros((3, 3), dtype=float)
-        self._iso = 0.
+        self._iso = 0.0
         self._aniso = np.zeros((3, 3), dtype=float)
         self._dmi = np.zeros(3, dtype=float)
 
         if matrix is None:
             self.iso = iso
             self.dmi = dmi
             self.aniso = aniso
@@ -82,103 +78,103 @@
         self._matrix = new_matrix
 
     @property
     def symm_matrix(self):
         r"""
         Symmetric part of exchange matrix.
 
-        .. math:: 
+        .. math::
 
-            J_symm = \dfrac{J + J^T}{2}
+            J_{symm} = \dfrac{J + J^T}{2}
         """
 
         return (self.matrix + self.matrix.T) / 2
 
     @property
     def asymm_matrix(self):
         """
         Asymmetric part of exchange matrix.
 
-        .. math:: 
+        .. math::
 
-            J_asymm = \dfrac{J - J^T}{2}
+            J_{asymm} = \dfrac{J - J^T}{2}
         """
 
         return (self.matrix - self.matrix.T) / 2
 
     @property
     def iso(self):
         r"""
         Value of isotropic exchange parameter.
 
-        Derived from the exchange matrix (:math:`\mathbf{J}`) as 
+        Derived from the exchange matrix (:math:`\mathbf{J}`) as
 
         .. math::
             J_{iso} = \dfrac{1}{3}Tr(\mathbf{J})
         """
 
         return np.trace(self.symm_matrix) / 3
 
     @iso.setter
     def iso(self, new_iso):
         if new_iso is not None:
             # correction is correct (see matrix update)
             new_iso = new_iso - self.iso
         else:
             new_iso = -self.iso
-        self.matrix = (self.matrix + (new_iso) * np.identity(3, dtype=float))
+        self.matrix = self.matrix + (new_iso) * np.identity(3, dtype=float)
 
     @property
     def iso_matrix(self):
         r"""
         Isotropic part of the exchange matrix.
 
-        Matrix form: 
+        Matrix form:
 
         .. code-block:: python
 
             [[J, 0, 0],
              [0, J, 0],
              [0, 0, J]]
         """
 
         return self.iso * np.identity(3, dtype=float)
 
     @property
     def aniso(self):
         r"""
-        3 x 3 matrix of symmetric anisotropic exchange. 
+        3 x 3 matrix of symmetric anisotropic exchange.
 
         .. code-block:: python
 
             [[J_xx, J_xy, J_xz],
              [J_xy, J_yy, J_yz],
              [J_xz, J_yz, J_zz]]
 
-        Derived from the exchange matrix (:math:`\mathbf{J}`) as 
+        Derived from the exchange matrix (:math:`\mathbf{J}`) as
 
         .. math::
-            \mathbf{J}_{aniso} = \mathbf{J}_{symm} - \dfrac{1}{3}Tr(\mathbf{J}) \cdot \mathbf{I}
+            \mathbf{J}_{aniso} = \mathbf{J}_{symm} - \dfrac{1}{3}Tr(\mathbf{J})
+            \cdot \mathbf{I}
 
         where :math:`\mathbf{I}` is a :math:`3\times3` identity matrix.
         """
 
         return self.symm_matrix - self.iso * np.identity(3, dtype=float)
 
     @aniso.setter
     def aniso(self, new_aniso):
         if new_aniso is not None:
             new_aniso = np.array(new_aniso, dtype=float)
             if new_aniso.shape != (3, 3):
-                raise ValueError("Aniso matrix shape have " +
-                                 "to be equal to (3, 3)")
+                raise ValueError("Aniso matrix shape have " + "to be equal to (3, 3)")
             # correction is correct (see matrix update)
             new_aniso = new_aniso - self.aniso
         else:
-            new_aniso = - self.aniso
+            new_aniso = -self.aniso
         self.matrix = self.matrix + new_aniso
 
     @property
     def aniso_diagonal(self):
         r"""
         Diagonal part of the symmetric anisotropic exchange.
 
@@ -202,46 +198,49 @@
         """
 
         return np.diag(np.diag(self.aniso))
 
     @property
     def dmi(self):
         r"""
-        Dzyaroshinsky-Moria interaction vector (Dx, Dy, Dz). 
+        Dzyaroshinsky-Moria interaction vector (Dx, Dy, Dz).
 
         .. code-block:: python
 
             [D_x, D_y, D_z]
         """
 
-        return np.array([self.asymm_matrix[1][2],
-                         self.asymm_matrix[2][0],
-                         self.asymm_matrix[0][1]],
-                        dtype=float)
+        return np.array(
+            [self.asymm_matrix[1][2], self.asymm_matrix[2][0], self.asymm_matrix[0][1]],
+            dtype=float,
+        )
 
     @dmi.setter
     def dmi(self, new_dmi):
         if new_dmi is not None:
             new_dmi = np.array(new_dmi, dtype=float)
             if new_dmi.shape != (3,):
-                raise ValueError(
-                    f"DMI have to be a 3 component vector. {new_dmi}")
+                raise ValueError(f"DMI have to be a 3 component vector. {new_dmi}")
             new_dmi = new_dmi - self.dmi
         else:
             new_dmi = -self.dmi
-        dmi_matrix = np.array([[0, new_dmi[2], -new_dmi[1]],
-                               [-new_dmi[2], 0, new_dmi[0]],
-                               [new_dmi[1], -new_dmi[0], 0]],
-                              dtype=float)
+        dmi_matrix = np.array(
+            [
+                [0, new_dmi[2], -new_dmi[1]],
+                [-new_dmi[2], 0, new_dmi[0]],
+                [new_dmi[1], -new_dmi[0], 0],
+            ],
+            dtype=float,
+        )
         self.matrix = self.matrix + dmi_matrix
 
     @property
     def dmi_matrix(self):
         r"""
-        Assymetric part of the exchange matrix.
+        Asymmetric part of the exchange matrix.
 
         .. code-block:: python
 
             [[0, D_z, -D_y],
              [-D_z, 0, D_x],
              [D_y, -D_x, 0]]
         """
```

### Comparing `rad-tools-0.5.9/rad_tools/exchange/model.py` & `rad-tools-0.6.0/rad_tools/exchange/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 r"""
 Exchange model.
 
 Write a tutorial with docstrings here.
 """
 
 from copy import deepcopy
-from math import sqrt, pi, cos, sin
+from math import cos, pi, sin, sqrt
 
 import numpy as np
 
-from rad_tools.exchange.template import ExchangeTemplate
 from rad_tools.exchange.bond import Bond
+from rad_tools.exchange.template import ExchangeTemplate
 
 
 class ExchangeModel:
     r"""
     Main entry point for the exchange model.
 
     Attributes
@@ -24,15 +24,15 @@
 
         .. code-block:: python
 
             {(Atom_1, Atom_2, R): bond, ...}
     magnetic_atoms : dict
         Dictionary with keys : str - marks of atoms and value : 1 x 3 array
         - coordinate of the atom in Angstroms.
-    noomagnetic_atoms : dist
+    nonmagnetic_atoms : dist
         Dictionary with keys : str - marks of atoms and value : 1 x 3 array
         - coordinate of the atom in Angstroms. Only non-magnetic atoms.
     cell : 3 x 3 array of floats
     a : 3 x 1 array
     b : 3 x 1 array
     c : 3 x 1 array
     len_a : float
@@ -70,30 +70,30 @@
 
         .. code-block:: python
 
             [[a_x  a_y  a_z],
              [b_x  b_y  b_z],
              [c_x  x_y  c_z]]
 
-        Default cell is orthonormal.
+        Default cell is orthonormal:
 
         .. code-block:: python
 
             np.identity(3, dtype=float)
         """
 
         return self._cell
 
     @cell.setter
     def cell(self, new_cell):
         new_cell = np.array(new_cell)
         if new_cell.shape != (3, 3):
             raise ValueError("Cell matrix shape have to be equal (3, 3)")
         if np.linalg.det(new_cell) == 0:
-            raise ValueError("Lattice vectors are complanar.")
+            raise ValueError("Lattice vectors are coplanar.")
         self._cell = new_cell
 
     @property
     def a(self):
         r"""
         First lattice vector :math:`\vec{a} = (a_x, a_y, a_z)`.
         """
@@ -226,32 +226,33 @@
         Returns
         -------
         cells : n x 3 array
             Array of n unit cells.
         """
 
         cells = set()
-        for atom1, atom2, R in self.bonds:
+        for atom1, atom2, R in self:
             cells.add(R)
         return np.array(list(cells))
 
     @property
     def number_spins_in_unit_cell(self):
         r"""
         Number of spins (or magnetic atoms) in the unit cell.
         """
 
         return len(self.magnetic_atoms)
 
     @property
     def space_dimensions(self):
         r"""
-        Model minimum and maximum coordiantes in real space.
+        Model minimum and maximum coordinates in real space.
 
-        Takes into account only an atom which has at least one bond associated with it.
+        Takes into account only an atom which has at least
+        one bond associated with it.
 
         Returns
         -------
         x_min : float
             Minimum x coordinate.
         y_min : float
             Minimum y coordinate.
@@ -263,15 +264,15 @@
             Maximum y coordinate.
         z_max : float
             Maximum z coordinate.
         """
 
         x_max, y_max, z_max = None, None, None
         x_min, y_min, z_min = None, None, None
-        for atom1, atom2, R in self.bonds:
+        for atom1, atom2, R in self:
             x1, y1, z1 = self.get_atom_coordinates(atom1)
             x2, y2, z2 = self.get_atom_coordinates(atom2, R)
             if x_max is None:
                 x_min, y_min, z_min = x1, y1, z1
                 x_max, y_max, z_max = x1, y1, z1
             x_max = max(x1, x2, x_max)
             y_max = max(y1, y2, y_max)
@@ -286,16 +287,16 @@
 
         Parameters
         ----------
         decimals : int, default 4
             Number of decimals after the comma.
         """
 
-        for atom1, atom2, R in self.bonds:
-            self.bonds[(atom1, atom2, R)].round(decimals)
+        for atom1, atom2, R in self:
+            self[(atom1, atom2, R)].round(decimals)
 
     def add_bond(self, bond: Bond, atom1, atom2, R):
         r"""
         Add one bond to the model.
 
         Parameters
         ----------
@@ -303,15 +304,16 @@
             An instance of :py:class:`Bond` class with the information about
             exchange parameters.
         atom1 : str
             Name of atom1 in (0, 0, 0) unit cell.
         atom2 : str
             Name of atom2 in R unit cell.
         R : tuple of ints
-            Vector of the unit cell for atom2. In the relative coordinates in real space.
+            Vector of the unit cell for atom2.
+            In the relative coordinates in real space.
         """
 
         self.bonds[(atom1, atom2, R)] = bond
 
     def remove_bond(self, atom1, atom2, R):
         r"""
         Remove one bond from the model.
@@ -362,20 +364,20 @@
         name : str
             Mark for the atom.
         """
 
         bonds_for_removal = []
         if name in self.magnetic_atoms:
             del self.magnetic_atoms[name]
-        for atom1, atom2, R in self.bonds:
+        for atom1, atom2, R in self:
             if atom1 == name or atom2 == name:
                 bonds_for_removal.append((atom1, atom2, R))
 
         for bond in bonds_for_removal:
-            del self.bonds[bond]
+            self.remove_bond(*bond)
 
     def get_atom_coordinates(self, atom, R=(0, 0, 0)):
         r"""
         Getter for the atom coordinates.
 
         Parameters
         ----------
@@ -459,21 +461,19 @@
 
         Returns
         -------
         distance : floats
             Distance between atom1 and atom2.
         """
 
-        return sqrt(np.sum(self.get_bond_vector(atom1, atom2, R)**2))
+        return sqrt(np.sum(self.get_bond_vector(atom1, atom2, R) ** 2))
 
-    def filter(self,
-               max_distance=None,
-               min_distance=None,
-               template=None,
-               R_vector=None):
+    def filter(
+        self, max_distance=None, min_distance=None, template=None, R_vector=None
+    ):
         r"""
         Filter the exchange entries based on the given conditions.
 
         The result will be defined by logical conjugate of the conditions.
         Saying so the filtering will be performed for each given condition
         one by one.
 
@@ -505,16 +505,15 @@
                 R_vector = {R_vector}
             elif type(R_vector) == list:
                 R_vector = set(R_vector)
             else:
                 raise TypeError("Type is not supported, supported: list.")
 
         bonds_for_removal = set()
-        for atom1, atom2, R in self.bonds:
-
+        for atom1, atom2, R in self:
             dis = self.get_distance(atom1, atom2, R)
 
             if max_distance is not None and dis > max_distance:
                 bonds_for_removal.add((atom1, atom2, R))
 
             if min_distance is not None and dis < min_distance:
                 bonds_for_removal.add((atom1, atom2, R))
@@ -523,28 +522,49 @@
                 bonds_for_removal.add((atom1, atom2, R))
             if template is not None and (atom1, atom2, R) not in template:
                 bonds_for_removal.add((atom1, atom2, R))
 
         for atom1, atom2, R in bonds_for_removal:
             self.remove_bond(atom1, atom2, R)
 
-    def filtered(self,
-                 max_distance=None,
-                 min_distance=None,
-                 template=None,
-                 R_vector=None):
+    def remove(self, template):
+        r"""
+        Remove bonds from the exchange model, based on the template.
+
+
+        .. note::
+            This method modifies the instance at which it is called.
+
+        Parameters
+        ----------
+        template : list or :py:class:`.ExchangeTemplate`.
+            List of pairs, which will remain in the model. ::
+
+                [(atom1, atom2, R), ...]
+        """
+
+        if isinstance(template, ExchangeTemplate):
+            template = template.get_list()
+        template = set(template)
+
+        for atom1, atom2, R in template:
+            self.remove_bond(atom1, atom2, R)
+
+    def filtered(
+        self, max_distance=None, min_distance=None, template=None, R_vector=None
+    ):
         r"""
         Create filtered exchange model based on the given conditions.
 
         The result will be defined by logical conjugate of the conditions.
         Saying so the filtering will be performed for each given condition
         one by one.
         Note: this method is not modifying the instance at which it is called.
-        It will create a new instance with sorted :py:attr:`bonds` and all the other
-        attributes will be copied (through :py:func:`deepcopy`).
+        It will create a new instance with sorted :py:attr:`bonds` and all
+        the other attributes will be copied (through :py:func:`deepcopy`).
 
         .. note::
             This method is not modifying the instance at which it is called.
             It will create a new instance with merged ``bonds`` and all the
             other attributes will be copied (through deepcopy).
 
         Parameters
@@ -565,18 +585,20 @@
         Returns
         -------
         filtered_model : :py:class:`.ExchangeModel`
             Exchange model after filtering.
         """
 
         filtered_model = deepcopy(self)
-        filtered_model.filter(max_distance=max_distance,
-                              min_distance=min_distance,
-                              template=template,
-                              R_vector=R_vector)
+        filtered_model.filter(
+            max_distance=max_distance,
+            min_distance=min_distance,
+            template=template,
+            R_vector=R_vector,
+        )
         return filtered_model
 
     def force_symmetry(self, template):
         r"""
         Force the model to have the symmetries of the template.
 
         Takes mean values of the parameters.
@@ -597,28 +619,26 @@
         self.filter(template=template)
 
         for name in template.names:
             bonds = template.names[name]
             symm_matrix = np.zeros((3, 3), dtype=float)
             dmi_module = 0
             for bond in bonds:
-                symm_matrix = (symm_matrix +
-                               self.bonds[bond].symm_matrix)
-                dmi_module = dmi_module + self.bonds[bond].dmi_module
+                symm_matrix = symm_matrix + self[bond].symm_matrix
+                dmi_module = dmi_module + self[bond].dmi_module
 
             symm_matrix = symm_matrix / len(bonds)
             dmi_module = dmi_module / len(bonds)
 
             for bond in bonds:
-                if self.bonds[bond].dmi_module != 0:
-                    asymm_factor = dmi_module / self.bonds[bond].dmi_module
+                if self[bond].dmi_module != 0:
+                    asymm_factor = dmi_module / self[bond].dmi_module
                 else:
                     asymm_factor = 0
-                self.bonds[bond].matrix = (symm_matrix +
-                                           self.bonds[bond].asymm_matrix * asymm_factor)
+                self[bond].matrix = symm_matrix + self[bond].asymm_matrix * asymm_factor
 
     def forced_symmetry(self, template):
         r"""
         Force the model to have the symmetries of the template.
 
         Takes mean values of the parameters.
         Respect the direction of the DMI vectors.
@@ -636,44 +656,46 @@
             Exchange model with forced symmetry.
         """
 
         new_model = deepcopy(self)
         new_model.force_symmetry(template=template)
         return new_model
 
-    def summary_as_txt(self,
-                       template: ExchangeTemplate,
-                       decimals=4,
-                       force_symmetry=False,
-                       isotropic=False,
-                       anisotropic=False,
-                       out_matrix=False,
-                       out_dmi=False):
+    def summary_as_txt(
+        self,
+        template: ExchangeTemplate,
+        decimals=4,
+        force_symmetry=False,
+        isotropic=False,
+        anisotropic=False,
+        out_matrix=False,
+        out_dmi=False,
+    ):
         r"""
         Return exchange model based on the template file in .txt format.
 
         Parameters
         ----------
         template : :py:class:`.ExchangeTemplate`
             Template of the desired exchange model.
             (see :ref:`rad-make-template`)
         accuracy : int, default 4
             Accuracy for the exchange values
         force_symmetry: bool, default False
-            Whenever to force the symmetry of the template exchange model.
+            Whether to force the symmetry of the template exchange model.
             If ``False`` then each individual bond is written, otherwise
             exchange parameters of the template model are written.
         isotropic : bool, default False
-            Whenever to output isotropic exchange.
+            Whether to output isotropic exchange.
         anisotropic : bool, default False
-            Whenever to output anisotropic exchange.
+            Whether to output anisotropic exchange.
         out_matrix : bool, default False
-            Whenever to output whole matrix exchange.
+            Whether to output whole matrix exchange.
         out_dmi : bool, default False
-            Whenever to output DMI exchange.
+            Whether to output DMI exchange.
 
         Returns
         -------
         summary : str
             Exchange information as a string.
         """
 
@@ -683,105 +705,110 @@
             self.filter(template=template)
         self.round(decimals=decimals)
         summary = ""
         for name in template.names:
             scalar_written = False
             for atom1, atom2, R in template.names[name]:
                 # Get values from the model
-                bond = self.bonds[(atom1, atom2, R)]
-                if not isinstance(bond, Bond):
-                    raise TypeError
+                bond = self[(atom1, atom2, R)]
                 iso = bond.iso
                 aniso = bond.aniso
                 dmi = bond.dmi
                 abs_dmi = bond.dmi_module
-                rel_dmi = abs_dmi/iso
+                rel_dmi = abs_dmi / iso
                 matrix = bond.matrix
 
                 if not force_symmetry:
-
                     # Write the values
                     summary += (
-                        f"{atom1:3} {atom2:3} " +
-                        f"({R[0]:2.0f}, {R[1]:2.0f}, {R[2]:2.0f})\n")
+                        f"{atom1:3} {atom2:3} "
+                        + f"({R[0]:2.0f}, {R[1]:2.0f}, {R[2]:2.0f})\n"
+                    )
                     if isotropic:
                         summary += f"    Isotropic: {iso:.{decimals}f}\n"
                     if anisotropic:
                         summary += (
-                            f"    Anisotropic:\n" +
-                            f"        {aniso[0][0]:{decimals+3}.{decimals}f}  " +
-                            f"{aniso[0][1]:{decimals+3}.{decimals}f}  " +
-                            f"{aniso[0][2]:{decimals+3}.{decimals}f}\n" +
-                            f"        {aniso[1][0]:{decimals+3}.{decimals}f}  " +
-                            f"{aniso[1][1]:{decimals+3}.{decimals}f}  " +
-                            f"{aniso[1][2]:{decimals+3}.{decimals}f}\n" +
-                            f"        {aniso[2][0]:{decimals+3}.{decimals}f}  " +
-                            f"{aniso[2][1]:{decimals+3}.{decimals}f}  " +
-                            f"{aniso[2][2]:{decimals+3}.{decimals}f}\n")
+                            f"    Anisotropic:\n"
+                            + f"        {aniso[0][0]:{decimals+3}.{decimals}f}  "
+                            + f"{aniso[0][1]:{decimals+3}.{decimals}f}  "
+                            + f"{aniso[0][2]:{decimals+3}.{decimals}f}\n"
+                            + f"        {aniso[1][0]:{decimals+3}.{decimals}f}  "
+                            + f"{aniso[1][1]:{decimals+3}.{decimals}f}  "
+                            + f"{aniso[1][2]:{decimals+3}.{decimals}f}\n"
+                            + f"        {aniso[2][0]:{decimals+3}.{decimals}f}  "
+                            + f"{aniso[2][1]:{decimals+3}.{decimals}f}  "
+                            + f"{aniso[2][2]:{decimals+3}.{decimals}f}\n"
+                        )
                     if out_matrix:
                         summary += (
-                            f"    Matrix:\n" +
-                            f"        {matrix[0][0]:{decimals+3}.{decimals}f}  " +
-                            f"{matrix[0][1]:{decimals+3}.{decimals}f}  " +
-                            f"{matrix[0][2]:{decimals+3}.{decimals}f}\n" +
-                            f"        {matrix[1][0]:{decimals+3}.{decimals}f}  " +
-                            f"{matrix[1][1]:{decimals+3}.{decimals}f}  " +
-                            f"{matrix[1][2]:{decimals+3}.{decimals}f}\n" +
-                            f"        {matrix[2][0]:{decimals+3}.{decimals}f}  " +
-                            f"{matrix[2][1]:{decimals+3}.{decimals}f}  " +
-                            f"{matrix[2][2]:{decimals+3}.{decimals}f}\n")
+                            f"    Matrix:\n"
+                            + f"        {matrix[0][0]:{decimals+3}.{decimals}f}  "
+                            + f"{matrix[0][1]:{decimals+3}.{decimals}f}  "
+                            + f"{matrix[0][2]:{decimals+3}.{decimals}f}\n"
+                            + f"        {matrix[1][0]:{decimals+3}.{decimals}f}  "
+                            + f"{matrix[1][1]:{decimals+3}.{decimals}f}  "
+                            + f"{matrix[1][2]:{decimals+3}.{decimals}f}\n"
+                            + f"        {matrix[2][0]:{decimals+3}.{decimals}f}  "
+                            + f"{matrix[2][1]:{decimals+3}.{decimals}f}  "
+                            + f"{matrix[2][2]:{decimals+3}.{decimals}f}\n"
+                        )
                     if out_dmi:
                         summary += (
-                            f"    |DMI|: {abs_dmi:.{decimals}f}\n" +
-                            f"    |DMI/J|: {rel_dmi:.{decimals}f}\n" +
-                            f"    DMI: {dmi[0]:.{decimals}f} " +
-                            f"{dmi[1]:.{decimals}f} " +
-                            f"{dmi[2]:.{decimals}f}\n")
+                            f"    |DMI|: {abs_dmi:.{decimals}f}\n"
+                            + f"    |DMI/J|: {rel_dmi:.{decimals}f}\n"
+                            + f"    DMI: {dmi[0]:.{decimals}f} "
+                            + f"{dmi[1]:.{decimals}f} "
+                            + f"{dmi[2]:.{decimals}f}\n"
+                        )
                     summary += "\n"
                 else:
                     if not scalar_written:
                         scalar_written = True
                         summary += f"{name}\n"
                         if isotropic:
                             summary += f"    Isotropic: {iso:.{decimals}f}\n"
                         if anisotropic:
                             summary += (
-                                f"    Anisotropic:\n" +
-                                f"        {aniso[0][0]:{decimals+3}.{decimals}f}  " +
-                                f"{aniso[0][1]:{decimals+3}.{decimals}f}  " +
-                                f"{aniso[0][2]:{decimals+3}.{decimals}f}\n" +
-                                f"        {aniso[1][0]:{decimals+3}.{decimals}f}  " +
-                                f"{aniso[1][1]:{decimals+3}.{decimals}f}  " +
-                                f"{aniso[1][2]:{decimals+3}.{decimals}f}\n" +
-                                f"        {aniso[2][0]:{decimals+3}.{decimals}f}  " +
-                                f"{aniso[2][1]:{decimals+3}.{decimals}f}  " +
-                                f"{aniso[2][2]:{decimals+3}.{decimals}f}\n")
+                                f"    Anisotropic:\n"
+                                + f"        {aniso[0][0]:{decimals+3}.{decimals}f}  "
+                                + f"{aniso[0][1]:{decimals+3}.{decimals}f}  "
+                                + f"{aniso[0][2]:{decimals+3}.{decimals}f}\n"
+                                + f"        {aniso[1][0]:{decimals+3}.{decimals}f}  "
+                                + f"{aniso[1][1]:{decimals+3}.{decimals}f}  "
+                                + f"{aniso[1][2]:{decimals+3}.{decimals}f}\n"
+                                + f"        {aniso[2][0]:{decimals+3}.{decimals}f}  "
+                                + f"{aniso[2][1]:{decimals+3}.{decimals}f}  "
+                                + f"{aniso[2][2]:{decimals+3}.{decimals}f}\n"
+                            )
                         if out_matrix:
                             summary += (
-                                f"    Matrix:\n" +
-                                f"        {matrix[0][0]:{decimals+3}.{decimals}f}  " +
-                                f"{matrix[0][1]:{decimals+3}.{decimals}f}  " +
-                                f"{matrix[0][2]:{decimals+3}.{decimals}f}\n" +
-                                f"        {matrix[1][0]:{decimals+3}.{decimals}f}  " +
-                                f"{matrix[1][1]:{decimals+3}.{decimals}f}  " +
-                                f"{matrix[1][2]:{decimals+3}.{decimals}f}\n" +
-                                f"        {matrix[2][0]:{decimals+3}.{decimals}f}  " +
-                                f"{matrix[2][1]:{decimals+3}.{decimals}f}  " +
-                                f"{matrix[2][2]:{decimals+3}.{decimals}f}\n")
+                                f"    Matrix:\n"
+                                + f"        {matrix[0][0]:{decimals+3}.{decimals}f}  "
+                                + f"{matrix[0][1]:{decimals+3}.{decimals}f}  "
+                                + f"{matrix[0][2]:{decimals+3}.{decimals}f}\n"
+                                + f"        {matrix[1][0]:{decimals+3}.{decimals}f}  "
+                                + f"{matrix[1][1]:{decimals+3}.{decimals}f}  "
+                                + f"{matrix[1][2]:{decimals+3}.{decimals}f}\n"
+                                + f"        {matrix[2][0]:{decimals+3}.{decimals}f}  "
+                                + f"{matrix[2][1]:{decimals+3}.{decimals}f}  "
+                                + f"{matrix[2][2]:{decimals+3}.{decimals}f}\n"
+                            )
                         if out_dmi:
                             summary += (
-                                f"    |DMI|: {abs_dmi:.{decimals}f}\n" +
-                                f"    |DMI/J|: {rel_dmi:.{decimals}f}\n")
+                                f"    |DMI|: {abs_dmi:.{decimals}f}\n"
+                                + f"    |DMI/J|: {rel_dmi:.{decimals}f}\n"
+                            )
                     if out_dmi:
                         summary += (
-                            f"    DMI: {dmi[0]:{decimals+3}.{decimals}f} " +
-                            f"{dmi[1]:{decimals+3}.{decimals}f} " +
-                            f"{dmi[2]:{decimals+3}.{decimals}f} " +
-                            f"({atom1:3} {atom2:3} " +
-                            f"{R[0]:2.0f} {R[1]:2.0f} {R[2]:2.0f})\n")
+                            f"    DMI: {dmi[0]:{decimals+3}.{decimals}f} "
+                            + f"{dmi[1]:{decimals+3}.{decimals}f} "
+                            + f"{dmi[2]:{decimals+3}.{decimals}f} "
+                            + f"({atom1:3} {atom2:3} "
+                            + f"{R[0]:2.0f} {R[1]:2.0f} {R[2]:2.0f})\n"
+                        )
             if force_symmetry:
                 summary += "\n"
 
         return summary
 
     def ferromagnetic_energy(self, theta=0, phi=0):
         r"""
@@ -789,53 +816,52 @@
 
         With Hamiltonian of the form:
 
         .. math::
 
             \hat{H} = - \sum_{i,j} \vec{S}_i J_{ij} \vec{S}_j
 
-        where spin vectors are normaized to 1 and :math:`J_{ij}` is the 
+        where spin vectors are normalized to 1 and :math:`J_{ij}` is the
         exchange matrix.
 
         Parameters
         ----------
         theta : float, default 0
             Angle between z axis an direction of the magnetization.
             :math:`0 < \theta < 180`
         phi : float, default 0
-            angle between x axis an projection of direction of the 
+            angle between x axis an projection of direction of the
             magnetization on xy plane.
             :math:`0 < \phi < 360`
 
         Returns
         -------
         energy : float
-            Energy of ferromagnetic model with magnetisation direction defined 
+            Energy of ferromagnetic model with magnetization direction defined
             by ``theta`` and ``phi``. In the units of J values.
         """
 
         theta = theta / 180 * pi
         phi = phi / 180 * pi
         energy = np.zeros((3, 3), dtype=float)
         for bond in self:
-            energy -= self.bonds[bond].matrix
-        spin_vector = np.array([cos(phi) * sin(theta),
-                                sin(phi) * sin(theta),
-                                cos(theta)])
+            energy -= self[bond].matrix
+        spin_vector = np.array(
+            [cos(phi) * sin(theta), sin(phi) * sin(theta), cos(theta)]
+        )
         energy = np.matmul(np.matmul(spin_vector, energy), spin_vector)
         return energy
 
 
 class ExchangeModelIterator:
-
     def __init__(self, exchange_model: ExchangeModel) -> None:
         self._bonds = list(exchange_model.bonds)
         self._index = 0
 
-    def __next__(self):
+    def __next__(self) -> Bond:
         if self._index < len(self._bonds):
             result = self._bonds[self._index]
             self._index += 1
             return result
         raise StopIteration
 
     def __iter__(self):
```

### Comparing `rad-tools-0.5.9/rad_tools/exchange/template.py` & `rad-tools-0.6.0/rad_tools/exchange/template.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 r"""
 Exchange template.
+
+Write a tutorial with docstrings here.
 """
 
 
 class ExchangeTemplate:
     r"""
     Store a template for sorting the exchange from TB2J file.
 
-    In addition stores the technical details for plotting, 
-    orbital decompozition, etc.
+    In addition stores the technical details for plotting,
+    orbital decomposition, etc.
 
     Attributes
     ----------
     names : dict
-        Dictionary of neighbours from the template file.
+        Dictionary of neighbors from the template file.
 
         .. code-block:: python
 
             {name : [(atom1, atom2, R), ...], ...}
 
     latex_names : dict
-        The dictionary of Letex version of names from `names`.
+        The dictionary of Latex version of names from `names`.
 
         .. code-block:: python
 
             {name : latex_name, ...}
     """
 
     def __init__(self) -> None:
-
         self.names = {}
         self.latex_names = {}
 
     def get_list(self):
         r"""
         Translate bonds present in the template into the list.
 
         Returns
         -------
-        plained_template : list
+        template_list : list
             List with the bond specifications:
 
             .. code-block:: python
 
                 [(atom_1, atom_2, R), ...]
         """
-        plained_template = []
+        template_list = []
         for name in self.names:
             for atom1, atom2, R in self.names[name]:
-                plained_template.append((atom1, atom2, R))
-        return plained_template
+                template_list.append((atom1, atom2, R))
+        return template_list
```

### Comparing `rad-tools-0.5.9/rad_tools/io/internal.py` & `rad-tools-0.6.0/rad_tools/io/internal.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,31 +3,37 @@
 """
 
 from rad_tools.exchange.template import ExchangeTemplate
 
 
 def read_template(filename):
     r"""
-    Read template from the template file.    
+    Read template from the template file.
+
 
     Parameters
     ----------
     filename : str
         Path to the template file.
 
     Returns
     -------
     template : :py:class:`.ExchangeTemplate`
         Exchange template.
+
+    Notes
+    -----
+    See also :ref:`Template specification <api>`
     """
+    # TODO change the link
 
     # Constants
-    major_sep = '=' * 20
-    minor_sep = '-' * 20
-    neighbors_flag = 'Neighbors template:'
+    major_sep = "=" * 20
+    minor_sep = "-" * 20
+    neighbors_flag = "Neighbors template:"
 
     template = ExchangeTemplate()
 
     with open(filename) as file:
         line = True
         while line:
             line = file.readline()
@@ -41,17 +47,15 @@
                         try:
                             latex_name = line.split()[1]
                         except IndexError:
                             latex_name = name
                         template.names[name] = []
                         template.latex_names[name] = latex_name
                         line = file.readline()
-                        while line and\
-                                minor_sep not in line and\
-                                major_sep not in line:
+                        while line and minor_sep not in line and major_sep not in line:
                             atom1 = line.split()[0]
                             atom2 = line.split()[1]
 
                             R = tuple(map(int, line.split()[2:]))
                             template.names[name].append((atom1, atom2, R))
                             line = file.readline()
                     if line and major_sep in line:
```

### Comparing `rad-tools-0.5.9/rad_tools/io/tb2j.py` & `rad-tools-0.6.0/rad_tools/io/tb2j.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 r"""
 Input-output from TB2J.
 """
 
 import numpy as np
 
-from rad_tools.exchange.model import ExchangeModel, Bond
+from rad_tools.exchange.model import Bond, ExchangeModel
 from rad_tools.routines import absolute_to_relative
 
 
 def read_exchange_model(filename, quiet=False) -> ExchangeModel:
     r"""
     Read exchange model from TB2J output file.
 
     Parameters
     ----------
     filename : str
         Path to the TB2J output file.
     quiet : bool, default True
-        Whenever to supress output.
+        Whether to suppress output.
 
-    Returns 
+    Returns
     -------
     model : :py:class:`.ExchangeModel`
-        Exchange model buid from TB2J file.
+        Exchange model build from TB2J file.
     """
 
-    major_sep = '=' * 90
-    minor_sep = '-' * 88
-    garbage = str.maketrans({'(': None,
-                             ')': None,
-                             '[': None,
-                             ']': None,
-                             ',': None,
-                             '\'': None})
-    cell_flag = 'Cell (Angstrom):'
-    atoms_flag = 'Atoms:'
-    atom_end_flag = 'Total'
-    exchange_flag = 'Exchange:'
-    iso_flag = 'J_iso:'
-    aniso_flag = 'J_ani:'
-    dmi_flag = 'DMI:'
+    major_sep = "=" * 90
+    minor_sep = "-" * 88
+    garbage = str.maketrans(
+        {"(": None, ")": None, "[": None, "]": None, ",": None, "'": None}
+    )
+    # Do not correct spelling, it is taken from TB2J.
+    cell_flag = "Cell (Angstrom):"
+    atoms_flag = "Atoms:"
+    atom_end_flag = "Total"
+    exchange_flag = "Exchange:"
+    iso_flag = "J_iso:"
+    aniso_flag = "J_ani:"
+    dmi_flag = "DMI:"
 
     file = open(filename, "r")
     model = ExchangeModel()
     line = True
     atoms = {}
 
     # Read everything before exchange
     while line:
         line = file.readline()
 
         # Read cell
         if line and cell_flag in line:
-            model.cell = np.array([
-                list(map(float, file.readline().split())),
-                list(map(float, file.readline().split())),
-                list(map(float, file.readline().split()))
-            ])
+            model.cell = np.array(
+                [
+                    list(map(float, file.readline().split())),
+                    list(map(float, file.readline().split())),
+                    list(map(float, file.readline().split())),
+                ]
+            )
 
         # Read atoms
         if line and atoms_flag in line:
             line = file.readline()
             line = file.readline()
             line = file.readline().split()
             while line and atom_end_flag not in line:
                 atoms[line[0]] = absolute_to_relative(
-                    model.cell, *tuple(map(float, line[1:4])))
+                    model.cell, *tuple(map(float, line[1:4]))
+                )
                 line = file.readline().split()
 
         # Check if the exchange section is reached
         if line and exchange_flag in line:
             break
 
     # Read exchange
@@ -89,19 +90,21 @@
 
             # Read isotropic exchange
             if line and iso_flag in line:
                 iso = float(line.split()[-1])
 
             # Read anisotropic exchange
             if line and aniso_flag in line:
-                aniso = np.array([
-                    list(map(float, file.readline().translate(garbage).split())),
-                    list(map(float, file.readline().translate(garbage).split())),
-                    list(map(float, file.readline().translate(garbage).split()))
-                ])
+                aniso = np.array(
+                    [
+                        list(map(float, file.readline().translate(garbage).split())),
+                        list(map(float, file.readline().translate(garbage).split())),
+                        list(map(float, file.readline().translate(garbage).split())),
+                    ]
+                )
 
             # Read DMI
             if line and dmi_flag in line:
                 dmi = tuple(map(float, line.translate(garbage).split()[-3:]))
 
         # Adding info from the exchange block to the ExchangeModel structure
         if atom1 not in model.magnetic_atoms:
@@ -109,15 +112,18 @@
         if atom2 not in model.magnetic_atoms:
             model.add_atom(atom2, *atoms[atom2])
         bond = Bond(iso=iso, aniso=aniso, dmi=dmi)
         model.add_bond(bond, atom1, atom2, R)
         computed_distance = model.get_distance(atom1, atom2, R)
         if abs(computed_distance - distance) > 0.001 and not quiet:
             print(
-                f"\nComputed distance is a different from the read one:\n  Computed: {computed_distance:.4f}\n  Read: {distance:.4f}\n")
+                f"\nComputed distance is a different from the read one:\n"
+                + f"  Computed: {computed_distance:.4f}\n  "
+                + f"Read: {distance:.4f}\n"
+            )
 
     # Fill non-magnetic atoms
     for atom in atoms:
         if atom not in model.magnetic_atoms:
             model.nonmagnetic_atoms[atom] = np.array(atoms[atom])
 
     return model
```

### Comparing `rad-tools-0.5.9/rad_tools/kpoints/__init__.py` & `rad-tools-0.6.0/rad_tools/kpoints/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 r"""
-Module for constracting the k-points paths and high-symmetry k-points [1]_. 
+Module for constructing the k-points paths and high-symmetry k-points [1]_. 
 
 Examples
 --------
 
 .. code-block:: python
 
     from rad_tools.kpoints import HighSymmetryPoints
 
     hexagonal = HighSymmetryPoints().hex()
 
 References
 ----------
 .. [1] 
     Setyawan, W. and Curtarolo, S., 2010. 
-    High-throughput electronic band structure calculations: Challenges and tools. 
+    High-throughput electronic band structure calculations: 
+    Challenges and tools. 
     Computational materials science, 49(2), pp.299-312.
 
     :DOI:`10.1016/j.commatsci.2010.05.010`
 """
 
-from rad_tools.kpoints.high_symmetry_point import HighSymmetryPoints
-from rad_tools.kpoints.kpoints import KPoints
+from .high_symmetry_point import HighSymmetryPoints
+from .kpoints import KPoints
+
+__all__ = ["HighSymmetryPoints", "KPoints"]
```

### Comparing `rad-tools-0.5.9/rad_tools/kpoints/kpoints.py` & `rad-tools-0.6.0/rad_tools/kpoints/kpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 
 class KPoints(HighSymmetryPoints):
     r"""
     K-points
     """
 
-    def __init__(self, kpoints=None, path=None) -> None:
-        super().__init__(kpoints, path)
+    def __init__(self, points=None, path=None) -> None:
+        super().__init__(points, path)
 
     @property
     def labels(self):
         r"""
         Labels of the high symmetry k points, ready to plot.
 
         Returns
@@ -38,31 +38,30 @@
     def labels_coordinates(self, b1=None, b2=None, b3=None):
         r"""
         Coordinates of the high symmetry k points.
 
         Returns
         -------
         coordinate_list : list of float
-            List of high symmetry k points coordinates in reciprocal space 
+            List of high symmetry k points coordinates in reciprocal space
             if ``b1``, ``b2``, ``b3`` are specified, in relative otherwise.
         """
 
-        coordinates_list = self.coordinates(
-            n=1, b1=b1, b2=b2, b3=b3, linear=True)
-        return np.concatenate(([coordinates_list[0]],
-                               coordinates_list[1:-1:2],
-                               [coordinates_list[-1]]))
+        coordinates_list = self.coordinates(n=1, b1=b1, b2=b2, b3=b3, linear=True)
+        return np.concatenate(
+            ([coordinates_list[0]], coordinates_list[1:-1:2], [coordinates_list[-1]])
+        )
 
     def coordinates(self, n=100, b1=None, b2=None, b3=None, linear=False):
         r"""
         Coordinates of all k points in the path.
 
-        Return coordinates in reciprocal space units if ``b1``, ``b2``, ``b3`` 
-        are specified, otherwise return in relative to the reciprocal 
-        lattice vectors coordinates. 
+        Return coordinates in reciprocal space units if ``b1``, ``b2``, ``b3``
+        are specified, otherwise return in relative to the reciprocal
+        lattice vectors coordinates.
 
         Parameters
         ----------
         n : int
             Number of k points between two high symmetry points + 1.
         b1 : 1 x 3 array
             First reciprocal lattice vector.
@@ -74,38 +73,35 @@
             Return linear coordinates for the plot.
 
         Returns
         -------
         k_points : N x 3 array
             Array of N total k points in the path.
 
-            :math:`N = i \cdot n`, 
+            :math:`N = i \cdot n`,
             where i - number of intervals between high symmetry k points.
         """
 
         point_list = []
         for i in range(0, len(self.path)):
             for j in range(1, len(self.path[i])):
-                first_point = self.kpoints[self.path[i][j-1]]
-                diff = (self.kpoints[self.path[i][j]] -
-                        self.kpoints[self.path[i][j-1]])
+                first_point = self.points[self.path[i][j - 1]]
+                diff = self.points[self.path[i][j]] - self.points[self.path[i][j - 1]]
 
                 # Move from relative to absolute coordinates
                 if b1 is not None and b2 is not None and b3 is not None:
-                    first_point = (first_point[0]*b1 +
-                                   first_point[1]*b2 +
-                                   first_point[2]*b3)
-                    diff = (diff[0]*b1 +
-                            diff[1]*b2 +
-                            diff[2]*b3)
+                    first_point = (
+                        first_point[0] * b1 + first_point[1] * b2 + first_point[2] * b3
+                    )
+                    diff = diff[0] * b1 + diff[1] * b2 + diff[2] * b3
                 # Move from (kx, ky, kz) to |k|
                 if linear:
-                    diff = sqrt(np.sum(np.array(diff)**2))
+                    diff = sqrt(np.sum(np.array(diff) ** 2))
                     if i == 0 and j == 1:
                         first_point = 0
                     else:
                         first_point = point_list[-1]
 
-                for step in range(0, n+1):
-                    point_list.append(first_point + step/n * diff)
+                for step in range(0, n + 1):
+                    point_list.append(first_point + step / n * diff)
 
         return np.array(point_list)
```

### Comparing `rad-tools-0.5.9/rad_tools/map.py` & `rad-tools-0.6.0/rad_tools/map.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 from tracemalloc import start
 
 
 class CalculationMap:
     r"""
     Mapper.
 
@@ -16,31 +14,28 @@
 
             {name : values, ...}
     """
 
     def __init__(self) -> None:
         self.parameters = {}
 
-    def add_parameter(self,
-                      name,
-                      values=None,
-                      range=None):
+    def add_parameter(self, name, values=None, range=None):
         r"""
         Add parameter to the class.
 
         Parameters
         ----------
-        name : str 
+        name : str
             The main identificator of the parameter.
         values : array-like
             Exact values of the parameter to be considered.
-        range : tuple 
-            Three numbers: start, stop, step. 
-            If ``values`` are not specified the ``range`` will be used to 
-            create them. If :math:`\vert stop - start\vert \ne n \cdot step`, 
+        range : tuple
+            Three numbers: start, stop, step.
+            If ``values`` are not specified the ``range`` will be used to
+            create them. If :math:`\vert stop - start\vert \ne n \cdot step`,
             where n - int, then the last point will be < `stop`.
         """
         if values is None:
             if range is None:
                 raise ValueError("Either values or range need to be specified")
             else:
                 values = []
```

### Comparing `rad-tools-0.5.9/rad_tools/routines.py` & `rad-tools-0.6.0/rad_tools/routines.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 r"""
 Collection of small routines and constants, 
 which may be used across the whole package.
 """
 
+import sys
+
+from math import asin, pi, sqrt
+
 import numpy as np
-from math import asin, sqrt, pi
 
-# Teminal colors
+# Terminal colours
 BLACK = "\u001b[30m"
 """
 ANSI escape code for black color of the text.
 """
 RED = "\u001b[31m"
 """
 ANSI escape code for red color of the text.
@@ -52,68 +55,140 @@
 ANSI escape code for ok messages.
 """
 ERROR = RED
 """
 ANSI escape code for errors.
 """
 
+__all__ = [
+    "get_named_colours",
+    "get_256_colours",
+    "cprint",
+    "atom_mark_to_latex",
+    "rot_angle",
+    "absolute_to_relative",
+    "winwait",
+]
+
+
+def get_named_colours(colour: str):
+    r"""
+    Get the colours for the terminal based on name.
+
+    Parameters
+    ----------
+    colour : str
+        Name of the colour.
+        Choices: black, red, green, yellow, blue, magenta, cyan, white.
+    """
+    colour_dict = {
+        "black": BLACK,
+        "red": RED,
+        "green": GREEN,
+        "yellow": YELLOW,
+        "blue": BLUE,
+        "magenta": MAGENTA,
+        "cyan": CYAN,
+        "white": WHITE,
+    }
+    colour = colour.lower()
+    if colour not in colour_dict:
+        return ""
+    return colour_dict[colour]
+
 
 def get_256_colours(n):
     r"""
     ANSI escape codes for terminal color with 256-colours support
-    (see: :ANSI:`wiki <>`).
+    (see: |ANSI|_).
 
     Parameters
     ----------
     n : int
         Integer from 0 to 255 to be mapped to colours.
 
     Returns
     -------
     str
         string with the ANSI escape code.
     """
 
     if type(n) != int or not 0 <= n <= 255:
-        raise ValueError(f'Integer n have to be in range 0 <= n <= 255. '
-                         f'You provided n = {n}, type<n> = {type(n)}')
-    return f'\033[38:5:{n}m'
+        raise ValueError(
+            f"Integer n have to be in range 0 <= n <= 255. "
+            f"You provided n = {n}, type<n> = {type(n)}"
+        )
+    return f"\033[38:5:{n}m"
+
+
+def cprint(*args, colour=None, **kwargs):
+    r"""
+    Add colour argument to the standard ``print()``.
+
+    Parameters
+    ----------
+    colour : str or int
+        Name or number for a colour. Number is used with the base of 256.
+        Name should comply with :py:func:`.get_named_colours`.
+
+    Example
+    -------
+    >>> import rad_tools as rad
+    >>> rad.cprint("Hellow world!", colour="green")
+    Hellow world!
+    >>> rad.cprint("Hellow world!", colour = 30)
+    Hellow world!
+    >>> rad.cprint("Hellow world!", colour=1342)
+    Hellow world!
+    """
+
+    if isinstance(colour, int):
+        colour = get_256_colours(colour % 256)
+    elif isinstance(colour, str):
+        colour = get_named_colours(colour)
+    else:
+        raise ValueError("Colour must be a string or integer")
+    if colour is not None:
+        print(colour, end="")
+    print(*args, **kwargs)
+    if colour is not None:
+        print(RESET, end="")
 
 
 def atom_mark_to_latex(mark):
     r"""
-    Latexifier for atom marks. 
+    Latexifier for atom marks.
 
     Cr12 -> Cr\ :sub:`12`\.
 
     Parameters
     ----------
     mark : str
         Mark of atom.
 
     Returns
     -------
     new_mark : str
         Latex version of the mark.
     """
-    numbers = '0123456789'
-    new_mark = '$'
+    numbers = "0123456789"
+    new_mark = "$"
     insert_underline = False
     for symbol in mark:
         if symbol in numbers and not insert_underline:
             insert_underline = True
-            new_mark += '_{'
+            new_mark += "_{"
         new_mark += symbol
-    new_mark += '}$'
+    new_mark += "}$"
     return new_mark
 
 
 def rot_angle(x, y, dummy=False):
     r"""
-    Rotational ange from 2D vector.
+    Rotational angle from 2D vector.
 
     Mathematically positive => counterclockwise.
     From [0 to 360)
 
     Parameters
     ----------
     x : float or int
@@ -122,29 +197,29 @@
         y coordinate of a vector.
     """
     # rot_cos = x / (x ** 2 + y ** 2) ** 0.5
     # rot_angle = m.acos(rot_cos) / m.pi * 180
     try:
         sin = abs(y) / sqrt(x**2 + y**2)
     except ZeroDivisionError:
-        raise ValueError('Angle is ill defined (x = y = 0).')
+        raise ValueError("Angle is ill defined (x = y = 0).")
     if x > 0:
         if y > 0:
             return asin(sin) / pi * 180
         elif y == 0:
             return 0
         elif y < 0:
             if not dummy:
                 return -asin(sin) / pi * 180
             return 360 - asin(sin) / pi * 180
     elif x == 0:
         if y > 0:
             return 90
         elif y == 0:
-            raise ValueError('Angle is ill defined (x = y = 0).')
+            raise ValueError("Angle is ill defined (x = y = 0).")
         elif y < 0:
             if not dummy:
                 return 90
             return 270
     elif x < 0:
         if y > 0:
             if not dummy:
@@ -156,128 +231,14 @@
             return 180
         elif y < 0:
             if not dummy:
                 return asin(sin) / pi * 180
             return 180 + asin(sin) / pi * 180
 
 
-def strip_digits(line: str):
-    r"""
-    Remove all digits from the string
-
-    Parameters
-    ----------
-    line : str
-        Input string.
-
-    Returns
-    -------
-    new_line : str
-        ``line`` without digits
-    """
-
-    new_line = ""
-    numbers = "1234567890"
-    for char in line:
-        if char not in numbers:
-            new_line += char
-    return new_line
-
-
-def two_points_distance(point1, point2):
-    r"""
-    Compute distance between two points.
-
-    Parameters
-    ----------
-    point1 : array
-        Coordinates of the first point. 
-
-        .. code-block:: python
-
-            [x1, y1, z1]
-
-    point2 : array
-        Coordinates of the second point. 
-
-        .. code-block:: python
-
-            [x2, y2, z2]
-
-    Returns
-    -------
-    distance : float
-        Distance between two points.
-    """
-
-    point1 = np.array(point1)
-    point2 = np.array(point2)
-    return sqrt(np.sum((point1 - point2)**2))
-
-
-def search_on_atoms(centre, atoms):
-    r"""
-    Search the closest atom to the given centre position.
-
-    Parameters
-    ----------
-    centre : array
-        xyz coordinates of the centre.
-    atoms : list
-        List of atom names and coordinates of the form: ::
-
-            [(name, [x, y, z]), ...]
-
-    Returns
-    -------
-    min_span : float
-        Distance from the centre to the closest atom.
-    name : str
-        Name of the closest atom.
-    """
-
-    min_span = 10000
-    name = "None"
-    for atom, a_coord in atoms:
-        if sqrt(np.sum((centre[1] - a_coord)**2)) < min_span:
-            min_span = sqrt(np.sum((centre[1] - a_coord)**2))
-            name = atom
-    return min_span, name
-
-
-def search_between_atoms(centre, atoms):
-    r"""
-    Search the closest bond centre to the given centre position.
-
-    Parameters
-    ----------
-    centre : array
-        xyz coordinates of the centre.
-    atoms : list
-        List of atom names and coordinates of the form: ::
-
-            [(name, [x, y, z]), ...]
-
-    Returns
-    -------
-    min_span : float
-        Distance from the centre to the bond`s centre.
-    name : str
-        Name of the closest bond`s centre (atom1-atom2).
-    """
-
-    pairs = []
-    for i, atom in enumerate(atoms):
-        for j in range(i+1, len(atoms)):
-            pair = f"{atom[0]}-{atoms[j][0]}"
-            p_coord = (atom[1]+atoms[j][1])/2
-            pairs.append([pair, p_coord])
-    return search_on_atoms(centre, pairs)
-
-
 def absolute_to_relative(cell, x, y, z):
     r"""
     Compute relative coordinates with respect to the unit cell.
 
     Parameters
     ----------
     cell : 3 x 3 array
@@ -298,12 +259,25 @@
     a = np.array(cell[0], dtype=float)
     b = np.array(cell[1], dtype=float)
     c = np.array(cell[2], dtype=float)
     v = np.array([x, y, z], dtype=float)
     if (v == np.zeros(3)).all():
         return np.zeros(3)
     B = np.array([np.dot(a, v), np.dot(b, v), np.dot(c, v)])
-    A = np.array([[np.dot(a, a), np.dot(a, b), np.dot(a, c)],
-                  [np.dot(b, a), np.dot(b, b), np.dot(b, c)],
-                  [np.dot(c, a), np.dot(c, b), np.dot(c, c)]])
+    A = np.array(
+        [
+            [np.dot(a, a), np.dot(a, b), np.dot(a, c)],
+            [np.dot(b, a), np.dot(b, b), np.dot(b, c)],
+            [np.dot(c, a), np.dot(c, b), np.dot(c, c)],
+        ]
+    )
     relative = np.linalg.solve(A, B)
     return relative
+
+
+def winwait():
+    r"""
+    Add "Press Enter to continue" behaviour to Windows.
+    """
+    if sys.platform == "win32":
+        cprint("Press Enter to continue", colour="green")
+        input()
```

### Comparing `rad-tools-0.5.9/rad_tools/score/rad_make_template_core.py` & `rad-tools-0.6.0/rad_tools/score/make_template.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,142 +1,175 @@
 from argparse import ArgumentParser
-from os.path import abspath, split
-from os import makedirs
-from datetime import datetime
 from calendar import month_name
+from datetime import datetime
+from os import makedirs
+from os.path import abspath, split
 
 import numpy as np
 
+from rad_tools import __version__ as version
 from rad_tools.io.tb2j import read_exchange_model
 from rad_tools.routines import OK, RESET, YELLOW
 
 
-def manager(output_name="template",
-            tb2j_filename=None,
-            R_vector=None,
-            max_distance=None,
-            min_distance=None,
-            distance=None):
+def manager(
+    output_name="template",
+    input_filename=None,
+    R_vector=None,
+    max_distance=None,
+    min_distance=None,
+    distance=None,
+    verbose=False,
+):
     r"""
-    Main function call of the rad-make-template.py script.
+    ``rad-make-template.py`` script.
 
-    Full documentation on the behaviour is available
-    :ref:`here <rad-make-template>`. Parameters of the function directly
-    corresponds to the arguments of the script.
-
-    If you want to have the behaviour of the rad-make-template.py script
-    but in a format of a fuction call use this function.
+    Full documentation on the behaviour is available in the
+    :ref:`User Guide <rad-make-template>`.
+    Parameters of the function directly
+    correspond to the arguments of the script.
     """
 
     if distance is not None:
         min_distance = distance
         max_distance = distance
 
     if R_vector is not None:
-        R_vector = np.array(R_vector[:len(R_vector) // 3 * 3],
-                            dtype=int).reshape((len(R_vector)//3, 3))
+        R_vector = np.array(R_vector[: len(R_vector) // 3 * 3], dtype=int).reshape(
+            (len(R_vector) // 3, 3)
+        )
         R_vector = list(map(tuple, R_vector.tolist()))
 
     try:
         makedirs(split(output_name)[0])
     except FileExistsError:
         pass
     except FileNotFoundError:
         pass
 
-    template = ('=' * 20 + "\n" +
-                "Neighbors template:\n" +
-                "i j R_a R_b R_c\n" +
-                '-' * 20 + "\n" +
-                "J1 $J_1$\n" +
-                "atom1 atom2  0  0  0\n" +
-                "atom1 atom2  1  0  0\n" +
-                "atom1 atom1 -1  0  2\n" +
-                '-' * 20 + "\n" +
-                "J2\n" +
-                "atom2 atom1  9  5 -3\n" +
-                "atom1 atom2  1  4  0\n" +
-                "atom2 atom2  1  0  2\n" +
-                '=' * 20 + "\n")
+    template = (
+        "=" * 20
+        + "\n"
+        + "Neighbors template:\n"
+        + "i j R_a R_b R_c\n"
+        + "-" * 20
+        + "\n"
+        + "J1 $J_1$\n"
+        + "atom1 atom2  0  0  0\n"
+        + "atom1 atom2  1  0  0\n"
+        + "atom1 atom1 -1  0  2\n"
+        + "-" * 20
+        + "\n"
+        + "J2\n"
+        + "atom2 atom1  9  5 -3\n"
+        + "atom1 atom2  1  4  0\n"
+        + "atom2 atom2  1  0  2\n"
+        + "=" * 20
+        + "\n"
+    )
     cd = datetime.now()
     with open(f"{output_name}.txt", "w") as file:
-        if tb2j_filename is None:
+        if input_filename is None:
             file.write(
-                f"Template is created " +
-                f"on {cd.day} {month_name[cd.month]} {cd.year}" +
-                f" at {cd.hour}:{cd.minute}:{cd.second} by rad-tools\n\n")
+                f"Template is created "
+                + f"on {cd.day} {month_name[cd.month]} {cd.year}"
+                + f" at {cd.hour}:{cd.minute}:{cd.second} by rad-tools {version}\n\n"
+            )
 
             file.write(template)
         else:
             file.write(
-                f"Template is created based on the file: {tb2j_filename}\n" +
-                f"on {cd.day} {month_name[cd.month]} {cd.year}" +
-                f" at {cd.hour}:{cd.minute}:{cd.second} by rad-tools\n\n")
-
-            model = read_exchange_model(tb2j_filename)
-            model.filter(min_distance=min_distance,
-                         max_distance=max_distance,
-                         R_vector=R_vector)
-            file.write('=' * 20 + "\n" +
-                       "Neighbors template:\n" +
-                       "i j R_a R_b R_c\n" +
-                       '-' * 20 + "\n" + "Name placeholder" + "\n")
+                f"Template is created based on the file: {input_filename}\n"
+                + f"on {cd.day} {month_name[cd.month]} {cd.year}"
+                + f" at {cd.hour}:{cd.minute}:{cd.second} by rad-tools {version}\n\n"
+            )
+
+            model = read_exchange_model(input_filename, quiet=not verbose)
+            model.filter(
+                min_distance=min_distance, max_distance=max_distance, R_vector=R_vector
+            )
+            file.write(
+                "=" * 20
+                + "\n"
+                + "Neighbors template:\n"
+                + "i j R_a R_b R_c\n"
+                + "-" * 20
+                + "\n"
+                + "Name placeholder"
+                + "\n"
+            )
             for atom1, atom2, R in model.bonds:
-                file.write(f"{atom1:4} {atom2:4} " +
-                           f"{R[0]:3.0f} {R[1]:3.0f} {R[2]:3.0f}\n")
-            file.write('=' * 20 + "\n")
-    print(f"{OK}Template draft is in " +
-          f"{abspath(output_name)}.txt{RESET}")
-    print(f"{YELLOW}Do not forget to correct the template draft " +
-          f"to your needs!{RESET}")
+                file.write(
+                    f"{atom1:4} {atom2:4} " + f"{R[0]:3.0f} {R[1]:3.0f} {R[2]:3.0f}\n"
+                )
+            file.write("=" * 20 + "\n")
+    print(f"{OK}Template draft is in " + f"{abspath(output_name)}.txt{RESET}")
+    print(
+        f"{YELLOW}Do not forget to correct the template draft "
+        + f"to your needs!{RESET}"
+    )
 
 
-def get_parser():
+def create_parser():
     parser = ArgumentParser(
-        description="Script for the creation of template`s template")
+        description="Script for the creation of template`s template"
+    )
 
-    parser.add_argument("-on", "--output-name",
-                        type=str,
-                        default='template',
-                        help="""
-                        Relative or absolute path to the template output file.
-                        """
-                        )
-    parser.add_argument("-tf", "--tb2j-filename",
-                        type=str,
-                        default=None,
-                        help="""
-                        Relative or absulute path to the *exchange.out* file,
-                        including the name and extention of the file itself.
-                        """
-                        )
-    parser.add_argument("-R", "--R-vector",
-                        type=int,
-                        nargs="*",
-                        default=None,
-                        help="""
-                        R vectors for filtering the model.
-                        """
-                        )
-    parser.add_argument("-maxd", "--max-distance",
-                        type=float,
-                        default=None,
-                        help="""
-                        (<=) Maximum distance.
-                        """
-                        )
-    parser.add_argument("-mind", "--min-distance",
-                        type=float,
-                        default=None,
-                        help="""
-                        (>=) Minimum distance.
-                        """
-                        )
-    parser.add_argument("-d", "--distance",
-                        type=float,
-                        default=None,
-                        help="""
-                        (=) Exact distance.
-                        """
-                        )
+    parser.add_argument(
+        "-on",
+        "--output-name",
+        metavar="filename",
+        type=str,
+        default="template",
+        help="Name for the template output file.",
+    )
+    parser.add_argument(
+        "-if",
+        "--input-filename",
+        metavar="filename",
+        type=str,
+        default=None,
+        help="Relative or absolute path to the 'exchange.out' file, "
+        + "including the name and extension of the file itself.",
+    )
+    parser.add_argument(
+        "-R",
+        "--R-vector",
+        metavar="R1a R1b R1c",
+        type=int,
+        nargs="*",
+        default=None,
+        help="R vectors for filtering the model.",
+    )
+    parser.add_argument(
+        "-maxd",
+        "--max-distance",
+        metavar="distance",
+        type=float,
+        default=None,
+        help="(<=) Maximum distance.",
+    )
+    parser.add_argument(
+        "-mind",
+        "--min-distance",
+        metavar="distance",
+        type=float,
+        default=None,
+        help="(>=) Minimum distance.",
+    )
+    parser.add_argument(
+        "-d",
+        "--distance",
+        metavar="distance",
+        type=float,
+        default=None,
+        help="(=) Exact distance.",
+    )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        default=False,
+        help="Verbose output, propagates to the called methods.",
+    )
 
     return parser
```

### Comparing `rad-tools-0.5.9/rad_tools/score/tb2j_plotter_core.py` & `rad-tools-0.6.0/rad_tools/score/plot_tb2j.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,124 +1,165 @@
 from argparse import ArgumentParser
-from os.path import join, abspath
-from os import makedirs
 from math import sqrt
+from os import makedirs
+from os.path import abspath, join
 
-from matplotlib import pyplot as plt
 import numpy as np
+from matplotlib import pyplot as plt
 
-from rad_tools.io.tb2j import read_exchange_model
 from rad_tools.io.internal import read_template
-from rad_tools.routines import atom_mark_to_latex, rot_angle, OK, RESET
+from rad_tools.io.tb2j import read_exchange_model
+from rad_tools.routines import OK, RESET, atom_mark_to_latex, rot_angle
 
 
-def manager(input_filename,
-            output_path='.',
-            output_name='exchange',
-            what_to_plot='iso',
-            draw_cells=False,
-            min_distance=None,
-            max_distance=None,
-            distance=None,
-            template_file=None,
-            R_vector=None,
-            scale_atoms=1,
-            scale_data=1,
-            title=None,
-            force_symmetry=False):
+def manager(
+    input_filename,
+    output_path=".",
+    output_name="exchange",
+    what_to_plot="iso",
+    draw_cells=False,
+    min_distance=None,
+    max_distance=None,
+    distance=None,
+    template_file=None,
+    R_vector=None,
+    scale_atoms=1,
+    scale_data=1,
+    title=None,
+    force_symmetry=False,
+    verbose=False,
+):
+    r"""
+    ``rad-plot-tb2j.py`` script.
+
+    Full documentation on the behaviour is available in the
+    :ref:`User Guide <rad-plot-tb2j>`.
+    Parameters of the function directly
+    correspond to the arguments of the script.
+    """
 
     if force_symmetry and template_file is None:
         raise ValueError("--force-symmetry option requires a template file.")
 
     if distance is not None:
         min_distance = distance
         max_distance = distance
 
     try:
         makedirs(output_path)
     except FileExistsError:
         pass
 
     if R_vector is not None:
-        R_vector = np.array(R_vector[:len(R_vector) // 3 * 3],
-                            dtype=int).reshape((len(R_vector)//3, 3))
+        R_vector = np.array(R_vector[: len(R_vector) // 3 * 3], dtype=int).reshape(
+            (len(R_vector) // 3, 3)
+        )
         R_vector = list(map(tuple, R_vector.tolist()))
 
-    model = read_exchange_model(input_filename)
+    model = read_exchange_model(input_filename, quiet=not verbose)
     if template_file is not None:
         template = read_template(template_file)
     else:
         template = None
-    model.filter(min_distance=min_distance,
-                 max_distance=max_distance,
-                 R_vector=R_vector,
-                 template=template)
+
     if force_symmetry:
         model.force_symmetry(template=template)
 
+    model.filter(
+        min_distance=min_distance,
+        max_distance=max_distance,
+        R_vector=R_vector,
+        template=template,
+    )
+
     dummy = True
-    ha = 'center'
+    ha = "center"
     x_min, y_min, z_min, x_max, y_max, z_max = model.space_dimensions
     X = max(abs(x_min), abs(x_max))
     Y = max(abs(y_min), abs(y_max))
     if X == 0 and Y == 0:
         X = Y = 1
     linewidth = 1
     fontsize = 11
     if what_to_plot == "all":
-        wtps = ['iso', 'distance', 'dmi']
+        wtps = ["iso", "distance", "dmi"]
     else:
         wtps = [what_to_plot]
     for wtp in wtps:
-
         if X < Y:
-            fig = plt.figure(figsize=(6.4*X/Y, 4.8))
+            fig = plt.figure(figsize=(6.4 * X / Y, 4.8))
         else:
-            fig = plt.figure(figsize=(6.4, 4.8*Y/X))
+            fig = plt.figure(figsize=(6.4, 4.8 * Y / X))
         ax = fig.add_axes([0.1, 0.1, 0.8, 0.8])
         ax.set_aspect("equal")
-        ax.set_xlabel('x, Angstroms')
-        ax.set_ylabel('y, Angstroms')
+        ax.set_xlabel("x, Angstroms")
+        ax.set_ylabel("y, Angstroms")
 
         for atom1, atom2, R in model:
             bond = model[(atom1, atom2, R)]
             dis = model.get_distance(atom1, atom2, R)
             x1, y1, z1 = model.get_atom_coordinates(atom1)
             x2, y2, z2 = model.get_atom_coordinates(atom2, R)
             xm = (x1 + x2) / 2
             ym = (y1 + y2) / 2
             zm = (z1 + z2) / 2
 
-            ax.scatter(x1, y1, s=100 * fig.dpi/72., c='white')
-            ax.scatter(x2, y2, s=100 * fig.dpi/72., c='white')
+            ax.scatter(x1, y1, s=100 * fig.dpi / 72.0, c="white")
+            ax.scatter(x2, y2, s=100 * fig.dpi / 72.0, c="white")
 
-            ax.text(x1, y1, atom_mark_to_latex(atom1),
-                    va='center', ha='center',
-                    fontsize=1.5 * fontsize * scale_atoms)
-            ax.text(x2, y2, atom_mark_to_latex(atom2),
-                    va='center', ha='center',
-                    fontsize=1.5 * fontsize * scale_atoms)
-            if wtp == 'iso':
-                ax.text(xm, ym, str(round(bond.iso, 4)),
-                        va='bottom', ha=ha,
-                        rotation_mode='anchor',
-                        rotation=rot_angle(x2 - x1, y2 - y1, dummy=dummy),
-                        fontsize=fontsize * scale_data)
-            elif wtp == 'distance':
-                ax.text(xm, ym, str(round(dis, 4)),
-                        va='bottom', ha=ha,
-                        rotation_mode='anchor',
-                        rotation=rot_angle(x2 - x1, y2 - y1, dummy=dummy),
-                        fontsize=fontsize * scale_data)
-            elif wtp == 'dmi':
-                ax.text(xm, ym, str(round(sqrt(np.sum(bond.dmi**2)), 4)),
-                        va='bottom', ha=ha,
-                        rotation_mode='anchor',
-                        rotation=rot_angle(x2 - x1, y2 - y1, dummy=dummy),
-                        fontsize=fontsize * scale_data)
+            ax.text(
+                x2,
+                y2,
+                atom_mark_to_latex(atom2),
+                va="center",
+                ha="center",
+                fontsize=1.5 * fontsize * scale_atoms,
+            )
+            ax.text(
+                x1,
+                y1,
+                atom_mark_to_latex(atom1),
+                va="center",
+                ha="center",
+                fontsize=1.5 * fontsize * scale_atoms,
+                color="#A04F4D",
+            )
+            if wtp == "iso":
+                ax.text(
+                    xm,
+                    ym,
+                    str(round(bond.iso, 4)),
+                    va="bottom",
+                    ha=ha,
+                    rotation_mode="anchor",
+                    rotation=rot_angle(x2 - x1, y2 - y1, dummy=dummy),
+                    fontsize=fontsize * scale_data,
+                )
+            elif wtp == "distance":
+                ax.text(
+                    xm,
+                    ym,
+                    str(round(dis, 4)),
+                    va="bottom",
+                    ha=ha,
+                    rotation_mode="anchor",
+                    rotation=rot_angle(x2 - x1, y2 - y1, dummy=dummy),
+                    fontsize=fontsize * scale_data,
+                )
+            elif wtp == "dmi":
+                ax.text(
+                    xm,
+                    ym,
+                    str(round(sqrt(np.sum(bond.dmi**2)), 4)),
+                    va="bottom",
+                    ha=ha,
+                    rotation_mode="anchor",
+                    rotation=rot_angle(x2 - x1, y2 - y1, dummy=dummy),
+                    fontsize=fontsize * scale_data,
+                )
 
         xlims = (ax.get_xlim()[0] - 0.5, ax.get_xlim()[1] + 0.5)
         ylims = (ax.get_ylim()[0] - 0.5, ax.get_ylim()[1] + 0.5)
 
         if draw_cells:
             cells = model.cell_list
             a_x, a_y, a_z = tuple(model.cell[0])
@@ -136,136 +177,163 @@
                 Ry_max = max(Ry, Ry_max)
                 Rz_min = min(Rz, Rz_min)
                 Rz_max = max(Rz, Rz_max)
 
             for i in range(Rx_min, Rx_max + 2):
                 for j in range(Ry_min, Ry_max + 2):
                     for k in range(Rz_min, Rz_max + 2):
-                        ax.plot([Rx_min * a_x + j * b_x,
-                                (Rx_max + 1) * a_x + j * b_x],
-                                [Rx_min * a_y + j * b_y,
-                                (Rx_max + 1) * a_y + j * b_y],
-                                linewidth=linewidth, color="#DFDFDF")
-                        ax.plot([i * a_x + Ry_min * b_x,
-                                i * a_x + (Ry_max + 1) * b_x],
-                                [i * a_y + Ry_min * b_y,
-                                i * a_y + (Ry_max + 1) * b_y],
-                                linewidth=linewidth, color="#DFDFDF")
-            ax.plot(np.array([0, a_x, a_x + b_x, b_x, 0]),
-                    np.array([0, a_y, a_y + b_y, b_y, 0]),
-                    linewidth=linewidth, color="#CA7371")
+                        ax.plot(
+                            [Rx_min * a_x + j * b_x, (Rx_max + 1) * a_x + j * b_x],
+                            [Rx_min * a_y + j * b_y, (Rx_max + 1) * a_y + j * b_y],
+                            linewidth=linewidth,
+                            color="#DFDFDF",
+                        )
+                        ax.plot(
+                            [i * a_x + Ry_min * b_x, i * a_x + (Ry_max + 1) * b_x],
+                            [i * a_y + Ry_min * b_y, i * a_y + (Ry_max + 1) * b_y],
+                            linewidth=linewidth,
+                            color="#DFDFDF",
+                        )
+            ax.plot(
+                np.array([0, a_x, a_x + b_x, b_x, 0]),
+                np.array([0, a_y, a_y + b_y, b_y, 0]),
+                linewidth=linewidth,
+                color="#CA7371",
+            )
 
         ax.set_xlim(*xlims)
         ax.set_ylim(*ylims)
 
         if title is not None:
             ax.set_title(title, fontsize=1.5 * fontsize)
 
-        png_path = join(output_path, f'{output_name}.{wtp}.png')
+        png_path = join(output_path, f"{output_name}.{wtp}.png")
         plt.savefig(png_path, dpi=400, bbox_inches="tight")
-        print(f'{OK}2D plot with {wtp} is in {abspath(png_path)}{RESET}')
+        print(f"{OK}2D plot with {wtp} is in {abspath(png_path)}{RESET}")
 
 
-def get_parser():
-    parser = ArgumentParser(
-        description="Script for visualisation of TB2J results")
-
-    parser.add_argument("-if", "--input-filename",
-                        type=str,
-                        required=True,
-                        help="""
-                        Relative or absulute path to the *exchange.out* file,
-                        including the name and extention of the file itself.
-                        """
-                        )
-    parser.add_argument("-op", "--output-path",
-                        type=str,
-                        default='.',
-                        help="""
-                        Relative or absolute path to the folder for saving outputs.
-                        """
-                        )
-    parser.add_argument("-on", "--output-name",
-                        type=str,
-                        default='exchange',
-                        help="""
-                        Seedname for the output files.
-                        """
-                        )
-    parser.add_argument("-wtp", "--what-to-plot",
-                        type=str,
-                        choices=['all', 'iso', 'distance', 'dmi'],
-                        default='all',
-                        help="""
-                        Type of data for display.
-                        """
-                        )
-    parser.add_argument("-dc", "--draw-cells",
-                        action="store_true",
-                        default=False,
-                        help="""
-                        Whenever to draw the cells.
-                        """
-                        )
-    parser.add_argument("-R", "--R-vector",
-                        type=int,
-                        nargs="*",
-                        default=None,
-                        help="""
-                        R vectors for filtering the model.
-                        """
-                        )
-    parser.add_argument("-maxd", "--max-distance",
-                        type=float,
-                        default=None,
-                        help="""
-                        (<=) Maximum distance.
-                        """
-                        )
-    parser.add_argument("-mind", "--min-distance",
-                        type=float,
-                        default=None,
-                        help="""
-                        (>=) Minimum distance.
-                        """
-                        )
-    parser.add_argument("-d", "--distance",
-                        type=float,
-                        default=None,
-                        help="""
-                        (=) Exact distance.
-                        """
-                        )
-    parser.add_argument("-tf", "--template-file",
-                        type=str,
-                        default=None,
-                        help="""
-                        Relative or absolute path to the template file,
-                        including the name and extention of the file.
-                        """)
-    parser.add_argument("-sa", "--scale-atoms",
-                        default=1,
-                        type=float,
-                        help="""
-                        Scale for the size of atom marks.
-                        """)
-    parser.add_argument("-sd", "--scale-data",
-                        default=1,
-                        type=float,
-                        help="""
-                        Scale for the size of data text.
-                        """)
-    parser.add_argument("-t", "--title",
-                        default=None,
-                        type=str,
-                        help="""
-                        Title for the plots.
-                        """)
-    parser.add_argument("-fs", "--force-symmetry",
-                        default=False,
-                        action="store_true",
-                        help="""
-                        Force the Exchange model to have the symmetry 
-                        of the template.
-                        """)
+def create_parser():
+    parser = ArgumentParser(description="Script for visualization of TB2J results")
+
+    parser.add_argument(
+        "-if",
+        "--input-filename",
+        metavar="filename",
+        type=str,
+        required=True,
+        help="Relative or absolute path to the 'exchange.out' file,"
+        + "including the name and extension of the file itself.",
+    )
+    parser.add_argument(
+        "-op",
+        "--output-path",
+        metavar="path",
+        type=str,
+        default=".",
+        help="Relative or absolute path to the folder for saving outputs.",
+    )
+    parser.add_argument(
+        "-on",
+        "--output-name",
+        metavar="filename",
+        type=str,
+        default="exchange",
+        help="Seedname for the output files.",
+    )
+    parser.add_argument(
+        "-wtp",
+        "--what-to-plot",
+        metavar="value",
+        type=str,
+        choices=["all", "iso", "distance", "dmi"],
+        default="all",
+        help="Type of data for display.",
+    )
+    parser.add_argument(
+        "-dc",
+        "--draw-cells",
+        action="store_true",
+        default=False,
+        help="Whether to draw the cells.",
+    )
+    parser.add_argument(
+        "-R",
+        "--R-vector",
+        metavar="R1a R1b R1c",
+        type=int,
+        nargs="*",
+        default=None,
+        help="R vectors for filtering the model.",
+    )
+    parser.add_argument(
+        "-maxd",
+        "--max-distance",
+        metavar="distance",
+        type=float,
+        default=None,
+        help="(<=) Maximum distance.",
+    )
+    parser.add_argument(
+        "-mind",
+        "--min-distance",
+        metavar="distance",
+        type=float,
+        default=None,
+        help="(>=) Minimum distance.",
+    )
+    parser.add_argument(
+        "-d",
+        "--distance",
+        metavar="distance",
+        type=float,
+        default=None,
+        help="(=) Exact distance.",
+    )
+    parser.add_argument(
+        "-tf",
+        "--template-file",
+        metavar="filename",
+        type=str,
+        default=None,
+        help="Relative or absolute path to the template file, "
+        + "including the name and extension of the file.",
+    )
+    parser.add_argument(
+        "-sa",
+        "--scale-atoms",
+        metavar="factor",
+        default=1,
+        type=float,
+        help="Scale for the size of atom marks.",
+    )
+    parser.add_argument(
+        "-sd",
+        "--scale-data",
+        metavar="factor",
+        default=1,
+        type=float,
+        help="Scale for the size of data text.",
+    )
+    parser.add_argument(
+        "-t",
+        "--title",
+        metavar="title",
+        default=None,
+        type=str,
+        help="Title for the plots.",
+    )
+    parser.add_argument(
+        "-fs",
+        "--force-symmetry",
+        default=False,
+        action="store_true",
+        help="Force the Exchange model to have the symmetry of the template.",
+    )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        default=False,
+        help="Verbose output, propagates to the called methods.",
+    )
 
     return parser
```

### Comparing `rad-tools-0.5.9/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.6.0/rad_tools.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,33 @@
 rad_tools/map.py
 rad_tools/routines.py
 rad_tools.egg-info/PKG-INFO
 rad_tools.egg-info/SOURCES.txt
 rad_tools.egg-info/dependency_links.txt
 rad_tools.egg-info/requires.txt
 rad_tools.egg-info/top_level.txt
+rad_tools/dos/__init__.py
+rad_tools/dos/dos.py
+rad_tools/dos/pdos.py
 rad_tools/exchange/__init__.py
 rad_tools/exchange/bond.py
 rad_tools/exchange/model.py
 rad_tools/exchange/template.py
 rad_tools/io/__init__.py
 rad_tools/io/internal.py
 rad_tools/io/tb2j.py
 rad_tools/kpoints/__init__.py
 rad_tools/kpoints/high_symmetry_point.py
 rad_tools/kpoints/kpoints.py
 rad_tools/score/__init__.py
-rad_tools/score/rad_dos_plotter_core.py
-rad_tools/score/rad_make_template_core.py
-rad_tools/score/tb2j_extractor_core.py
-rad_tools/score/tb2j_plotter_core.py
+rad_tools/score/extract_tb2j.py
+rad_tools/score/identify_wannier_centres.py
+rad_tools/score/make_template.py
+rad_tools/score/plot_dos.py
+rad_tools/score/plot_tb2j.py
 scripts/compute-energies.py
-scripts/identify-wannier-centres.py
 scripts/phonopy-plotter.py
-scripts/rad-dos-plotter.py
+scripts/rad-extract-tb2j.py
+scripts/rad-identify-wannier-centres.py
 scripts/rad-make-template.py
-scripts/tb2j-extractor.py
-scripts/tb2j-plotter.py
+scripts/rad-plot-dos.py
+scripts/rad-plot-tb2j.py
```

### Comparing `rad-tools-0.5.9/scripts/compute-energies.py` & `rad-tools-0.6.0/scripts/compute-energies.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #! /usr/local/bin/python3
 
 from argparse import ArgumentParser, RawTextHelpFormatter
 from subprocess import run
 
 
 def J_values(FM, AFM1, AFM2, AFM3):
-
-    J2 = -(FM - AFM1)*13605/8/8
-    J3 = -(FM - AFM2)*13605/2/2/8 - J2
-    J1 = -(AFM2 - AFM3)*13605/8/2/8 + J3
+    J2 = -(FM - AFM1) * 13605 / 8 / 8
+    J3 = -(FM - AFM2) * 13605 / 2 / 2 / 8 - J2
+    J1 = -(AFM2 - AFM3) * 13605 / 8 / 2 / 8 + J3
 
     return J1, J2, J3
 
 
 def compute(filename):
     FM = {}
     AFM1 = {}
@@ -62,45 +61,50 @@
         dis_list = [key for key in FM[mode]]
         dis_list.sort()
         for dis in dis_list:
             ISOK = True
             try:
                 fm = FM[mode][dis]
             except KeyError:
-                print(
-                    f"mode {mode}, displacement {dis/100:.2f} FM : problem with scf")
+                print(f"mode {mode}, displacement {dis/100:.2f} FM : problem with scf")
                 ISOK = False
             try:
                 afm1 = AFM1[mode][dis]
             except KeyError:
                 print(
-                    f"mode {mode}, displacement {dis/100:.2f} AFM1 : problem with scf")
+                    f"mode {mode}, displacement {dis/100:.2f} AFM1 : problem with scf"
+                )
                 ISOK = False
             try:
                 afm2 = AFM2[mode][dis]
             except KeyError:
                 print(
-                    f"mode {mode}, displacement {dis/100:.2f} AFM2 : problem with scf")
+                    f"mode {mode}, displacement {dis/100:.2f} AFM2 : problem with scf"
+                )
                 ISOK = False
             try:
                 afm3 = AFM3[mode][dis]
             except KeyError:
                 print(
-                    f"mode {mode}, displacement {dis/100:.2f} AFM3 : problem with scf")
+                    f"mode {mode}, displacement {dis/100:.2f} AFM3 : problem with scf"
+                )
                 ISOK = False
             if ISOK:
                 J1, J2, J3 = J_values(fm, afm1, afm2, afm3)
                 print(f"Mode {mode}, displacement {dis/100:.2f}")
                 print(f"    J1 = {J1:.6f} J2 = {J2:.6f} J3 = {J3:.6f}")
 
 
 if __name__ == "__main__":
     parser = ArgumentParser(formatter_class=RawTextHelpFormatter)
-    parser.add_argument("filename", type=str,
-                        help="""File with grepped lines.
+    parser.add_argument(
+        "filename",
+        type=str,
+        help="""File with grepped lines.
 Example grep:
 
 grep "!" *mode/*F*/{neg,pos}/crsbr.scf*out > summary.txt
-    """)
+    """,
+    )
     args = parser.parse_args()
 
     compute(args.filename)
```

### Comparing `rad-tools-0.5.9/scripts/identify-wannier-centres.py` & `rad-tools-0.6.0/rad_tools/score/identify_wannier_centres.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,132 +1,132 @@
 #! /usr/local/bin/python3
 
 from argparse import ArgumentParser
-from os.path import split, join
+from os.path import join, split
 
 import numpy as np
 
-from rad_tools.routines import strip_digits, WARNING, RESET, \
-    search_on_atoms, search_between_atoms
+from rad_tools.routines import cprint
 
 
-def identify(filename, span, output_path, out_name, nocolor=False):
-    separation_tolerance = 10E-5
+def manager(filename, span, output_path, output_name, no_colour=False):
+    r"""
+    ``rad-identify-wannier-centres.py`` script.
+
+    Full documentation on the behaviour is available in the
+    :ref:`User Guide <rad-identify-wannier-centres>`.
+    Parameters of the function directly
+    correspond to the arguments of the script.
+    """
+
+    head, tail = split(filename)
+    if output_path is None:
+        output_path = head
+    if output_name is None:
+        output_name = tail + "_identified"
+    separation_tolerance = 10e-8
 
     # Read atoms and centres
     atom_counter = {}
     with open(filename, "r") as file:
         n = int(file.readline())
         file_stats = file.readline()
         centres = []
         atoms = []
         for _ in range(0, n):
             line = file.readline().split()
             if line[0] == "X":
-                centres.append([f"X",
-                                np.array(list(map(float, line[1:])))])
+                centres.append([f"X", np.array(list(map(float, line[1:])))])
             else:
                 if line[0] in atom_counter:
                     atom_counter[line[0]] += 1
                 else:
                     atom_counter[line[0]] = 1
-                atoms.append([f"{line[0]}{atom_counter[line[0]]}",
-                              np.array(list(map(float, line[1:])))])
+                atoms.append(
+                    [
+                        f"{line[0]}{atom_counter[line[0]]}",
+                        np.array(list(map(float, line[1:]))),
+                    ]
+                )
 
     # Identify centres localization
     for centre in centres:
-        min_span_atom, atom = search_on_atoms(
-            centre, atoms)
-        min_span_pair, pair = search_between_atoms(
-            centre, atoms)
-        if min_span_atom > span and min_span_pair > span:
-            if not nocolor:
-                print(f"{WARNING}", end="")
-            print(f"Centre {centre} unindentified, " +
-                  "try to increase span")
-            if not nocolor:
-                print(f"{RESET}", end="")
-            print(f"    span limit = {span}\n" +
-                  f"    minimum distance to the atom = {min_span_atom:.8f} " +
-                  f"({atom})\n"
-                  f"    minimum distance to the bond`s centre = {min_span_pair:.8f} " +
-                  f"({pair})\n")
-            if abs(min_span_atom - min_span_pair) < separation_tolerance:
-                centre[0] = f"None, closest: {atom}"
-            elif min_span_atom < min_span_pair:
-                centre[0] = f"None, closest: {atom}"
+        min_span = 10000
+        name = "None"
+        for atom, a_coord in atoms:
+            if np.linalg.norm((centre[1] - a_coord)) < min_span:
+                min_span = np.linalg.norm((centre[1] - a_coord))
+                name = atom
+        if min_span - span > separation_tolerance:
+            if no_colour:
+                print(f"Centre {centre} unidentified, " + "try to increase span")
             else:
-                centre[0] = f"None, closest: {pair}"
-        elif abs(min_span_atom - min_span_pair) < separation_tolerance:
-            centre[0] = f"{atom} or {pair}"
-        elif min_span_atom < min_span_pair:
-            centre[0] = atom
+                cprint(
+                    f"Centre {centre} unidentified, " + "try to increase span",
+                    colour="yellow",
+                )
+            print(
+                f"    span limit = {span}\n"
+                + f"    minimum distance to the atom ({name}) = {min_span:.8f}\n"
+            )
+            centre[0] = f"None, closest: {name} ({min_span:.8f})"
         else:
-            centre[0] = pair
+            centre[0] = name
 
     # Write the output
-    with open(join(output_path, out_name), "w") as file:
+    with open(join(output_path, output_name), "w") as file:
         file.write(f"{len(atoms) + len(centres):6.0f}\n")
         file.write(f"{file_stats}")
         for centre, coordinate in centres:
-            file.write(f"X      " +
-                       f"{coordinate[0]:14.8f}   " +
-                       f"{coordinate[1]:14.8f}   " +
-                       f"{coordinate[2]:14.8f}" +
-                       f"   ->   {centre}\n")
+            file.write(
+                f"X      "
+                + f"{coordinate[0]:14.8f}   "
+                + f"{coordinate[1]:14.8f}   "
+                + f"{coordinate[2]:14.8f}"
+                + f"   ->   {centre}\n"
+            )
         for atom, coordinate in atoms:
-            file.write(f"{strip_digits(atom):2}     " +
-                       f"{coordinate[0]:14.8f}   " +
-                       f"{coordinate[1]:14.8f}   " +
-                       f"{coordinate[2]:14.8f}" +
-                       f"   ->   {atom}\n")
-
-
-if __name__ == "__main__":
-    parser = ArgumentParser(
-        description=("Identify wannier centres with respect to the atom " +
-                     "or to the point between the atom`s pair"))
-    parser.add_argument("filename",
-                        type=str,
-                        help="""
-                        Rellative or absolute path to the _centres.xyz file
-                        """)
-    parser.add_argument("-s", "--span",
-                        type=float,
-                        default=0.1,
-                        help="""
-                        Distance tolerance between centre and atom. (in Angstrom)
-                        """)
-    parser.add_argument("-op", "--output-path",
-                        type=str,
-                        default=None,
-                        help="""
-                        Relative or absolute path to the folder
-                        for saving outputs.
-                        """
-                        )
-    parser.add_argument("-on", "--output-name",
-                        type=str,
-                        default=None,
-                        help="""
-                        Seedname for the output files.
-                        """
-                        )
-    parser.add_argument("-nc", "--no-colour",
-                        action="store_true",
-                        default=False,
-                        help="""
-                        Turn off coloured output.
-                        """
-                        )
-    args = parser.parse_args()
-    print(args)
-
-    head, tail = split(args.filename)
-    if args.output_path is None:
-        args.output_path = head
-    if args.output_name is None:
-        args.output_name = tail + "_identified"
-
-    identify(args.filename, args.span,
-             output_path=args.output_path, out_name=args.output_name,
-             nocolor=args.no_colour)
+            file.write(
+                f"{atom.translate(str.maketrans('','','0123456789')):2}     "
+                + f"{coordinate[0]:14.8f}   "
+                + f"{coordinate[1]:14.8f}   "
+                + f"{coordinate[2]:14.8f}"
+                + f"   ->   {atom}\n"
+            )
+
+
+def create_parser():
+    parser = ArgumentParser()
+    parser.add_argument(
+        "filename",
+        type=str,
+        help="Relative or absolute path to the _centres.xyz file",
+    )
+    parser.add_argument(
+        "-s",
+        "--span",
+        type=float,
+        default=0.1,
+        help="Distance tolerance between centre and atom. (in Angstroms)",
+    )
+    parser.add_argument(
+        "-op",
+        "--output-path",
+        type=str,
+        default=None,
+        help="Relative or absolute path to the folder for saving outputs.",
+    )
+    parser.add_argument(
+        "-on",
+        "--output-name",
+        type=str,
+        default=None,
+        help="Seedname for the output files.",
+    )
+    parser.add_argument(
+        "-nc",
+        "--no-colour",
+        action="store_true",
+        default=False,
+        help="Turn off coloured output.",
+    )
+    return parser
```

### Comparing `rad-tools-0.5.9/scripts/phonopy-plotter.py` & `rad-tools-0.6.0/scripts/phonopy-plotter.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,86 +4,93 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import yaml
 
 
 def plot(file, kp=None, constant=1, on="output"):
-    data_file = open(file, 'r')
+    data_file = open(file, "r")
     data = yaml.load(data_file, Loader=yaml.FullLoader)
     data_file.close()
     X = []
     Y = []
     K_points = []
     miny = None
     maxy = None
-    for i, point in enumerate(data['phonon']):
-        for j, band in enumerate(data['phonon'][i]['band']):
-            data['phonon'][i]['band'][j]['frequency'] *= constant
-    for i, point in enumerate(data['phonon']):
+    for i, point in enumerate(data["phonon"]):
+        for j, band in enumerate(data["phonon"][i]["band"]):
+            data["phonon"][i]["band"][j]["frequency"] *= constant
+    for i, point in enumerate(data["phonon"]):
         print(i)
-        X.append(point['distance'])
-        Y.append(list(map(lambda x: x['frequency'], point['band'])))
-        if i == 0 or i == len(data['phonon']) - 1 or data['phonon'][i]['q-position'] == data['phonon'][i + 1]['q-position']:
-            K_points.append(point['distance'])
+        X.append(point["distance"])
+        Y.append(list(map(lambda x: x["frequency"], point["band"])))
+        if (
+            i == 0
+            or i == len(data["phonon"]) - 1
+            or data["phonon"][i]["q-position"] == data["phonon"][i + 1]["q-position"]
+        ):
+            K_points.append(point["distance"])
         if not miny:
             miny = min(Y[-1])
         if not maxy:
             maxy = max(Y[-1])
         miny = min(min(Y[-1]), miny)
         maxy = max(max(Y[-1]), maxy)
 
     print(K_points)
 
     fig, ax = plt.subplots()
     X = np.array(X)
     Y = np.array(Y)
-    ax.plot(X, Y, color='red')
-    ax.set_ylabel('Phonon frequency (THz)', fontsize=15)
+    ax.plot(X, Y, color="red")
+    ax.set_ylabel("Phonon frequency (THz)", fontsize=15)
     ax.set_xlim(X[0], X[-1])
     if kp is None or len(kp) != len(K_points):
         if kp is None:
             kp = []
-        print(f'\033[93m'
-              f'{len(K_points)} k-points expected, only {len(kp)} k-points are provided. '
-              f'Please, check the input.'
-              f'\nProvided K-points: {kp}'
-              f'\x1b[0m')
+        print(
+            f"\033[93m"
+            f"{len(K_points)} k-points expected, only {len(kp)} k-points are provided. "
+            f"Please, check the input."
+            f"\nProvided K-points: {kp}"
+            f"\x1b[0m"
+        )
     if kp and len(kp) == len(K_points):
         for i, k in enumerate(kp):
-            if k == 'G':
-                kp[i] = '$\Gamma$'
+            if k == "G":
+                kp[i] = "$\Gamma$"
         ax.xaxis.set_ticks(K_points, kp, fontsize=15)
         for k_point in K_points:
-            ax.vlines(k_point, 0, 1, transform=ax.get_xaxis_transform(),
-                      color='black', linewidths=0.5)
+            ax.vlines(
+                k_point,
+                0,
+                1,
+                transform=ax.get_xaxis_transform(),
+                color="black",
+                linewidths=0.5,
+            )
     plt.show()
     if constant != 1:
         output = yaml.dump(data)
         with open(f"{on}.yaml", "w") as file:
             file.write(output)
 
 
-if __name__ == '__main__':
-    parser = ArgumentParser(description='Fit Exchange parameters map')
+if __name__ == "__main__":
+    parser = ArgumentParser(description="Fit Exchange parameters map")
 
-    parser.add_argument("-file",
-                        type=str,
-                        default='band.yaml',
-                        help="Path to the band.yaml file")
-    parser.add_argument("-kp",
-                        type=str,
-                        default=None,
-                        nargs='*',
-                        help="K-path, example: -kp G X R Y G")
-    parser.add_argument("-constant",
-                        type=float,
-                        default=1,
-                        help="Constant for conversion. "
-                        "The values will be multiplied by it")
-    parser.add_argument("-on",
-                        type=str,
-                        default="output",
-                        help="output name file")
+    parser.add_argument(
+        "-file", type=str, default="band.yaml", help="Path to the band.yaml file"
+    )
+    parser.add_argument(
+        "-kp", type=str, default=None, nargs="*", help="K-path, example: -kp G X R Y G"
+    )
+    parser.add_argument(
+        "-constant",
+        type=float,
+        default=1,
+        help="Constant for conversion. " "The values will be multiplied by it",
+    )
+    parser.add_argument("-on", type=str, default="output", help="output name file")
     args = parser.parse_args()
     if args.file:
         plot(args.file, kp=args.kp, constant=args.constant, on=args.on)
```

