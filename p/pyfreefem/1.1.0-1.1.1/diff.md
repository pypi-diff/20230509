# Comparing `tmp/pyfreefem-1.1.0-py3-none-any.whl.zip` & `tmp/pyfreefem-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 27975 bytes, number of entries: 9
+Zip file size: 29601 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      800 b- defN 23-Jan-30 15:19 pyfreefem/__init__.py
--rw-r--r--  2.0 unx    13599 b- defN 23-Apr-28 07:23 pyfreefem/freefemrunner.py
--rw-r--r--  2.0 unx     8245 b- defN 23-Apr-28 07:23 pyfreefem/io.py
--rw-r--r--  2.0 unx    21163 b- defN 23-Apr-28 07:23 pyfreefem/preprocessor.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Apr-28 11:34 pyfreefem-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4178 b- defN 23-Apr-28 11:34 pyfreefem-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 11:34 pyfreefem-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-28 11:34 pyfreefem-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      713 b- defN 23-Apr-28 11:34 pyfreefem-1.1.0.dist-info/RECORD
-9 files, 83949 bytes uncompressed, 26757 bytes compressed:  68.1%
+-rw-r--r--  2.0 unx    18700 b- defN 23-May-05 09:43 pyfreefem/freefemrunner.py
+-rw-r--r--  2.0 unx    11199 b- defN 23-May-01 14:03 pyfreefem/io.py
+-rw-r--r--  2.0 unx    21241 b- defN 23-May-01 14:10 pyfreefem/preprocessor.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-09 08:05 pyfreefem-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4178 b- defN 23-May-09 08:05 pyfreefem-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-09 08:05 pyfreefem-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-09 08:05 pyfreefem-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      714 b- defN 23-May-09 08:05 pyfreefem-1.1.1.dist-info/RECORD
+9 files, 92083 bytes uncompressed, 28383 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: pyfreefem/io.py
 Comment: 
 
 Filename: pyfreefem/preprocessor.py
 Comment: 
 
-Filename: pyfreefem-1.1.0.dist-info/LICENSE
+Filename: pyfreefem-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyfreefem-1.1.0.dist-info/METADATA
+Filename: pyfreefem-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyfreefem-1.1.0.dist-info/WHEEL
+Filename: pyfreefem-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyfreefem-1.1.0.dist-info/top_level.txt
+Filename: pyfreefem-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyfreefem-1.1.0.dist-info/RECORD
+Filename: pyfreefem-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyfreefem/freefemrunner.py

