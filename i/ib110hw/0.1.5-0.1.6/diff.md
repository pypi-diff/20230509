# Comparing `tmp/ib110hw-0.1.5.tar.gz` & `tmp/ib110hw-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Skola\SBAPR\ib110hw\dist\tmpaa5tutr1\ib110hw-0.1.5.tar", last modified: Mon May  8 22:05:20 2023, max compression
+gzip compressed data, was "C:\Skola\SBAPR\ib110hw\dist\tmpi3f1tgnd\ib110hw-0.1.6.tar", last modified: Mon May  8 22:47:34 2023, max compression
```

## Comparing `ib110hw-0.1.5.tar` & `ib110hw-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/
--rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.5/LICENSE
--rw-rw-rw-   0        0        0    30454 2023-05-08 22:05:20.000000 ib110hw-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    30013 2023-05-01 15:32:55.000000 ib110hw-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 22:05:20.000000 ib110hw-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-05-08 22:05:09.000000 ib110hw-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw/
-drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw/automaton/
--rw-rw-rw-   0        0        0     2412 2023-04-17 13:09:33.000000 ib110hw-0.1.5/src/ib110hw/automaton/base.py
--rw-rw-rw-   0        0        0     8339 2023-04-17 13:10:40.000000 ib110hw-0.1.5/src/ib110hw/automaton/dfa.py
--rw-rw-rw-   0        0        0     8592 2023-04-17 13:11:16.000000 ib110hw-0.1.5/src/ib110hw/automaton/nfa.py
--rw-rw-rw-   0        0        0     1461 2023-04-17 08:06:18.000000 ib110hw-0.1.5/src/ib110hw/automaton/utils.py
--rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.5/src/ib110hw/automaton/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw/turing/
--rw-rw-rw-   0        0        0     1227 2023-05-01 15:28:06.000000 ib110hw-0.1.5/src/ib110hw/turing/base.py
--rw-rw-rw-   0        0        0     8055 2023-05-01 15:27:18.000000 ib110hw-0.1.5/src/ib110hw/turing/dtm.py
--rw-rw-rw-   0        0        0     1974 2023-04-30 22:14:51.000000 ib110hw-0.1.5/src/ib110hw/turing/idk.py
--rw-rw-rw-   0        0        0     8461 2023-05-01 15:31:58.000000 ib110hw-0.1.5/src/ib110hw/turing/mtm.py
--rw-rw-rw-   0        0        0     3535 2023-05-01 15:33:06.000000 ib110hw-0.1.5/src/ib110hw/turing/tape.py
--rw-rw-rw-   0        0        0     2549 2023-05-01 15:36:59.000000 ib110hw-0.1.5/src/ib110hw/turing/utils.py
--rw-rw-rw-   0        0        0     8750 2023-05-01 15:37:48.000000 ib110hw-0.1.5/src/ib110hw/turing/_helpers.py
--rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.5/src/ib110hw/turing/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.5/src/ib110hw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    30454 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw.egg-info/requires.txt
--rw-rw-rw-   0        0        0      671 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/tests/
--rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.5/tests/test_dfa.py
--rw-rw-rw-   0        0        0     2363 2023-05-01 15:18:14.000000 ib110hw-0.1.5/tests/test_dtm.py
--rw-rw-rw-   0        0        0     2022 2023-05-01 15:18:12.000000 ib110hw-0.1.5/tests/test_mtm.py
--rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.5/tests/test_nfa.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/
+-rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0    30454 2023-05-08 22:47:34.000000 ib110hw-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    30013 2023-05-01 15:32:55.000000 ib110hw-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 22:47:34.000000 ib110hw-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-05-08 22:38:08.000000 ib110hw-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw/
+drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw/automaton/
+-rw-rw-rw-   0        0        0     2412 2023-04-17 13:09:33.000000 ib110hw-0.1.6/src/ib110hw/automaton/base.py
+-rw-rw-rw-   0        0        0     8339 2023-04-17 13:10:40.000000 ib110hw-0.1.6/src/ib110hw/automaton/dfa.py
+-rw-rw-rw-   0        0        0     8592 2023-04-17 13:11:16.000000 ib110hw-0.1.6/src/ib110hw/automaton/nfa.py
+-rw-rw-rw-   0        0        0     1461 2023-04-17 08:06:18.000000 ib110hw-0.1.6/src/ib110hw/automaton/utils.py
+-rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.6/src/ib110hw/automaton/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw/turing/
+-rw-rw-rw-   0        0        0     1227 2023-05-01 15:28:06.000000 ib110hw-0.1.6/src/ib110hw/turing/base.py
+-rw-rw-rw-   0        0        0     6270 2023-05-08 22:36:18.000000 ib110hw-0.1.6/src/ib110hw/turing/dtm.py
+-rw-rw-rw-   0        0        0     6962 2023-05-08 22:36:08.000000 ib110hw-0.1.6/src/ib110hw/turing/mtm.py
+-rw-rw-rw-   0        0        0     3535 2023-05-01 15:33:06.000000 ib110hw-0.1.6/src/ib110hw/turing/tape.py
+-rw-rw-rw-   0        0        0     2419 2023-05-08 22:35:52.000000 ib110hw-0.1.6/src/ib110hw/turing/utils.py
+-rw-rw-rw-   0        0        0     8749 2023-05-08 22:36:41.000000 ib110hw-0.1.6/src/ib110hw/turing/_helpers.py
+-rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.6/src/ib110hw/turing/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.6/src/ib110hw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    30454 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      645 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/tests/
+-rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.6/tests/test_dfa.py
+-rw-rw-rw-   0        0        0     2363 2023-05-01 15:18:14.000000 ib110hw-0.1.6/tests/test_dtm.py
+-rw-rw-rw-   0        0        0     2022 2023-05-01 15:18:12.000000 ib110hw-0.1.6/tests/test_mtm.py
+-rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.6/tests/test_nfa.py
```

### Comparing `ib110hw-0.1.5/LICENSE` & `ib110hw-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.5/PKG-INFO` & `ib110hw-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib110hw
-Version: 0.1.5
+Version: 0.1.6
 Summary: UNKNOWN
 Home-page: https://github.com/pilatmartin/ib110hw
 Author: Martin Pilát
 Author-email: 8pilatmartin8@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ib110hw-0.1.5/README.md` & `ib110hw-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.5/setup.py` & `ib110hw-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ib110hw",
