# Comparing `tmp/OncoAMBER-1.2.1.tar.gz` & `tmp/OncoAMBER-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.2.1.tar", last modified: Thu May  4 20:50:26 2023, max compression
+gzip compressed data, was "OncoAMBER-1.2.2.tar", last modified: Tue May  9 21:53:09 2023, max compression
```

## Comparing `OncoAMBER-1.2.1.tar` & `OncoAMBER-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-04 20:50:26.531339 OncoAMBER-1.2.1/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-04 20:50:26.437125 OncoAMBER-1.2.1/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-04 20:50:26.000000 OncoAMBER-1.2.1/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      588 2023-05-04 20:50:26.000000 OncoAMBER-1.2.1/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-04 20:50:26.000000 OncoAMBER-1.2.1/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.2.1/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-04 20:50:26.000000 OncoAMBER-1.2.1/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-04 20:50:26.000000 OncoAMBER-1.2.1/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-04 20:50:26.530945 OncoAMBER-1.2.1/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.2.1/README.md
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-04 20:50:26.529459 OncoAMBER-1.2.1/amber/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.2.1/amber/BasicGeometries.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.2.1/amber/BetaDistributionCalibration.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     2055 2023-05-01 16:41:03.000000 OncoAMBER-1.2.1/amber/Cell.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    22475 2023-05-04 19:20:45.000000 OncoAMBER-1.2.1/amber/Process.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.2.1/amber/ReadAndWrite.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.2.1/amber/ScalarField.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.2.1/amber/Terminal.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    14776 2023-05-04 20:49:39.000000 OncoAMBER-1.2.1/amber/Vessel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     5571 2023-05-03 20:48:53.000000 OncoAMBER-1.2.1/amber/Voxel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    24068 2023-05-04 15:26:46.000000 OncoAMBER-1.2.1/amber/World.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      308 2023-05-01 16:41:03.000000 OncoAMBER-1.2.1/amber/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.2.1/amber/config.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.2.1/amber/save_alpha_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.2.1/amber/save_beta_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-04 20:50:26.531420 OncoAMBER-1.2.1/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     3010 2023-05-04 20:50:19.000000 OncoAMBER-1.2.1/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-09 21:53:09.507895 OncoAMBER-1.2.2/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-09 21:53:09.421601 OncoAMBER-1.2.2/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-09 21:53:09.000000 OncoAMBER-1.2.2/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      588 2023-05-09 21:53:09.000000 OncoAMBER-1.2.2/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-09 21:53:09.000000 OncoAMBER-1.2.2/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.2.2/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-09 21:53:09.000000 OncoAMBER-1.2.2/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-09 21:53:09.000000 OncoAMBER-1.2.2/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-09 21:53:09.507476 OncoAMBER-1.2.2/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.2.2/README.md
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-09 21:53:09.506114 OncoAMBER-1.2.2/amber/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.2.2/amber/BasicGeometries.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.2.2/amber/BetaDistributionCalibration.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2066 2023-05-09 16:56:51.000000 OncoAMBER-1.2.2/amber/Cell.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    22511 2023-05-08 22:21:34.000000 OncoAMBER-1.2.2/amber/Process.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.2.2/amber/ReadAndWrite.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.2.2/amber/ScalarField.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.2.2/amber/Terminal.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    15144 2023-05-09 14:51:38.000000 OncoAMBER-1.2.2/amber/Vessel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5539 2023-05-09 21:39:18.000000 OncoAMBER-1.2.2/amber/Voxel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    26564 2023-05-09 21:44:59.000000 OncoAMBER-1.2.2/amber/World.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      308 2023-05-01 16:41:03.000000 OncoAMBER-1.2.2/amber/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.2.2/amber/config.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.2.2/amber/save_alpha_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.2.2/amber/save_beta_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-09 21:53:09.507998 OncoAMBER-1.2.2/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3010 2023-05-09 21:52:59.000000 OncoAMBER-1.2.2/setup.py
```

### Comparing `OncoAMBER-1.2.1/OncoAMBER.egg-info/PKG-INFO` & `OncoAMBER-1.2.2/OncoAMBER.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.2.1
+Version: 1.2.2
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.2.1/OncoAMBER.egg-info/SOURCES.txt` & `OncoAMBER-1.2.2/OncoAMBER.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.1/PKG-INFO` & `OncoAMBER-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.2.1
+Version: 1.2.2
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.2.1/README.md` & `OncoAMBER-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.1/amber/BasicGeometries.py` & `OncoAMBER-1.2.2/amber/BasicGeometries.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.1/amber/BetaDistributionCalibration.py` & `OncoAMBER-1.2.2/amber/BetaDistributionCalibration.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.1/amber/Cell.py` & `OncoAMBER-1.2.2/amber/Cell.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 import numpy as np
-
+import scipy.stats as stats
+from scipy.stats import gamma
 class Cell (object):
     def __init__(self, radius, cycle_hours, cycle_std, radiosensitivity, o2_to_vitality_factor, type = 'NormalCell'):
         self.radius = radius
         self.necrotic = False
         self.usual_cycle_length = cycle_hours
         self.cycle_length_std = cycle_std
