# Comparing `tmp/gliderflight-1.1.0.tar.gz` & `tmp/gliderflight-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gliderflight-1.1.0.tar", last modified: Mon Mar  2 10:24:22 2020, max compression
+gzip compressed data, was "gliderflight-1.2.0.tar", last modified: Tue May  9 09:25:09 2023, max compression
```

## Comparing `gliderflight-1.1.0.tar` & `gliderflight-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2020-03-02 10:24:22.000000 gliderflight-1.1.0/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       84 2018-09-25 06:07:00.000000 gliderflight-1.1.0/MANIFEST.in
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     9930 2020-03-02 10:24:22.000000 gliderflight-1.1.0/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     7528 2020-03-02 10:23:10.000000 gliderflight-1.1.0/README.rst
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2020-03-02 10:24:22.000000 gliderflight-1.1.0/data/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    50848 2018-08-31 19:50:00.000000 gliderflight-1.1.0/data/U_kalman_datasetIII.npy
--rw-rw-r--   0 lucas     (1000) lucas     (1000)   630800 2018-08-31 19:50:00.000000 gliderflight-1.1.0/data/gliderflight_data.npy
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2020-03-02 10:24:22.000000 gliderflight-1.1.0/examples/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1272 2019-03-20 08:28:59.000000 gliderflight-1.1.0/examples/create_data_file.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1956 2018-09-25 06:07:00.000000 gliderflight-1.1.0/examples/my_first_example.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2020-03-02 10:24:22.000000 gliderflight-1.1.0/gliderflight/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      176 2020-03-02 09:34:20.000000 gliderflight-1.1.0/gliderflight/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    39081 2020-02-17 14:08:47.000000 gliderflight-1.1.0/gliderflight/gliderflight.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     9341 2018-12-12 13:09:00.000000 gliderflight-1.1.0/gliderflight/glidertrim.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2020-03-02 10:24:22.000000 gliderflight-1.1.0/gliderflight.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     9930 2020-03-02 10:24:22.000000 gliderflight-1.1.0/gliderflight.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      461 2020-03-02 10:24:22.000000 gliderflight-1.1.0/gliderflight.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2020-03-02 10:24:22.000000 gliderflight-1.1.0/gliderflight.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       77 2020-03-02 10:24:22.000000 gliderflight-1.1.0/gliderflight.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       72 2020-03-02 10:24:22.000000 gliderflight-1.1.0/gliderflight.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       13 2020-03-02 10:24:22.000000 gliderflight-1.1.0/gliderflight.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       72 2018-12-10 10:34:00.000000 gliderflight-1.1.0/requirements.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2020-03-02 10:24:22.000000 gliderflight-1.1.0/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1682 2020-03-02 09:47:18.000000 gliderflight-1.1.0/setup.py
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2023-05-09 09:25:09.844744 gliderflight-1.2.0/
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)     1100 2018-08-31 19:50:00.000000 gliderflight-1.2.0/LICENSE
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)       84 2018-09-25 06:07:00.000000 gliderflight-1.2.0/MANIFEST.in
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     8217 2023-05-09 09:25:09.844744 gliderflight-1.2.0/PKG-INFO
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     7528 2023-05-08 11:26:34.000000 gliderflight-1.2.0/README.rst
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2023-05-09 09:25:09.840744 gliderflight-1.2.0/data/
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)    50848 2018-08-31 19:50:00.000000 gliderflight-1.2.0/data/U_kalman_datasetIII.npy
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)   630800 2018-08-31 19:50:00.000000 gliderflight-1.2.0/data/gliderflight_data.npy
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2023-05-09 09:25:09.842744 gliderflight-1.2.0/examples/
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)     1272 2019-03-20 08:28:59.000000 gliderflight-1.2.0/examples/create_data_file.py
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)     1956 2018-09-25 06:07:00.000000 gliderflight-1.2.0/examples/my_first_example.py
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     1003 2022-02-25 13:59:32.000000 gliderflight-1.2.0/examples/steady_state_example.py
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2023-05-09 09:25:09.842744 gliderflight-1.2.0/gliderflight/
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)      192 2023-05-09 09:24:04.000000 gliderflight-1.2.0/gliderflight/__init__.py
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)    48411 2022-12-12 12:35:00.000000 gliderflight-1.2.0/gliderflight/gliderflight.py
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)     9747 2023-05-04 13:32:10.000000 gliderflight-1.2.0/gliderflight/glidertrim.py
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2023-05-09 09:25:09.843744 gliderflight-1.2.0/gliderflight.egg-info/
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)     8217 2023-05-09 09:25:09.000000 gliderflight-1.2.0/gliderflight.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)      539 2023-05-09 09:25:09.000000 gliderflight-1.2.0/gliderflight.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)        1 2023-05-09 09:25:09.000000 gliderflight-1.2.0/gliderflight.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)       60 2023-05-09 09:25:09.000000 gliderflight-1.2.0/gliderflight.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)       61 2023-05-09 09:25:09.000000 gliderflight-1.2.0/gliderflight.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)       13 2023-05-09 09:25:09.000000 gliderflight-1.2.0/gliderflight.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)       73 2022-02-25 13:52:23.000000 gliderflight-1.2.0/requirements.txt
+-rw-r--r--   0 lucas     (1001) kdt       (1030)       38 2023-05-09 09:25:09.844744 gliderflight-1.2.0/setup.cfg
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)     1682 2020-03-02 09:47:18.000000 gliderflight-1.2.0/setup.py
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2023-05-09 09:25:09.844744 gliderflight-1.2.0/test/
+-rw-rw-r--   0 lucas     (1001) kdt       (1030)     1029 2020-04-07 11:46:26.000000 gliderflight-1.2.0/test/test.py
+-rw-r--r--   0 lucas     (1001) kdt       (1030)       85 2021-02-08 15:54:33.000000 gliderflight-1.2.0/test/test_glidertrim.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gliderflight-1.1.0/README.rst` & `gliderflight-1.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
    # gm.alpha # angle of attack
    # gm.ug    # horizontal speed
    # gm.wg    # vertical speed
    # gm.w     # vertical water velocity
    
    # if we want to run a model with a given set of parameters
 
