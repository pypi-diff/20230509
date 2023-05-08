# Comparing `tmp/ib110hw-0.1.4.tar.gz` & `tmp/ib110hw-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Skola\SBAPR\ib110hw\dist\tmptxq5pl5a\ib110hw-0.1.4.tar", last modified: Thu Apr 20 22:37:21 2023, max compression
+gzip compressed data, was "C:\Skola\SBAPR\ib110hw\dist\tmpaa5tutr1\ib110hw-0.1.5.tar", last modified: Mon May  8 22:05:20 2023, max compression
```

## Comparing `ib110hw-0.1.4.tar` & `ib110hw-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/
--rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.4/LICENSE
--rw-rw-rw-   0        0        0    26734 2023-04-20 22:37:21.000000 ib110hw-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    26293 2023-04-17 08:42:12.000000 ib110hw-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 22:37:21.000000 ib110hw-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-04-20 22:33:40.000000 ib110hw-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw/
-drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw/automaton/
--rw-rw-rw-   0        0        0     2412 2023-04-17 13:09:33.000000 ib110hw-0.1.4/src/ib110hw/automaton/base.py
--rw-rw-rw-   0        0        0     8339 2023-04-17 13:10:40.000000 ib110hw-0.1.4/src/ib110hw/automaton/dfa.py
--rw-rw-rw-   0        0        0     8592 2023-04-17 13:11:16.000000 ib110hw-0.1.4/src/ib110hw/automaton/nfa.py
--rw-rw-rw-   0        0        0     1461 2023-04-17 08:06:18.000000 ib110hw-0.1.4/src/ib110hw/automaton/utils.py
--rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.4/src/ib110hw/automaton/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw/turing/
--rw-rw-rw-   0        0        0     1239 2023-04-06 00:41:42.000000 ib110hw-0.1.4/src/ib110hw/turing/base.py
--rw-rw-rw-   0        0        0     4606 2023-04-11 17:53:39.000000 ib110hw-0.1.4/src/ib110hw/turing/dtm.py
--rw-rw-rw-   0        0        0     5704 2023-04-06 00:44:32.000000 ib110hw-0.1.4/src/ib110hw/turing/mtm.py
--rw-rw-rw-   0        0        0     3474 2023-04-06 00:42:49.000000 ib110hw-0.1.4/src/ib110hw/turing/tape.py
--rw-rw-rw-   0        0        0     1246 2023-04-17 08:14:21.000000 ib110hw-0.1.4/src/ib110hw/turing/utils.py
--rw-rw-rw-   0        0        0     5031 2023-04-17 08:11:17.000000 ib110hw-0.1.4/src/ib110hw/turing/_helpers.py
--rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.4/src/ib110hw/turing/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.4/src/ib110hw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    26734 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/tests/
--rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.4/tests/test_dfa.py
--rw-rw-rw-   0        0        0     2369 2023-04-02 20:51:44.000000 ib110hw-0.1.4/tests/test_dtm.py
--rw-rw-rw-   0        0        0     2028 2023-04-02 20:51:33.000000 ib110hw-0.1.4/tests/test_mtm.py
--rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.4/tests/test_nfa.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/
+-rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0    30454 2023-05-08 22:05:20.000000 ib110hw-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    30013 2023-05-01 15:32:55.000000 ib110hw-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 22:05:20.000000 ib110hw-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-05-08 22:05:09.000000 ib110hw-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw/
+drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw/automaton/
+-rw-rw-rw-   0        0        0     2412 2023-04-17 13:09:33.000000 ib110hw-0.1.5/src/ib110hw/automaton/base.py
+-rw-rw-rw-   0        0        0     8339 2023-04-17 13:10:40.000000 ib110hw-0.1.5/src/ib110hw/automaton/dfa.py
+-rw-rw-rw-   0        0        0     8592 2023-04-17 13:11:16.000000 ib110hw-0.1.5/src/ib110hw/automaton/nfa.py
+-rw-rw-rw-   0        0        0     1461 2023-04-17 08:06:18.000000 ib110hw-0.1.5/src/ib110hw/automaton/utils.py
+-rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.5/src/ib110hw/automaton/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw/turing/
+-rw-rw-rw-   0        0        0     1227 2023-05-01 15:28:06.000000 ib110hw-0.1.5/src/ib110hw/turing/base.py
+-rw-rw-rw-   0        0        0     8055 2023-05-01 15:27:18.000000 ib110hw-0.1.5/src/ib110hw/turing/dtm.py
+-rw-rw-rw-   0        0        0     1974 2023-04-30 22:14:51.000000 ib110hw-0.1.5/src/ib110hw/turing/idk.py
+-rw-rw-rw-   0        0        0     8461 2023-05-01 15:31:58.000000 ib110hw-0.1.5/src/ib110hw/turing/mtm.py
+-rw-rw-rw-   0        0        0     3535 2023-05-01 15:33:06.000000 ib110hw-0.1.5/src/ib110hw/turing/tape.py
+-rw-rw-rw-   0        0        0     2549 2023-05-01 15:36:59.000000 ib110hw-0.1.5/src/ib110hw/turing/utils.py
+-rw-rw-rw-   0        0        0     8750 2023-05-01 15:37:48.000000 ib110hw-0.1.5/src/ib110hw/turing/_helpers.py
+-rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.5/src/ib110hw/turing/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.5/src/ib110hw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    30454 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      671 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 22:05:20.000000 ib110hw-0.1.5/src/ib110hw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 22:05:20.000000 ib110hw-0.1.5/tests/
+-rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.5/tests/test_dfa.py
+-rw-rw-rw-   0        0        0     2363 2023-05-01 15:18:14.000000 ib110hw-0.1.5/tests/test_dtm.py
+-rw-rw-rw-   0        0        0     2022 2023-05-01 15:18:12.000000 ib110hw-0.1.5/tests/test_mtm.py
+-rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.5/tests/test_nfa.py
```

### Comparing `ib110hw-0.1.4/LICENSE` & `ib110hw-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.4/PKG-INFO` & `ib110hw-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib110hw
-Version: 0.1.4
+Version: 0.1.5
 Summary: UNKNOWN
 Home-page: https://github.com/pilatmartin/ib110hw
 Author: Martin Pilát
 Author-email: 8pilatmartin8@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -392,15 +392,24 @@
 # this method either adds a transition, or overwrites the existing one
 # the difference compared to the DFA is that it takes a *set* of next states
 automaton.set_transition("s1", {"s2"}, "1")
 ```
 
 # TURING MACHINE
 
-This library supports **deterministic** and **multi-tape** Turing machines. You can find the implementation in the module `turing`.
+This library supports **deterministic** and **multi-tape** Turing machines. You can find the implementation in the module `turing`. Consider the class located in the base.py as abstract, its only purpose is to avoid duplicity in the implementation of these models.
+
+In order to create a Turing machine you will need to specify the seven-tuple `(Q, Σ, Γ, δ, q0, q_acc, q_rej)`, where:
+
+- The set of states `Q` is represented by `Set[str]`
+- The set of alphabet symbols `Σ` is represented by `Set[str]`
+- The transition function `δ` is represented by either `DTMTransitions` or `MTMTransitions`. These types are described below.
+- The initial state `q0` is represented by `str`
+- The accepting state `q_acc` is represented by `str`
+- The rejecting state `q_rej` is represented by `str`
 
 ## Tape
 
 The implementation of the tape for the Turing machine can be found in the file `tape.py`. The tape class is only used internally by the `DTM` and `MTM` objects - you will *probably* not use it directly.
 
 ```python
 from ib110hw.turing.tape import Tape