-        self.doubling_time = self.random_doubling_time(self.usual_cycle_length, self.cycle_length_std) #new cells have a random doubling time
+        self.gamma_shape = (self.usual_cycle_length / self.cycle_length_std) ** 2
+        self.gamma_scale = self.cycle_length_std ** 2 / self.usual_cycle_length
+        self.doubling_time = self.random_doubling_time() #new cells have a random doubling time
         self.volume = 4/3 * np.pi * self.radius**3
         self.oxygen = 1.0
         self.radiosensitivity = radiosensitivity
         self.o2_to_vitality_factor = o2_to_vitality_factor
         if type != 'NormalCell' and type != 'TumorCell':
             print(type + ' is not a valid cell type')
             raise ValueError('Cell type must be either NormalCell or TumorCell')
         self.type = type
         self.time_before_death = None
-        self.time_spent_cycling = self.random_doubling_time(self.usual_cycle_length, self.cycle_length_std) #new cells have already been cycling for a random amount of time
+        self.time_spent_cycling = self.random_time_spent_cycling() #new cells have already been cycling for a random amount of time
     def duplicate(self): #returns a new cell with the same properties
         cell = Cell(self.radius, self.usual_cycle_length, self.cycle_length_std, self.radiosensitivity, self.o2_to_vitality_factor, self.type)
         cell.time_spent_cycling = 0 #the new cell has not been cycling yet
         return cell
 
     def vitality(self):
         factor = self.o2_to_vitality_factor
         vitality = self.oxygen * factor
         vitality = min(vitality, 1.0)
         return vitality #needs to be normalized between 0 and 1
 
     def radiosensitivity(self):
         return self.radiosensitivity*self.oxygen
 
-    def random_doubling_time(self, mu = None, sigma = None):
-        if mu is None:
-            mu = self.usual_cycle_length
-        if sigma is None:
-            sigma = self.cycle_length_std
-        #return a sample of a gamma distribution with mean cycle_hours
-        shape = (mu / sigma) ** 2
-        scale = sigma ** 2 / mu
-        return np.random.gamma(shape = shape, scale = scale)
+    def random_doubling_time(self):
+        return np.random.gamma(shape = self.gamma_shape, scale = self.gamma_scale)
 
+    def random_time_spent_cycling(self):
+        longest_possible_time = self.doubling_time
+        return np.random.uniform(0, longest_possible_time)
```

### Comparing `OncoAMBER-1.2.1/amber/Process.py` & `OncoAMBER-1.2.2/amber/Process.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 
         print('Graphics : ', self.config.show_tumor_and_vessels_3D, self.config.show_slices)
 
         DPI = 100
         size = world.half_length
 
         if self.config.show_angiogenesis_metrics:
-            world.show_angiogenesis_metrics(False)
+            first = (t == 0)
+            world.show_angiogenesis_metrics(False, first)
         #plot vasculature
         if self.config.show_tumor_and_vessels_3D:
             fig, axes = plt.subplots(nrows=1, ncols=1, figsize=(25, 25), dpi=150, subplot_kw={'projection': '3d'})
             fig.suptitle('Visualization at time t = ' + str(t) + ' hours', fontsize=16)
             axes.set_xlim(-size, size)
             axes.set_ylim(-size, size)
             axes.set_zlim(-size, size)
```

### Comparing `OncoAMBER-1.2.1/amber/ReadAndWrite.py` & `OncoAMBER-1.2.2/amber/ReadAndWrite.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.1/amber/ScalarField.py` & `OncoAMBER-1.2.2/amber/ScalarField.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.1/amber/Terminal.py` & `OncoAMBER-1.2.2/amber/Terminal.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.1/amber/Vessel.py` & `OncoAMBER-1.2.2/amber/Vessel.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         mother_vessel = self.get_vessel(vessel_id)
         if mother_vessel is None:
             raise ValueError("Vessel with id {} does not exist".format(vessel_id))
         # split the path in two parts
         path = mother_vessel.path
         if len(path) < 3:
             raise ValueError("Vessel with id {} has a path with less than 3 points".format(vessel_id))