-   fm = DynamicGLiderModel(dt=1, rho0=1024, k1=0.02, k2=0.92)
+   fm = DynamicGliderModel(dt=1, rho0=1024, k1=0.02, k2=0.92)
    # copy the settings from the steady state model
    fm.copy_settings(gm)
 
    solution = fm.solve(data)
    
    # solution is now a named tuple, according to the definition:
    # Modelresult = namedtuple("Modelresult", "t u w U alpha pitch ww")
```

### Comparing `gliderflight-1.1.0/data/U_kalman_datasetIII.npy` & `gliderflight-1.2.0/data/U_kalman_datasetIII.npy`

 * *Files identical despite different names*

### Comparing `gliderflight-1.1.0/data/gliderflight_data.npy` & `gliderflight-1.2.0/data/gliderflight_data.npy`

 * *Files identical despite different names*

### Comparing `gliderflight-1.1.0/examples/create_data_file.py` & `gliderflight-1.2.0/examples/create_data_file.py`

 * *Files identical despite different names*

### Comparing `gliderflight-1.1.0/examples/my_first_example.py` & `gliderflight-1.2.0/examples/my_first_example.py`

 * *Files identical despite different names*

### Comparing `gliderflight-1.1.0/gliderflight/gliderflight.py` & `gliderflight-1.2.0/gliderflight/gliderflight.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,41 @@
-#Copyright (c) 2018 Helmholtz Zentrum Geesthacht, Germany
+#Copyright (c) 2018-2020 Helmholtz Zentrum Geesthacht, Germany
 #                   Lucas Merckelbach, lucas.merckelbach@hzg.de
 
-from collections import namedtuple
+from collections import namedtuple, defaultdict
 
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.optimize import fsolve, fmin as fminimize
-
-
-Modelresult = namedtuple("Modelresult", "t u w U alpha pitch ww")
-
-REFERENCE_VALUES = dict(Cd0=0.15, Vg=62, epsilon=5e-10, ah=3.8, mg=65)
+from scipy.integrate import solve_ivp, RK45
+from functools import partial
+import concurrent.futures
+from multiprocessing import cpu_count
+
+#import warnings
+#warnings.filterwarnings('error')
+from logging import getLogger
+
+logger = getLogger('gliderflight')
+
+
+Modelresult = namedtuple("Modelresult", "t u w U alpha pitch ww depth")
+Diagnostics = namedtuple("Diagnostics", "t rho U FB FD FL")
+
+REFERENCE_VALUES = dict(Cd0=0.15, Vg=62, epsilon=5e-10, ah=3.8, mg=65, Cd1=10)
+UNITS = defaultdict(lambda  : "-", Cd1="s^{-2}",S="m^2", mg="kg",
+                    Vg="m^3", Cd1_hull="s^{-2}", aw = "s^{-1}", ah="s^{-1}")
+
+DEBUG_PARALLEL_EXECUTION = False # Set to True to run the parallel
+                                 # jobs sequentially. This is useful
+                                 # when the intergration does not
+                                 # complete for some reason and throws
+                                 # an error. In parallel exectution it
+                                 # is not possible to inspect the
+                                 # trace.
 
 class ModelParameterError(BaseException):
     pass
 
 class ModelParameters(object):
     '''Configuration class for glider model parameters
 
@@ -42,14 +63,15 @@
 
     '''
     
 
     def __init__(self, parameterised_parameters_dict):
         
         self.parameters = 'Cd0 Cd1 S eOsborne AR Omega mg epsilon Vg Cd1_hull aw ah'.split()
+        self.parameter_units = dict([(k,UNITS[k]) for k in self.parameters]) 
         self.parametersAoa = 'Cd0 Cd1 eOsborne AR Omega S Cd1_hull ah aw'.split()
         self.parameterised_parameters = parameterised_parameters_dict
         self._parameterised_parameters = list(self.parameterised_parameters)
        
         for i in self.parameters:
             self.__dict__[i]=None
         self.__aoa_parameter_changed=True
@@ -337,14 +359,80 @@
 
     # providing easy access to useful computational results as attributes
     def __get_modelresult(self, p):
         if self.modelresult:
             i = self.modelresult._fields.index(p)
             return self.modelresult[i]
 