-    version="0.1.5",
+    version="0.1.6",
     author="Martin Pilát",
     author_email="8pilatmartin8@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ib110hw-0.1.5/src/ib110hw/automaton/base.py` & `ib110hw-0.1.6/src/ib110hw/automaton/base.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.5/src/ib110hw/automaton/dfa.py` & `ib110hw-0.1.6/src/ib110hw/automaton/dfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.5/src/ib110hw/automaton/nfa.py` & `ib110hw-0.1.6/src/ib110hw/automaton/nfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.5/src/ib110hw/automaton/utils.py` & `ib110hw-0.1.6/src/ib110hw/automaton/utils.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.5/src/ib110hw/turing/base.py` & `ib110hw-0.1.6/src/ib110hw/turing/base.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.5/src/ib110hw/turing/dtm.py` & `ib110hw-0.1.6/src/ib110hw/turing/mtm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,160 +1,179 @@
 from copy import deepcopy
 from time import sleep
-from typing import Dict, Optional, Set, Tuple, List, IO
+from typing import Dict, List, Optional, Set, Tuple, IO
 
-from base import BaseTuringMachine, MAX_STEPS_ERROR_MSG
-from tape import Direction, Tape, START_SYMBOL
-from _helpers import dtm_config_to_md, clear_console, close_file, get_step_direction
+from .base import BaseTuringMachine, MAX_STEPS_ERROR_MSG
+from .tape import Direction, Tape, START_SYMBOL
+from ._helpers import clear_console, close_file, mtm_config_to_md, get_step_direction
 
-DTMRule = Tuple[str, str, Direction]
-DTMRules = Dict[str, DTMRule]
-DTMTransitions = Dict[str, DTMRules]
+Symbols = Tuple[str, ...]
+Directions = Tuple[Direction, ...]
 
+MTMRule = Tuple[str, Symbols, Directions]
+MTMRules = Dict[Symbols, MTMRule]
+MTMTransitions = Dict[str, MTMRules]
 