-
+        visible = mother_vessel.visible
         split_index = np.where((path == branching_point))[0][0]
         path_begin, path_end = np.split(path, [split_index])
         #remove the first element of path_end to keep the same point distribution in space
         path_end = np.delete(path_end, 0, 0)
         mother_vessel.path = path_begin  # reduce the mother vessel path. It stops growing
         mother_vessel.in_growth = False
 
@@ -155,16 +155,19 @@
         vessel_end = Vessel(path_end, mother_vessel.radius, self.config.vessel_step_size, parent_id= mother_vessel.id, children_ids=mother_vessel.children_ids, in_growth= mother_vessel.in_growth)
         for child_id in vessel_end.children_ids:
             child = self.get_vessel(child_id)
             child.parent_id = vessel_end.id
         #choose random point around branching point
         #random_point = branching_point + np.array([random.uniform(-mother_vessel.step, mother_vessel.step), random.uniform(-mother_vessel.step, mother_vessel.step), random.uniform(-mother_vessel.step, mother_vessel.step)])
         # the radius has to be updated later
+        mother_vessel.visible = visible
+        vessel_end.visible = visible
 
         vessel_new = Vessel([branching_point], self.config.radius_root_vessels, self.config.vessel_step_size, parent_id= mother_vessel.id)  # the radius has to be updated later
+        vessel_new.visible = True
         mother_vessel.children_ids = [vessel_end.id, vessel_new.id]
         self.list_of_vessels.append(vessel_end)
         self.list_of_vessels.append(vessel_new)
         # update the mother vessel
 
 
     def add_vessel(self, vessel: Vessel):
@@ -316,7 +319,13 @@
                 self.print_vessel_tree_recursive(vessels, root_vessel.children_ids, indent + 2)
 
     def compute_VSL(self):
         list_VSL = np.array([])
         for vessel in self.list_of_vessels:
             list_VSL = np.append(list_VSL, vessel.length())
         return list_VSL
+
+    def compute_diameters(self):
+        list_diameters = np.array([])
+        for vessel in self.list_of_vessels:
+            list_diameters = np.append(list_diameters, vessel.radius*2)
+        return list_diameters
```

### Comparing `OncoAMBER-1.2.1/amber/Voxel.py` & `OncoAMBER-1.2.2/amber/Voxel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
 def sigmoid(L, x, x0, k):
     return L/(1 + np.exp(-k*(x-x0)))
 
 class Voxel(object): #extra parameters are max_occupancy, viscosity
-        def __init__(self, position = np.array([0,0,0]), half_length = 0.1, viscosity = 100, list_of_cells_in=None, oxygen = 0, voxel_number = 0):
+        def __init__(self, position, half_length, viscosity, list_of_cells_in=None, oxygen = 0, voxel_number = 0):
                 if list_of_cells_in is None:
                         list_of_cells_in = []
                 self.position = position
                 self.half_length = half_length
                 self.list_of_cells = list_of_cells_in
                 self.list_of_necrotic_cells = []
                 self.oxygen = oxygen
```

### Comparing `OncoAMBER-1.2.1/amber/World.py` & `OncoAMBER-1.2.2/amber/World.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,20 @@
             for j in range(self.number_of_voxels):
                 for k in range(self.number_of_voxels):
                     position = np.array([
                         i * voxel_length - self.half_length + voxel_length / 2,
                         j * voxel_length - self.half_length + voxel_length / 2,
                         k * voxel_length - self.half_length + voxel_length / 2
                     ])
-                    self.voxel_list.append(Voxel(position, self.half_length / self.number_of_voxels, voxel_number=i * self.number_of_voxels ** 2 + j * self.number_of_voxels + k))
+                    self.voxel_list.append(Voxel(position, self.half_length / self.number_of_voxels, viscosity= self.config.viscosity, voxel_number=i * self.number_of_voxels ** 2 + j * self.number_of_voxels + k))
         self.vasculature = VasculatureNetwork(self.config)
+        self.o_volume_values = []
+        self.o_length_values = []
+        self.o_bifurcation_values = []
+        self.o_VSL_values = []
 
     def initiate_vasculature(self, list_of_mother_vessels):
         self.vasculature = VasculatureNetwork(self.config, list_of_mother_vessels)
         return
 
     def vasculature_growth(self, dt, splitting_rate, macro_steps=1, micro_steps=10, weight_direction=0.5, weight_vegf=0.5, weight_pressure=0.5, radius_pressure_sensitive = False):
         print('Vasculature growth')