@@ -424,14 +433,31 @@
                     #           ^
 
 tape.clear()        # |   |
                     #   ^
 
 ```
 
+The module `tape` also contains enum for the direction of tape head:
+
+```python
+class Direction(Enum):
+    LEFT = -1
+    STAY = 0
+    RIGHT = 1
+    
+    # shorthand aliases
+    L = -1
+    S = 0
+    R = 1
+
+    def __repr__(self):
+        return self.name
+```
+
 ## Deterministic Turing Machine (DTM)
 
 The following DTM checks whether the input string is a palindrome:
 
 ```python
 from ib110hw.turing.dtm import DTM, DTMTransitions
 
@@ -473,16 +499,16 @@
         "X": ("mark", "X", Direction.RIGHT)
     }
 }
 
 machine: DTM = DTM(
     states={"init", "mark", "gotoEndA", "checkA", "gotoEndB", "checkB", "accept", "reject"},
     input_alphabet={"a", "b"},
-    acc_states={"accept"},
-    rej_states={"reject"},
+    acc_states="accept",
+    rej_states="reject",
     initial_state="init",
     transitions=transitions
 )
 
 machine.write_to_tape("aabbabbaa")
 ```
 
@@ -497,51 +523,107 @@
 function: DTMransitions = {
     "init": {
         ">": ("next", ">", Direction.RIGHT)
         }
 }
 ```
 
-# Multi-tape Turing Machine (MTM)
+### Loading From a File
+
+DTM can also be loaded from a file. Format is shown below:
+
+```
+# name of the initial state
+init init
+
+# name of the accepting state
+acc acc
+
+# name of the rejecting state
+rej rej
+
+# alphabet characters without start_symbol
+alphabet a b
+
+---
+
+# current read -> next write direction(L, R, S)
+# ! underscore (_) is used to depict <space> !
+init    > -> mark   > R
+mark    a -> foundA X R
+mark    b -> foundB X R
+mark    X -> acc    X S
+mark    _ -> acc    _ S
+foundA  a -> foundA a R
+foundA  b -> foundA b R
+foundA  X -> checkA X L
+foundA  _ -> checkA _ L
+checkA  a -> back   X L
+checkA  b -> acc    b S
+checkA  X -> rej    X S
+foundB  a -> foundB a R
+foundB  b -> foundB b R
+foundB  X -> checkB X L
+foundB  _ -> checkB _ L
+checkB  a -> reject a S
+checkB  b -> reject X L
+checkB  X -> reject X S
+back    a -> back   a L
+back    b -> back   b L
+back    X -> mark   X R
+
+```
+
+The file above can then be simply loaded using the `load_dtm_from_file(...)`:
+
+```python
+from ib110hw.turing.utils import load_dtm_from_file
+
+machine = load_dtm_from_file("./dtm_file")
+```
+
+## Multi-tape Turing Machine (MTM)
+
+On top of the properties required to create DTM, you will need to specify the number of tapes as well. The default tape count is set to 2.
 
 The following MTM has the same function as the DTM above:
 
 ```python
 from ib110hw.turing.mtm import MTM, MTMTransitions
 from ib110hw.turing.tape import Direction
 
 transitions: MTMTransitions = {
     "init": {
-        (">", ""): ("copy", (">", ""), (Direction.RIGHT, Direction.STAY))
+        (">", ""): ("copy", (">", ""), (Direction.R, Direction.S))
     },
     "copy": {
-        ("a", ""): ("copy", ("a", "a"), (Direction.RIGHT, Direction.RIGHT)),
-        ("b", ""): ("copy", ("b", "b"), (Direction.RIGHT, Direction.RIGHT)),
-        ("", ""): ("goToStart", ("", ""), (Direction.LEFT, Direction.STAY)),
+        ("a", ""): ("copy", ("a", "a"), (Direction.R, Direction.R)),
+        ("b", ""): ("copy", ("b", "b"), (Direction.R, Direction.R)),
+        ("", ""): ("goToStart", ("", ""), (Direction.L, Direction.S)),
     },
     "goToStart": {
-        ("a", ""): ("goToStart", ("a", ""), (Direction.LEFT, Direction.STAY)),
-        ("b", ""): ("goToStart", ("b", ""), (Direction.LEFT, Direction.STAY)),
-        (">", ""): ("check", (">", ""), (Direction.RIGHT, Direction.LEFT))
+        ("a", ""): ("goToStart", ("a", ""), (Direction.L, Direction.S)),
+        ("b", ""): ("goToStart", ("b", ""), (Direction.L, Direction.S)),
+        (">", ""): ("check", (">", ""), (Direction.R, Direction.L))
     },
     "check": {
-        ("a", "a"): ("check", ("a", "a"), (Direction.RIGHT, Direction.LEFT)),
-        ("b", "b"): ("check", ("b", "b"), (Direction.RIGHT, Direction.LEFT)),
-        ("", ""): ("accept", ("", ""), (Direction.STAY, Direction.STAY)),
-        ("a", "b"): ("reject", ("a", "b"), (Direction.STAY, Direction.STAY)),
-        ("b", "a"): ("reject", ("b", "a"), (Direction.STAY, Direction.STAY)),
+        ("a", "a"): ("check", ("a", "a"), (Direction.R, Direction.L)),
+        ("b", "b"): ("check", ("b", "b"), (Direction.R, Direction.L)),
+        ("", ""): ("accept", ("", ""), (Direction.S, Direction.S)),
+        ("a", "b"): ("reject", ("a", "b"), (Direction.S, Direction.S)),
+        ("b", "a"): ("reject", ("b", "a"), (Direction.S, Direction.S)),
     }
 }
 
 machine: MTM = MTM(
     states={"init", "goToEnd", "goToStart", "check", "accept", "reject"},
     initial_state="init",
     input_alphabet={"a", "b"},
-    acc_states={"accept"},
-    rej_states={"reject"},
+    acc_states="accept",
+    rej_states="reject",
     transitions=transitions)
 
 machine.write_to_tape("aabbabbaa")
 ```
 
 ### MTM Transition Function
 
