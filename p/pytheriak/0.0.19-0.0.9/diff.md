# Comparing `tmp/pytheriak-0.0.19.tar.gz` & `tmp/pytheriak-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytheriak-0.0.19.tar", last modified: Tue May  9 08:49:07 2023, max compression
+gzip compressed data, was "pytheriak-0.0.9.tar", last modified: Fri Feb 10 23:22:33 2023, max compression
```

## Comparing `pytheriak-0.0.19.tar` & `pytheriak-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 08:49:07.022887 pytheriak-0.0.19/
--rw-rw-rw-   0        0        0    35823 2023-02-10 14:34:06.000000 pytheriak-0.0.19/LICENSE
--rw-rw-rw-   0        0        0       28 2023-02-10 15:45:08.000000 pytheriak-0.0.19/MANIFEST.in
--rw-rw-rw-   0        0        0     3132 2023-05-09 08:49:07.009816 pytheriak-0.0.19/PKG-INFO
--rw-rw-rw-   0        0        0     2649 2023-02-13 21:28:44.000000 pytheriak-0.0.19/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 08:49:07.022887 pytheriak-0.0.19/setup.cfg
--rw-rw-rw-   0        0        0      776 2023-05-09 08:46:05.000000 pytheriak-0.0.19/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:49:06.990791 pytheriak-0.0.19/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 08:49:07.000795 pytheriak-0.0.19/src/pytheriak/
--rw-rw-rw-   0        0        0        0 2023-02-10 17:09:11.000000 pytheriak-0.0.19/src/pytheriak/__init__.py
--rw-rw-rw-   0        0        0     4333 2023-05-09 08:37:04.000000 pytheriak-0.0.19/src/pytheriak/hdfwriter.py
--rw-rw-rw-   0        0        0    31020 2023-05-09 08:19:13.000000 pytheriak-0.0.19/src/pytheriak/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:49:07.007795 pytheriak-0.0.19/src/pytheriak.egg-info/
--rw-rw-rw-   0        0        0     3132 2023-05-09 08:49:06.000000 pytheriak-0.0.19/src/pytheriak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-05-09 08:49:06.000000 pytheriak-0.0.19/src/pytheriak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 08:49:06.000000 pytheriak-0.0.19/src/pytheriak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-09 08:49:06.000000 pytheriak-0.0.19/src/pytheriak.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-09 08:49:06.000000 pytheriak-0.0.19/src/pytheriak.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-10 23:22:33.146962 pytheriak-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2023-02-10 14:34:06.000000 pytheriak-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-02-10 15:45:08.000000 pytheriak-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      748 2023-02-10 23:22:33.144419 pytheriak-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-02-10 13:54:53.000000 pytheriak-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-02-10 23:22:33.147440 pytheriak-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      752 2023-02-10 23:21:44.000000 pytheriak-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-10 23:22:33.123741 pytheriak-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-02-10 23:22:33.132419 pytheriak-0.0.9/src/pytheriak/
+-rw-rw-rw-   0        0        0        0 2023-02-10 17:09:11.000000 pytheriak-0.0.9/src/pytheriak/__init__.py
+-rw-rw-rw-   0        0        0    22402 2023-02-10 23:14:41.000000 pytheriak-0.0.9/src/pytheriak/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-02-10 23:22:33.144419 pytheriak-0.0.9/src/pytheriak.egg-info/
+-rw-rw-rw-   0        0        0      748 2023-02-10 23:22:32.000000 pytheriak-0.0.9/src/pytheriak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-02-10 23:22:32.000000 pytheriak-0.0.9/src/pytheriak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-10 23:22:32.000000 pytheriak-0.0.9/src/pytheriak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-02-10 23:22:32.000000 pytheriak-0.0.9/src/pytheriak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-02-10 23:22:32.000000 pytheriak-0.0.9/src/pytheriak.egg-info/top_level.txt
```

### Comparing `pytheriak-0.0.19/LICENSE` & `pytheriak-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytheriak-0.0.19/setup.py` & `pytheriak-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 with open("README.md", "r") as rm:
     long_description = rm.read()
 
 setup(
     name="pytheriak",
-    version="0.0.19",
+    version="0.0.9",
     description="Wrappers to call and read_out theriak from python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    py_modules=["pytheriak.wrapper", "pytheriak.hdfwriter"],
+    py_modules=["pytheriak.wrapper"],
     package_dir={"": "src"},
     python_requires=">=3.10",
     install_requires=["numpy >= 1.23", ],
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "Development Status :: 2 - Pre-Alpha",
```

### Comparing `pytheriak-0.0.19/src/pytheriak/wrapper.py` & `pytheriak-0.0.9/src/pytheriak/wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,60 +37,14 @@
         else:
             block = theriak_output[start_idx:end_idx]
 
         residual_output = theriak_output[end_idx:]
         return block, residual_output
 
     @staticmethod
-    def extract_solution_subblocks(block_phases: list, verbose: bool = True):
-        """Used in Rock.add_minerals()
-
-        Args:
-            block_phases (list): block_phases from blocks (splitted theriak output)
-            verbose (bool): turn on/off verbose mode, if False no Warnings will be printed, if activities do not match.
-
-        Returns:
-            dict: Dict with phase name (only solution phases) as keys, and output-lines of that corresponding phase in subblocks (list)
-        """
-        block_solution_phases = {}
-        solution_phase_list = []
-
-        # solution phases are marked bijectively by "  0" followed by the solution number in this block
-        start_key = "   0"
-        start_indices = [idx for idx, line in enumerate(block_phases) if line.startswith(start_key)]
-        # shift start_idx and append last line as last end_idx
-        end_indices = start_indices[1:]
-        end_indices.append(len(block_phases))
-
-        for start_idx, end_idx in zip(start_indices, end_indices):
-            solution_subblock = block_phases[start_idx:end_idx]
-
-            # if minimisation failed, subblock layout changes!
-            # check for "activity test", if present remove additional lines.
-            if any("activity test:" in line for line in solution_subblock):
-                cut_idx = solution_subblock.index(" ")
-                solution_subblock = solution_subblock[:cut_idx]
-                # replace the "**" marks with "  ", so that the solution subblock can be treated like one of a succesful minimisation afterwards.
-                solution_subblock = [string.replace("**", "  ") for string in solution_subblock]
-                if verbose:
-                    print("WARNING: Minimisation might have failed. End-member activities of solutions might be wrong.")
-
-            # filter out lines containing info about site occupancy or element fractions (e.g. XMg, Al(pfu))
-            # the lines containing end-member fractions and activities are the only ones ending with a double-space "  "
-            # this is represented with the regex pattern: "Any digit""Space""Space""End of string" = "\d\s\s$"
-            solution_subblock = [line for line in solution_subblock if len(re.findall(pattern=r"\d\s\s$", string=line)) == 1]
-
-            # extract solution name from first line / 3rd entry of the solution subblock
-            solution_name = solution_subblock[0].split()[2]
-            solution_phase_list.append(solution_name)
-            block_solution_phases[solution_name] = solution_subblock
-
-        return block_solution_phases
-
-    @staticmethod
     def check_for_corrupted_bulk(bulk: str):
         """Checks if bulk has an non-zero amount of all elemetns in the system.
         If this is not the case, theriak will remove the element from the bulk. Resulting in an unwanted reduction of the systems components.
         In this case the element_idx list would no longer be globally valid!
 
         Args:
             bulk (str): A bulk in the THERIN format
@@ -103,54 +57,40 @@
 
         if len(matches) == 0:
             return True
         else:
             print("WARNING: Corrupted bulk, THERIN bulk (str) contains an element which is 0.")
             return False
 
-    def __init__(self, programs_dir: str, database: str, theriak_version: str, verbose: bool = True):
+    def __init__(self, programs_dir: str, database: str, theriak_version: str, cwd: str):
         """Creates a TherCaller intance.
         For calling theriak, the theriak.ini file must be copied from the programs folder to the working directory.
 
         Args:
             programs_dir (str): Path to the Programs directory of TheriakDomino
             database (str): Name of the database
             theriak_version (str): version of theriak, lookup in programs folder.
 
         """
+        self.cwd = Path(cwd)
 
         self.theriak_exe = Path(programs_dir) / "theriak"
         self.database = database
 
         self.theriak_version = theriak_version
 
-        self.verbose_mode = verbose
-
-    def call_theriak(self, pressure: int, temperature: int, bulk: str):
-        """Execute theriak.exe and returns the OUT as string.
-
-        Args:
-            pressure (int): Pressure in [bar].
-            temperature (int): Temperature in [deg C]
-            bulk (str): Bulk composition in the THERIN format. Elements in capital letters (e.g. SI, AL) and moles in brackets.
-
-        Returns:
-            str: Theriak output.
-        """
-        self.pressure = pressure
-        self.temperature = temperature
-
         # create theriak input for subprocess.run(), "\n" is interpreted as "enter"
         self.theriak_input = self.database + "\n" + "no\n"
 
+    def call_theriak(self, pressure: int, temperature: int, bulk: str):
         # write THERIN
         self.therin_PT = "    " + str(temperature) + "    " + str(pressure)
         self.therin_bulk = "1   " + bulk + "    *"
 
-        with open("THERIN", "w") as therin_file:
+        with open(self.cwd / "THERIN", "w") as therin_file:
             therin_file.write(self.therin_PT)
             therin_file.write("\n")
             therin_file.write(self.therin_bulk)
 
         # call theriak
         out = subprocess.run([self.theriak_exe],
                              input=self.theriak_input,
@@ -159,121 +99,93 @@
 
         theriak_output = out.stdout
 
         return theriak_output
 
     def check_minimisation(self, theriak_output: str):
         """Checks for theriak calls with failed minimisation.
-        If and only if a minimisation fails, this will be marked in the theriak output by "**" before the activities of EM in solutions.
+        If and only if a minimisation fails, this will be marked in the theriak output by "**" before the activities of Em in solutions.
         Additionally below the activities block the "** activity test:" is listed for the failed solution phases.
 
         This function checks for a succesful minimisation.
         For debugginng assistance it prints the THERIN, where the minimisation failed.
 
         Args:
             theriak_output (str): The output of a theriak call, equiv to the OUT file.
 
         Returns:
             bool: State, if theriak call gave resultet in a succesful minimisation.
         """
         substring_if_minimisation_fail = "activity test"
 
         if substring_if_minimisation_fail in theriak_output:
-            if self.verbose_mode is True:
-                print("WARNING: Minimisation possibly failed. For the following THERIN:")
-                print(self.therin_PT)
-                print(self.therin_bulk)
+            print("WARNING: Detected a failed minimisation. For the following THERIN:")
+            print(self.therin_PT)
+            print(self.therin_bulk)
 
             return False
 
         elif substring_if_minimisation_fail not in theriak_output:
             return True
 
-    def read_theriak(self, theriak_output: str):
-        """Reads theriak output
-        Information of interest is extracted as blocks, which then can be further processed by other methods.
-
-        Args:
-            theriak_output (str): Theriak out from TherCaller.call_theriak
-
-        Returns:
-            dict: blocks, a dict containing the extracted block of interest from the theriak output
-            list: element_list, element-idx list globally valid for all compositional data
-            bool: output_line_overflow
-            bool: fluids_stable
-        """
+    def read_theriak(self, theriak_output: str, pressure: int, temperature: int):
         theriak_output = theriak_output.splitlines()
 
-        # extract blocks of interest from theriak output
+        """
+        extract blocks of interest from theriak output
+        """
         # 1) bulk rock composition
         start_key_bulk = " composition:        N           N             mol%"
         end_key_bulk = " considered phases:"
         block_bulk, residual_output = TherCaller.output_block_finder(theriak_output, start_key_bulk, end_key_bulk, True)
 
         # 2) G_system
         start_key_Gsys = " equilibrium assemblage:"
         end_key_Gsys = "         phase                   N         mol%                                   x              x         activity       act.(x)"
         block_Gsys, residual_output = TherCaller.output_block_finder(residual_output, start_key_Gsys, end_key_Gsys, False)
 
-        # 3) equilibrium assemblage, stable phases
-        start_key_phases = "         phase                   N         mol%                                   x              x         activity       act.(x)"
-        end_key_phases = " volumes and densities of stable phases:"
-        block_phases, residual_output = TherCaller.output_block_finder(residual_output, start_key_phases, end_key_phases, True)
-
-        # 4) volume and densities of stable phases
+        # 3) volume and densities of stable phases
         start_key_volume = " volumes and densities of stable phases:"
         # choose end_key_volume, so that always present independent if fluids are stable or not (this will affect the text of the theriak output)
         end_key_volume = " compositions of stable phases [ mol% ]:"
         # don't pass the residual output here, because the fluid block comes before end_key_volume in the theriak output
         block_volume, residual_output_NOT_TO_USE = TherCaller.output_block_finder(residual_output, start_key_volume, end_key_volume, True)
 
-        # 5) gases and fluids
+        # 4) gases and fluids
         start_key_fluid = "  gases and fluids       N       volume/mol  volume[ccm]               wt/mol       wt [g]              density [g/ccm]"
         end_key_fluid = " H2O content of stable phases:"
         try:
             block_fluid, residual_output = TherCaller.output_block_finder(residual_output, start_key_fluid, end_key_fluid, True)
             fluids_stable = True
         # catch the ValueError, when no stable fluid phases predicted the block_fluid wont show in theriak output.
         except ValueError:
-            if self.verbose_mode:
-                print("WARNING: No fluid phase stable at given P-T-X. Water-sat. conditions not fulfilled.")
-            # set a state, to disable adding fluids to the rock later on. Set an empty list as placeholder instead of the fluid block.
+            print("WARNING: No fluid phase stable at given P-T-X. Water-sat. conditions not fulfilled.")
+            # set a state, to disabkle adding fluids to the rock later on. Set an empty list as placeholder instead of the fluid block.
             fluids_stable = False
             block_fluid = []
 
-        # 6) phase compositions; elements in moles in stable phases + in total system (=bulk)
+        # 5) phase compositions; elements in moles in stable phases + in total system (=bulk)
         start_key_elements = " elements in stable phases:"
         end_key_elements = " elements per formula unit:"
         block_elements, residual_output = TherCaller.output_block_finder(residual_output, start_key_elements, end_key_elements, False)
 
-        # 7) phase composition: elements per formula unit
+        # 6) phase composition: elements per formula unit
         start_key_composition = " elements per formula unit:"
         end_key_composition = " activities of all phases:"
         block_composition, residual_output = TherCaller.output_block_finder(residual_output, start_key_composition, end_key_composition, True)
 
-        # 8) activities of all phases: delta_G above stable plain
+        # 7) activities of all phases: delta_G above stable plain
         start_key_deltaG = " activities of all phases:"
         end_key_deltaG = " chemical potentials of components:"
         block_deltaG, residual_output = TherCaller.output_block_finder(residual_output, start_key_deltaG, end_key_deltaG, True)
 
-        # 9) chemical potential of components
-        # ## future addition.
+        # 8) chemical potential of components
+        # ## OPTIONAL, to be discussed if necessary.
 
-        # 10) extract subblocks from block_phases for end-member properties of solution phases
-        solution_subblocks = TherCaller.extract_solution_subblocks(block_phases=block_phases, verbose=self.verbose_mode)
-
-        blocks = {"block_bulk": block_bulk,
-                  "block_Gsys": block_Gsys,
-                  "block_phases": block_phases,
-                  "block_solutions": solution_subblocks,
-                  "block_volume": block_volume,
-                  "block_fluid": block_fluid,
-                  "block_elements": block_elements,
-                  "block_composition": block_composition,
-                  "block_deltaG": block_deltaG}
+        blocks = [block_bulk, block_Gsys, block_volume, block_fluid, block_elements, block_composition, block_deltaG]
 
         # check for line overflow: ("elements in bulk" > 10) in "elements in stable phases:"
         # if last line in compostion block starts with an indendation, then there is line overflow in the output
         output_line_overflow = False
         if block_composition[-1].startswith("                    "):
             # pass this as a state attribute to the rock object
             output_line_overflow = True
@@ -283,49 +195,27 @@
         # catch a second line of elements in output
         if output_line_overflow:
             additional_elements = block_elements[4].split()
             element_list += additional_elements
         # drop last element "E" (only for testing in theriak)
         element_list = element_list[:-1]
 
-        return blocks, element_list, output_line_overflow, fluids_stable
-
-    def create_rock(self, blocks: dict, output_line_overflow: bool, fluids_stable: bool):
-        rock = Rock(pressure=self.pressure, temperature=self.temperature)
+        """
+        Create Rock
+        """
+        rock = Rock(pressure=pressure, temperature=temperature)
         rock.add_therin_to_reproduce(PT=self.therin_PT, bulk=self.therin_bulk)
-        rock.add_bulk_rock_composition(block_bulk=blocks["block_bulk"])
-        rock.add_g_system(block_Gsys=blocks["block_Gsys"])
-        rock.add_bulk_density(block_volume=blocks["block_volume"])
-        rock.add_minerals(block_volume=blocks["block_volume"], block_solutions=blocks["block_solutions"], block_composition=blocks["block_composition"],
-                          block_elements=blocks["block_elements"], output_line_overflow=output_line_overflow, verbose=self.verbose_mode)
+        rock.add_bulk_rock_composition(block_bulk=blocks[0])
+        rock.add_g_system(block_Gsys=blocks[1])
+        rock.add_minerals(block_volume=blocks[2], block_composition=blocks[5], block_elements=blocks[4], element_list=element_list, output_line_overflow=output_line_overflow)
         if fluids_stable:
-            rock.add_fluids(block_fluid=blocks["block_fluid"], block_solutions=blocks["block_solutions"], block_composition=blocks["block_composition"],
-                            block_elements=blocks["block_elements"], output_line_overflow=output_line_overflow)
-        rock.add_deltaG(block_deltaG=blocks["block_deltaG"])
+            rock.add_fluids(block_fluid=blocks[3], block_composition=blocks[5], element_list=element_list, output_line_overflow=output_line_overflow)
+        rock.add_deltaG(block_deltaG=blocks[6])
         rock.add_g_system_per_mol()
-
-        return rock
-
-    def minimisation(self, pressure: int, temperature: int, bulk: str, return_failed_minimisation: bool = False):
-        # A compositon of call_theriak --> check_minimisation --> read_theriak; returning a rock, ele_list
-        theriak_output = TherCaller.call_theriak(self, pressure=pressure, temperature=temperature, bulk=bulk)
-        minimisation_state = TherCaller.check_minimisation(self, theriak_output=theriak_output)
-        if return_failed_minimisation:
-            # overwrite minimisation_state
-            minimisation_state = True
-
-        if minimisation_state:
-            blocks, element_list, output_line_overflow, fluids_stable = TherCaller.read_theriak(self, theriak_output=theriak_output)
-            rock = TherCaller.create_rock(self, blocks=blocks, output_line_overflow=output_line_overflow, fluids_stable=fluids_stable)
-
-            return rock, element_list
-
-        else:
-            # for a failed minimisation return the raw theriak output. And an empty list instead of the element_list
-            return theriak_output, []
+        return rock, theriak_output, blocks, element_list
 
 
 class Rock:
     """_summary_
     A "Rock" is defined by 3 parameters: (P, T, bulk composition).
     Rock()-instances are created by TherCaller.call_theriak() as the result of a Gibb's Energy minimisation done by theriak.
 
@@ -386,35 +276,17 @@
         """
         self.mineral_assemblage = []
         self.fluid_assemblage = []
         self.mineral_delta_G = None
         self.g_system = None
         self.pressure = pressure
         self.temperature = temperature
-        self.bulk_composition_moles = None
+        self.bulk_composition_n = None
         self.bulk_composition_mol_percent = None
 
-    def __dir__(self):
-        """Overwrite dir() to only return objects attriubutes holding thermodynamic state properties.
-
-        Returns:
-            (list): List of Rock-attrs holding state properties of minimised system.
-        """
-        return ["mineral_assemblage",
-                "fluid_assemblage",
-                "mineral_delta_G",
-                "g_system",
-                "g_system_per_mol_of_input",
-                "pressure",
-                "temperature",
-                "bulk_composition_moles",
-                "bulk_composition_mol_percent",
-                "therin_PT",
-                "therin_bulk"]
-
     def add_therin_to_reproduce(self, PT: str, bulk: str):
         """Passes THERIN strings from the TherCaller.call-theriak() to the Rock object
 
         Args:
             PT (str): THERIN first line
             bulk (str): THERIN second line
         """
@@ -431,15 +303,15 @@
         # convert to str --> float
         bulk_mol_list = [float(n) for n in bulk_mol_list]
         # extract 4th entry, mol% in bulk
         bulk_mol_percent_list = [n.split()[4] for n in block_bulk]
         # convert to str --> float
         bulk_mol_percent_list = [float(n) for n in bulk_mol_percent_list]
 
-        self.bulk_composition_moles = bulk_mol_list
+        self.bulk_composition_n = bulk_mol_list
         self.bulk_composition_mol_percent = bulk_mol_percent_list
 
     def add_g_system(self, block_Gsys: list):
         """Reads G(System) from respective theriak output block and saves it to self.g_system
 
         Args:
             block_Gsys (list): block_Gsys from blocks (splitted theriak output --> generated by TherCaller.call_theriak())
@@ -450,94 +322,78 @@
         g_system = g_system_line.split()[5]
         # transfrom str --> float
         g_system = float(g_system)
 
         self.g_system = g_system
 
     def add_g_system_per_mol(self):
-        composition_list = self.bulk_composition_moles
+        composition_list = self.bulk_composition_n
         sum_mol_input_elements = np.sum(composition_list)
         # divide the g_system by the molar sum of all inputed elements;
         # doing this makes the g_sys independent from the absolute input used (depends on personal format choice)
         self.g_system_per_mol_of_input = self.g_system / sum_mol_input_elements
 
-    def add_bulk_density(self, block_volume: list):
-        """Reads the bulk density of solid phases form te respective theriak output block.
-        Attention: Depending on the activated melt model, melts can be included in solid phases, therefore affecting also bulk density.
-
-        Args:
-            block_volume (list): block_volume from blocks (splitted theriak output --> generated by TherCaller.call_theriak())
-        """
-        bulk_properties_line = [line for line in block_volume if line.startswith("  total of solids")][0]
-        bulk_density = bulk_properties_line.split()[-1]
-        # transform str --> float
-        bulk_density = float(bulk_density)
-
-        self.bulk_density = bulk_density
-
-    def add_minerals(self, block_volume: list, block_solutions: list, block_composition: list,
-                     block_elements: list, output_line_overflow: bool, verbose: bool = True):
+    def add_minerals(self, block_volume: list, block_composition: list, block_elements: list, element_list: list, output_line_overflow: bool):
         temp_name_list = Rock.get_mineral_list(block_volume=block_volume)
 
         for temp_name in temp_name_list:
             mineral = Mineral(phase_name=temp_name)
             mineral.add_phase_properties(block_volume=block_volume, temp_name=temp_name)
             mineral.add_composition_apfu(block_composition=block_composition,
                                          temp_name=temp_name,
                                          output_line_overflow=output_line_overflow)
             mineral.add_composition_moles(block_elements=block_elements,
                                           temp_name=temp_name,
                                           output_line_overflow=output_line_overflow)
 
-            if temp_name in block_solutions.keys():
-                mineral.add_endmember_properties(solution_phase_subblock=block_solutions[temp_name])
-
             self.mineral_assemblage.append(mineral)
 
-    def add_fluids(self, block_fluid: list, block_solutions: list, block_composition: list,
-                   block_elements: list, output_line_overflow: bool):
+    def add_fluids(self, block_fluid: list, block_composition: list, block_elements: list, output_line_overflow: bool):
         fluid_name_list = Rock.get_fluid_list(block_fluid=block_fluid)
 
         for fluid_name in fluid_name_list:
             fluid = Fluid(phase_name=fluid_name)
             fluid.add_phase_properties(block_fluid=block_fluid, temp_name=fluid_name)
             fluid.add_composition_apfu(block_composition=block_composition,
                                        temp_name=fluid_name,
                                        output_line_overflow=output_line_overflow)
             fluid.add_composition_moles(block_elements=block_elements,
                                         temp_name=fluid_name,
                                         output_line_overflow=output_line_overflow)
 
-            if fluid_name in block_solutions.keys():
-                fluid.add_endmember_properties(solution_phase_subblock=block_solutions[fluid_name])
-
             self.fluid_assemblage.append(fluid)
 
     def add_deltaG(self, block_deltaG: list):
         # remove title
         block_deltaG = block_deltaG[5:]
         # search idx of delimiter stable / metastable phases
         delimiter = block_deltaG.index("--------------------------------------------------------------------")
         block_deltaG = block_deltaG[delimiter+1:]
         metastable_list = [i.split() for i in block_deltaG if (i.startswith(" S") or i.startswith(" P"))]
         # look for the first occurence of "0.00000E+00"
         idx_of_firstZEROS = [i.index("0.00000E+00") for i in metastable_list]
         metastable_list_names = [i[2] for i in metastable_list]
         metastable_list_deltaG = [i[idx + 1] for i, idx in zip(metastable_list, idx_of_firstZEROS)]
-        metastable_list_deltaG = [float(i) for i in metastable_list_deltaG]
-
-        mineral_delta_G = dict(zip(metastable_list_names, metastable_list_deltaG))
-        self.mineral_delta_G = mineral_delta_G
+        # try:
+        #     metastable_list_deltaG = [i[1].split()[0] for i in metastable_list]
+        #     print("!!!! METASTABLE LIST correct !!!")
+        #     print(metastable_list)
+        # except IndexError:
+        #     print("!!!! METASTABLE LIST FAIL !!!")
+        #     print(metastable_list)
+        #     print("!!!! block_deltaG !!!")
+        #     print(block_deltaG)
+        metastable_list = np.array([metastable_list_names, metastable_list_deltaG])
+        metastable_list = np.transpose(metastable_list).tolist()
+        self.mineral_delta_G = metastable_list
 
 
 class Phase:
     def __init__(self, phase_name) -> None:
         self.name = phase_name
-        # A Phase is a priori a pure phase, only add_endmember_properties() updates this state attribute to True for solutions.
-        self.solution_phase: bool = False
 
     def add_composition_apfu(self, block_composition: list, temp_name: str, output_line_overflow: bool):
         """_summary_
 
         Args:
             block_composition (list): block_composition from blocks (splited theriak output)
             temp_name (str): _description_
@@ -554,15 +410,15 @@
             phase_composition += additional_line.split()
 
         # drop first (Phase name) and last ("E"-composition) entry
         phase_composition = phase_composition[1:-1]
         # convert composition to float
         phase_composition = [float(x) for x in phase_composition]
 
-        self.composition_apfu = phase_composition
+        self.composition = phase_composition
         # important to also save Oxygen, to calculate Fe3
 
     def add_composition_moles(self, block_elements: list, temp_name: str, output_line_overflow: bool):
         # get list entry (str of an output line), that startswith temp_name
         phase_composition_line = [i for i in block_elements if i.startswith(" " + temp_name)]
         phase_composition = phase_composition_line[0].split()
         if output_line_overflow:
@@ -574,37 +430,14 @@
         # drop first (Phase name) and last ("E"-composition) entry
         phase_composition = phase_composition[1:-1]
         # convert composition to float
         phase_composition = [float(x) for x in phase_composition]
 
         self.composition_moles = phase_composition
 
-    def add_endmember_properties(self, solution_phase_subblock: list):
-        # update state-attribute to mark phase as solution
-        self.solution_phase = True
-        # read the solution phase subblock
-        lines = [line.split() for line in solution_phase_subblock]
-        # get rid off additional entries in the first line (pre-fix, phase, N, mol%)
-        first_line = lines[0][5:]
-        lines[0] = first_line
-
-        endmember_activities = {}
-        endmember_fractions = {}
-
-        for line in lines:
-            endmember_name = line[0]
-            activity = float(line[-2])
-            fraction = float(line[-4])
-
-            endmember_activities[endmember_name] = activity
-            endmember_fractions[endmember_name] = fraction
-
-        self.endmember_activities = endmember_activities
-        self.endmember_fractions = endmember_fractions
-
 
 class Mineral(Phase):
     def add_phase_properties(self, block_volume: list, temp_name: str):
         # get list entry (str of an output line), that startswith temp_name
         phase_properties_line = [i for i in block_volume if i.startswith("  " + temp_name)]
         phase_properties_line = phase_properties_line[0].split()
         # extract the physical properties by indexing
```
