# Comparing `tmp/pqinput-0.0.32.tar.gz` & `tmp/pqinput-0.0.321.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqinput-0.0.32.tar", last modified: Mon May  8 12:38:56 2023, max compression
+gzip compressed data, was "pqinput-0.0.321.tar", last modified: Tue May  9 08:49:19 2023, max compression
```

## Comparing `pqinput-0.0.32.tar` & `pqinput-0.0.321.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-08 12:38:56.931608 pqinput-0.0.32/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.32/LICENSE.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1935 2023-05-08 12:38:56.931608 pqinput-0.0.32/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1363 2023-02-20 12:29:30.000000 pqinput-0.0.32/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-08 12:38:56.931608 pqinput-0.0.32/pqinput/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      119 2023-05-04 15:25:36.000000 pqinput-0.0.32/pqinput/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8430 2023-05-08 12:37:23.000000 pqinput-0.0.32/pqinput/drawPES.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    14188 2023-05-08 12:35:42.000000 pqinput-0.0.32/pqinput/inpxml.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-08 12:38:56.931608 pqinput-0.0.32/pqinput.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1935 2023-05-08 12:38:56.000000 pqinput-0.0.32/pqinput.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      226 2023-05-08 12:38:56.000000 pqinput-0.0.32/pqinput.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-08 12:38:56.000000 pqinput-0.0.32/pqinput.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-08 12:38:56.000000 pqinput-0.0.32/pqinput.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      541 2023-05-08 12:38:32.000000 pqinput-0.0.32/pyproject.toml
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-08 12:38:56.931608 pqinput-0.0.32/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      652 2023-05-08 12:38:38.000000 pqinput-0.0.32/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-09 08:49:19.119986 pqinput-0.0.321/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.321/LICENSE.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1936 2023-05-09 08:49:19.119986 pqinput-0.0.321/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1363 2023-02-20 12:29:30.000000 pqinput-0.0.321/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-09 08:49:19.115986 pqinput-0.0.321/pqinput/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      119 2023-05-04 15:25:36.000000 pqinput-0.0.321/pqinput/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8419 2023-05-08 12:48:15.000000 pqinput-0.0.321/pqinput/drawPES.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    14375 2023-05-09 08:46:46.000000 pqinput-0.0.321/pqinput/inpxml.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-09 08:49:19.119986 pqinput-0.0.321/pqinput.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1936 2023-05-09 08:49:19.000000 pqinput-0.0.321/pqinput.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      226 2023-05-09 08:49:19.000000 pqinput-0.0.321/pqinput.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-09 08:49:19.000000 pqinput-0.0.321/pqinput.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-09 08:49:19.000000 pqinput-0.0.321/pqinput.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      542 2023-05-08 12:50:19.000000 pqinput-0.0.321/pyproject.toml
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-09 08:49:19.119986 pqinput-0.0.321/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      653 2023-05-08 12:50:26.000000 pqinput-0.0.321/setup.py
```

### Comparing `pqinput-0.0.32/LICENSE.txt` & `pqinput-0.0.321/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.32/PKG-INFO` & `pqinput-0.0.321/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.32
+Version: 0.0.321
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.32/README.md` & `pqinput-0.0.321/README.md`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.32/pqinput/drawPES.py` & `pqinput-0.0.321/pqinput/drawPES.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     [plt.close() if not showfig else plt.show()]
         
     return fig, ax
 
 
 # %% if __name__==__main__
 if __name__=='__main__':
-    import pqinput.inpxml as inx
+    import inpxml 
     mass = 12500
     propapar = {'dt': 4.138276,'steps': 1000,'wcycle': 100,'dir': 'propa_files','nfile': 'norm'}
     # Kinect energy operators
     T_CO = {'head':'T', 'name':"GridNablaSq", 'mass':mass, 'key':'T'}
     Tref = {'head':'T','ref':'T'}
     # Potential energy surfaces
     Vg = {'head':'V', 'name':"GridPotential", 'file':'CO/pots/pot_VSp'}
@@ -181,15 +181,15 @@
     WFpar = {'type':'Multistate', 'states':4,
              'file':["CO/efs_{}/ef_{}".format(ef[1][i], ef[0][i]) for i in range(len(ef[0]))], 
              'index':[iwf[i] for i in range(len(iwf))], 'normalize':True}
     filteropes = [{'expeconly':{'name':'Multistate', 'states':'4', 'unity':'False', 'header':"mu{}".format(ind)}, 
                    'm{}'.format(ind):{'name':'GridPotential', 'file':'CO/mu/mu'}}
                    for ind in [2.1, 2.3, 3.1] ]
     
-    prop = inx.InpXML()
+    prop = inpxml.InpXML()
     prop.program('propa', propapar, WFpar)
     prop.propagation('Cheby', Hparams)
     #%%
     # prop.addfilter('filterpost', filteropes)
     # prop.show()
     #legend=['G','E','Gl','Gr',],
     draw_PESs(prop, yrange=(0,20), xrange=(1.5,5), legend=['G','E','Gl','Gr',], offsetlabel=['wx', 'wy'] ,
```