@@ -215,19 +219,17 @@
         neighbors = [n for n in neighbors if 0 <= n < num_voxels ** 3]
         neighbors_voxels = [self.voxel_list[n] for n in neighbors]
         return neighbors_voxels
 
     def compute_exchange_matrix(self, dt, pressure_threshold):
         V = self.voxel_list[0].volume
         total_voxels = self.total_number_of_voxels
-
         # Extract pressure and viscosity values for all voxels
         pressures = np.array([voxel.pressure() for voxel in self.voxel_list])
         viscosities = np.array([voxel.viscosity for voxel in self.voxel_list])
-
         # Initialize migration matrix with zeros
         migration_matrix = sparse.lil_matrix((total_voxels, total_voxels), dtype=np.float32)
 
         for i in range(total_voxels):
             voxel_i = self.voxel_list[i]
             voxel_pressure = pressures[i]
             viscosity = viscosities[i]
@@ -236,16 +238,19 @@
             neighbors = self.find_neighbors(voxel_i)
 
             for neighbor in neighbors:
                 j = neighbor.voxel_number
 
                 pressure_diff = voxel_pressure - pressures[j]
                 if pressure_diff > pressure_threshold:
+
                     t_res = (V / pressure_diff) * viscosity
-                    if self.config.verbose: print('t_res = ', t_res)
+                    if self.config.verbose:
+                        print('V, pressure diff, viscosity ', V, pressure_diff, viscosity)
+                        print('t_res = ', t_res)
                     n_events = dt / t_res
                     migration_matrix[i, j] = n_events
 
         # Convert the lil_matrix to a csr_matrix for faster arithmetic operations
         migration_matrix = migration_matrix.tocsr()
 
         return migration_matrix
@@ -472,52 +477,90 @@
     def measure_tumor_volume(self):
         volume = 0
         for voxel in self.voxel_list:
             if voxel.number_of_tumor_cells() > 3:
                 volume += voxel.volume
         return volume
 
-    def show_angiogenesis_metrics(self, real = True):
+    def show_angiogenesis_metrics(self, real=True, first=True):
         # Extract the voxel values for each parameter
         volume = self.voxel_list[0].volume
-        side = self.voxel_list[0].half_length*2
+        side = self.voxel_list[0].half_length * 2
         if real:
-            volume_values = [voxel.vessel_volume/volume for voxel in self.voxel_list]
-            length_values = [voxel.vessel_length/volume for voxel in self.voxel_list]
+            volume_values = [voxel.vessel_volume / volume for voxel in self.voxel_list]
+            length_values = [voxel.vessel_length / volume for voxel in self.voxel_list]
 
         else:
-            capillary_volume = side*np.pi*self.config.effective_vessel_radius**2
-            volume_values = [voxel.oxygen*capillary_volume/volume for voxel in self.voxel_list]
-            length_values = [voxel.oxygen*side/volume for voxel in self.voxel_list]
+            capillary_volume = side * np.pi * self.config.effective_vessel_radius ** 2
+            volume_values = [voxel.oxygen * capillary_volume / volume for voxel in self.voxel_list]
+            length_values = [voxel.oxygen * side / volume for voxel in self.voxel_list]
 
         bifurcation_values = [voxel.bifurcation_density / volume for voxel in self.voxel_list]
         VSL_values = self.vasculature.compute_VSL()
-        # Calculate mean and median values
-        volume_mean = np.mean(volume_values)
-        volume_median = np.median(volume_values)
+        diameters_values = self.vasculature.compute_diameters()
+
+        # save values
+        if first:
+            self.o_diameters = diameters_values
+            self.o_length_values = length_values
+            self.o_bifurcation_values = bifurcation_values
+            self.o_VSL_values = VSL_values
+
+        # Compute statistics for current distribution
+        diameter_mean = np.mean(diameters_values)
+        diameter_median = np.median(diameters_values)
         length_mean = np.mean(length_values)
         length_median = np.median(length_values)
         bifurcation_mean = np.mean(bifurcation_values)
         bifurcation_median = np.median(bifurcation_values)
         VSL_mean = np.mean(VSL_values)
         VSL_median = np.median(VSL_values)
 
         # Plot histograms for each parameter
         fig, axes = plt.subplots(2, 2, figsize=(10, 8))