@@ -553,26 +635,78 @@
 function: MTMransitions = {
     "init": {
         (">", ""): ("next", (">", "a"), (Direction.RIGHT, Direction.LEFT))
         }
 }
 ```
 
+MTM can also be loaded from a file. Format is shown below:
+
+```
+# name of the initial state
+init init
+
+# name of the accepting state
+acc acc
+
+# name of the rejecting state
+rej rej
+
+# alphabet characters without start_symbol
+alphabet a b c
+
+# the amount of tapes (>= 2)
+tapes 2
+
+---
+
+# current (reads) -> next [writes] [directions]([L(eft), R(ight), S(tay)])
+# ! _ (underscore) is used to depict <space> !
+# such spacing is not required
+init        (> _) -> copy         (> _) (R S)
+copy        (a _) -> copy         (a a) (R R)
+copy        (b _) -> copy         (b b) (R R)
+copy        (_ _) -> goToStart    (_ _) (L S)
+goToStart   (a _) -> goToStart    (a _) (L S)
+goToStart   (b _) -> goToStart    (b _) (L S)
+goToStart   (> _) -> check        (> _) (R L)
+check       (a a) -> check        (a a) (R L)
+check       (b b) -> check        (b b) (R L)
+check       (_ _) -> acc          (_ _) (S S)
+check       (a b) -> rej          (a b) (S S)
+check       (b a) -> rej          (b a) (S S)
+
+```
+
+The file above can then be simply loaded using the `load_dtm_from_file(...)`:
+
+```python
+from ib110hw.turing.utils import load_mtm_from_file
+
+machine = load_mtm_from_file("./mtm_file")
+```
+
 # DTM and MTM Simulation
 
 You can simulate the Turing machine using the provided function `simulate(...)`. By default, every step of the Turing machine will be printed to console with 0.5s delay in-between. This behavior can be changed by setting the `to_console` and `delay` parameters. If the parameter `to_console` is set to `False`, the delay will be ignored.
 
 ```python
 machine.simulate(to_console=True, delay=0.3) # True
 ```
 
+There is also an option to simulate the calculation step-by-step, i.e., the TM will wait for user input (arrow keys). It allows for going back and forward in the calculation. This can be enabled by setting the `step_by_step` parameter to `True`. The `delay` and `to_console` parameters are ignored.
+
+```python
+machine.simulate(step_by_step=True)
+```
+
 If you want to look at the whole history, you can set parameter `to_file` to `True`. Every step will be printed to file based on the path provided in the parameter `path`. Default path is set to `./simulation.md`.
 
 ```python
-turing.simulate(to_console=False, to_file=True, path="~/my_simulation.md") # True
+machine.simulate(to_console=False, to_file=True, path="~/my_simulation.md") 
 ```
 
 The `BaseTuringMachine` class contains the attribute `max_steps` to avoid infinite looping. By default, it is set to 100. The computation will stop if the simulation exceeds the value specified by this attribute. This can be an issue on larger inputs, so setting it to a bigger number may be needed.
 
 ```python
 turing.max_steps = 200
 ```
```