-class DTM(BaseTuringMachine):
+
+class MTM(BaseTuringMachine):
     """
-    Represents a Deterministic Turing Machine
+    Represents a Multi-tape Turing Machine
     """
 
     def __init__(
         self,
         states: Set[str] = None,
         input_alphabet: Set[str] = None,
         acc_state: str = "accept",
-        rej_states: str = "reject",
-        transitions: DTMTransitions = None,
-        tape: Tape = None,
+        rej_state: str = "reject",
+        transitions: MTMTransitions = None,
+        tape_count: int = 2,
+        tapes: List[Tape] = None,
         initial_state: str = "init",
         start_symbol: str = START_SYMBOL,
-    ) -> None:
+    ):
         super().__init__(
             states,
             input_alphabet,
             acc_state,
-            rej_states,
+            rej_state,
             initial_state,
             start_symbol,
         )
         self.transitions = transitions if transitions is not None else {}
-        self.tape = tape or Tape()
+        self.tapes = tapes or [deepcopy(Tape()) for _ in range(tape_count)]
+        self.tape_count = tape_count or len(tapes)
 
-    def get_transition(self, state: str, read: str) -> Optional[DTMRule]:
+    def get_transition(self, state: str, read: Symbols) -> Optional[MTMRule]:
         """
-        Gets the transition based on the provided state and read symbol.
+        Returns the transition based on the current state and read symbols.
 
         Args:
-            state (str): Current state of the DTM.
-            read (str): Symbol read by the tape head.
+            state (str): Current state.
+            read (Symbols): Current read symbols.
 
         Returns:
-            DTMRule: Transition based on the provided parms if exists, None otherwise.
+            Optional[MTMRule]: Transition based on the provided params if exists, None otherwise.
         """
         return self.transitions.get(state, {}).get(read, None)
 
-    def write_to_tape(self, input_str: str) -> None:
+    def write_to_tape(self, input_str: str, index: int = 0) -> None:
         """
-        Writes the provided string on the tape.
+        Writes the provided string on the tape on the index.
 
         Args:
             input_str (str): String to be written on the tape.
+            index (int, optional): Index of the tape to be updated. Defaults to 0.
+        """
+        self.tapes[index].write(self.start_symbol + input_str)
+
+    def clear_tape(self, index: int) -> None:
+        """
+        Clears the tape on the index.
+
+        Args:
+            index (int): Index of the tape.
         """
-        self.tape.write(self.start_symbol + input_str)
+        self.tapes[index].clear()
 
-    def clear_tape(self) -> None:
+    def clear_tapes(self) -> None:
+        """
+        Clears all the tapes
         """
-        Clears the contents of the tape.
+        for tape in self.tapes:
+            tape.clear()
+
+    def read_tape(self, index: int = 0) -> str:
+        """
+        Reads contents of a tape by index.
+
+        Returns:
+            str: String written on the tape on index.
         """
-        self.tape.clear()
+        return self.tapes[index].read()
 
-    def read_tape(self) -> str:
+    def get_current_symbols(self) -> Symbols:
         """
-        Reads contents of the tape.
+        Gets the current symbols read by tape heads.
 
         Returns:
-            str: String written on the tape.
+            Symbols: Symbols read by the tape heads.
         """
-        return self.tape.read()
+        return tuple((tape.current.value for tape in self.tapes))
 
     def simulate(
         self,
         to_console: bool = True,
         to_file: bool = False,
         path: str = "simulation.md",
         delay: float = 0.5,
         step_by_step: bool = False,
     ) -> bool:
-        """
-        Simulates the machine on its current tape configuration.
+        """Simulates the machine on its current tape configuration.
 
         Args:
             to_console (bool, optional): Set to False if you only want to see the result. Defaults to True.
             to_file (bool, optional): Set to True if you want to save every step to the file. Defaults to False.
             path (str, optional): Path to the .md file with the step history. Defaults to "simulation.md".
             delay (float, optional): The delay (s) between each step when printing to console. Defaults to 0.5.
             step_by_step (bool, optional): Set to True if you want the simulation wait after each step. Defaults to False.
 
         Returns:
             bool: False if the machine rejects the word or exceeds the 'max_steps' value, True otherwise.
         """
         state: str = self.initial_state
-        steps: int = 0
-        rule: Optional[DTMRule] = None
+        steps: int = 1
+        rule: Optional[MTMRule] = None
         output_file: Optional[IO] = open(path, "w") if to_file else None
 
         # key pressed by user when the 'step_by_step' is enabled, can be <left|right|esc>
         pressed_key: str = "right"
-
-        # remember the previous state and tape configuration to be able to go back and forth
-        prev_states: List[Tuple[str, Tape]] = []
+        prev_states: List[Tuple[str, List[Tape]]] = []
 
         def get_rule_string() -> str:
             """
             Parse the current configuration to string shown to user.
             """
-            row = self.get_transition(state, self.tape.current.value)
+            row = self.get_transition(state, self.get_current_symbols())
             step_index = steps if row else steps - 1
-            next_step = f"{state}, '{self.tape.current.value}'"
+            next_step = f"{state}, {self.get_current_symbols()}"
 
-            return f"{step_index}. ({next_step}) -> {row}\n"
+            return f"{step_index}. ({next_step}) -> {row}"
 
         def write_machine_configuration() -> None:
             """
             Write the configuration string to all enabled outputs.
             """
             rule_str = get_rule_string()
 
             if output_file:
-                output_file.write(dtm_config_to_md(self.tape, rule_str))
+                output_file.write(mtm_config_to_md(self.tapes, rule_str))
 
             if to_console or step_by_step:
                 clear_console()
-                print(f"{rule_str}\n{self.tape}")
+                print(rule_str, "\n\n")
+
+                for i, t in enumerate(self.tapes):
+                    print(f"Tape {i}\n{t}")
+
                 sleep(0 if step_by_step else delay)
 
         def go_forward() -> None:
-            """
-            Goes one step forward in the computation.
-            """
-            nonlocal steps, rule, prev_states
-            rule = self.get_transition(state, self.tape.current.value)
-            prev_states.append((state, deepcopy(self.tape)))
+            nonlocal rule, steps
+            rule = self.get_transition(state, self.get_current_symbols())
+            prev_states.append((state, deepcopy(self.tapes)))
             steps += 1
 
         def go_back() -> None:
-            """
-            Goes one step back in the computation.
-            Does nothing if there is no previous step.
-            """
             if not prev_states:
                 return
 
             nonlocal steps, state
             steps -= 1
-            state, self.tape = prev_states.pop()
+            state, self.tapes = prev_states.pop()
 
         while steps <= (self.max_steps + 1):
             write_machine_configuration()
 
             if state == self.acc_state:
                 close_file(output_file)
                 return True
@@ -173,72 +192,20 @@
 
             go_forward()
 
             if not rule or rule[0] == self.rej_state:
                 close_file(output_file)
                 return False
 
-            state, write, direction = rule
-            self.tape.write_symbol(write)
-            self.tape.move(direction)
+            state, write, directions = rule
+            for direction, tape, symbol in zip(directions, self.tapes, write):
+                tape.write_symbol(symbol)
+                tape.move(direction)
 
         close_file(output_file)
         print(MAX_STEPS_ERROR_MSG.format(self.max_steps))
 
         return False
 
 
 if __name__ == "__main__":
-    transitions = {
-        "init": {
-            ">": ("findA", ">", Direction.R),
-        },
-        "findA": {
-            "a": ("findB", "a", Direction.R),
-            "b": ("findA", "b", Direction.R),
-            "c": ("findA", "c", Direction.R),
-        },
-        "findB": {
-            "a": ("findB", "a", Direction.R),
-            "b": ("markC", "b", Direction.R),
-            "c": ("findA", "c", Direction.R),
-        },
-        "markC": {
-            "a": ("shiftA", "X", Direction.R),
-            "b": ("shiftB", "X", Direction.R),
-            "c": ("shiftC", "X", Direction.R),
-            "": ("findA", "c", Direction.R),
-        },
-        "shiftA": {
-            "a": ("shiftA", "a", Direction.R),
-            "b": ("shiftB", "a", Direction.R),
-            "c": ("shiftC", "a", Direction.R),
-            "": ("goBack", "a", Direction.L),
-        },
-        "shiftB": {
-            "a": ("shiftA", "b", Direction.R),
-            "b": ("shiftB", "b", Direction.R),
-            "c": ("shiftC", "b", Direction.R),
-            "": ("goBack", "b", Direction.L),
-        },
-        "shiftC": {
-            "a": ("shiftA", "c", Direction.R),
-            "b": ("shiftB", "c", Direction.R),
-            "c": ("shiftC", "c", Direction.R),
-            "": ("goBack", "c", Direction.L),
-        },
-        "goBack": {
-            "a": ("goBack", "a", Direction.L),
-            "b": ("goBack", "b", Direction.L),
-            "c": ("goBack", "c", Direction.L),
-            "X": ("findA", "c", Direction.R),
-        },
-    }
-
-    machine = DTM(
-        states={*transitions.keys()},
-        input_alphabet={"a", "b", "c"},
-        transitions=transitions,
-    )
-
-    machine.write_to_tape("abba")
-    print(machine.simulate(step_by_step=True))
+    pass
```

### Comparing `ib110hw-0.1.5/src/ib110hw/turing/tape.py` & `ib110hw-0.1.6/src/ib110hw/turing/tape.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.5/src/ib110hw/turing/utils.py` & `ib110hw-0.1.6/src/ib110hw/turing/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from dtm import DTM
-from mtm import MTM
-from _helpers import (
+from .dtm import DTM
+from .mtm import MTM
+from ._helpers import (
     read_file,
     get_dtm_configuration,
     get_mtm_configuration,
     get_dtm_transition_function,
     validate_dtm_configuration,
     validate_mtm_configuration,
     validate_dtm_transitions,
     validate_mtm_transitions,
     get_mtm_transition_function,
 )
 from typing import Optional
 from sys import stderr
 
 
-def load_dtm_from_file(file_path: str) -> Optional[DTM]:
+def import_dtm(file_path: str) -> Optional[DTM]:
     """
     Loads a DTM from a file if it is valid.
     Returns None if the configuration is invalid and prints the error to stderr.
 
     Args:
         file_path (str): Path to the file with configuration.
 