-        axes[0, 0].hist(volume_values, bins=20, color='blue')
-        axes[0, 0].set_title(f'Vessel volume density, mean: {volume_mean:.2f}, median: {volume_median:.2f}')
-        axes[0, 1].hist(length_values, bins=20, color='green')
-        axes[0, 1].set_title(f'Vessel length density, mean: {length_mean:.2f}, median: {length_median:.2f}')
-        axes[1, 0].hist(bifurcation_values, bins=20, color='red')
-        axes[1, 0].set_title(
-            f'Voxel bifurcation density, mean: {bifurcation_mean:.2f}, median: {bifurcation_median:.2f}')
-        axes[1, 1].hist(VSL_values, bins=20, color='purple')
-        axes[1, 1].set_title(f'Vessel segment length, mean: {VSL_mean:.2f}, median: {VSL_median:.2f}')
+
+        # Plot histogram for original distribution
+        axes[0, 0].hist(self.o_diameters, bins=20, color='gray', alpha=0.5, label='Original')
+        axes[0, 1].hist(self.o_length_values, bins=20, color='gray', alpha=0.5, label='Original')
+        axes[1, 0].hist(self.o_bifurcation_values, bins=20, color='gray', alpha=0.5, label='Original')
+        axes[1, 1].hist(self.o_VSL_values, bins=20, color='gray', alpha=0.5, label='Original')
+
+        # Plot histogram for current distribution
+        axes[0, 0].hist(diameters_values, bins=20, color='blue', alpha=0.5, label='Current')
+        axes[0, 1].hist(length_values, bins=20, color='green', alpha=0.5, label='Current')
+        axes[1, 0].hist(bifurcation_values, bins=20, color='red', alpha=0.5, label='Current')
+        axes[1, 1].hist(VSL_values, bins=20, color='purple', alpha=0.5, label='Current')
+
+        # Add titles and legend to the histograms
+        axes[0, 0].set_title(f'Vessel diameters\nMean: {diameter_mean:.2f}, Median: {diameter_median:.2f}')
+        axes[0, 0].legend()
+        axes[0, 1].set_title(f'Vessel length density\nMean: {length_mean:.2f}, Median: {length_median:.2f}')
+        axes[1, 0].legend()
+        axes[1, 0].set_title(f'Vessel bifurcation density\nMean: {bifurcation_mean:.2f}, Median: {bifurcation_median:.2f}')
+        axes[0, 1].legend()
+        axes[1, 1].set_title(f'Vessel segment length\nMean: {VSL_mean:.2f}, Median: {VSL_median:.2f}')
+        axes[1, 1].legend()
+
+        fig.suptitle('Angiogenesis Metrics')
+        fig.tight_layout()
+        # Show the plot
         plt.show()
 
+        #print a table with the values of the metrics for the current distribution, mean, median, std, min, max
+        print('Angiogenesis Metrics')
+        print('Diameters')
+        print(f'Mean: {diameter_mean:.2f}, Median: {diameter_median:.2f}, Std: {np.std(diameters_values):.2f}, Min: {np.min(diameters_values):.2f}, Max: {np.max(volume_values):.2f}')
+        print('Length density')
+        print(f'Mean: {length_mean:.2f}, Median: {length_median:.2f}, Std: {np.std(length_values):.2f}, Min: {np.min(length_values):.2f}, Max: {np.max(length_values):.2f}')
+        print('Bifurcation density')
+        print(f'Mean: {bifurcation_mean:.2f}, Median: {bifurcation_median:.2f}, Std: {np.std(bifurcation_values):.2f}, Min: {np.min(bifurcation_values):.2f}, Max: {np.max(bifurcation_values):.2f}')
+        print('Vessel segment length')
+        print(f'Mean: {VSL_mean:.2f}, Median: {VSL_median:.2f}, Std: {np.std(VSL_values):.2f}, Min: {np.min(VSL_values):.2f}, Max: {np.max(VSL_values):.2f}')
+
+
```

### Comparing `OncoAMBER-1.2.1/amber/save_alpha_dataframe6.csv` & `OncoAMBER-1.2.2/amber/save_alpha_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.1/amber/save_beta_dataframe6.csv` & `OncoAMBER-1.2.2/amber/save_beta_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.2.1/setup.py` & `OncoAMBER-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Package meta-data
 NAME = 'OncoAMBER'
 DESCRIPTION = 'Agent-based model of tumor growth and response to radiation therapy'
 URL = 'https://github.com/lvkunz/AMBER'
 EMAIL = 'lvkunz@mgh.harvard.edu'
 AUTHOR = 'Louis Kunz'
 REQUIRES_PYTHON = '>=3.8.2'
-VERSION = '1.2.1'
+VERSION = '1.2.2'
 
 # Required packages for this module to be executed
 REQUIRED = ['numpy', 'pandas', 'scipy']
 
 # Optional packages
 EXTRAS = { 'plots' :['matplotlib', 'seaborn'] }
```