```diff
@@ -1,140 +1,170 @@
-# This file is part []reeFEM.
+# This file is part of PyFreeFEM.
 #
 # PyFreeFEM is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 #
 # PyFreeFEM is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # A copy of the GNU General Public License is included below.
 # For further information, see <http://www.gnu.org/licenses/>.
+    
+
+"""Module FreeFemRunner"""
+
 from os import path
 from .preprocessor import Preprocessor
 import os.path
 import shutil
 from .io import display, exec2, ExecException, readFFMatrix, readFFArray,   \
                    writeFFArray, writeFFMatrix 
 import tempfile
 import numpy as np
 import scipy.sparse as sp
 import pymedit
-
+    
 
 
 class FreeFemRunner:
-    """A class to run a FreeFem code given by an interpreter or raw code."""
-    
-    def __init__(self, code, config=dict(), run_dir=None,
-                 run_file=None, debug=0, plot=False, 
-                 macro_files=[]):
-        """
-        Usage
-        _____
-        Load a single file .edp file
-        >>> runner=FreeFemRunner('solveState.edp')
-
-        Load a list of files (to be assembled consecutively)
-        >>> runner=FreeFemRunner(['params.edp','solveState.edp'])
-
-        Load a single file with an updated configuration
-        >>> runner=FreeFemRunner('solveState.edp',{'ITER':'0010'})
-
-        Load raw code
-        >>> code = "mesh Th=square(10,10);"
-            runner=FreeFemRunner(code)
-
-        Load a pyfreefem.Preprocessor object
-        >>> preproc = Preprocessor('solveState.edp')
-            runner = FreeFemRunner(preproc)
-
-        Then execute the code with `~FreeFemRunner.execute':
-        >>> runner.execute();
-            runner.execute({'Re':30}); # Update magic variable value
-
-        It is possible to execute the code in parallel with ff-mpirun by using
-        >>> # Run on 4 cpus with ff-mpirun -np 4
-            runner.execute(ncpu=4); 
-        >>> # Run on 1 cpu with ff-mpirun -np 1
-            runner.execute(ncpu=1,with_mpi=1);
-
-        Note that in that case, a magic variable 'WITH_MPI' is automatically
-        assigned and set to 1, which is useful to make adaptations in the 
-        source code, e.g. 
-        ```
-        IF WITH_MPI
-        /* Instructions to do if the code is parallel */
-        ELSE
-        /* Instructions to do if the code is not parallel */
-        int mpirank = 0; 
-        int mpisize = 1;
-        ENDIF
-        ```
-
-        Parameters 
-        ----------
-
-        :param code:    raw text code, instance of Preprocessor, or files
-
-        :param config:  a default assignment of magic variables
-                        which can be modified later on during the execute() 
-                        operation.
-
-        :param run_dir: where the running script will be written. If this 
-                        argument is speficied, then run_dir is not 
-                        deleted after the FreeFEM execution.
+    """A class to run a FreeFem ``.edp`` scripts    
+    supporting PyFreeFEM meta-language.   
 
-        :param run_file: name of the written script
+    **Usage**
 
-        :param debug:   tuning for verbosity. The FreeFEM command is 
-                        is displayed if debug>=1.
-                        Details of the parsing operation are displayed if 
-                        debug>=10.
+    * Load a single file .edp file
+        
+      .. code:: python    
+
+         runner=FreeFemRunner('solveState.edp')
+
+    * Load a list of files (to be assembled consecutively)
+
+      .. code:: python    
+
+         runner=FreeFemRunner(['params.edp','solveState.edp'])
+
+    * Load a single file with an updated configuration
+
+      .. code:: python    
+
+         runner=FreeFemRunner('solveState.edp',{'ITER':'0010'})
+
+    * Load raw code
+
+      .. code:: python    
+
+         code = "mesh Th=square(10,10);"
+         runner=FreeFemRunner(code)
+
+    * Load a pyfreefem.Preprocessor object
+
+      .. code:: python    
+
+         preproc = Preprocessor('solveState.edp')
+         runner = FreeFemRunner(preproc)
+
+    Then execute the code with :meth:`pyfreefem.FreeFemRunner.execute`:
+
+    .. code:: python    
+
+       runner.execute();
+       runner.execute({'Re':30}); # Update magic variable value
+
+
+
+    :param script:    Either:   
+
+                      * raw FreeFEM code   (e.g. ``script="mesh Th=square(3,3)"``) 
+
+                      * name of ``.edp`` script file (e.g. ``script="script.edp"``) 
+
+                      * list of names of ``.edp`` script files to be appended   
+                        in the generated executable ``.edp`` script     
+                        (e.g. ``script=['script1.edp','script2.edp','script3.edp']``)
+
+                      * instance of :mod:`pyfreefem.preprocessor.Preprocessor`
 
-        :param plot: (default False). If set to True, then FreeFEM is run
-                        with the graphical -wg option.
+    :param config:  a default assignment of magic variables
+                    which can be modified later on during the execute() 
+                    operation.  
+                        
+                    Example: ```{'N':10, 'RES':'high'}```.  
+                        
+                    .. note::   
+                        
+                       The values of the magic variables are converted to   
+                       strings in the interpreted executable ``.edp`` script.   
 
-        :param macro_files: list of enhanced .edp dependency files
-                        (with meta-instructions)
-                        which are also to be parsed and placed in the 
-                        run folder of the final executable.
-
-        :param verbosity:     : verbosity level of FreeFem output
-
-        Executing the code creates (by default) a temporary file which is
-        to be executed by FreeFEM and which is removed after the python 
-        execution. This behavior can be changed by using the
-        `run_dir` and `run_file` arguments. 
-
-        Note : for some usage, it is necessary to modify the
-               FreeFem command. This can be achieved by
-               updating the method `~FreeFemRunner.cmd`
-               See pyfreefem/examples/hello_world_vglrun.py 
+    :type config:      dict
 
+    :param run_dir:    running directory where the executable script is written    
+                       when calling :meth:`pyfreefem.FreeFemRunner.execute`.   
+                       If ``run_dir`` is ``None``, then a temporary directory     
+                       is created for this purpose and deleted after execution.     
+                       The temporary name directory can be retrieved by using the   
+                       ``run_dir`` attribute of the :class:`pyfreefem.FreeFemRunner`    
+                       instance or from the ``$RUNDIR`` magic variable.
+
+    :param run_file:   Name of the generated executable ``.edp`` script. If   
+                       ``run_file`` is ``None``, then ``run_file`` is set to: 
+                          
+                       * ``run_file=script`` if ``script`` is the name of a file 
+
+                       * ``run_file=script[0]`` if ``script`` is a list and   
+                         ``script[0]`` is the name of a file 
+                          
+                       * ``run.edp`` if none of the previous case applies.
+
+    :param debug:       More and more debugging information with a flexible level of verbosity    
+                        are displayed as this parameter is set to a larger and larger value.
+                        Details of the parsing operation are displayed if 
+                        ``debug>=10`` (default ``debug=0``).
+    :type debug:        int
+
+    :param plot: (default: ``False``). enables  
+                     ``FreeFem++`` graphics (``-wg`` option) which are disabled 
+                     by default.
+
+    :param macro_files: List of enhanced .edp macro files
+                        supporting meta-instructions
+                        which are also parsed and placed in the 
+                        run folder of the final executable. For instance:   
+                            
+                        .. code:: python    
+                            
+                           FreeFemRunner('script.edp',macro_files=['macros.edp','params.edp'])
+
+    """
+    
+    def __init__(self, script, config=dict(), run_dir=None,
+                 run_file=None, debug=0,  plot=False,
+                 macro_files=[]):
+        """
         """
         self.freefemFiles = dict()
         self.debug = int(debug)
-        self.plot = plot
         self.run_file = run_file
         self.run_time = -1
         self.exports = []
+        self.plot = plot
 
-        #: pyfreefem standard output.   
-        #: After calling :py:meth:`pyfreefem.FreeFemRunner.execute` 
-        #: py:attr:`pyfreefem.FreeFemRunner.rets` is a tuple    
+        #: Captured output of FreeFem++ process.   
+        #: After calling :meth:`pyfreefem.FreeFemRunner.execute`,
+        #: `rets` is a tuple    
         #: containing:  
         #:  
         #: * rets[0]: the return code   
         #: * rets[1]: stdout    
         #: * rets[2]: stderr    