+    def remove_duplicate_time_entries(self, data):
+        # remove any entries in data that have duplicate time stamps.
+        t = data['time']
+        condition = np.ones(t.shape, int)
+        condition[1:] = np.diff(t)!=0
+        for k, v in data.items():
+            if not v is None:
+                data[k] = v.compress(condition)
+        if not self.mask is None:
+            self.mask = self.mask.compress(condition)
+        return data
+
+    def ensure_monotonicity(self, data, T_search_span=600):
+        '''
+        Ensure monotonicity of the data series.
+
+        Parameters
+        ----------
+        data : dict
+             dictionary with environment data.
+        T_search_span : float (600)
+             time span to search back in time for time gaps
+        
+        Returns
+        -------
+        dict
+            dictionary with updated environment data.
+
+        Notes
+        -----
+
+        Some times the glider clock gets corrected when it deviates
+        too much from the GPS time. This happens of course at the
+        surface. It can be that time is stepped backwards, which
+        means that the timestamps are not monotonic any more. The
+        strategy we adopt here is, because it happens at the
+        surface, we look if there is a time gap (due to data
+        transmission for example) in the interval 10 minutes prior
+        the time shift. Then we simply move this section of time
+        backwards as well. If this is not possible, we undo the time
+        correction and move all timeseries forward in time.
+
+        '''
+        data = self.remove_duplicate_time_entries(data)
+        t = data['time']
+        indices = np.arange(t.shape[0])
+        delta_t = np.diff(t)
+        delta_t_mean = np.median(delta_t)
+        idx = np.where(np.diff(t)<0)[0]
+        #loop through all time shifts, if any:
+        for m in idx:
+            dt_inv = delta_t[m]
+            logger.info(f"Detected a time reversal of {dt_inv:.1f} seconds for t={t[m]:.0f} seconds.")
+            k = max(0, m-int(T_search_span * delta_t_mean))
+            dt_fwd = delta_t[k:m].max()    
+            if dt_fwd > -dt_inv + delta_t_mean:
+                # we can easily correct because there is a time forward larger then we move back in time, some time before T_search_span.
+                i = k + np.argmax(delta_t[k:m])
+                t[i+1:m+1] += dt_inv - delta_t_mean # delta_t_mean is required as not to create a time duplicate.
+                logger.info("Time reversal is repaired.")
+            else:
+                # just undo the time shift for all later timestamps
+                t[m+1:] -= dt_inv
+                logger.info("Time reversal is undone.")
+        return data
+    
     @property        
     def t(self):
         ''' time (s)'''
         return self.__get_modelresult('t')
     @property        
     def U(self):
         ''' incident water velocity (m s$^{-1}$) '''
@@ -475,29 +563,36 @@
                              full_output=1)
                 num_result, result, err, mesg = tmp
                 aoas[i] = num_result
             self.ifun = interp1d(self.pitch_i, aoas)
         #
         idx = np.where(np.logical_and(np.abs(pitch)>=self.pitch_i.min(),
                                       np.abs(pitch)<=self.pitch_i.max()))[0]
-        aoa = np.zeros_like(pitch)
-        aoa[idx] = self.ifun(abs(pitch[idx]))*np.sign(pitch[idx])
+        if isinstance(pitch, float):
+            aoa = self.ifun(abs(pitch))*np.sign(pitch)
+        else:
+            aoa = np.zeros_like(pitch)
+            aoa[idx] = self.ifun(abs(pitch[idx]))*np.sign(pitch[idx])
         return aoa
         
     def solve_model(self, rho, FB, pitch, Fg):
         ''' Solves first for angle of attack and then incident velocity
         
         Not intended to be called directly.
         '''
         alpha = self.solve_for_angle_of_attack(pitch)
         
         q=(FB-Fg)*np.sin(pitch+alpha)/(self.Cd0+self.Cd1*alpha**2)
         Usquared=2.*q/rho/self.S
-        jdx = np.where(Usquared<0)[0]
-        Usquared[jdx]=0
+        if isinstance(Usquared, float):
+            if Usquared<0:
+                Usquared=0
+        else:
+            jdx = np.where(Usquared<0)[0]
+            Usquared[jdx]=0
         U = Usquared**0.5
         return alpha, U
 
     def solve(self, data=None):
         ''' Solve the model
 
         Solves the flight model.
@@ -525,15 +620,14 @@
         >>> gm.define(mg=70, Vg=68)
         >>> data = dict(time=time, pressure=P, pitch=pitch, buoyancy_change=vb, density=rho)
         >>> gm.solve(data)
         >>> plot(gm.U)
         '''
         if data is None:
             data = self.input_data
-            
         pitch = data['pitch']
         rho = data['density']
         try:
             dhdt = data['dhdt']
         except KeyError:
             dhdt = self.compute_dhdt(data['time'], data['pressure'])
             data['dhdt'] = dhdt
@@ -542,15 +636,17 @@
                                                         data['buoyancy_change'])
         FB, Fg = self.compute_FB_and_Fg(pressure, rho, Vbp)
         alpha, U = self.solve_model(rho, FB, pitch, Fg)
         wg = np.sin(pitch+alpha)*U
         ug = np.cos(pitch+alpha)*U
         ww = dhdt - wg
         q, L,D = self.compute_lift_and_drag(alpha, U, rho)