### Comparing `ib110hw-0.1.4/README.md` & `ib110hw-0.1.5/src/ib110hw.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: ib110hw
+Version: 0.1.5
+Summary: UNKNOWN
+Home-page: https://github.com/pilatmartin/ib110hw
+Author: Martin Pilát
+Author-email: 8pilatmartin8@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 This library was created for the course **IB110 - Introduction to Informatics** at [MUNI FI](https://www.fi.muni.cz/).
 
 # INSTALLATION
 
 Python version >=3.6 is required in order to use the library.
 Using virtual environment for installation is of course optional, but recommended.
 
@@ -377,15 +392,24 @@
 # this method either adds a transition, or overwrites the existing one
 # the difference compared to the DFA is that it takes a *set* of next states
 automaton.set_transition("s1", {"s2"}, "1")
 ```
 
 # TURING MACHINE
 
-This library supports **deterministic** and **multi-tape** Turing machines. You can find the implementation in the module `turing`.
+This library supports **deterministic** and **multi-tape** Turing machines. You can find the implementation in the module `turing`. Consider the class located in the base.py as abstract, its only purpose is to avoid duplicity in the implementation of these models.
+
+In order to create a Turing machine you will need to specify the seven-tuple `(Q, Σ, Γ, δ, q0, q_acc, q_rej)`, where:
+
+- The set of states `Q` is represented by `Set[str]`
+- The set of alphabet symbols `Σ` is represented by `Set[str]`
+- The transition function `δ` is represented by either `DTMTransitions` or `MTMTransitions`. These types are described below.
+- The initial state `q0` is represented by `str`
+- The accepting state `q_acc` is represented by `str`
+- The rejecting state `q_rej` is represented by `str`
 
 ## Tape
 
 The implementation of the tape for the Turing machine can be found in the file `tape.py`. The tape class is only used internally by the `DTM` and `MTM` objects - you will *probably* not use it directly.
 
 ```python
 from ib110hw.turing.tape import Tape
@@ -409,14 +433,31 @@
                     #           ^
 
 tape.clear()        # |   |
                     #   ^
 
 ```
 
+The module `tape` also contains enum for the direction of tape head:
+
+```python
+class Direction(Enum):
+    LEFT = -1
+    STAY = 0
+    RIGHT = 1
+    
+    # shorthand aliases
+    L = -1
+    S = 0
+    R = 1
+
+    def __repr__(self):
+        return self.name
+```
+
 ## Deterministic Turing Machine (DTM)
 
 The following DTM checks whether the input string is a palindrome:
 
 ```python
 from ib110hw.turing.dtm import DTM, DTMTransitions
 
@@ -458,16 +499,16 @@
         "X": ("mark", "X", Direction.RIGHT)
     }
 }
 
 machine: DTM = DTM(
     states={"init", "mark", "gotoEndA", "checkA", "gotoEndB", "checkB", "accept", "reject"},
     input_alphabet={"a", "b"},
-    acc_states={"accept"},
-    rej_states={"reject"},
+    acc_states="accept",
+    rej_states="reject",
     initial_state="init",
     transitions=transitions
 )
 
 machine.write_to_tape("aabbabbaa")
 ```
 
@@ -482,51 +523,107 @@
 function: DTMransitions = {
     "init": {
         ">": ("next", ">", Direction.RIGHT)
         }
 }
 ```
 
-# Multi-tape Turing Machine (MTM)
+### Loading From a File
+
+DTM can also be loaded from a file. Format is shown below:
+
+```
+# name of the initial state
+init init
+
+# name of the accepting state
+acc acc
+
+# name of the rejecting state
+rej rej
+
+# alphabet characters without start_symbol
+alphabet a b
+
+---
+
+# current read -> next write direction(L, R, S)
+# ! underscore (_) is used to depict <space> !
+init    > -> mark   > R
+mark    a -> foundA X R
+mark    b -> foundB X R
+mark    X -> acc    X S
+mark    _ -> acc    _ S
+foundA  a -> foundA a R
+foundA  b -> foundA b R
+foundA  X -> checkA X L
+foundA  _ -> checkA _ L
+checkA  a -> back   X L
+checkA  b -> acc    b S
+checkA  X -> rej    X S
+foundB  a -> foundB a R
+foundB  b -> foundB b R
+foundB  X -> checkB X L
+foundB  _ -> checkB _ L
+checkB  a -> reject a S
+checkB  b -> reject X L
+checkB  X -> reject X S
+back    a -> back   a L
+back    b -> back   b L
+back    X -> mark   X R
+
+```
+
+The file above can then be simply loaded using the `load_dtm_from_file(...)`:
+
+```python
+from ib110hw.turing.utils import load_dtm_from_file
+
+machine = load_dtm_from_file("./dtm_file")
+```
+
+## Multi-tape Turing Machine (MTM)
+
+On top of the properties required to create DTM, you will need to specify the number of tapes as well. The default tape count is set to 2.
 
 The following MTM has the same function as the DTM above:
 
 ```python
 from ib110hw.turing.mtm import MTM, MTMTransitions
 from ib110hw.turing.tape import Direction
 
 transitions: MTMTransitions = {
     "init": {
-        (">", ""): ("copy", (">", ""), (Direction.RIGHT, Direction.STAY))
+        (">", ""): ("copy", (">", ""), (Direction.R, Direction.S))
     },
     "copy": {
-        ("a", ""): ("copy", ("a", "a"), (Direction.RIGHT, Direction.RIGHT)),
-        ("b", ""): ("copy", ("b", "b"), (Direction.RIGHT, Direction.RIGHT)),
-        ("", ""): ("goToStart", ("", ""), (Direction.LEFT, Direction.STAY)),
+        ("a", ""): ("copy", ("a", "a"), (Direction.R, Direction.R)),
+        ("b", ""): ("copy", ("b", "b"), (Direction.R, Direction.R)),
+        ("", ""): ("goToStart", ("", ""), (Direction.L, Direction.S)),
     },
     "goToStart": {
-        ("a", ""): ("goToStart", ("a", ""), (Direction.LEFT, Direction.STAY)),
-        ("b", ""): ("goToStart", ("b", ""), (Direction.LEFT, Direction.STAY)),
-        (">", ""): ("check", (">", ""), (Direction.RIGHT, Direction.LEFT))
+        ("a", ""): ("goToStart", ("a", ""), (Direction.L, Direction.S)),
+        ("b", ""): ("goToStart", ("b", ""), (Direction.L, Direction.S)),
+        (">", ""): ("check", (">", ""), (Direction.R, Direction.L))
     },
     "check": {
-        ("a", "a"): ("check", ("a", "a"), (Direction.RIGHT, Direction.LEFT)),
-        ("b", "b"): ("check", ("b", "b"), (Direction.RIGHT, Direction.LEFT)),
-        ("", ""): ("accept", ("", ""), (Direction.STAY, Direction.STAY)),
-        ("a", "b"): ("reject", ("a", "b"), (Direction.STAY, Direction.STAY)),
-        ("b", "a"): ("reject", ("b", "a"), (Direction.STAY, Direction.STAY)),
+        ("a", "a"): ("check", ("a", "a"), (Direction.R, Direction.L)),
+        ("b", "b"): ("check", ("b", "b"), (Direction.R, Direction.L)),
+        ("", ""): ("accept", ("", ""), (Direction.S, Direction.S)),
+        ("a", "b"): ("reject", ("a", "b"), (Direction.S, Direction.S)),
+        ("b", "a"): ("reject", ("b", "a"), (Direction.S, Direction.S)),
     }
 }
 
 machine: MTM = MTM(
     states={"init", "goToEnd", "goToStart", "check", "accept", "reject"},
     initial_state="init",
     input_alphabet={"a", "b"},
-    acc_states={"accept"},
-    rej_states={"reject"},
+    acc_states="accept",
+    rej_states="reject",
     transitions=transitions)
 
 machine.write_to_tape("aabbabbaa")
 ```
 
 ### MTM Transition Function
 