-        #: * rets[3]: the whole standard output
+        #: * rets[3]: the whole standard output (mix of stdout and stderr)
         self.rets = tuple() 
 
         # create temporary directory if needed
         self.__context__ = False
 
         if run_dir is None:
             self.tempdir = tempfile.TemporaryDirectory(prefix="pyfreefem_")
@@ -145,26 +175,29 @@
         if not os.path.exists(self.run_dir):
             os.makedirs(self.run_dir)
             display("Create "+self.run_dir, level=10, debug=self.debug,
                     color="magenta")
         self.ffexport_dir = self.run_dir+'/ffexport'
         self.ffimport_dir = self.run_dir+'/ffimport'
 
-        if isinstance(code, Preprocessor):
-            self.preprocessor = code
+        if isinstance(script, Preprocessor):
+            self.preprocessor = script
         else:
-            self.preprocessor = Preprocessor(code, config, debug=self.debug-10)
+            self.preprocessor = Preprocessor(script, config, debug=self.debug-10)
+                
+        #: Dictionary of magic variables.   
+        #: This dictionary is updated after calling :meth:`pyfreefem.FreeFemRunner.execute`.
         self.config = config
 
 
         if self.run_file is None:
-            if isinstance(code,list) and os.path.isfile(code[0]):
-                self.run_file = os.path.basename(code[0])
-            elif os.path.isfile(code):
-                self.run_file = os.path.basename(code)
+            if isinstance(script,list) and os.path.isfile(script[0]):
+                self.run_file = os.path.basename(script[0])
+            elif os.path.isfile(script):
+                self.run_file = os.path.basename(script)
             else:
                 self.run_file = "run.edp"
 
         self.macro_files = macro_files
         #self.macro_files.append(os.path.dirname(__file__)+"/edp/io.edp")
         
     def import_variables(self, **kwargs):
@@ -189,45 +222,53 @@
                 var.save(self.ffimport_dir+"/mesh3D_"+varname+".mesh")
             else:   
                 raise Exception("Error, type "+str(type(var)) + " is unknown for pyfreefem import." 
                                 " Supported types are float, np.ndarray, pymedit.mesh.Mesh and "    
                                 "pymedit.mesh3D.Mesh3D.")
 
     def parse(self, config):    
-        """ Parse"""
+        """Returns the parsed executable ``.edp`` script without executing it.
+
+           :param config:  a default assignment of magic variables
+                           which can be modified later on during the execute() 
+                           operation.  
+                               
+                           Example: ```{'N':10, 'RES':'high'}```.  
+                               
+                           .. note::   
+                               
+                              The values of the magic variables are converted to   
+                              strings in the interpreted executable ``.edp`` script.   
+            :return: a parsed ``.edp`` script.  For instance:   
+                
+                     .. code:: python   
+                        
+                        script="mesh Th=square($N,$N);" 
+                        FreeFemRunner(script).parse({'N':10})
+                            
+                     .. code:: freefem 
+                        
+                        mesh Th=square(10,10);
+                
+          
+        """
         return self.preprocessor.parse(config)
 
-    def write_edp_file(self, config=dict(), **kwargs):
+    def _write_edp_file(self, config=dict()):
         """
         Write the parsed .edp file in the running directory.
 
         Arguments
         ---------
 
             config      : a dictionary of magic variable which updates the 
                           default FreeFemRunner.config assignment.
-
-            ncpu        : the number of CPUs for a run with ff-mpirun
-
-            with_mpi    :  will run with ff-mpirun even if ncpu=1
-
-            target_file : file name of the output .edp file to be written
         """
-        ncpu = int(kwargs.get('ncpu', 1))
-        self.config.update(config)
-        if ncpu > 1 or kwargs.get('with_mpi', False):
-            config.update({'WITH_MPI': 1})
-        else:
-            config.update({'WITH_MPI': 0})
-
         target_file = path.join(self.run_dir, self.run_file)
 
-        self.config.update({'RUNDIR':self.run_dir})
-        self.config.update({'FFEXPORTDIR':self.ffexport_dir})
-        self.config.update({'FFIMPORTDIR':self.ffimport_dir})
         code = self.parse(config)
         
         f = open(target_file, "w")
         f.write(code)
         f.close()
         display("Write "+target_file, level=10, debug=self.debug,
                 color="magenta")
@@ -249,57 +290,109 @@
                     color="magenta")
         return self
 
     def __exit__(self, type, value, traceback):
         pass
             
 