@@ -43,15 +43,15 @@
         acc_state=acc,
         rej_state=rej,
         initial_state=init,
         transitions=transitions,
     )
 
 
-def load_mtm_from_file(file_path: str) -> Optional[MTM]:
+def import_mtm(file_path: str) -> Optional[MTM]:
     """
     Loads a MTM from a file if it is valid.
     Returns None if the configuration is invalid and prints the error to stderr.
 
     Args:
         file_path (str): Path to the file with configuration.
 
@@ -77,10 +77,8 @@
         initial_state=init,
         tape_count=tape_count,
         transitions=transitions,
     )
 
 
 if __name__ == "__main__":
-    machine = load_dtm_from_file("./test.txt")
-    machine.write_to_tape("abbabba")
-    machine.simulate(step_by_step=True)
+    pass
```

### Comparing `ib110hw-0.1.5/src/ib110hw/turing/_helpers.py` & `ib110hw-0.1.6/src/ib110hw/turing/_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from os import name, system
 from typing import IO, List, Tuple, Set, Optional, Callable
-from tape import Tape, Direction
+from .tape import Tape, Direction
 from itertools import takewhile, dropwhile
 from pynput import keyboard
 import re
 
 
 def clear_console() -> None:
     if name == "posix":
@@ -266,15 +266,15 @@
 
         if not function.get(curr_state):
             function[curr_state] = {}
 
         function[curr_state][tuple(underscore_to_space(clean(reads)))] = (
             next_state.strip(),
             tuple(underscore_to_space(clean(writes))),
-            tuple([parse_direction(d) for d in clean(directions)]),
+            tuple(parse_direction(d) for d in clean(directions)),
         )
 
     return function
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `ib110hw-0.1.5/src/ib110hw.egg-info/PKG-INFO` & `ib110hw-0.1.6/src/ib110hw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib110hw
-Version: 0.1.5
+Version: 0.1.6
 Summary: UNKNOWN
 Home-page: https://github.com/pilatmartin/ib110hw
 Author: Martin Pilát
 Author-email: 8pilatmartin8@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ib110hw-0.1.5/src/ib110hw.egg-info/SOURCES.txt` & `ib110hw-0.1.6/src/ib110hw.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 src/ib110hw/automaton/dfa.py
 src/ib110hw/automaton/nfa.py
 src/ib110hw/automaton/utils.py
 src/ib110hw/turing/__init__.py
 src/ib110hw/turing/_helpers.py
 src/ib110hw/turing/base.py
 src/ib110hw/turing/dtm.py
-src/ib110hw/turing/idk.py
 src/ib110hw/turing/mtm.py
 src/ib110hw/turing/tape.py
 src/ib110hw/turing/utils.py
 tests/test_dfa.py
 tests/test_dtm.py
 tests/test_mtm.py
 tests/test_nfa.py
```

### Comparing `ib110hw-0.1.5/tests/test_dfa.py` & `ib110hw-0.1.6/tests/test_dfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.5/tests/test_dtm.py` & `ib110hw-0.1.6/tests/test_dtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.5/tests/test_mtm.py` & `ib110hw-0.1.6/tests/test_mtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.5/tests/test_nfa.py` & `ib110hw-0.1.6/tests/test_nfa.py`

 * *Files identical despite different names*