@@ -538,32 +635,86 @@
 function: MTMransitions = {
     "init": {
         (">", ""): ("next", (">", "a"), (Direction.RIGHT, Direction.LEFT))
         }
 }
 ```
 
+MTM can also be loaded from a file. Format is shown below:
+
+```
+# name of the initial state
+init init
+
+# name of the accepting state
+acc acc
+
+# name of the rejecting state
+rej rej
+
+# alphabet characters without start_symbol
+alphabet a b c
+
+# the amount of tapes (>= 2)
+tapes 2
+
+---
+
+# current (reads) -> next [writes] [directions]([L(eft), R(ight), S(tay)])
+# ! _ (underscore) is used to depict <space> !
+# such spacing is not required
+init        (> _) -> copy         (> _) (R S)
+copy        (a _) -> copy         (a a) (R R)
+copy        (b _) -> copy         (b b) (R R)
+copy        (_ _) -> goToStart    (_ _) (L S)
+goToStart   (a _) -> goToStart    (a _) (L S)
+goToStart   (b _) -> goToStart    (b _) (L S)
+goToStart   (> _) -> check        (> _) (R L)
+check       (a a) -> check        (a a) (R L)
+check       (b b) -> check        (b b) (R L)
+check       (_ _) -> acc          (_ _) (S S)
+check       (a b) -> rej          (a b) (S S)
+check       (b a) -> rej          (b a) (S S)
+
+```
+
+The file above can then be simply loaded using the `load_dtm_from_file(...)`:
+
+```python
+from ib110hw.turing.utils import load_mtm_from_file
+
+machine = load_mtm_from_file("./mtm_file")
+```
+
 # DTM and MTM Simulation
 
 You can simulate the Turing machine using the provided function `simulate(...)`. By default, every step of the Turing machine will be printed to console with 0.5s delay in-between. This behavior can be changed by setting the `to_console` and `delay` parameters. If the parameter `to_console` is set to `False`, the delay will be ignored.
 
 ```python
 machine.simulate(to_console=True, delay=0.3) # True
 ```
 
+There is also an option to simulate the calculation step-by-step, i.e., the TM will wait for user input (arrow keys). It allows for going back and forward in the calculation. This can be enabled by setting the `step_by_step` parameter to `True`. The `delay` and `to_console` parameters are ignored.
+
+```python
+machine.simulate(step_by_step=True)
+```
+
 If you want to look at the whole history, you can set parameter `to_file` to `True`. Every step will be printed to file based on the path provided in the parameter `path`. Default path is set to `./simulation.md`.
 
 ```python
-turing.simulate(to_console=False, to_file=True, path="~/my_simulation.md") # True
+machine.simulate(to_console=False, to_file=True, path="~/my_simulation.md") 
 ```
 
 The `BaseTuringMachine` class contains the attribute `max_steps` to avoid infinite looping. By default, it is set to 100. The computation will stop if the simulation exceeds the value specified by this attribute. This can be an issue on larger inputs, so setting it to a bigger number may be needed.
 
 ```python
 turing.max_steps = 200
 ```
 
 ### Simulation in PyCharm
 
 For the optimal visualization of the simulation in PyCharm you need to **enable** the `Terminal emulation`.
 
 You can do so by going to `Run > Edit configurations ...` and then checking the `Emulate terminal in output console` box.
+
+
```

### Comparing `ib110hw-0.1.4/setup.py` & `ib110hw-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ib110hw",
-    version="0.1.4",
+    version="0.1.5",
     author="Martin Pilát",
     author_email="8pilatmartin8@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    install_requires=[
+        "pynput",
+    ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     url="https://github.com/pilatmartin/ib110hw",
 )
```

### Comparing `ib110hw-0.1.4/src/ib110hw/automaton/base.py` & `ib110hw-0.1.5/src/ib110hw/automaton/base.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.4/src/ib110hw/automaton/dfa.py` & `ib110hw-0.1.5/src/ib110hw/automaton/dfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.4/src/ib110hw/automaton/nfa.py` & `ib110hw-0.1.5/src/ib110hw/automaton/nfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.4/src/ib110hw/automaton/utils.py` & `ib110hw-0.1.5/src/ib110hw/automaton/utils.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.4/src/ib110hw/turing/base.py` & `ib110hw-0.1.5/src/ib110hw/turing/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
         return object.__new__(cls)
 
     def __init__(
         self,
         states: Set[str],
         input_alphabet: Set[str],
-        acc_states: Set[str],
-        rej_states: Set[str],
+        acc_state: str = "accept",
+        rej_state: str = "reject",
         initial_state: str = "init",
         start_symbol: str = ">",
     ) -> None:
         self.states = states or set()
         self.input_alphabet = input_alphabet or set()
-        self.acc_states = acc_states or set()
-        self.rej_states = rej_states or set()
+        self.acc_state = acc_state
+        self.rej_state = rej_state
         self.initial_state = initial_state
         self.start_symbol = start_symbol
 
         # After exceeding max_steps value, the turing machine will be considered as looping.
         # Change this value for more complex scenarios.
         self.max_steps = 100