-        self.modelresult = Modelresult(data["time"], ug, wg, U, alpha, pitch, ww)  
+        self.modelresult = Modelresult(data["time"], ug, wg, U, alpha, pitch, ww, ww*0)
+        self.diagnostics = Diagnostics(data["time"], rho, U, FB, D, L)
+        
         return self.modelresult
     
 
 class DynamicGliderModel(ModelParameters, GliderModel):
     ''' Dynamic glider model implementation
 
     This class inherits from ModelParameters and GliderModel. The physcis are
@@ -570,16 +666,17 @@
         added mass fraction perpendicular to longitudinal direction
     alpha_linear : float
         angle (rad) up to which the parameterisation is considered linear
     alpha_stall : float
         angle (rad) up to which no lift will be generated (stalling angle)
     max_depth_considered_surface : float
         depth as reported by the pressure sensor which is considered the surface (u=w=0)
-
-
+    max_CPUs : int
+        maximum number of CPUs to use (clips at system availabel CPUs)
+    
 
     The only method provided by this class that is of interest to the user is solve().
     The input to solve is a dictionary with time, pressure, pitch, buoyancy change density.
 
     Methods inherited from ModelParameters can be used to define/set model coefficients, and 
     to copy settings from another model instance.
     
@@ -601,41 +698,24 @@
     >>>dm.define(mg=70)
     >>>dm.define(Vg=68, Cd0=0.15)
     >>>dm.solve(dict(time=tctd, pressure=P, pitch=pitch, buoyancy_change=buoyancy_drive, density=density))
     >>>print(dm.U)
     '''
 
     def __init__(self, dt=None, rho0=None, k1=0.20, k2=0.92, alpha_linear=90, alpha_stall=90,
-                 max_depth_considered_surface=0.5):
-        ''' Constructor
-
-        :param dt: time step (s)
-        :param rho0: background density (kg m$^{-3}$)
-        :param k1: added mass fraction in longitudinal direction
-        :param k2: added mass fraction perpendicular to longitudinal direction
-        :param alpha_linear: angle in degree, up to where lift force is linear with angle of attack
-        :param alpha_stall: angle in degree where stall occurs
-        :param max_depth_considered_surface: depths shallower than this are considered at the surface and (u,v)=0
-        :type dt: float
-        :type rho0: float
-        :type k1: float
-        :type k2: float
-        :type alpha_linear: float
-        :type alpha_stall: float
-        :type max_depth_considered_surface: float
-
-        '''
+                 max_depth_considered_surface=0.5, max_CPUs=None):
         ModelParameters.__init__(self, dict(aw=self.awEstimate, Cd1=self.cd1Estimate))
         GliderModel.__init__(self, rho0=rho0)
         self.k1 = k1
         self.k2 = k2 
         self.alpha_linear = alpha_linear*np.pi/180 # 90 degrees : disable
         self.alpha_stall = 90*np.pi/180 # 90 degrees: disable
         self.dt = dt
         self.max_depth_considered_surface = max_depth_considered_surface
+        self.max_CPUs = max_CPUs
         
     def stall_factor(self, alpha):
         alpha_abs = abs(alpha)
         if alpha_abs<self.alpha_linear:
             r = 1.
         else:
             d_alpha = alpha_abs - self.alpha_linear
@@ -745,112 +825,203 @@
         denom = self.mg**2 + (m22+m11)*self.mg + m11*m22
         M11 = ((m22-m11)*C2 + m11 + self.mg) / denom
         M12 = ((m22-m11)*CS) / denom
         M21 = M12
         M22 = (-(m22-m11)*C2 + m22 + self.mg) / denom
         return M11, M12, M21, M22
 
-    def RK4_parallel(self, h, M, FBg, pitch, rho, at_surface, Cd0, u, w, nproc=24):
-        N = len(u)
-        n = N//nproc
-        _u = np.zeros_like(u)
-        _w = np.zeros_like(u)
-        for p in range(nproc):
-            print(f"Process {p}")
-            s = slice(p*n, (p+1)*n)
-            _M = (m[s] for m in M)
-            _u[s], _w[s] = self.RK4(h, _M, FBg[s], pitch[s], rho[s], at_surface[s], Cd0, u[s], w[s])
-           
+    def _compute_time_intervals(self, ncpu, tm, lead_time=300):
+        dt = tm.ptp()/ncpu
+        intervals = []
+        for i in range(ncpu):
+            t0=tm[0]+i*dt
+            t1=tm[0]+(i+1)*dt
+            tm_eval = tm.compress(np.logical_and(tm>=t0, tm<=t1))
+            if i>0:
+                t0-=lead_time
+            if len(tm_eval) > 0: # if zero we have no data to evaluate, integration crashes.
+                intervals.append((t0, t1, tm_eval))
+        return intervals
     
-    def integrate(self, data, dt=None):
+    def _integrate_rk45_fun(self, t, uw, rho_fun=None, pitch_fun=None, FBg_fun=None,
+                            m11_fun=None, m12_fun=None, m21_fun=None,
+                            m22_fun=None, Cd0_fun=None, at_surface_fun=None):
+        u, w, z= uw
+        if at_surface_fun(t):
+            uw1 = -uw/5.    # this has the effect that the velocity
+                            # approaches 0 with a timescale of 5
+                            # seconds.
+        else:
+            U = (u**2 + w**2)**(0.5)
+            _pitch = pitch_fun(t)
+            alpha = np.arctan2(w, u) - _pitch
+            q, L, D = self.compute_lift_and_drag(alpha, U, rho_fun(t), Cd0_fun(t))
+            Fx = -np.cos(_pitch + alpha) * D + np.sin(_pitch + alpha)*L
+            Fy = -np.cos(_pitch + alpha) * L - np.sin(_pitch + alpha)*D + FBg_fun(t)
+            uw1 = np.array([(m11_fun(t)*Fx + m12_fun(t)*Fy),
+                            (m21_fun(t)*Fx + m22_fun(t)*Fy),
+                            w])
+        return uw1
+
+        
+    def integrate(self, data):
         ''' integrate system
 
         not to be called directly
         '''
         tm = data['time']
         pitch = data['pitch']
         m_water_pressure = data['pressure']
         rho = data['density']
         m_de_oil_vol = data['buoyancy_change']
         dhdt = data['dhdt']
         pressure, Vbp = self.convert_pressure_Vbp_to_SI(m_water_pressure, m_de_oil_vol)