-    def execute(self, config=dict(), **kwargs):
+    def execute(self, config=dict(), debug = None, verbosity = -1,  
+                ncpu = 1, with_mpi = False, plot = None, level = 1):
         """
-        Parse with the input config, save the code in .edp file
-        and call FreeFEM.
+        Parse the script with the input config, save the code in an ``.edp`` file
+        and execute FreeFEM on it.
+
+        .. code:: python
 
-        Usage:
-            >>> runner = FreeFemRunner('solveState.edp')
+            runner = FreeFemRunner('solveState.edp')
             runner.execute();
             runner.execute({"ITER" : "0024"});
 
-        Options
-        -------
-        config    :  dictionary of updated magic variable values
-                     Warning : a "SET" instruction in the .edp file
-                     always has the precedence over the values specified
-                     by `config`
-
-        debug       :  execute the edp file with an updated level of verbosity
-
-        target_file : change of location to write the .edp file.
-
-        silent      : (default False) if set to True, there will be no standard 
-                      output displayed in the shell (although it will still be 
-                      returned in the output variables stdout, stderr and mix).
-
-        Returns
-        -------
-
-        returncode   :  the return code of the FreeFEM process
-        stdout       :  the standard output
-        stderr       :  the standard error output
-        mix          :  the integrality of the of the FreeFEM process output 
+        :param config: Dictionary of magic variable values. This    
+                       parameter takes precedence over the default configuration    
+                       specified in the :class:`pyfreefem.FreeFemRunner` constructor.
+                        
+                       .. warning::
+
+                          A "SET" instruction in the .edp file
+                          always has the precedence over the values specified
+                          by `config`. See :ref:`set`.
+
+        :type config: dict
+
+        :param debug:  debugging parameter which takes precedence over the default value    
+                       specified in the  :class:`pyfreefem.FreeFemRunner` constructor.  
+        :type debug:   int
+
+        :param verbosity: (default ``-1``). If ``verbosity`` is set to a value    
+                          ``0`` or greater, the standard output of the ``FreeFem++``    
+                          command will be displayed during execution with the   
+                          level of verbosity corresponding to the option ``-v verbosity``.  
+                          No display is shown if ``verbosity<0``.   
+
+        :type verbosity: int
+
+        :param ncpu: number of compute nodes to be used (option ``-np`` of ``ff-mpirun``). 
+        :type ncpu: int
+
+        :param with_mpi: execute the interpreted ``.edp`` script with ``ff-mpirun``.
+
+                        .. code:: python    
+
+                           # Run on 4 cpus with ff-mpirun -np 4
+                           runner.execute(ncpu=4); 
+                           # Run on 1 cpu with ff-mpirun -np 1
+                           runner.execute(ncpu=1,with_mpi=1);
+
+                        Note that in that case, a magic variable ``WITH_MPI`` is automatically
+                        assigned and set to 1, which is useful to make adaptations in the 
+                        source code, e.g. 
+                              
+                        .. code:: freefem
+
+                           IF WITH_MPI
+                           /* Instructions to do if the code is parallel */
+                           ELSE
+                           /* Instructions to do if the code is not parallel */
+                           int mpirank = 0; 
+                           int mpisize = 1;
+                           ENDIF
 
+        :type with_mpi: boolean
+            
+        :param plot: Enables or disables  ``FreeFem++`` graphics (``-wg`` option) which are disabled 
+                     by default.    This parameter takes precedence over    
+                     the ``plot`` parameter of the  
+                     :class:`pyfreefem.FreeFemRunner` constructor.
+
+        :type plot: boolean
+        :param level: set a custom level for PyFreeFEM debugging informations.  
+                      Namely, the executed ``FreeFem++`` command and further    
+                      PyFreeFEM operations will be shown if ``debug>=level``.
+
+        :return exports:    a dictionary containing FreeFEM exported variables. 
+                            See :ref:`export`.
+        :rtype: dict: 
         """
-        debug = kwargs.pop('debug', self.debug)
+        debug = self.debug if debug is None else debug  
+        plot = self.plot if plot is None else plot
+
+        config.update({'RUNDIR':self.run_dir})
+        config.update({'FFEXPORTDIR':self.ffexport_dir})
+        config.update({'FFIMPORTDIR':self.ffimport_dir})
+
         config.update({'DEBUG':debug})
-        target_file = self.write_edp_file(config, **kwargs)
-        verbosity = kwargs.get('verbosity',-1)
+        if ncpu > 1 or with_mpi:
+            config.update({'WITH_MPI': 1})
+        else:
+            config.update({'WITH_MPI': 0})
+        self.config.update(config)
+        target_file = self._write_edp_file(config)
         silent = verbosity < 0
         if silent:
             verbosity = 0
-        kwargs.update(verbosity=verbosity)
-        level = kwargs.pop('level',1)
 
         self.exports = dict()
         if not os.path.exists(self.run_dir):
             os.makedirs(self.run_dir)
 
         # Clean the ffexport_dir 
         if os.path.exists(self.ffexport_dir):
@@ -307,15 +400,16 @@
         os.makedirs(self.ffexport_dir)
         display("Reset directory "+self.ffexport_dir, level=10, debug=self.debug, 
                 color="magenta")
 
 
         try:
             returncode, stdout, stderr, mix = \