```

### Comparing `ib110hw-0.1.4/src/ib110hw/turing/tape.py` & `ib110hw-0.1.5/src/ib110hw/turing/tape.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 
 
 class Direction(Enum):
     LEFT = -1
     STAY = 0
     RIGHT = 1
 
+    # shorthand aliases
+    L = -1
+    S = 0
+    R = 1
+
     def __repr__(self):
         return self.name
 
 
 class Cell:
     """Represents one cell of a Turing machine memory tape."""
```

### Comparing `ib110hw-0.1.4/src/ib110hw/turing/utils.py` & `ib110hw-0.1.5/src/ib110hw/turing/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,86 @@
-from .dtm import DTM
-from ._helpers import (
+from dtm import DTM
+from mtm import MTM
+from _helpers import (
     read_file,
-    get_configuration,
+    get_dtm_configuration,
+    get_mtm_configuration,
     get_dtm_transition_function,
-    validate_configuration,
+    validate_dtm_configuration,
+    validate_mtm_configuration,
     validate_dtm_transitions,
+    validate_mtm_transitions,
+    get_mtm_transition_function,
 )
 from typing import Optional
 from sys import stderr
 
 
 def load_dtm_from_file(file_path: str) -> Optional[DTM]:
     """
     Loads a DTM from a file if it is valid.
     Returns None if the configuration is invalid and prints the error to stderr.
 
     Args:
         file_path (str): Path to the file with configuration.
 
     Returns:
-        Optional[DTM]: DTM if configuratin is valid, None otherwise.
+        Optional[DTM]: DTM if the configuration is valid, None otherwise.
     """
     definition = read_file(file_path)
 
-    config_err = validate_configuration(definition)
+    config_err = validate_dtm_configuration(definition)
     transitions_err = validate_dtm_transitions(definition)
     if config_err or transitions_err:
         print(config_err or transitions_err, file=stderr)
         return None
 
-    init, acc, rej, abc = get_configuration(definition)
+    init, acc, rej, abc = get_dtm_configuration(definition)
     transitions = get_dtm_transition_function(definition)
 
     return DTM(
         states={*transitions.keys()},
         input_alphabet=abc,
-        acc_states=acc,
+        acc_state=acc,
+        rej_state=rej,
         initial_state=init,
-        rej_states=rej,
+        transitions=transitions,
+    )
+
+
+def load_mtm_from_file(file_path: str) -> Optional[MTM]:
+    """
+    Loads a MTM from a file if it is valid.
+    Returns None if the configuration is invalid and prints the error to stderr.
+
+    Args:
+        file_path (str): Path to the file with configuration.
+
+    Returns:
+        Optional[MTM]: MTM if the configuration is valid, None otherwise.
+    """
+    definition = read_file(file_path)
+
+    config_err = validate_mtm_configuration(definition)
+    transitions_err = validate_mtm_transitions(definition)
+    if config_err or transitions_err:
+        print(config_err or transitions_err, file=stderr)
+        return None
+
+    init, acc, rej, abc, tape_count = get_mtm_configuration(definition)
+    transitions = get_mtm_transition_function(definition)
+
+    return MTM(
+        states={*transitions.keys()},
+        input_alphabet=abc,
+        acc_state=acc,
+        rej_state=rej,
+        initial_state=init,
+        tape_count=tape_count,
         transitions=transitions,
     )
 
 
 if __name__ == "__main__":
-    pass
+    machine = load_dtm_from_file("./test.txt")
+    machine.write_to_tape("abbabba")
+    machine.simulate(step_by_step=True)
```

### Comparing `ib110hw-0.1.4/src/ib110hw.egg-info/PKG-INFO` & `ib110hw-0.1.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: ib110hw
-Version: 0.1.4
-Summary: UNKNOWN
-Home-page: https://github.com/pilatmartin/ib110hw
-Author: Martin Pilát
-Author-email: 8pilatmartin8@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 This library was created for the course **IB110 - Introduction to Informatics** at [MUNI FI](https://www.fi.muni.cz/).
 
 # INSTALLATION
 
 Python version >=3.6 is required in order to use the library.
 Using virtual environment for installation is of course optional, but recommended.
 
@@ -392,15 +377,24 @@
 # this method either adds a transition, or overwrites the existing one
 # the difference compared to the DFA is that it takes a *set* of next states
 automaton.set_transition("s1", {"s2"}, "1")
 ```
 
 # TURING MACHINE
 
-This library supports **deterministic** and **multi-tape** Turing machines. You can find the implementation in the module `turing`.
+This library supports **deterministic** and **multi-tape** Turing machines. You can find the implementation in the module `turing`. Consider the class located in the base.py as abstract, its only purpose is to avoid duplicity in the implementation of these models.
+
+In order to create a Turing machine you will need to specify the seven-tuple `(Q, Σ, Γ, δ, q0, q_acc, q_rej)`, where:
+
+- The set of states `Q` is represented by `Set[str]`
+- The set of alphabet symbols `Σ` is represented by `Set[str]`
+- The transition function `δ` is represented by either `DTMTransitions` or `MTMTransitions`. These types are described below.
+- The initial state `q0` is represented by `str`
+- The accepting state `q_acc` is represented by `str`
+- The rejecting state `q_rej` is represented by `str`
 
 ## Tape
 
 The implementation of the tape for the Turing machine can be found in the file `tape.py`. The tape class is only used internally by the `DTM` and `MTM` objects - you will *probably* not use it directly.
 
 ```python
 from ib110hw.turing.tape import Tape
@@ -424,14 +418,31 @@
                     #           ^
 
 tape.clear()        # |   |
                     #   ^
 
 ```
 
+The module `tape` also contains enum for the direction of tape head:
+
+```python
+class Direction(Enum):
+    LEFT = -1
+    STAY = 0
+    RIGHT = 1
+    
+    # shorthand aliases
+    L = -1
+    S = 0
+    R = 1
+
+    def __repr__(self):
+        return self.name
+```
+
 ## Deterministic Turing Machine (DTM)
 
 The following DTM checks whether the input string is a palindrome:
 
 ```python
 from ib110hw.turing.dtm import DTM, DTMTransitions
 
@@ -473,16 +484,16 @@
         "X": ("mark", "X", Direction.RIGHT)
     }
 }
 
 machine: DTM = DTM(
     states={"init", "mark", "gotoEndA", "checkA", "gotoEndB", "checkB", "accept", "reject"},
     input_alphabet={"a", "b"},
-    acc_states={"accept"},
-    rej_states={"reject"},
+    acc_states="accept",
+    rej_states="reject",
     initial_state="init",
     transitions=transitions
 )
 
 machine.write_to_tape("aabbabbaa")
 ```
 
@@ -497,51 +508,107 @@
 function: DTMransitions = {
     "init": {
         ">": ("next", ">", Direction.RIGHT)
         }
 }
 ```
 