-
-        h = dt or 2.
-        ti = np.arange(tm.min(), tm.max()+h, h)
-        pitch = np.interp(ti, tm, pitch)
-        pressure = np.interp(ti, tm, pressure)
-        rho = np.interp(ti, tm, rho)
-        Vbp = np.interp(ti, tm, Vbp)
-        dhdt = np.interp(ti, tm, dhdt)
-        # if model coefficients are callable, assume they are interpolating functions
         mg = Vg = Cd0 = None
         if callable(self.mg):
             mg = self.mg(ti)
+        else:
+            mg = self.mg
         if callable(self.Vg):
             Vg = self.Vg(ti)
-        if callable(self.Cd0):
+        else:
+            Vg = self.Vg
+        if callable(self.Cd0): # we need to evaluate Cd inside the
+                               # force balance and depends on the
+                               # unknown u,w vector. So we need to
+                               # make an interpolating function
+                               # later. Make sure Cd0 is length tm.
             Cd0 = self.Cd0(ti)
-            
+        else:
+            Cd0 = self.Cd0 * np.ones_like(tm)
+
         FB, Fg = self.compute_FB_and_Fg(pressure, rho, Vbp, mg, Vg)
         M = self.compute_inverted_mass_matrix(pitch)
-
-        u = np.zeros_like(FB)
-        w = np.zeros_like(FB)
+        FBg = FB-Fg
         threshold = self.max_depth_considered_surface * 1e4 # in Pa.
-        self.RK4(h, M, FB-Fg, pitch, rho, pressure<threshold, Cd0, u, w)
-        #self.RK4_parallel(h, M, FB-Fg, pitch, rho, pressure<threshold, Cd0, u, w, nproc=24)
-
+        at_surface = pressure<threshold
+        
+        # create interpolating functions of the variables we need
+        options = dict(bounds_error=False, fill_value="extrapolate")
+        m11_fun = interp1d(tm, M[0], **options)
+        m12_fun = interp1d(tm, M[1], **options)
+        m21_fun = interp1d(tm, M[2], **options)
+        m22_fun = interp1d(tm, M[3], **options)
+        pitch_fun = interp1d(tm, pitch, **options)
+        rho_fun = interp1d(tm, rho, **options)
+        FBg_fun = interp1d(tm, FBg, **options)
+        at_surface_fun = interp1d(tm, at_surface, **options)
+        Cd0_fun = interp1d(tm, Cd0, **options)
+        self.tmp_at_surface_fun = at_surface_fun
+        # function to integrate:
+        arg_funs = dict(rho_fun=rho_fun, pitch_fun=pitch_fun,
+                        FBg_fun = FBg_fun, m11_fun=m11_fun, m12_fun=m12_fun, m21_fun=m21_fun,
+                        m22_fun=m22_fun, Cd0_fun=Cd0_fun, at_surface_fun=at_surface_fun)
+        
+        ncpu = cpu_count()
+        if not self.max_CPUs is None:
+            ncpu = min(ncpu, self.max_CPUs)
+        intervals = [(k, interval) for k, interval in enumerate(self._compute_time_intervals(ncpu, tm, lead_time=300))]
+        
+        if not DEBUG_PARALLEL_EXECUTION:
+            logger.info(f"Parallel execution using {len(intervals)} processes.")
+            with concurrent.futures.ProcessPoolExecutor(ncpu) as p:
+                results = p.map(partial(self.process_fun, **arg_funs), intervals)
+            results = list(results)
+        else:
+            logger.info("Forcing serial execution.")
+            results=[]
+            for i, interval in enumerate(intervals):
+                #if i<7:
+                #    continue
+                logger.info(f"Processing interval {i}/{len(intervals)}...")
+                results.append(self.process_fun(interval, **arg_funs))
+        u, w, z = self.assemble_results(results, intervals)
         gamma = np.arctan2(w, u)
         alpha = gamma - pitch
         Umag = (u**2 + w**2)**(0.5)
         ur = np.cos(pitch)*u + np.sin(pitch)*w
         wr = -np.sin(pitch)*u + np.cos(pitch)*w