-                exec2(self.cmd(target_file, **kwargs),
+                exec2(self.cmd(target_file, ncpu=ncpu, verbosity= verbosity, with_mpi=with_mpi,
+                               plot=plot),
                        debug=debug, level=level, silent=silent)
         except ExecException as e:
             display(e.args[0], level = 0, debug = 0)
             display('\n'.join(e.mix.splitlines()[-40:]), level=0, debug=0)
             e.args = []
             raise e
 
@@ -331,26 +425,44 @@
                 with open(self.ffexport_dir+'/'+file) as f:
                     self.exports[file[4:]] = float(f.read())
             if file.startswith('array_'):
                 self.exports[file[6:]] = readFFArray(self.ffexport_dir+'/'+file)
             if file.startswith('matrix_'):
                 self.exports[file[7:]] = readFFMatrix(self.ffexport_dir+'/'+file)
 
-        self.rets =(returncode, stdout, stderr, mix) #: pyfreefem standard output
+        self.rets =(returncode, stdout, stderr, mix)
         return self.exports
 
 
-    def cmd(self, target_file, **kwargs):
-        """Return the shell command that is to be run."""
-        ncpu = kwargs.get('ncpu', 1)
-        if ncpu > 1 or kwargs.get('with_mpi', False):
+    def cmd(self, target_file, ncpu=1, with_mpi=False, verbosity = None, plot=False):
+        """Returns the shell command that is to be run when calling the method :meth:`pyfreefem.FreeFemRunner.execute`.  
+            
+        :param target_file: name of the final executable file.  
+        :param with_mpi: (default: ``False``). If set to ``True``, then     
+                         :meth:`pyfreefem.FreeFemRunner.execute` will call ``ff-mpirun``.
+        :type with_mpi: boolean
+
+        :param ncpu: number of compute nodes to be used (option ``-np`` of ``ff-mpirun``). 
+        :param verbosity: option '-v` of FreeFEM. This option is not specified if   
+                          ``verbosity`` is ``None``.
+
+        :param plot: (default: ``False``). If set to ``True``, then     
+                         :meth:`pyfreefem.FreeFemRunner.execute` will use the   
+                         ``-wg`` option (with graphics). Otherwise,     
+                         FreeFem will be called with ``-nw`` option.
+        :type plot: boolean
+            
+        :returns: Shell command for executing FreeFEM with ``target_file`` input 
+                 script.
+        """
+        if ncpu > 1 or with_mpi:    
             cmd = f"ff-mpirun -np {ncpu}"
         else:
             cmd = "FreeFem++"
         cmd += " " + target_file
-        if 'verbosity' in kwargs:
-            cmd = cmd+" -v "+str(kwargs['verbosity'])
-        if self.plot or kwargs.get('plot', False):
+        if not verbosity is None:
+            cmd = cmd+" -v "+str(int(verbosity))
+        if plot:    
             cmd = cmd+" -wg"
-        elif not kwargs.get('with_mpi', False):
+        elif not with_mpi:
             cmd += " -nw"
         return cmd
```

## pyfreefem/io.py

```diff
@@ -8,21 +8,25 @@
 # PyFreeFEM is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # A copy of the GNU General Public License is included below.
 # For further information, see <http://www.gnu.org/licenses/>.
+"""PyFreeFEM input/output functions."""
+    
+
 import scipy.sparse as sp
 import numpy as np
 import time
 import sys
 import subprocess
 import threading
 import queue
+    
 
 try:
     import colored as col
 
     def colored(text, color=None, attr=None):
         if color:
             text = col.stylize(text, col.fg(color))
@@ -32,30 +36,40 @@
 except:
     def colored(text, color=None, attr=None):
         return text
 
 
 def display(message, level=0, debug=0, color=None, attr=None, end='\n',
             flag=None):
-    """ Display function with tunable level of verbosity
+    """A function for displaying messages with a flexible tunable level of verbosity.
+
 
-    INPUTS
-    ------
+    :param message:  Text to be printed.
+    :param level:   Level of importance of the message which will be actually 
+                       printed if ``debug >= level`` or if ``flag`` is ``stdout`` or ``stderr``.
+    :type level: int
+    :param debug: Desired level of verbosity; the higher and the more information will  
+                  be displayed.
+    :type debug: int
+    :param color: Color of the displayed message. Follows the convention of the     
+                  `colored <https://pypi.org/project/colored/>`_ package.
+    :param attr:  Formatting of the displayed message. Follows the  
+                  convention of the     
+                  `colored <https://pypi.org/project/colored/>`_ package.
 
-    message        :   text to be printed
-    level          :   level of importance of the message; will be actually 
-                       printed if debug >= level
-    debug          :   current verbosity level
-    color, attr    :   formattings with the `colored` package
-    end            :   if set to '', will remove the final line carriage return
-    flag           :   an extra indicator equal to None, 'stdout' or 'stderr',
-                       the last two indicating that the text 
-                       passed to display comes from the standard output or 
-                       or error of a shell command. 
-                       Useful if display is overrided.
+    :param end:   character appended to the end of a message. Will remove the   
+                  final line carriage return if ``end=''``.  
+
+    :param flag:  an indicator to use to indicate if the argument ``message`` comes     
+                  from ``stdout`` or ``stderr`` pipe. 
+    
+    .. note::   
+        
+       For advanced projects, it can be useful to override :func:`pyfreefem.io.display`,  
+       for instance to redirect messages to a file.
     """
     if color or attr:
         message = colored(message, color, attr)
     if debug >= level or flag in ['stdout','stderr']:
         print(message, end=end, flush=True)
 
 tclock = dict()
@@ -64,71 +78,75 @@
     tclock[ref] = time.time()
 
 def toc(ref=0):
     global tclock
     return format(time.time()-tclock[ref],"0.2f")+"s"
 
 class ExecException(Exception):
+    """ An exception raised when a FreeFem++ subprocess fails"""
     def __init__(self, message, returncode, stdout, stderr, mix):
         super().__init__(message)
         self.returncode = returncode
         self.stdout = stdout
         self.stderr = stderr
         self.mix = mix
 
-def readFFArray(ffarray):
+def readFFArray(ffarray : str):
     """
-    Read an array stored in the file `ffarray` created by FreeFem++.
-    For instance, if an .edp file has run
-    ```
-        real[int] table = [1, 2, 3, 4, 5];
-        {
-            ifstream f("file.gp");
-            f << table;
-        }
-    ```
+    Read an FreeFEM array stored in a file ``ffarray``. 
+        
+    For instance, if the following ``.edp`` file is executed:
+
+    .. code:: freefem
+
+       real[int] table = [1, 2, 3, 4, 5];
+       {
+           ifstream f("file.gp");
+           f << table;
+       }
+
     Then
-    >>> readFFArray("file.gp") 
+        
+    .. code:: python
+
+       readFFArray("file.gp") 
 
-    returns the numpy array [1, 2, 3, 4, 5]
+    returns the numpy array [1, 2, 3, 4, 5].    
+        
+    :param ffarray: file name of a FreeFEM array stored with ``ifstream``.
+    :return: numpy array identical to ``ffarray``.
     """
     with open(ffarray, "r") as f:
         return np.asarray([float(x) for line in f.readlines()[1:]
                            for x in line.split()])
 
 
-def writeFFArray(A: np.array, fileName):
+def writeFFArray(A: np.array, fileName: str):
     """
-    Store a numpy array into a FreeFEM array file
+    Store a numpy array into a FreeFEM array file that can be read with ``ofstream``.
 
-    Input
-    _____
-
-    A         :  a numpy array
-    fileName  :  the file in which the array will be saved
+    :param A:  a `numpy.array <https://numpy.org/doc/stable/reference/generated/numpy.array.html>`_ data structure
+    :param fileName: an output file name to save the array ``A``.   
     """
     text = f"{len(A)}\t\n"
     lines = [A[5*k:5*(k+1)] for k in range(0, int(np.ceil(len(A)/5)))]
     for line in lines:
         text += ''.join([f"\t  {x}" for x in line])+"\n"
     text = text[:-1]+"\t"
     with open(fileName, "w") as f:
         f.write(text)
 
 
 def writeFFMatrix(A, fileName):
     """
-    Convert a scipy sparse matrix to a FreeFEM sparse matrix file
-
-    Input
-    -----
-
-    A        : a scipy sparse matrix or a numpy dense matrix
-    fileName : the file in which the sparse matrix will be saved
+    Save a dense or a sparse matrix into a FreeFEM matrix file that can be read with ``ofstream``. 
 
+    :param A: A `scipy.sparse.csc_matrix <https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csc_matrix.html>`_  
+              or a `numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_ dense matrix.
+    :param fileName: output file name for saving the matrix ``A``.  
     """
     if isinstance(A,np.ndarray):
         preamble = " ".join(map(str,A.shape))+"\t\n"
         preamble += "\n".join(["\t   "+"   ".join(map(str,line)) for line in A.tolist()])
         preamble += "\n\t"
     else:
         (I, J, V) = sp.find(A)
@@ -140,29 +158,44 @@
         lines = [f"     {i}     {j} {d}" for (i, j, d) in zip(I, J, V)]
         preamble = preamble+"\n".join(lines)
         preamble += "\n"
     with open(fileName, "w") as f:
         f.write(preamble)
 
 
-def readFFMatrix(ffmatrix):
+def readFFMatrix(ffmatrix : str):
     """
-    Read a matrix stored in the file `ffmatrix` created by FreeFEM.
-    For instance, if an .edp file has run 
-    ```
-        matrix table = [[1, 2, 3, 4, 5],[1, 2, 3, 4, 5]];
-        {
-            ifstream f("file.gp");
-            f << table;
-        }
-    ```
+    Read a matrix file generated by a FreeFEM script. For instance,     
+    if the following ``.edp`` file is run:  
+        
+    .. code:: freefem
+
+       matrix table = [[1, 2, 3, 4, 5],[1, 2, 3, 4, 5]];
+       {
+           ifstream f("file.gp");
+           f << table;
+       }
+    
     Then
-    >>> readFFMatrix("file.gp") 
+        
+    .. code:: python
+
+       readFFMatrix("file.gp") 
+
+    returns the numpy matrix [[1, 2, 3, 4, 5],[1, 2, 3, 4, 5]]. 
+        
+    If the matrix stored by the FreeFEM script is a sparse matrix, then :func:`pyfreefem.io.readFFMatrix`   
+    returns a `scipy.sparse.csc_matrix <https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csc_matrix.html>`_.
+
+    If it is a dense matrix, then :func:`pyfreefem.io.readFFMatrix` returns a `numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_.
+        
+    :param ffmatrix: file name of a FreeFEM matrix stored with ``ifstream``.
+    :return: A `numpy.ndarray` matrix if `ffmatrix` contains a dense matrix, or a `scipy.sparse.csc_matrix` if  
+             `ffmatrix` contains a sparse matrix.
 
-    returns the numpy matrix [[1, 2, 3, 4, 5],[1, 2, 3, 4, 5]].
     """
     with open(ffmatrix, 'r') as f:
         lines = f.readlines()
     i = []
     j = []
     data = []
     if lines[0].startswith('#  HashMatrix'):
@@ -193,19 +226,41 @@
 
 
 def enqueue_process(process, queue):
     process.wait()
     queue.put('x')
 
     
-def exec2(cmd, **kwargs):
-    """ Interface with subprocess.Popen """
-    debug = kwargs.pop('debug', 0)
-    level = kwargs.pop('level', 1)
-    silent = kwargs.pop('silent', True)
+def exec2(cmd, debug=0, level=1, silent=True):
+    """Interface with `subprocess.Popen <https://docs.python.org/fr/3/library/subprocess.html>`_.   
+       Execute a shell command ``cmd`` and pass standard output and standard errors 
+       to the function :func:`pyfreefem.io.display`.
+        
+       :param cmd: A shell command. For instance ``cmd="FreeFem++ script.edp -v 1 -wg"``.
+       :type cmd: str
+        
+       :param debug: An input ``debug`` parameter, tuning the desired level of verbosity.   
+                     The command ``cmd`` will be displayed if ``debug>=level``
+       :type debug: int
+
+       :param level: Degree of importance of the executed ``command``.
+                     The command ``cmd`` will be displayed if ``debug>=level``
+       :type level: int
+        
+       :param silent: If set to ``True``, no standard output will be displayed.
+       :type silent: boolean
+        
+       .. note::    
+            
+          By default, the standard output is displayed whatever the value of level and  
+          debug because :func:`pyfreefem.io.display` prints ``stdout`` and ``stderr``   
+          by watching its ``flag`` argument. Use a custom :func:`pyfreefem.io.display`    
+          function to change this behaviour.
+
+    """
     display(colored(cmd, color="indian_red_1a"), level=level, debug=debug, end='',
             flag='shell')
     # Put a line break to separate from the stdout 
     if not silent:
         display("",level=level,debug=debug,flag='')
     tic(121)
     proc = subprocess.Popen("stdbuf -oL "+cmd,shell=True,
```

## pyfreefem/preprocessor.py

```diff
@@ -10,52 +10,72 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # A copy of the GNU General Public License is included below.
 # For further information, see <http://www.gnu.org/licenses/>.
 import re
 
-from IPython.core import macro
 from .io import colored, display
 import os
+    
+"""PyFreeFEM parsing module"""
 
-# If this variable is set to false, then \\ are ignored
+#: Enable or disable the parsing of double backslash ``\\``.   
 ENABLE_LINE_BREAKS = True
-# Update this variable if you wish to use another character than
-# $ for magic variables
+
 MAGIC_CHARACTER = '$'
+""" Prefix character for magic variables (by default ``$``)."""
 
 
 class Preprocessor():
-    """This class allows to convert a FreeFEM code with enhanced
-    preprocessing instructions. These must be inserted directly in the .edp
-    file or provided to the class.  It could also be used to preprocess other
-    scripts than FreeFEM code.
-
-    A configuration dictionary `config` is assembled while parsing the .edp
-    file, whose default values can be set by the user. This dictionary allows to
-    exchange information between FreeFEM scripts and a running instance of
-    python. The keys of the dictionary are called "magic variables" and their
-    values can be obtained in the FreeFem code using the dollar character $.
-
-    Then the `Preprocessor.parse()' instruction converts the enhanced .edp file 
-    into executable FreeFEM code. 
-
-    Supported instructions are:
-        - IF / ELSE / ENDIF
-        - IFEQ / ELSE / ENDIF
-        - IFDEF / ELSE / ENDIF
-        - FOR / ENDFOR
-        - DEFAULT
-        - SET 
-        - INCLUDE
-        - IMPORT 
-        - SET_TEXTVAR / END_TEXTVAR
+    """A class that parses FreeFEM ``.edp`` scripts with enhanced
+    PyFreeFEM meta-language instructions (see :ref:`language`).
+        
+    The :class:`pyfreefem.preprocessor.Preprocessor` class is used by
+    :class:`pyfreefem.FreeFemRunner` for parsing FreeFEM ``.edp`` scripts with enhanced
+    preprocessing instructions and converting it into a proper, executable
+    ``.edp`` code. The usage is similar to ``pyfreefem.FreeFemRunner``:
+    
+    .. code:: python
+    
+       from pyfreefem import Preprocessor
+       # Parse a single file
+       preproc=Preprocessor('solveState.edp')
+    
+       # Parse a list of files (to be assembled consecutively)
+       preproc=Preprocessor(['params.edp','solveState.edp'])
+    
+       # Parse a single file with an updated configuration
+        preproc=Preprocessor('solveState.edp',{'ITER':'0010'})
+    
+        # Parse raw code
+       code = \"""DEFAULT (n,30)
+       mesh Th=square($n,$n);
+       preproc=Preprocessor(code)\"""
+    
+       # Then parse these files with `Preprocessor.parse':
+       parsedCode=preproc.parse();
+       parsedCode=preproc.parse({'n':'0001'});# Parse with a different configuration
+    
+    A configuration dictionary ``config`` containing the updated (or
+    predefined) values of magic variables is assembled while parsing the
+    ``.edp`` file.
+        
+
+    :param script:  single file name, list of
+                    file names or raw ``.edp`` script
+
+    :param config: (optional) a dictionary of magic variables with default values
+
+    :param included: (optional) a list of file names that must not be
+                included. Usually empty, used for implementation
+                purposes.
 
-    See the doc and examples for more detailed usage
+    :param debug:  A tuning parameter for flexible verbose output, allowing to
+                   check the behavior of the parsing.
     """
     ACTIONS = {'IF': '__execute_if',
                'ENDIF': '__execute_endif',
                'ELSE': '__execute_else',
                'IFEQ': '__execute_ifeq',
                'IFDEF': '__execute_ifdef',
                'FOR': '__execute_for',
@@ -64,66 +84,32 @@
                'SET':  '__execute_set',
                'DEBUG': '__execute_debug',
                'INCLUDE': '__execute_include',
                'SET_TEXTVAR': '__execute_set_textvar',
                'END_TEXTVAR': '__execute_end_textvar',
                'IMPORT':'__execute_import'}
 
-    def __init__(self, fileNames, parse_config=dict(), included=set(), debug=0):
-        """Initialize an PyFreeFEM preprocessor.
-
-        Usage
-        -----
-
-        Parse a single file
-        >>> preproc=Preprocessor('solveState.edp')
-
-        Parse a list of files (to be assembled consecutively)
-        >>> preproc=Preprocessor(['params.edp','solveState.edp'])
-
-        Parse a single file with an updated configuration
-        >>> preproc=Preprocessor('solveState.edp',{'ITER':'0010'})
-
-        Parse raw code
-        >>> code = "mesh Th=square(10,10);"
-            preproc=Preprocessor(code)
-
-        Then parse these files with `Preprocessor.parse':
-        >>>  parsedCode=preproc.parse();
-             parsedCode=preproc.parse({'ITER':'0001'});# Update magic variable
-
-        Parameters
-        ----------
-
-        fileNames :     some source code, a single file name or a list of
-                        file names to parse consecutively
-
-        parse_config : (optional) a dictionary of magic variables values
-
-        included   : (optional) a list of file names that must not be
-                    included. Usually empty, used for implementation
-                    purposes.
-
-        debug     : A tuning parameter for the verbosity, allows to
-                    check the behavior of the parsing.
-        """
+    def __init__(self, script, config=dict(), included=set(), debug=0):
         self.code = []
         self.files = []
         self.debug = debug
         self.interpreted = ''
         self.state = []
         self.position = 0
+
+        #: Dictionary of magic variables.   
+        #: This dictionary is updated after calling :meth:`pyfreefem.preprocessor.Preprocessor.parse`.
         self.config = dict()
         self.stackFor = dict()
         self.imports = []
-        if isinstance(fileNames, str):
-            self.files = [fileNames]
+        if isinstance(script, str):
+            self.files = [script]
         else:
-            self.files = fileNames
-        self.initConfig = parse_config
+            self.files = script
+        self.initConfig = config
         for fileName in self.files:
             if len(fileName.splitlines())==1:
                 display("Including "+fileName, 1, debug, 'green')
                 try:
                     with open(fileName, "r") as f:
                         self.code = self.code+f.readlines()
                 except:
@@ -134,46 +120,50 @@
                     self.code[-1] = self.code[-1][:-1]  # Remove extra \n
             else:
                 self.code = self.code+[x+'\n' for x in fileName.splitlines()]
                 self.code[-1] = self.code[-1][:-1]  # Remove extra \n
         self.initialIncluded = set(included)
 
     def replace(self, string, config=None):
-        """Replace a string containing magic variables with their values
-        INPUTS : 
-            string : string to replace
-            config : (default: None). The magic variables are replaced      
-                     according to the values given by `config`
-                     If not specified, config is set to be the internal 
-                     config variable of the Preprocessor object
+        """Replace a string containing magic variables with their values provided   
+           by the ``config`` parameter.
+
+           :param string: string to replace
+           :param config: (default: None). The magic variables are replaced      
+                          according to the values given by `config`
+                          If not specified, config is set to be the attribute
+                          :attr:`pyfreefem.preprocessor.Preprocessor.config`.
         """
         if config is None:
             config = self.config
         keys = list(config.keys())
         keys.sort(reverse=True)
         ret = string
         for key in keys:
             replacement = str(config[key])
             ret = ret.replace(MAGIC_CHARACTER+'{'+key+'}', replacement)
             ret = ret.replace(MAGIC_CHARACTER+key, replacement)
         return ret
 
     def parse(self, config=dict()):
-        """Parse the .edp code provided to the Preprocessor.
-        The internal configuration can be updated according to the dictionary
-        `config` provided by the user.
-
-        >>>  preproc = Preprocessor(file.edp)
-             parsedCode=preproc.parse({'hmin':'0.002'})
-
-        Once the `parse` operation has been called, the internal
-        configuration has been updated and can be accessed from
-        the `~Preprocessor.config` dictionary.
-
-        >>>  print(preproc.config)
+        """Parse the ``.edp`` script provided to the :class:`pyfreefem.preprocessor.Preprocessor`   
+        instance.
+            
+        :param config: a configuration for the magic variable that takes precedence over    
+                       the default ``config`` value provided to the 
+                       :class:`pyfreefem.preprocessor.Preprocessor` constructor. 
+
+                       .. code:: python
+
+                          preproc = Preprocessor('file.edp')
+                          parsedCode=preproc.parse({'hmin':'0.002'})
+
+        Once the :meth:`pyfreefem.preprocessor.Preprocessor.parse` has been called,  
+        the parameter :attr:`pyfreefem.preprocessor.Preprocessor.config` is   
+        updated.    
         """
         # Set the cursor at position 0 and initialize the configuration
         # with the values supplied at initialization
         self.position = 0
         self.interpreted = ''
         self.state = []
         self.imports = []
@@ -527,9 +517,12 @@
         if self.debug > 1:
             display(colored("Interpreted : ", "green") +
                   colored(line[:-1], "blue"),2,self.debug)
         self.position += 1
 
         
     def set(self, assign):
-        """Update the config dictionary"""
+        """Update the config dictionary 
+            
+        :param assign: New values for the dictionary :attr:`pyfreefem.preprocessor.Preprocessor.config`.
+        :type assign: dict"""
         self.config.update(assign)
```

## Comparing `pyfreefem-1.1.0.dist-info/LICENSE` & `pyfreefem-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyfreefem-1.1.0.dist-info/METADATA` & `pyfreefem-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfreefem
-Version: 1.1.0
+Version: 1.1.1
 Summary: Package PyFreeFEM for interfacing Python and FreeFEM.
 Home-page: https://pyfreefem.readthedocs.io/en/latest/
 Author: Florian Feppon
 Author-email: florian.feppon@kuleuven.be
 License: GNU GPL version 3
 Keywords: FreeFEM
 Classifier: Programming Language :: Python :: 3
```