-# Multi-tape Turing Machine (MTM)
+### Loading From a File
+
+DTM can also be loaded from a file. Format is shown below:
+
+```
+# name of the initial state
+init init
+
+# name of the accepting state
+acc acc
+
+# name of the rejecting state
+rej rej
+
+# alphabet characters without start_symbol
+alphabet a b
+
+---
+
+# current read -> next write direction(L, R, S)
+# ! underscore (_) is used to depict <space> !
+init    > -> mark   > R
+mark    a -> foundA X R
+mark    b -> foundB X R
+mark    X -> acc    X S
+mark    _ -> acc    _ S
+foundA  a -> foundA a R
+foundA  b -> foundA b R
+foundA  X -> checkA X L
+foundA  _ -> checkA _ L
+checkA  a -> back   X L
+checkA  b -> acc    b S
+checkA  X -> rej    X S
+foundB  a -> foundB a R
+foundB  b -> foundB b R
+foundB  X -> checkB X L
+foundB  _ -> checkB _ L
+checkB  a -> reject a S
+checkB  b -> reject X L
+checkB  X -> reject X S
+back    a -> back   a L
+back    b -> back   b L
+back    X -> mark   X R
+
+```
+
+The file above can then be simply loaded using the `load_dtm_from_file(...)`:
+
+```python
+from ib110hw.turing.utils import load_dtm_from_file
+
+machine = load_dtm_from_file("./dtm_file")
+```
+
+## Multi-tape Turing Machine (MTM)
+
+On top of the properties required to create DTM, you will need to specify the number of tapes as well. The default tape count is set to 2.
 
 The following MTM has the same function as the DTM above:
 
 ```python
 from ib110hw.turing.mtm import MTM, MTMTransitions
 from ib110hw.turing.tape import Direction
 
 transitions: MTMTransitions = {
     "init": {
-        (">", ""): ("copy", (">", ""), (Direction.RIGHT, Direction.STAY))
+        (">", ""): ("copy", (">", ""), (Direction.R, Direction.S))
     },
     "copy": {
-        ("a", ""): ("copy", ("a", "a"), (Direction.RIGHT, Direction.RIGHT)),
-        ("b", ""): ("copy", ("b", "b"), (Direction.RIGHT, Direction.RIGHT)),
-        ("", ""): ("goToStart", ("", ""), (Direction.LEFT, Direction.STAY)),
+        ("a", ""): ("copy", ("a", "a"), (Direction.R, Direction.R)),
+        ("b", ""): ("copy", ("b", "b"), (Direction.R, Direction.R)),
+        ("", ""): ("goToStart", ("", ""), (Direction.L, Direction.S)),
     },
     "goToStart": {
-        ("a", ""): ("goToStart", ("a", ""), (Direction.LEFT, Direction.STAY)),
-        ("b", ""): ("goToStart", ("b", ""), (Direction.LEFT, Direction.STAY)),
-        (">", ""): ("check", (">", ""), (Direction.RIGHT, Direction.LEFT))
+        ("a", ""): ("goToStart", ("a", ""), (Direction.L, Direction.S)),
+        ("b", ""): ("goToStart", ("b", ""), (Direction.L, Direction.S)),
+        (">", ""): ("check", (">", ""), (Direction.R, Direction.L))
     },
     "check": {
-        ("a", "a"): ("check", ("a", "a"), (Direction.RIGHT, Direction.LEFT)),
-        ("b", "b"): ("check", ("b", "b"), (Direction.RIGHT, Direction.LEFT)),
-        ("", ""): ("accept", ("", ""), (Direction.STAY, Direction.STAY)),
-        ("a", "b"): ("reject", ("a", "b"), (Direction.STAY, Direction.STAY)),
-        ("b", "a"): ("reject", ("b", "a"), (Direction.STAY, Direction.STAY)),
+        ("a", "a"): ("check", ("a", "a"), (Direction.R, Direction.L)),
+        ("b", "b"): ("check", ("b", "b"), (Direction.R, Direction.L)),
+        ("", ""): ("accept", ("", ""), (Direction.S, Direction.S)),
+        ("a", "b"): ("reject", ("a", "b"), (Direction.S, Direction.S)),
+        ("b", "a"): ("reject", ("b", "a"), (Direction.S, Direction.S)),
     }
 }
 
 machine: MTM = MTM(
     states={"init", "goToEnd", "goToStart", "check", "accept", "reject"},
     initial_state="init",
     input_alphabet={"a", "b"},
-    acc_states={"accept"},
-    rej_states={"reject"},
+    acc_states="accept",
+    rej_states="reject",
     transitions=transitions)
 
 machine.write_to_tape("aabbabbaa")
 ```
 
 ### MTM Transition Function
 