-        return Modelresult(ti, u, w, Umag, alpha, pitch, dhdt-w)
+        return Modelresult(tm, u, w, Umag, alpha, pitch, dhdt-w, z)
+
+        
+    def assemble_results(self, results, intervals):
+        success = True
+        y = []
+        for r in results:
+            if r is None: # integration failed.
+                success = False
+                continue 
+            y.append(r.y)
+            success &= r.success
+        u, w, z = np.hstack(y)
+        return u, w, z
+        
+    def process_fun(self, interval, **arg_funs):
+        k, (t0, t1, tm) = interval
+        fun = partial(self._integrate_rk45_fun, **arg_funs)
+        if DEBUG_PARALLEL_EXECUTION:
+            # triggers an error if solve_ivp fails.
+            result = solve_ivp(fun, (t0, t1), y0=np.array([0.0,0.0, 0.0]), t_eval=tm, first_step=0.25)
+        else:
+            # handle the error
+            try:
+                result = solve_ivp(fun, (t0, t1), y0=np.array([0.0,0.0,0.0]), t_eval=tm, first_step=0.25)
+            except ValueError as e:
+                m = f"Solving for interval {k} failed.\nInterval from {t0:.1f} - {t1:.1f}."
+                logger.error(m)
+                result = None
+        return result
 
     def solve(self, data=None):
         ''' Solve the model
 
         Solves the flight model.
 
         Parameters
         ----------
         data : dict or None
             environment data (see Notes)
-        
         Returns
         -------
         modelresult : Modelresult
             model result (named tuple with arrays of computed results)
 
         Notes
         -----
         The data supplied should contain at least time, pressure, pitch, buoyancy_change and
         density, as reported by the glider. Depth rate (dhdt) will be added if not already present.
         Other data are ignored.
 
+        The intergration of the model maps the results on the time vector. For this to work successfully
+        it is essential that there are no time duplicates or time reversals. The latter can occur when
+        the system clock is updated with GPS time. 
+
+        Use the methods :func:`~gliderflight.GliderModel.remove_duplicate_time_entries` and
+        :func:`~gliderflight.GliderModel.ensure_monotonicity`.
+
         Examples
         --------
         >>> dm = DynamciGliderModel(dt=1, k1=0.2, k2=0.98, rho0=1024)
         >>> dm.define(mg=70, Vg=68)
         >>> data = dict(time=time, pressure=P, pitch=pitch, buoyancy_change=vb, density=rho)
         >>> dm.solve(data)
         >>> plot(dm.U)
         '''
 
         if data is None:
             data = self.input_data
-            
+
         pitch = data['pitch']
         try:
             dhdt = data['dhdt']
         except KeyError:
             dhdt = self.compute_dhdt(data['time'], data['pressure'])
             data['dhdt'] = dhdt
 
-        integration_result = self.integrate(data, self.dt)
+        integration_result = self.integrate(data)
         self.modelresult = Modelresult(*[np.interp(data['time'],
                                                    integration_result.t, v) for v in integration_result])
         return self.modelresult
 
     
 class Calibrate(object):
     ''' Generic class providing the calibration machinery for steady-state and dynamic flight models 
@@ -862,18 +1033,23 @@
           at the start of the dive, pycnoclines, etc.
         * run the calibration.
        
 
         Logical operators are used to mask data:
 
         OR, AND, and NAND are implemented, and work on the *mask*
-
+    
+        Parameters
+        ----------
+        xtol : float
+            tolerance in error in the parameters to be minimised.
     '''
-    def __init__(self):
+    def __init__(self, xtol=1e-4):
         self.mask=None
+        self.xtol = xtol
         
     def set_mask(self,mask):
         '''Set a mask 
 
         Masks those data that should not be used to calibrate.
        
         Parameters
@@ -964,17 +1140,18 @@
 
         Notes
         -----
         A mask is automatically created (including all data) when this method is called.
         '''
         if dhdt is None:
             dhdt = self.compute_dhdt(time, pressure)
-        self.input_data = dict(time=time ,pressure=pressure, pitch=pitch, buoyancy_change=buoyancy_change,
-                               density=density, dhdt=dhdt, u_relative=u_relative, w_relative=w_relative,
-                               U_relative=U_relative)
+        data = dict(time=time ,pressure=pressure, pitch=pitch, buoyancy_change=buoyancy_change,
+                    density=density, dhdt=dhdt, u_relative=u_relative, w_relative=w_relative,
+                    U_relative=U_relative)
+        self.input_data = data
         mask=np.zeros(time.shape,'int').astype(bool) # use all data by default
         self.set_mask(mask)
         
                         
     def cost_function(self,x,parameters, constraints, weights, verbose):
         ''' Cost-function used to optimise parameters
 
@@ -994,22 +1171,39 @@
         verbose : bool
             print intermediate results during optimising if set True
         
         Returns
         -------
         mse : float
             RMS value of exposed measurements (not masked)
+
+
+        Constraints
+        -----------
+
+        Different constraints can be applied, and if more than one, their relative contribution is set with weights.
+
+        Valid options:
+        
+        dhdt : the error is computed from the difference between modelled w and observed dhdt
+        w_relative : the error is computed from the difference between modelled w and w_relative (set separately to data dictionary)
+        u_relative : the error is computed from the difference between modelled u and u_relative (set separately to data dictionary)
+        U_relative : the error is computed from the difference between modelled U and U_relative (set separately to data dictionary)
+        
+        depth : (experimental) the error is computed from the modelled and observed glider depth.
+
         '''
         # set the data
         kwds=dict([(_p,_x*REFERENCE_VALUES[_p]) for _p,_x in zip(parameters,x)])
         self.define(**kwds) # ensures that aoa is reinitialised if necessary
         self.solve(self.input_data)
         U = self.modelresult.U
         alpha = self.modelresult.alpha
-
+        depth_mod = self.modelresult.depth
+        
         if not isinstance(weights, np.ndarray):
             weights = weights or np.ones_like(constraints, float)/len(constraints)
 
         w_mod = U*np.sin(self.input_data['pitch']+alpha)
         u_mod = U*np.cos(self.input_data['pitch']+alpha)
 
         error = 0
@@ -1026,14 +1220,17 @@
                 elif constraint == 'U_relative':
                     error += weight * (U - self.input_data['U_relative'])**2
                 else:
                     raise NotImplementedError()
         else:
             if constraints[0] == 'dhdt' and len(constraints)==1:
                 error += weights * (w_mod - self.input_data['dhdt'])**2