### Comparing `pqinput-0.0.32/pqinput/inpxml.py` & `pqinput-0.0.321/pqinput/inpxml.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,16 +98,17 @@
         if isinstance(args, str): args = args.split('_') # single string format
         path = ''
         if len(args)==3: path, key, new_value = args # if path is '' is meant to set a main attribute
         elif len(args)==2: key, new_value = args
         element = (getattr(self, storage_name).find(path) if path else getattr(self, storage_name))
         if element is None: 
             raise AttributeError('setter path do not point to a defined attribute.')
+       
         element.set(key, str(new_value))
-        show(element)
+        # show(element)
         
         # READ MORE ABOUT XPATH AND IF ITS USEFUL
         
     return propriety
 # %% 
 '''-------------------------------------------------------------------------'''
 '''                                Class                                    '''
@@ -133,41 +134,51 @@
     
     Properties:
         show: prints out the class text in readable xml format
         
         
     * comments from QDng documentation
     """
-    qdng = et.Element("qdng") # Root of the XML tree: self.qdng, with the tag-headline 
+    # Attributes as properties
+    qdng = typed_property('qdng')
+    prog = typed_property('program')    
+    wavefunc = typed_property('wavefunction')
+    propag = typed_property('propagation')
+    hamilt = typed_property('hamiltonian')
+    filterpost = typed_property('filterpost')
+    # Defined operations and programs so far
     
     def __init__(self, qdng_params=None): # Initiate the input layout 
-        if qdng_params: dict2attr(self.qdng, qdng_params)
+        self._qdng = et.Element("qdng") 
+        # Root of the XML tree: self._qdng, with the tag-headline 
+
+        if qdng_params: dict2attr(self._qdng, qdng_params)
         
     def __str__(self): # define string format for printing
-        return f'{et.tostring(self.qdng, pretty_print=True).decode()}'    
+        return f'{et.tostring(self._qdng, pretty_print=True).decode()}'    
     
     @property
     def show(self): # printing property
         '''Print out the full text in readable xml format
         Useful for debugging '''
-        print(self)     
-    
+        print(self)    
+
 # %% 
     ''' METHODS '''
     ######################## Write file ########################
     def writexml(self, file_name='test_file', txt=False):
         """ Write the constructed lxml element to a XML file. """
-        tree = et.ElementTree(self.qdng)
+        tree = et.ElementTree(self._qdng)
         if file_name.endswith('.txt'): 
             txt = True 
             file_name = file_name.strip('.txt')
         tree.write(file_name + ('.txt' if txt else '.xml'), pretty_print=True)
         
     def modify(self, path, key, new_value):
-        self.qdng.find(path).set(key, str(new_value))
+        self._qdng.find(path).set(key, str(new_value))
         
     def define_wavefunction(self, wfp):
         if wfp['type'] == 'file':
             wfel = et.Element('wf')
             wfel.set('file', wfp['file'])
             
         elif wfp['type'] == 'LC':
@@ -184,65 +195,63 @@
             
             for ii, index in enumerate(wfp['index']):
                 wfstate = et.SubElement(wfel, 'wf'+str(index), file=str(wfp['file'][ii]))
                 if 'coeff2' in wfp.keys(): wfstate.set('coeff2', wfp['coeff2'][ii])
         else:
             raise SyntaxError('Wavefunction type not defined.')
         self._wavefunction = wfel
-        return wfel
+        # return wfel
     
     # %% 
     """ Programs """
-    def program(self, ptype, program_parameters, wf_parameters):
+    def def_program(self, ptype, program_parameters, wf_parameters):
         """ Main program for the calculation. Either propagation or eigenfunction derivation.
                 
         Args:
             ptype (string) type of program:
             _either 'propa' or 'eigen'
             program_parameters (dict) program parameters dictionary:
             _format: {'dt':num, 'steps':num, 'directory':str,'Nef':num, 'conv':num }
             wf_parameters (dict) wavefunction parameters dictionary:
             _format: {'name':str, 'states':num, 'file':[strs, ], 'normalize':True or None}
             
         """
         '''MAIN PROGRAM'''
         if not ptype in ['propa','eigen']: raise SyntaxError('Program not defined.')  
-        self._program = subelem(self.qdng, program_parameters, ptype )
+        self._program = subelem(self._qdng, program_parameters, ptype )
         # Create self._program as a lxml child element of qdng
         '''WAVEFUNCTION'''
         self.define_wavefunction(wf_parameters)
         # define wavefunction parameters
         
-    prog = typed_property('program')    
-    wavefunc = typed_property('wavefunction')
+    
     
     # %% 
     """ Operators """
     def def_hamiltonian(self, Hp):    
         Hel = et.SubElement(self._propagation, 'hamiltonian')
         # Create a lxml element to be appended to the self.propag 
-        
         if Hp['type'] == 'Sum': 
             Hel.set('name', Hp['type'])
             self.states = 1
             [subelem(Hel, opes) for opes in Hp['Opes']]
             # set hamiltonian of Sum type, creating subelements for each operator
         elif Hp['type'] == 'Multistate':
             Hel.set('name', Hp['type'])
             self.states = 0
             if None == Hp['Mels']:
                 raise SyntaxError('Include states for the Multistate hamiltonian!')
             else:
                 for mel in Hp['Mels'][:]:
-                    # iterate through Hamiltonian matrix elements (mel)
-                    self.states += 1
+                    # iterate through Hamiltonian matrix elements (mel)                    
                     if len(mel['head'])<3: # easy way to set Hamiltonian matrix element 'mi.i'
                         mel['head'] = (f"m{mel['head'][1]}.{mel['head'][1]}")
                     elif len(mel['head'])==3:
                         mel['head'] = (f"m{mel['head'][1]}.{mel['head'][2]}")
+                    if mel['head'][1]==mel['head'][3]: self.states += 1
                     branch = subelem(Hel, mel)
                     if 'Opes' in  mel.keys():
                         for ind in range(len(mel['Opes'])):
                             branch.append( dict2elem(mel['Opes'][ind])) 
         self._hamiltonian = Hel
             
         
@@ -272,16 +281,15 @@
             raise SyntaxError('Propagator type not defined.')
         # others propagators
         try:
             self._program.append( self._wavefunction ) # append wavefunction after the propagation
         except:
             raise SyntaxError('Wavefunction was not properly defined for propa.')    
 
-    propag = typed_property('propagation')
-    hamilt = typed_property('hamiltonian')
+
     
     def def_filterpost(self, filter_list):
         # Define the filterpost operation, must be called after propagation
         filterpost = et.Element('filterpost')
         for dic in filter_list:
             for opes, values in dic.items():
                 for keys in values.keys():
@@ -296,17 +304,15 @@
         return filterpost
     
     def filter(self, ftype, params):
         # add filter to calculation
         if ftype == 'filterpost':
             if not isinstance(params, list): params = [params]
             self._filterpost = self.def_filterpost(params)    
-            
-    
-    filterpost = typed_property('filterpost')
+
         
 # %% Name == Main 
 if __name__ == "__main__":
     
     dt, steps = 20, 1000
     propag, hamilt = 'Cheby', 'Sum'
     Nef, conv = 20, 1e-9
@@ -335,17 +341,16 @@
              'file':["MgH/efs_{}/ef_{}".format(ef[i], vib[i]) for i in range(len(ef))], 
              'index':[wf[i] for i in range(len(wf))], 'normalize':True}
     filteropes = [{'expeconly':{'name':'Multistate', 'states':WFparams['states'], 'unity':'False', 'header':"mu{}".format(ind)}, 
                    'm{}'.format(ind):{'name':'GridPotential', 'file':'MgH/mu/mu_Sig0Sig1'}}
                    for ind in [2.1,] ]
     #%%
     prop = InpXML()
-    prop.program('propa', nparams, WFparams)
+    prop.def_program('propa', nparams, WFparams)
     prop.propagation('Cheby', Hparams)
-    prop.filter('filterpost', filteropes)
+    # prop.filter('filterpost', filteropes)
     prop.hamilt = 'name', 'b'
 
-
     prop.show
     # prop.writexml(txt=True)
```

### Comparing `pqinput-0.0.32/pqinput.egg-info/PKG-INFO` & `pqinput-0.0.321/pqinput.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.32
+Version: 0.0.321
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.32/pyproject.toml` & `pqinput-0.0.321/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pqinput"
-version = "0.0.32"
+version = "0.0.321"
 authors = [
   { name="Lucas Borges", email="lucas.borges@fysik.su.se" },
 ]
 description = "Create input files for QDng calculations"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pqinput-0.0.32/setup.py` & `pqinput-0.0.321/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name = "pqinput",
-    version = "0.0.32",
+    version = "0.0.321",
     author = "Lucas Borges",
     author_email = "lucas.borges@fysik.su.se",
     description = ("additional functions for QDng calculations setups."),
     license = "MIT",
     keywords = "qdng",
     url = "https://gitlab.fysik.su.se/lucas.borges/inputxml",
     packages=setuptools.find_packages(),
```