@@ -553,34 +620,84 @@
 function: MTMransitions = {
     "init": {
         (">", ""): ("next", (">", "a"), (Direction.RIGHT, Direction.LEFT))
         }
 }
 ```
 
+MTM can also be loaded from a file. Format is shown below:
+
+```
+# name of the initial state
+init init
+
+# name of the accepting state
+acc acc
+
+# name of the rejecting state
+rej rej
+
+# alphabet characters without start_symbol
+alphabet a b c
+
+# the amount of tapes (>= 2)
+tapes 2
+
+---
+
+# current (reads) -> next [writes] [directions]([L(eft), R(ight), S(tay)])
+# ! _ (underscore) is used to depict <space> !
+# such spacing is not required
+init        (> _) -> copy         (> _) (R S)
+copy        (a _) -> copy         (a a) (R R)
+copy        (b _) -> copy         (b b) (R R)
+copy        (_ _) -> goToStart    (_ _) (L S)
+goToStart   (a _) -> goToStart    (a _) (L S)
+goToStart   (b _) -> goToStart    (b _) (L S)
+goToStart   (> _) -> check        (> _) (R L)
+check       (a a) -> check        (a a) (R L)
+check       (b b) -> check        (b b) (R L)
+check       (_ _) -> acc          (_ _) (S S)
+check       (a b) -> rej          (a b) (S S)
+check       (b a) -> rej          (b a) (S S)
+
+```
+
+The file above can then be simply loaded using the `load_dtm_from_file(...)`:
+
+```python
+from ib110hw.turing.utils import load_mtm_from_file
+
+machine = load_mtm_from_file("./mtm_file")
+```
+
 # DTM and MTM Simulation
 
 You can simulate the Turing machine using the provided function `simulate(...)`. By default, every step of the Turing machine will be printed to console with 0.5s delay in-between. This behavior can be changed by setting the `to_console` and `delay` parameters. If the parameter `to_console` is set to `False`, the delay will be ignored.
 
 ```python
 machine.simulate(to_console=True, delay=0.3) # True
 ```
 
+There is also an option to simulate the calculation step-by-step, i.e., the TM will wait for user input (arrow keys). It allows for going back and forward in the calculation. This can be enabled by setting the `step_by_step` parameter to `True`. The `delay` and `to_console` parameters are ignored.
+
+```python
+machine.simulate(step_by_step=True)
+```
+
 If you want to look at the whole history, you can set parameter `to_file` to `True`. Every step will be printed to file based on the path provided in the parameter `path`. Default path is set to `./simulation.md`.
 
 ```python
-turing.simulate(to_console=False, to_file=True, path="~/my_simulation.md") # True
+machine.simulate(to_console=False, to_file=True, path="~/my_simulation.md") 
 ```
 
 The `BaseTuringMachine` class contains the attribute `max_steps` to avoid infinite looping. By default, it is set to 100. The computation will stop if the simulation exceeds the value specified by this attribute. This can be an issue on larger inputs, so setting it to a bigger number may be needed.
 
 ```python
 turing.max_steps = 200
 ```
 
 ### Simulation in PyCharm
 
 For the optimal visualization of the simulation in PyCharm you need to **enable** the `Terminal emulation`.
 
 You can do so by going to `Run > Edit configurations ...` and then checking the `Emulate terminal in output console` box.
-
-
```

### Comparing `ib110hw-0.1.4/src/ib110hw.egg-info/SOURCES.txt` & `ib110hw-0.1.5/src/ib110hw.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 LICENSE
 README.md
 setup.py
 src/ib110hw/__init__.py
 src/ib110hw.egg-info/PKG-INFO
 src/ib110hw.egg-info/SOURCES.txt
 src/ib110hw.egg-info/dependency_links.txt
+src/ib110hw.egg-info/requires.txt
 src/ib110hw.egg-info/top_level.txt
 src/ib110hw/automaton/__init__.py
 src/ib110hw/automaton/base.py
 src/ib110hw/automaton/dfa.py
 src/ib110hw/automaton/nfa.py
 src/ib110hw/automaton/utils.py
 src/ib110hw/turing/__init__.py
 src/ib110hw/turing/_helpers.py
 src/ib110hw/turing/base.py
 src/ib110hw/turing/dtm.py
+src/ib110hw/turing/idk.py
 src/ib110hw/turing/mtm.py
 src/ib110hw/turing/tape.py
 src/ib110hw/turing/utils.py
 tests/test_dfa.py
 tests/test_dtm.py
 tests/test_mtm.py
 tests/test_nfa.py
```

### Comparing `ib110hw-0.1.4/tests/test_dfa.py` & `ib110hw-0.1.5/tests/test_dfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.4/tests/test_dtm.py` & `ib110hw-0.1.5/tests/test_dtm.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         "checkA",
         "gotoEndB",
         "checkB",
         "accept",
         "reject",
     },
     input_alphabet={"a", "b"},
-    acc_states={"accept"},
-    rej_states={"reject"},
+    acc_state="accept",
+    rej_state="reject",
     initial_state="init",
     transitions={
         "init": {
             ">": ("mark", ">", Direction.RIGHT),
         },
         "mark": {
             "a": ("foundA", "X", Direction.RIGHT),
```

### Comparing `ib110hw-0.1.4/tests/test_mtm.py` & `ib110hw-0.1.5/tests/test_mtm.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from turing.tape import Direction
 
 
 PALINDROME_MACHINE: MTM = MTM(
     states={"init", "goToEnd", "goToStart", "check", "accept", "reject"},
     initial_state="init",
     input_alphabet={"a", "b"},
-    acc_states={"accept"},
-    rej_states={"reject"},
+    acc_state="accept",
+    rej_state="reject",
     transitions={
         "init": {(">", ""): ("copy", (">", ""), (Direction.RIGHT, Direction.STAY))},
         "copy": {
             ("a", ""): ("copy", ("a", "a"), (Direction.RIGHT, Direction.RIGHT)),
             ("b", ""): ("copy", ("b", "b"), (Direction.RIGHT, Direction.RIGHT)),
             ("", ""): ("goToStart", ("", ""), (Direction.LEFT, Direction.STAY)),
         },
```

### Comparing `ib110hw-0.1.4/tests/test_nfa.py` & `ib110hw-0.1.5/tests/test_nfa.py`

 * *Files identical despite different names*