+            elif constraints[0] == 'depth' and len(constraints)==1:
+                _rho_mean = self.input_data['density'].mean()
+                error += weights * (depth_mod + self.input_data['pressure']*1e5/9.81/_rho_mean)**2
             else:
                 raise NotImplementedError()
         error = error.compress(~self.mask)
         mse = np.nanmean(error)
         if verbose:
             s="  ".join(["{:s}={:.4g}".format(k,v) for k,v in kwds.items()])
             print("Error: {:.7e}  -  {}".format(mse, s))
@@ -1081,16 +1278,16 @@
         The default measurement to evaluate the model against is the depth rate dhdt. If not specified when
         setting the input data using the set_input_data() method, it is computed automatically. Other velocity
         components that are to be used to calibrate the model have to be set specifically.
         '''
         constraints = self.__ensure_iterable(constraints)
         x0=[self.__dict__[i]/REFERENCE_VALUES[i] for i in p] # scale the parameters to order 1
         args = (p, constraints, weights, verbose)
-        R=fminimize(self.cost_function,x0,args=args,disp=False)
-        rv=dict([(k,v) for k,v in zip(p,R)])
+        R=fminimize(self.cost_function,x0,args=args,disp=False, xtol=self.xtol)
+        rv=dict([(k,v*REFERENCE_VALUES[k]) for k,v in zip(p,R)])
         return rv
 
     def __ensure_booltype(self, mask):
         if mask.dtype==bool:
             return mask
         else:
             return mask.astype(bool)
@@ -1111,13 +1308,17 @@
     def __init__(self, rho0=None):
         SteadyStateGliderModel.__init__(self, rho0)
         Calibrate.__init__(self)
 
 
 class DynamicCalibrate(DynamicGliderModel, Calibrate):
     ''' Dynamic glider flight model, with calibration interface '''
-    def __init__(self, rho0=None, k1=0.02, k2=0.92, dt = None):
-        DynamicGliderModel.__init__(self, dt=dt, rho0=rho0, k1=k1, k2=k2)
-        Calibrate.__init__(self)
+    def __init__(self, rho0=None, k1=0.02, k2=0.92, dt = None, alpha_linear=90, alpha_stall=90,
+                 max_depth_considered_surface=0.5, max_CPUs=None):
+        DynamicGliderModel.__init__(self, dt=dt, rho0=rho0, k1=k1, k2=k2,
+                                    alpha_linear=alpha_linear, alpha_stall=alpha_stall,
+                                    max_depth_considered_surface=max_depth_considered_surface,
+                                    max_CPUs=max_CPUs)
+        Calibrate.__init__(self, xtol=1e-2)
```

### Comparing `gliderflight-1.1.0/gliderflight/glidertrim.py` & `gliderflight-1.2.0/gliderflight/glidertrim.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,32 +6,30 @@
 import os
 import sys
 
 import numpy as np
 import matplotlib
 matplotlib.use('TkAgg')
 from matplotlib import pyplot
-from matplotlib.dates import epoch2num, DateFormatter
 
 import gsw
 
 import dbdreader
 import gliderflight
 
 
 DEFAULTS = dict(target_density=1025, mg=65, Vg=65e-3, minlimitdepth=10, maxlimitdepth=30,
-                cond_a=1.0, cond_b=0., buoyancy_engine='shallow',latitude=54, longitude=8,
+                cond_a=1.0, cond_b=0., buoyancy_engine='shallow',
                 calibrate_epsilon='no')
 class UI(object):
     CONFIGFILE=os.path.join(os.environ['HOME'],'.glidertrimrc')    
-    FLOAT_OPTIONS = "target_density mg Vg minlimitdepth maxlimitdepth cond_a cond_b latitude longitude".split()
+    FLOAT_OPTIONS = "target_density mg Vg minlimitdepth maxlimitdepth cond_a cond_b".split()
     STR_OPTIONS = ["buoyancy_engine", "calibrate_epsilon"]
     UNITS = dict(mg="kg", Vg="m^3", minlimitdepth="m", maxlimitdepth="m", cond_a="m/S",
-                 cond_b="-", buoyancy_engine="shallow|deep", latitude='decimal deg',
-                 longitude='decimal deg', calibrate_epsilon='yes|no',
+                 cond_b="-", buoyancy_engine="shallow|deep", calibrate_epsilon='yes|no',
                  target_density='kg/m^3')
     
     def __init__(self):
         self.configparser=configparser.ConfigParser()
         self.settings = {}
 
     def get_glidername_and_filenames(self):
@@ -111,28 +109,34 @@
     def read_dbds(self, fns, settings):
         if settings['buoyancy_engine']=='shallow':
             buoyancy_variable='m_ballast_pumped'
         elif settings['buoyancy_engine']=='deep':
             buoyancy_variable='m_de_oil_vol'
         else:
             raise ValueError('Unknown buoyancy engine. Accepted values: (shallow|deep)')
-        dbd = dbdreader.MultiDBD(filenames=fns, include_paired=True)
-        tmp = dbd.get_sync("sci_ctd41cp_timestamp",["sci_water_pressure",
-                                                    "sci_water_cond",
-                                                    "sci_water_temp",
-                                                    "m_pitch",
-                                                    "m_battpos",
-                                                    buoyancy_variable])
-        _, tctd, P, C, T, pitch, battpos, buoyancy_change = tmp.compress(tmp[3]>0.01, axis=1)
+        dbd = dbdreader.MultiDBD(filenames=fns, complement_files = True)
+        try:
+            tmp = dbd.get_CTD_sync("m_pitch", "m_battpos", buoyancy_variable)
+        except dbdreader.DbdError:
+            tmp = dbd.get_sync("sci_water_cond", "sci_water_temp", "sci_water_pressure",
+                               "m_pitch", "m_battpos", buoyancy_variable)
+        try:
+            (_,lat), (_,lon) = dbd.get("m_gps_lat", "m_gps_lon")
+        except dbdreader.DbdError:
+            latitude = float(input("Provide decimal latitude:"))
+            longitude = float(input("Provide decimal longitude:"))
+        else:
+            latitude = np.median(lat)
+            longitude = np.median(lon)
+        condition = np.logical_and(tmp[2]>0.01, np.isfinite(np.sum(tmp, axis=0)))
+        tctd, C, T, P, pitch, battpos, buoyancy_change = np.compress(condition, tmp, axis=1)
         SP = gsw.SP_from_C(C*10, T, P*10)
-        SA = gsw.SA_from_SP(SP, P*10, settings['longitude'], settings['latitude'])
+        SA = gsw.SA_from_SP(SP, P*10, longitude, latitude)
         density = gsw.rho_t_exact(SA, T, P*10)
-        
-        #density = fast_gsw.rho(C*10, T, P*10, settings['longitude'], settings['latitude'])
-
+        #density = fast_gsw.rho(C*10, T, P*10, longitude, latitude)
         data = dict(time=tctd, pressure=P, pitch=pitch,
                     buoyancy_change=buoyancy_change, battpos=battpos, density=density)
         self.model.input_data = data
         mask=np.zeros(tctd.shape,'int').astype(bool) # use all data by default
         self.model.set_mask(mask)
         self.model.OR(P*10<settings['minlimitdepth'])
         self.model.OR(P*10>settings['maxlimitdepth'])
@@ -162,17 +166,22 @@
         return coefs
 
     def report(self, results, settings):
         print()
         print()
         print("Drag coefficient Cd    : %f (-)"%(self.model.Cd0))
         print("Glider volume Vg       : %f (m^3)"%(self.model.Vg))
-        print("Glider compressibility : %f (*e-10)"%(self.model.epsilon))
+        print("Glider compressibility : %f (*e-10)"%(self.model.epsilon*1e10))
         print("Glider density         : %f (kg/m^3)"%((self.model.mg/self.model.Vg)))
-        print("Weight change          : %f (g)"%((settings['target_density']-(self.model.mg/self.model.Vg))*self.model.Vg*1000.))
+        weight_change = (settings['target_density']-(self.model.mg/self.model.Vg))*self.model.Vg*1000.
+        if weight_change <0:
+            s = "removed"
+        else:
+            s = "added"
+        print("Weight change          : %f (g) to be %s."%(abs(weight_change), s))
         #
         print()
         print("Estimated pitch relationship:")
         coefs = self.estimate_pitch_relation(settings)
         print("tan(pitch) = T1 * buoyancy(m^3) + T2 * battpos(m) + T3 (tan(pitch0)) + T4 P (kbar)")
         print("T1 :",coefs[0])
         print("T2 :",coefs[1])
@@ -193,20 +202,20 @@
         ax[0].plot(mr.ww, z, label='w_water', color='C0', alpha=0.5)
         ax[0].plot(np.convolve(mr.ww, np.ones(15)/15, 'same'),
                    z, label='w_water', color='C5')
         ax[0].plot(mr.w, z, label='w_glider', color='C1')
         ax[0].plot(mr.U, z, label='U_glider', color='C3')
         ax[1].plot(zi*0+settings['target_density'], zi, label='Target density')
         ax[1].plot(self.model.input_data['density'], z, label='Density')
-        rho_g = self.model.mg/(self.model.Vg*(1-self.model.epsilon*1e-10*Pi*1e5))
+        rho_g = self.model.mg/(self.model.Vg*(1-self.model.epsilon*Pi*1e5))
         ax[1].plot(rho_g, zi, label='Glider density', color='C2')
         for i in range(1, 5):
-            rho_g = (50e-3*i+self.model.mg)/(self.model.Vg*(1-self.model.epsilon*1e-10*Pi*1e5))
+            rho_g = (50e-3*i+self.model.mg)/(self.model.Vg*(1-self.model.epsilon*Pi*1e5))
             ax[1].plot(rho_g, zi, color='C2', ls='--', alpha=0.5)
-            rho_g = (-50e-3*i+self.model.mg)/(self.model.Vg*(1-self.model.epsilon*1e-10*Pi*1e5))
+            rho_g = (-50e-3*i+self.model.mg)/(self.model.Vg*(1-self.model.epsilon*Pi*1e5))
             ax[1].plot(rho_g, zi, color='C2', ls='--', alpha=0.5)
         ax[0].set_ylabel('Depth (m)')
         ax[0].set_xlabel('Velocity (m/s)')
         ax[1].set_xlabel('Density (kg/m^3)')
         ax[0].legend()
         ax[1].legend()
         ax[0].invert_yaxis()
@@ -221,7 +230,20 @@
 
     model = Model(fns, ui.settings)
     model.read_dbds(fns, ui.settings)
     results = model.calibrate(ui.settings)
     model.report(results, ui.settings)
     model.graphic_report(results, ui.settings)
     input("Press enter to exit")
+
+
+
+def test():
+    sys.argv.append("comet-nsb3201907")
+    import glob
+    fns = glob.glob("/home/lucas/even/trim/comet*.dbd")
+    for fn in fns:
+        sys.argv.append(fn)
+    main()
+
+    
+
```

### Comparing `gliderflight-1.1.0/setup.py` & `gliderflight-1.2.0/setup.py`

 * *Files identical despite different names*

