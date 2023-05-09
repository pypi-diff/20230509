# Comparing `tmp/asdm-0.0.2.tar.gz` & `tmp/asdm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\stammm\Documents\Development\APIs\ASDM\dist\.tmp-qpgi0wgz\asdm-0.0.2.tar", last modified: Tue May  9 13:00:30 2023, max compression
+gzip compressed data, was "C:\Users\stammm\Documents\Development\APIs\ASDM\dist\.tmp-bka79tw5\asdm-0.0.3.tar", last modified: Tue May  9 13:35:32 2023, max compression
```

## Comparing `asdm-0.0.2.tar` & `asdm-0.0.3.tar`

### file list

```diff
@@ -1,140 +1,135 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:30.501308 asdm-0.0.2/
--rw-rw-rw-   0        0        0     2510 2023-05-09 12:46:45.000000 asdm-0.0.2/.gitignore
--rw-rw-rw-   0        0        0   221649 2023-05-09 12:51:57.000000 asdm-0.0.2/1-SD_modelling.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:29.783754 asdm-0.0.2/ASDM/
--rw-rw-rw-   0        0        0   104145 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/ASDM.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:29.803755 asdm-0.0.2/ASDM/Diagrams/
--rw-rw-rw-   0        0        0    81560 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/Diagrams/ASDM.excalidraw
--rw-rw-rw-   0        0        0    18071 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/Diagrams/EngineOOP.excalidraw
--rw-rw-rw-   0        0        0   100587 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/Diagrams/Parser1.png
--rw-rw-rw-   0        0        0   259595 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/Diagrams/Parser2.png
--rw-rw-rw-   0        0        0     8887 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/MCMC.py
--rw-rw-rw-   0        0        0     4486 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/Optimizer.py
--rw-rw-rw-   0        0        0    36629 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/Parser.excalidraw
--rw-rw-rw-   0        0        0      505 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/Parser_XMILE.py
--rw-rw-rw-   0        0        0     2313 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/Payoff.py
--rw-rw-rw-   0        0        0     3727 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/Probability.py
--rw-rw-rw-   0        0        0      616 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/SpeedComparison.py
--rw-rw-rw-   0        0        0     2349 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/Utilities.py
--rw-rw-rw-   0        0        0       21 2023-05-09 12:58:02.000000 asdm-0.0.2/ASDM/__init__.py
--rw-rw-rw-   0        0        0     3178 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/test_Behaviour.py
--rw-rw-rw-   0        0        0     3535 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/test_Engine.py
--rw-rw-rw-   0        0        0      796 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/test_MultipleRuns.py
--rw-rw-rw-   0        0        0     2417 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/test_Parser.py
--rw-rw-rw-   0        0        0     2328 2023-04-16 16:50:21.000000 asdm-0.0.2/ASDM/test_Solver.py
--rw-rw-rw-   0        0        0       79 2023-04-16 16:07:35.000000 asdm-0.0.2/ASDM.code-workspace
--rw-rw-rw-   0        0        0     1082 2023-04-16 16:07:35.000000 asdm-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5707 2023-05-09 13:00:30.500313 asdm-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      568 2023-05-09 12:47:38.000000 asdm-0.0.2/Pipfile
--rw-rw-rw-   0        0        0   140652 2023-05-09 12:48:22.000000 asdm-0.0.2/Pipfile.lock
--rw-rw-rw-   0        0        0     4065 2023-05-09 12:46:45.000000 asdm-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:29.676753 asdm-0.0.2/apps/
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:29.853755 asdm-0.0.2/apps/ERM/
--rw-rw-rw-   0        0        0    43567 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/ERM/3-From_XMILE.ipynb
--rw-rw-rw-   0        0        0     2173 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/ERM/ERM_ASDM_app.py
--rw-rw-rw-   0        0        0    64961 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/ERM/Elective Recovery Model.stmx
--rw-rw-rw-   0        0        0   255859 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/ERM/Elective Recovery Model.xlsx
--rw-rw-rw-   0        0        0   118770 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/ERM/Elective_Recovery_Model.PNG
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:29.885755 asdm-0.0.2/apps/Goal_Gap/
--rw-rw-rw-   0        0        0    11354 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Goal_Gap/Goal_gap_model.png
--rw-rw-rw-   0        0        0     3570 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Goal_Gap/Revised_Goal_Gap.py
--rw-rw-rw-   0        0        0    16090 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Goal_Gap/Revised_Goal_Gap.stmx
--rw-rw-rw-   0        0        0      911 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Goal_Gap/goal_gap.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:29.892756 asdm-0.0.2/apps/Smoking_Cessation/
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:29.933757 asdm-0.0.2/apps/Smoking_Cessation/ASDM/
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:29.941758 asdm-0.0.2/apps/Smoking_Cessation/ASDM/Diagrams/
--rw-rw-rw-   0        0        0    81560 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Smoking_Cessation/ASDM/Diagrams/ASDM.excalidraw
--rw-rw-rw-   0        0        0    85788 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Smoking_Cessation/ASDM/Engine.py
--rw-rw-rw-   0        0        0     8856 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Smoking_Cessation/ASDM/MCMC.py
--rw-rw-rw-   0        0        0     4486 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Smoking_Cessation/ASDM/Optimizer.py
--rw-rw-rw-   0        0        0      505 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Smoking_Cessation/ASDM/Parser_XMILE.py
--rw-rw-rw-   0        0        0     2313 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Smoking_Cessation/ASDM/Payoff.py
--rw-rw-rw-   0        0        0     3727 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Smoking_Cessation/ASDM/Probability.py
--rw-rw-rw-   0        0        0     2349 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Smoking_Cessation/ASDM/Utilities.py
--rw-rw-rw-   0        0        0        0 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Smoking_Cessation/ASDM/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-05-09 12:46:45.000000 asdm-0.0.2/apps/Smoking_Cessation/smoking_cessation.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:29.976760 asdm-0.0.2/asdm.egg-info/
--rw-rw-rw-   0        0        0     5707 2023-05-09 13:00:29.000000 asdm-0.0.2/asdm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4712 2023-05-09 13:00:29.000000 asdm-0.0.2/asdm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 13:00:29.000000 asdm-0.0.2/asdm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      414 2023-05-09 13:00:29.000000 asdm-0.0.2/asdm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-09 13:00:29.000000 asdm-0.0.2/asdm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:29.679751 asdm-0.0.2/assets/
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:29.986761 asdm-0.0.2/assets/images/
--rw-rw-rw-   0        0        0    11354 2023-05-09 12:46:45.000000 asdm-0.0.2/assets/images/Goal_gap_model.png
--rw-rw-rw-   0        0        0     7502 2023-05-09 12:46:45.000000 asdm-0.0.2/assets/images/Infection_model.png
--rw-rw-rw-   0        0        0    63503 2023-05-09 12:46:45.000000 asdm-0.0.2/assets/images/Simplified_patient_flow_model.png
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:30.014758 asdm-0.0.2/notebooks/
--rw-rw-rw-   0        0        0     3294 2023-05-09 12:46:45.000000 asdm-0.0.2/notebooks/0-Performance_comparison.ipynb
--rw-rw-rw-   0        0        0   404613 2023-05-09 12:46:45.000000 asdm-0.0.2/notebooks/2-SD_model_calibration.ipynb
--rw-rw-rw-   0        0        0    74650 2023-05-09 12:46:45.000000 asdm-0.0.2/notebooks/ValidateOutcome.ipynb
--rw-rw-rw-   0        0        0     1292 2023-05-09 12:57:52.000000 asdm-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     6474 2023-05-09 12:46:45.000000 asdm-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 13:00:30.501308 asdm-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-04-16 16:50:21.000000 asdm-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:30.042760 asdm-0.0.2/tests/
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:30.313763 asdm-0.0.2/tests/BuiltInTestModels/
--rw-rw-rw-   0        0        0    14838 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Array_cross_reference.stmx
--rw-rw-rw-   0        0        0    14475 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Array_cross_reference_inference.stmx
--rw-rw-rw-   0        0        0    13368 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Array_parallel_reference.stmx
--rw-rw-rw-   0        0        0    13213 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Basic_math.stmx
--rw-rw-rw-   0        0        0    12870 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Built_in_vars.stmx
--rw-rw-rw-   0        0        0    15020 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Conveyor.stmx
--rw-rw-rw-   0        0        0    15841 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Conveyor_initialisation.stmx
--rw-rw-rw-   0        0        0    15841 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Conveyor_leakage.stmx
--rw-rw-rw-   0        0        0    18784 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Conveyor_leakage1.stmx
--rw-rw-rw-   0        0        0    18280 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Conveyor_leakage2.stmx
--rw-rw-rw-   0        0        0    15999 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Delays.stmx
--rw-rw-rw-   0        0        0    14193 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Delays2.stmx
--rw-rw-rw-   0        0        0    13767 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Goal_gap.stmx
--rw-rw-rw-   0        0        0    14512 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Goal_gap_array.stmx
--rw-rw-rw-   0        0        0    14119 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Graph_function.stmx
--rw-rw-rw-   0        0        0    13920 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/History.stmx
--rw-rw-rw-   0        0        0    13246 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/IF_THEN_ELSE.stmx
--rw-rw-rw-   0        0        0    13222 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/INIT.stmx
--rw-rw-rw-   0        0        0    12865 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Isolated_var.stmx
--rw-rw-rw-   0        0        0    14306 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/LOOKUP.stmx
--rw-rw-rw-   0        0        0    14013 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Logic.stmx
--rw-rw-rw-   0        0        0    16221 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/MOD.stmx
--rw-rw-rw-   0        0        0    15257 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/MOD_arrayed.stmx
--rw-rw-rw-   0        0        0    13528 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Min_Max.stmx
--rw-rw-rw-   0        0        0    18132 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Modules.stmx
--rw-rw-rw-   0        0        0    14466 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Non-negative_stocks.stmx
--rw-rw-rw-   0        0        0    19817 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Non-negative_stocks_with_flows.stmx
--rw-rw-rw-   0        0        0    20825 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Smooth.stmx
-drwxrwxrwx   0        0        0        0 2023-05-09 13:00:30.498310 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/
--rw-rw-rw-   0        0        0      615 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Array_cross_reference.csv
--rw-rw-rw-   0        0        0      329 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Array_cross_reference_inference.csv
--rw-rw-rw-   0        0        0      133 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Array_parallel_reference.csv
--rw-rw-rw-   0        0        0      101 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Basic_math.csv
--rw-rw-rw-   0        0        0       77 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Built_in_vars.csv
--rw-rw-rw-   0        0        0      318 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Conveyor.csv
--rw-rw-rw-   0        0        0      434 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Conveyor_initialisation.csv
--rw-rw-rw-   0        0        0     1677 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Conveyor_leakage.csv
--rw-rw-rw-   0        0        0      903 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Conveyor_leakage1.csv
--rw-rw-rw-   0        0        0     1024 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Conveyor_leakage2.csv
--rw-rw-rw-   0        0        0      518 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Delays.csv
--rw-rw-rw-   0        0        0       95 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Delays2.csv
--rw-rw-rw-   0        0        0     1619 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Goal_gap.csv
--rw-rw-rw-   0        0        0     3920 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Goal_gap_array.csv
--rw-rw-rw-   0        0        0      539 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Graph_function.csv
--rw-rw-rw-   0        0        0      129 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/History.csv
--rw-rw-rw-   0        0        0      139 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/IF_THEN_ELSE.csv
--rw-rw-rw-   0        0        0      623 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/INIT.csv
--rw-rw-rw-   0        0        0       23 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Isolated_var.csv
--rw-rw-rw-   0        0        0      578 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/LOOKUP.csv
--rw-rw-rw-   0        0        0      198 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Logic.csv
--rw-rw-rw-   0        0        0     1196 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/MOD.csv
--rw-rw-rw-   0        0        0      397 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/MOD_arrayed.csv
--rw-rw-rw-   0        0        0      840 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Min_Max.csv
--rw-rw-rw-   0        0        0      154 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Modules.csv
--rw-rw-rw-   0        0        0      129 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Non-negative_stocks.csv
--rw-rw-rw-   0        0        0      570 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Non-negative_stocks_with_flows.csv
--rw-rw-rw-   0        0        0     3842 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Smooth.csv
--rw-rw-rw-   0        0        0      111 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Time_related_functions.csv
--rw-rw-rw-   0        0        0       75 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Time_unit.csv
--rw-rw-rw-   0        0        0    15665 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Time_related_functions.stmx
--rw-rw-rw-   0        0        0    12864 2023-05-09 12:46:45.000000 asdm-0.0.2/tests/BuiltInTestModels/Time_unit.stmx
--rw-rw-rw-   0        0        0      208 2023-04-16 16:07:35.000000 asdm-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     3101 2023-04-16 16:50:21.000000 asdm-0.0.2/tests/run_tests.py
--rw-rw-rw-   0        0        0     2262 2023-04-16 16:07:35.000000 asdm-0.0.2/tests/test_goal_gap_model.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.892359 asdm-0.0.3/
+-rw-rw-rw-   0        0        0     2151 2023-05-09 13:32:07.000000 asdm-0.0.3/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.621353 asdm-0.0.3/ASDM/
+-rw-rw-rw-   0        0        0   106858 2023-05-09 13:32:07.000000 asdm-0.0.3/ASDM/ASDM.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.633351 asdm-0.0.3/ASDM/Diagrams/
+-rw-rw-rw-   0        0        0    81560 2023-05-09 13:20:53.000000 asdm-0.0.3/ASDM/Diagrams/ASDM.excalidraw
+-rw-rw-rw-   0        0        0    18071 2023-05-09 13:20:53.000000 asdm-0.0.3/ASDM/Diagrams/EngineOOP.excalidraw
+-rw-rw-rw-   0        0        0    36629 2023-05-09 13:32:07.000000 asdm-0.0.3/ASDM/Diagrams/Parser.excalidraw
+-rw-rw-rw-   0        0        0   100587 2023-05-09 13:20:53.000000 asdm-0.0.3/ASDM/Diagrams/Parser1.png
+-rw-rw-rw-   0        0        0   259595 2023-05-09 13:20:53.000000 asdm-0.0.3/ASDM/Diagrams/Parser2.png
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.659351 asdm-0.0.3/ASDM/Inference/
+-rw-rw-rw-   0        0        0     8887 2023-05-09 13:32:07.000000 asdm-0.0.3/ASDM/Inference/MCMC.py
+-rw-rw-rw-   0        0        0     4486 2023-05-09 13:32:07.000000 asdm-0.0.3/ASDM/Inference/Optimizer.py
+-rw-rw-rw-   0        0        0     2313 2023-05-09 13:32:07.000000 asdm-0.0.3/ASDM/Inference/Payoff.py
+-rw-rw-rw-   0        0        0     3727 2023-05-09 13:32:07.000000 asdm-0.0.3/ASDM/Inference/Probability.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 13:32:07.000000 asdm-0.0.3/ASDM/Inference/__init__.py
+-rw-rw-rw-   0        0        0     2349 2023-05-09 13:20:53.000000 asdm-0.0.3/ASDM/Utilities.py
+-rw-rw-rw-   0        0        0       21 2023-05-09 13:32:07.000000 asdm-0.0.3/ASDM/__init__.py
+-rw-rw-rw-   0        0        0   220612 2023-05-09 13:32:07.000000 asdm-0.0.3/Demo_SD_modelling.ipynb
+-rw-rw-rw-   0        0        0     1082 2023-04-16 16:07:35.000000 asdm-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5074 2023-05-09 13:35:32.891357 asdm-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-05-09 13:20:53.000000 asdm-0.0.3/Pipfile
+-rw-rw-rw-   0        0        0   140908 2023-05-09 13:20:53.000000 asdm-0.0.3/Pipfile.lock
+-rw-rw-rw-   0        0        0     3432 2023-05-09 13:34:58.000000 asdm-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.575351 asdm-0.0.3/apps/
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.666352 asdm-0.0.3/apps/ERM/
+-rw-rw-rw-   0        0        0    43567 2023-05-09 13:20:53.000000 asdm-0.0.3/apps/ERM/3-From_XMILE.ipynb
+-rw-rw-rw-   0        0        0     2173 2023-05-09 13:20:53.000000 asdm-0.0.3/apps/ERM/ERM_ASDM_app.py
+-rw-rw-rw-   0        0        0    64961 2023-05-09 13:20:53.000000 asdm-0.0.3/apps/ERM/Elective Recovery Model.stmx
+-rw-rw-rw-   0        0        0   255859 2023-05-09 13:20:53.000000 asdm-0.0.3/apps/ERM/Elective Recovery Model.xlsx
+-rw-rw-rw-   0        0        0   118770 2023-05-09 13:20:53.000000 asdm-0.0.3/apps/ERM/Elective_Recovery_Model.PNG
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.673353 asdm-0.0.3/apps/Goal_Gap/
+-rw-rw-rw-   0        0        0    11354 2023-05-09 13:20:53.000000 asdm-0.0.3/apps/Goal_Gap/Goal_gap_model.png
+-rw-rw-rw-   0        0        0     3570 2023-05-09 13:20:53.000000 asdm-0.0.3/apps/Goal_Gap/Revised_Goal_Gap.py
+-rw-rw-rw-   0        0        0    16090 2023-05-09 13:20:53.000000 asdm-0.0.3/apps/Goal_Gap/Revised_Goal_Gap.stmx
+-rw-rw-rw-   0        0        0      911 2023-05-09 13:20:53.000000 asdm-0.0.3/apps/Goal_Gap/goal_gap.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.674352 asdm-0.0.3/apps/Smoking_Cessation/
+-rw-rw-rw-   0        0        0     2001 2023-05-09 13:20:53.000000 asdm-0.0.3/apps/Smoking_Cessation/smoking_cessation.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.696354 asdm-0.0.3/asdm.egg-info/
+-rw-rw-rw-   0        0        0     5074 2023-05-09 13:35:32.000000 asdm-0.0.3/asdm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4534 2023-05-09 13:35:32.000000 asdm-0.0.3/asdm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 13:35:32.000000 asdm-0.0.3/asdm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      414 2023-05-09 13:35:32.000000 asdm-0.0.3/asdm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-09 13:35:32.000000 asdm-0.0.3/asdm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.576351 asdm-0.0.3/assets/
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.701353 asdm-0.0.3/assets/images/
+-rw-rw-rw-   0        0        0    11354 2023-05-09 13:20:53.000000 asdm-0.0.3/assets/images/Goal_gap_model.png
+-rw-rw-rw-   0        0        0     7502 2023-05-09 13:20:53.000000 asdm-0.0.3/assets/images/Infection_model.png
+-rw-rw-rw-   0        0        0    63503 2023-05-09 13:20:53.000000 asdm-0.0.3/assets/images/Simplified_patient_flow_model.png
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.710352 asdm-0.0.3/notebooks/
+-rw-rw-rw-   0        0        0   224222 2023-05-09 13:32:07.000000 asdm-0.0.3/notebooks/ValidateSimuOutcomes.ipynb
+-rw-rw-rw-   0        0        0     1292 2023-05-09 13:20:53.000000 asdm-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     6474 2023-05-09 13:24:58.000000 asdm-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 13:35:32.892359 asdm-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-04-16 16:50:21.000000 asdm-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.728353 asdm-0.0.3/tests/
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.763354 asdm-0.0.3/tests/BuiltInTestModels/
+-rw-rw-rw-   0        0        0    14838 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Array_cross_reference.stmx
+-rw-rw-rw-   0        0        0    14475 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Array_cross_reference_inference.stmx
+-rw-rw-rw-   0        0        0    13368 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Array_parallel_reference.stmx
+-rw-rw-rw-   0        0        0    13213 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Basic_math.stmx
+-rw-rw-rw-   0        0        0    12870 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Built_in_vars.stmx
+-rw-rw-rw-   0        0        0    15020 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Conveyor.stmx
+-rw-rw-rw-   0        0        0    15841 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Conveyor_initialisation.stmx
+-rw-rw-rw-   0        0        0    15841 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Conveyor_leakage.stmx
+-rw-rw-rw-   0        0        0    18784 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Conveyor_leakage1.stmx
+-rw-rw-rw-   0        0        0    18280 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Conveyor_leakage2.stmx
+-rw-rw-rw-   0        0        0    15999 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Delays.stmx
+-rw-rw-rw-   0        0        0    14193 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Delays2.stmx
+-rw-rw-rw-   0        0        0    13767 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Goal_gap.stmx
+-rw-rw-rw-   0        0        0    14512 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Goal_gap_array.stmx
+-rw-rw-rw-   0        0        0    14119 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Graph_function.stmx
+-rw-rw-rw-   0        0        0    13920 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/History.stmx
+-rw-rw-rw-   0        0        0    13246 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/IF_THEN_ELSE.stmx
+-rw-rw-rw-   0        0        0    13222 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/INIT.stmx
+-rw-rw-rw-   0        0        0    12865 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Isolated_var.stmx
+-rw-rw-rw-   0        0        0    14306 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/LOOKUP.stmx
+-rw-rw-rw-   0        0        0    14013 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Logic.stmx
+-rw-rw-rw-   0        0        0    16221 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/MOD.stmx
+-rw-rw-rw-   0        0        0    15257 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/MOD_arrayed.stmx
+-rw-rw-rw-   0        0        0    13528 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Min_Max.stmx
+-rw-rw-rw-   0        0        0    14466 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Non-negative_stocks.stmx
+-rw-rw-rw-   0        0        0    19817 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Non-negative_stocks_with_flows.stmx
+-rw-rw-rw-   0        0        0    20825 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Smooth.stmx
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.797355 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/
+-rw-rw-rw-   0        0        0      615 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Array_cross_reference.csv
+-rw-rw-rw-   0        0        0      329 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Array_cross_reference_inference.csv
+-rw-rw-rw-   0        0        0      133 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Array_parallel_reference.csv
+-rw-rw-rw-   0        0        0      101 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Basic_math.csv
+-rw-rw-rw-   0        0        0       77 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Built_in_vars.csv
+-rw-rw-rw-   0        0        0      318 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Conveyor.csv
+-rw-rw-rw-   0        0        0      434 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Conveyor_initialisation.csv
+-rw-rw-rw-   0        0        0     1677 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Conveyor_leakage.csv
+-rw-rw-rw-   0        0        0      903 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Conveyor_leakage1.csv
+-rw-rw-rw-   0        0        0     1024 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Conveyor_leakage2.csv
+-rw-rw-rw-   0        0        0      518 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Delays.csv
+-rw-rw-rw-   0        0        0       95 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Delays2.csv
+-rw-rw-rw-   0        0        0     1619 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Goal_gap.csv
+-rw-rw-rw-   0        0        0     3920 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Goal_gap_array.csv
+-rw-rw-rw-   0        0        0      539 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Graph_function.csv
+-rw-rw-rw-   0        0        0      129 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/History.csv
+-rw-rw-rw-   0        0        0      139 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/IF_THEN_ELSE.csv
+-rw-rw-rw-   0        0        0      623 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/INIT.csv
+-rw-rw-rw-   0        0        0       23 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Isolated_var.csv
+-rw-rw-rw-   0        0        0      578 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/LOOKUP.csv
+-rw-rw-rw-   0        0        0      198 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Logic.csv
+-rw-rw-rw-   0        0        0     1196 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/MOD.csv
+-rw-rw-rw-   0        0        0      397 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/MOD_arrayed.csv
+-rw-rw-rw-   0        0        0      840 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Min_Max.csv
+-rw-rw-rw-   0        0        0      154 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Modules.csv
+-rw-rw-rw-   0        0        0      129 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Non-negative_stocks.csv
+-rw-rw-rw-   0        0        0      570 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Non-negative_stocks_with_flows.csv
+-rw-rw-rw-   0        0        0     3842 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Smooth.csv
+-rw-rw-rw-   0        0        0      111 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Time_related_functions.csv
+-rw-rw-rw-   0        0        0       75 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Time_unit.csv
+-rw-rw-rw-   0        0        0    15665 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Time_related_functions.stmx
+-rw-rw-rw-   0        0        0    12864 2023-05-09 13:20:53.000000 asdm-0.0.3/tests/BuiltInTestModels/Time_unit.stmx
+drwxrwxrwx   0        0        0        0 2023-05-09 13:35:32.890357 asdm-0.0.3/tests/Discarded/
+-rw-rw-rw-   0        0        0    79877 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/Discarded/EngineArrays.py
+-rw-rw-rw-   0        0        0   346078 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/Discarded/EngineArraysTest.ipynb
+-rw-rw-rw-   0        0        0     1093 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/Discarded/EngineArraysTest.py
+-rw-rw-rw-   0        0        0    28482 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/Discarded/EngineNew0.py
+-rw-rw-rw-   0        0        0    49461 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/Discarded/EngineNew1.py
+-rw-rw-rw-   0        0        0    50683 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/Discarded/EngineNew2.py
+-rw-rw-rw-   0        0        0    33753 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/Discarded/EngineOOP.py
+-rw-rw-rw-   0        0        0    42726 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/Discarded/EngineStatic.py
+-rw-rw-rw-   0        0        0    12723 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/Discarded/Var.py
+-rw-rw-rw-   0        0        0     2248 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/Discarded/sly_example.py
+-rw-rw-rw-   0        0        0     3101 2023-04-16 16:50:21.000000 asdm-0.0.3/tests/run_tests.py
+-rw-rw-rw-   0        0        0     3183 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/test_Behaviour.py
+-rw-rw-rw-   0        0        0     3467 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/test_Engine.py
+-rw-rw-rw-   0        0        0      622 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/test_Externals.py
+-rw-rw-rw-   0        0        0      801 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/test_MultipleRuns.py
+-rw-rw-rw-   0        0        0     2422 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/test_Parser.py
+-rw-rw-rw-   0        0        0     2333 2023-05-09 13:32:07.000000 asdm-0.0.3/tests/test_Solver.py
```

### Comparing `asdm-0.0.2/.gitignore` & `asdm-0.0.3/.gitignore`

 * *Files 19% similar despite different names*

```diff
@@ -133,32 +133,18 @@
 
 # OS
 .DS_Store
 
 # Customised
 TestModels/
 Notes/
-Discarded/
+Ignored/
 
 BuiltInTestModels/*.isdb
 
-Smoking_Cessation_Model.png
-Smoking_Cessation_ASDM_model.ipynb
-Fix_Smoking_Cessation_ASDM_model.ipynb
-ASDM/ValidationOutcomeSmokingCessation.ipynb
-3-From_XMILE_ERM.ipynb
-ply/
-sly/
-Notes/
-
-ASDM/ValidationOutcomeSmokingCessation.ipynb
-3-From_XMILE_ERM.ipynb
-3-From_XMILE_Endoscopy.ipynb
-Elective Recovery Model flattened.xlsx
-
-.vscode/launch.json
+.vscode/
 asdm.csv
 stella.csv
-ValidateSimuOutcomes.ipynb
 comparison.csv
 asdm_outcome.csv
 stella_outocome.csv
+ASDM.code-workspace
```

### Comparing `asdm-0.0.2/1-SD_modelling.ipynb` & `asdm-0.0.3/Demo_SD_modelling.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910657051282051%*

 * *Differences: {"'cells'": "{1: {'execution_count': 10}, 3: {'execution_count': 11}, 4: {'execution_count': 12, "*

 * *            "'outputs': {0: {'execution_count': 12}}}, 5: {'execution_count': 13}, 6: "*

 * *            "{'execution_count': 14}, 8: {'execution_count': 15}, 9: {'execution_count': 16, "*

 * *            "'outputs': {0: {'execution_count': 16}}}, 10: {'execution_count': 17}, 11: "*

 * *            "{'execution_count': 18, 'outputs': {0: {'data': {'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAArcAAAINCAYAAAAkzFdkAAAAO […]*

```diff
@@ -5,15 +5,15 @@
             "metadata": {},
             "source": [
                 "# 1 Examples on SD model building and simulation"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from ASDM.ASDM import Structure\n",
                 "from ASDM.Utilities import plot_time_series\n",
                 "from IPython.display import Image"
             ]
@@ -28,15 +28,15 @@
                 "- Add stock, flow, and auxiliaries to model\n",
                 "- Run simulation and export the result\n",
                 "- Visualise simulation outcome by graph"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
                 "class GoalGap(Structure):\n",
                 "    def __init__(self):\n",
                 "        super(GoalGap, self).__init__()\n",
                 "        self.add_stock(\"Stock\", 100, in_flows=['Flow'])\n",
@@ -44,48 +44,48 @@
                 "        self.add_aux(\"Adjustment_time\", 5)\n",
                 "        self.add_aux(\"Gap\", \"Goal-Stock\")\n",
                 "        self.add_flow(\"Flow\", \"Gap/Adjustment_time\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/plain": [
                             "<IPython.core.display.Image object>"
                         ]
                     },
-                    "execution_count": 3,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "Image('assets/images/Goal_gap_model.png')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "goal_gap_model = GoalGap()\n",
                 "goal_gap_model.simulate(time=20, dt=1)\n",
                 "df_goal_gap = goal_gap_model.export_simulation_result()\n",
                 "# df_goal_gap"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/plain": [
                             "<Figure size 800x600 with 1 Axes>"
@@ -111,15 +111,15 @@
                 "#### Functionalities tested:\n",
                 "- Support for non-linear functions such as MIN, MAX, enabled through built-in python functions\n",
                 "- Support for stochastic functions such as random binomial (rbinom), enabled through Scipy"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [],
             "source": [
                 "class PatientFlow(Structure):\n",
                 "    def __init__(self):\n",
                 "        super(PatientFlow, self).__init__()\n",
                 "        self.add_stock(\"Waiting_list\", 100, in_flows=['GP_referrals'], out_flows=['Hospital_admission_rate'])\n",
@@ -148,54 +148,54 @@
                 "        # mapping SD functions to Python functions\n",
                 "        self.custom_functions['MAX'] = max\n",
                 "        self.custom_functions['MIN'] = min"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "iVBORw0KGgoAAAANSUhEUgAAA5IAAAEaCAYAAABjDWiOAAABPWlDQ1BJQ0MgUHJvZmlsZQAAKJFjYGASSCwoyGFhYGDIzSspCnJ3UoiIjFJgf8rAxsAOhoqJycUFjgEBPkAlDDAaFXy7xsAIoi/rgsxySz7xSWlz9+m3+8u9tixvuICpHgVwpaQWJwPpP0CclFxQVMLAwJgAZCuXlxSA2C1AtkgR0FFA9gwQOx3CXgNiJ0HYB8BqQoKcgewrQLZAckZiCpD9BMjWSUIST0diQ+0FAQ6PAAVXI2MjAk4lHZSkVpSAaOf8gsqizPSMEgVHYAilKnjmJevpKBgZGBkyMIDCG6L68w1wODKKcSDE0hYxMJiIAxnXEWJZfAwMu4GOFZZHiKmpAb20g4Fhv0VBYlEi3AGM31iK06AeY+TezsDAOu3//8/hDAzsmgwMf6////97+///f5cxMDDfYmA48A0ARXBel55NEU8AAABiZVhJZk1NACoAAAAIAAIBEgADAAAAAQABAACHaQAEAAAAAQAAACYAAAAAAAOShgAHAAAAEgAAAFCgAgAEAAAAAQAAA5KgAwAEAAAAAQAAARoAAAAAQVNDSUkAAABTY3JlZW5zaG90H1yQlwAAAj1pVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IlhNUCBDb3JlIDUuNC4wIj4KICAgPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4KICAgICAgPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIKICAgICAgICAgICAgeG1sbnM6ZXhpZj0iaHR0cDovL25zLmFkb2JlLmNvbS9leGlmLzEuMC8iCiAgICAgICAgICAgIHhtbG5zOnRpZmY9Imh0dHA6Ly9ucy5hZG9iZS5jb20vdGlmZi8xLjAvIj4KICAgICAgICAgPGV4aWY6VXNlckNvbW1lbnQ+U2NyZWVuc2hvdDwvZXhpZjpVc2VyQ29tbWVudD4KICAgICAgICAgPGV4aWY6UGl4ZWxYRGltZW5zaW9uPjkxNDwvZXhpZjpQaXhlbFhEaW1lbnNpb24+CiAgICAgICAgIDxleGlmOlBpeGVsWURpbWVuc2lvbj4yODI8L2V4aWY6UGl4ZWxZRGltZW5zaW9uPgogICAgICAgICA8dGlmZjpPcmllbnRhdGlvbj4xPC90aWZmOk9yaWVudGF0aW9uPgogICAgICA8L3JkZjpEZXNjcmlwdGlvbj4KICAgPC9yZGY6UkRGPgo8L3g6eG1wbWV0YT4KYH/68QAAQABJREFUeAHsnQdgFGX6xp+Z3SQQeg29F2kCIk1AQcUu9t7Lnd7Z/uep5+l5p2c5Pc9ez97Ojl0BC0VEQECaIL2G3jvJ7sz8n3c3wRApIQmS3X0+XbI7O/OV38zsfM/3vt/7OQETlERABERABERABERABERABERABESgiATcIu6n3URABERABERABERABERABERABEQgRkBCUheCCIiACIiACIiACIiACIiACIjAPhGQkNwnXNpZBERABERABERABERABERABERAQlLXgAiIgAiIgAiIgAiIgAiIgAiIwD4RkJDcJ1zaWQREQAREQAREQAREQAREQAREQEJS14AIiIAIiIAIiIAIiIAIiIAIiMA+EZCQ3Cdc2lkEREAEREAEREAEREAEREAEREBCUteACIiACIiACIiACIiACIiACIjAPhGQkNwnXNpZBERABERABERABERABERABERAQlLXgAiIgAiIgAiIgAiIgAiIgAiIwD4RkJDcJ1zaWQREQAREQAREQAREQAREQAREQEJS14AIiIAIiIAIiIAIiIAIiIAIiMA+EZCQ3Cdc2lkEREAEREAEREAEREAEREAEREBCUteACIiACIiACIiACIiACIiACIjAPhEI79Pe2lkEREAEUpjA9u3Axo0BfB+oXNlBZmYKw1DTRUAEREAEREAEUpqAhGRKn341XgREYG8Etm4FFi/2sXwZ/y4KkJ0dwKOQrFMHaNLE4V8HDRo6qFLF2VtW+l4EREAEREAEREAEkoaAEzAlTWvUEBEQAREoRQJr1wYY9IWPN1/3sXBugNp1HXTr6aBiReD77ygqFwaoVsPBGec4OOusEOrWk5gsRfzKSgREQAREQAREoAwTkJAswydHVRMBEThwBJYuCXDXP6JYvRq4+o8ujjwqhFDo1/WZMN7HU0962LAeuO+BEFq31tTzX1PSFhEQAREQAREQgWQjICGZbGdU7REBESgxgRUrAtx4QxSt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",
                         "text/plain": [
                             "<IPython.core.display.Image object>"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "Image('assets/images/Simplified_patient_flow_model.png')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [],
             "source": [
                 "patient_flow_model = PatientFlow()\n",
                 "patient_flow_model.clear_last_run()\n",
                 "patient_flow_model.simulate(time=20, dt=1)\n",
                 "df_patient_flow = patient_flow_model.export_simulation_result()\n",
                 "# df_patient_flow"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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fuW209vjqExN/XD1uXMltituvvlmLV26VPfee69WrlypiRMnOvxH+XS1HdOZM2dq06ZNeuSRR9S5c2c1a9ZMf/rTn1RSUmJXrnnz5nb3CwsLddtttzn8Zpf27du70CMAgC9yObl97LHHZBiGJk2apHnz5ikiIsK2LygoSB06dKjzVbLGKDTQcRJWVZ82fWQNtepo0VGH624tssgaalWfNn3cqreuzjnnHI9/5VV0dLSys7Nt98vKyvTll1/qsssuc1h+x44dKi8v16OPPio/v4o3DtasWWNXJigoyLZGtVJiYqLKysp09OhRXXTRRQ7r7tGjh+1DRpW2bdvmdp/OREJCgtLT0zVv3rxq+zp16qSgoCBt3bpV8fHxkiqSye3bt3vle2Kjo6N1/PhxnThxwpb47d69+4zrdfT8SdL//u//6i9/+YueeOIJ7d27VxMmTHCpvoSEBD377LP65ZdfHF693bp1q2666SZdc801kiqS1kOHDtVab58+fbR371517tzZpXYAABoHl5Pbyheijh07auDAgdWu5qA6fz9/3dvvXs3YMkMWWewSXIsqrljN6jfLdqXXU44dO6brrrtOkyZNUkJCglq0aKHPPvtMixYt0qhRozwaa/DgwZoxY4bWr1+vTp06afHixcrLy3NavnPnziotLdWTTz6pkSNHauvWrXr66aftynTo0EGFhYVKT09X7969FRoaqq5du2rs2LEaP368Hn30USUmJuqnn35Senq6EhISNGLECN11110aNGiQHnnkEY0aNUobN27Uu+967kq4K2bPnq1evXrpjjvu0O23366goCBt3rxZ1113nVq3bq0pU6boz3/+s1q2bKn27dtr0aJFKioq0uTJkxu0nZLUv39/hYaG6r777tNdd92lTz75pNZlK67o0KGDPvzwQ914440KDg5W69atJVW8+3Pttdfqz3/+s4YOHaq2bdu6VN+YMWM0f/58jR49WgsWLFBsbKx27dqluLg4JSUlqUuXLnr99dc1cuRIWSwWzZkzx6Ury7NmzdKAAQN055136uabb1bz5s21d+9ebdq0SU899dQZHQMAgPe4tOa2oKDA9ndiYqJ+++03FRQUOLzB3pD4IVp86WK1CW1jt90aatXiSxfXy/fchoWFqX///lqyZIkuvvhinXvuuZozZ45uueUWj79oT5o0SRMmTND48eN1ySWX6Oyzz3Z61VaSevfurcWLF+vhhx/Wueeeq5deekkLFiywKzNw4EDdfvvtuuGGGxQdHa1FixZJqvh0/fjx43XPPfeoW7duGj16tLZv3257C3nAgAFasWKFHn/8cfXu3Vvvvfee7r//fo/2tzZdu3bVe++9p88//1z9+vVTUlKS3nzzTQUEVPwfuXDhQqWkpGjcuHHq06ePvvnmG23cuNHhN5DUt5YtW+rFF1/UO++8o169eumVV16xfe3amXjwwQd16NAhderUSdHR9ktzKpefTJo0yeX6goKC9N5776lNmza68sor1atXLy1cuNC2PGXx4sWKiorSwIEDNXLkSCUnJ6tPnz611FpxRTgjI0Nff/21LrroIiUmJmru3LmKi4tzr8MAAJ9iMU5fdOeAv7+/srOz1aZNG/n5+TlcJ1f5QTNHb0f6uoKCAkVERCg/P1/h4eF2+06ePKmDBw+qY8eOCgkJqXOMsvIy7Ty6Uz8V/aTo0Gj1adPH41dsAV/3z3/+U9OnT9eRI0ca3Y8oeOpcAACom5rytapcWpbwwQcf2Na6bd682TMtbGL8/fx1QcwF3m4G4BVFRUXKzs7WwoULddtttzW6xBYA0Hi4lNxecskltr87duyodu3aVbt6axiGvv/+e8+2DvAxw4cP13//+1+H++677z7dd999DdyixmHRokV66KGHdPHFF2v27Nl2++bPn6/58+c7fNxFF11k96tqAADUxqVlCVVVXaJQ1bFjx9SmTRuWJcDUfvzxR/32228O97Vs2ZLveq6DX375pdovtFVq1qyZzjrrrAZukWOcCwDAuzy6LKEqZz/iUFhYyAkfpucriZaZ8E8BAMCTXE5uZ8yYIUm2r9qp+mX7ZWVl+uSTT3Teeed5vIEAAACAq1xObnft2iWp4srtnj177D4QEhQUpN69e2vmzJmeb6GPcHP1BgCT4RwAAI2Dy8lt5bckTJw4UY8//niNax3MJDAwUBaLRT/99JOio6Nd+rlQAOZiGIZ++uknhz+FDADwLW5/oKyh/fjjj5o1a5Y2bNigoqIide7cWStXrtT5558vqeJFJy0tTStWrFBeXp4GDRqk5cuXq0uXLi7HqG2BcmFhoX744Qeu3ABNmMViUdu2bRUWFubtpgBAk1RvHyg7ceKEFi5cqPT0dB09erTaz1x+++237rfWiV9//VWDBg3SZZddpg0bNig6Olr79++3+zWnRYsW6YknntDq1avVsWNHzZkzR8nJydq7d6/HPuAWFhamLl26qLS01CP1AWh8AgMDbb+KBgDwXW4ntzfffLMyMjI0btw4xcbG1uvb9A8//LDatWunlStX2rZ17NjR9rdhGHrsscd0//33a9SoUZKkF154QVarVW+88YZuvPFGj7XF39+fFzYAAAAf53Zyu2HDBq1fv16DBg2qj/bYeeutt5ScnKzrrrtOGRkZOuuss3THHXfolltukSQdPHhQOTk5GjJkiO0xERER6t+/vzIzM50mt8XFxSouLrbdLygoqN+OAAAAoEH4ufuAqKioBvtOym+//da2fnbjxo2aMmWK7rrrLq1evVqSlJOTI0myWq12j7NarbZ9jixYsEARERG2W7t27eqvEwAAAGgwbie3f/vb3zR37lwVFRXVR3vslJeXq0+fPpo/f74SExN166236pZbbtHTTz99RvXOnj1b+fn5ths/GwwAAGAObi9LePTRR3XgwAFZrVZ16NCh2tfi7Ny502ONi42N1TnnnGO3rUePHvr3v/8tSYqJiZEk5ebmKjY21lYmNze3xh+UCA4OVnBwsMfaCQAAAN/gdnI7evToemiGY4MGDVJWVpbdtq+//lrx8fGSKj5cFhMTo/T0dFsyW1BQoE8++URTpkxpsHYCAADAN7id3KalpdVHOxyaPn26Bg4cqPnz5+v666/Xp59+qn/84x/6xz/+IanieyenTZum//u//1OXLl1sXwUWFxfXoEk4AAAAfIPbyW1DuuCCC7Ru3TrNnj1bDz74oDp27KjHHntMY8eOtZX5y1/+ohMnTujWW29VXl6eLrzwQr377rse+45bAAAANB5u/0JZWVmZlixZojVr1ujw4cMqKSmx2//LL794tIENwdVfvAAAAIB3uJqvuf1tCfPmzdPixYt1ww03KD8/XzNmzNC1114rPz8/PfDAA2fSZgAAAOCMuJ3cvvTSS1qxYoXuueceBQQEaMyYMXr22Wc1d+5cbdu2rT7aCAAAALjE7eQ2JydHvXr1kiSFhYUpPz9fknTVVVdp/fr1nm0dAAAA4Aa3k9u2bdsqOztbktSpUye99957kqTt27fz3bEAAADwKreT22uuuUbp6emSpKlTp2rOnDnq0qWLxo8fr0mTJnm8gQAAAICr3P62hNNlZmYqMzNTXbp00ciRIz3VrgbFtyUAAAD4NlfztTP+ntukpCQlJSWdaTUAAADAGXM7uX3hhRdq3D9+/Pg6NwYAAAA4E24vS4iKirK7X1paqqKiIgUFBSk0NJQfcQAAAIDH1duPOPz66692t8LCQmVlZenCCy/UK6+8ckaNBgAAAM6E28mtI126dNHChQt19913e6I6AAAAoE48ktxKUkBAgI4cOeKp6gAAAAC3uf2BsrfeesvuvmEYys7O1lNPPaVBgwZ5rGEAAACAu9xObkePHm1332KxKDo6WoMHD9ajjz7qqXYBAAAAbnM7uS0vL6+PdgAAAABnrM5rbn/++WcVFBR4si0AAADAGXEruc3Ly1Nqaqpat24tq9WqqKgoxcTEaPbs2SoqKqqvNgIAAAAucXlZwi+//KKkpCT9+OOPGjt2rHr06CFJ2rt3r5588klt2rRJH330kb744gtt27ZNd911V701GgAAAHDE5eT2wQcfVFBQkA4cOCCr1Vpt39ChQzVu3Di99957euKJJzzeUAAAAKA2Lie3b7zxhp555plqia0kxcTEaNGiRbryyiuVlpamCRMmeLSRAAAAgCtcXnObnZ2tnj17Ot1/7rnnys/PT2lpaR5pGAAAAOAul5Pb1q1b69ChQ073Hzx4UG3atPFEmwAAAIA6cTm5TU5O1l//+leVlJRU21dcXKw5c+Zo2LBhHm0cAAAA4A6LYRiGKwV/+OEHnX/++QoODlZqaqq6d+8uwzC0b98+LVu2TMXFxdq+fbvat29f3232uIKCAkVERCg/P1/h4eHebg4AAABO42q+5vIHytq2bavMzEzdcccdmj17tipzYovFoiuuuEJPPfVUo0xsAQAAYB5u/fxux44dtWHDBv3666/av3+/JKlz585q2bJlvTQOAAAAcIdbyW2lqKgo9evXz9NtAQAAAM6IWz+/CwAAAPgyklsAAACYBsktAAAATIPkFgAAAKZBcgsAAADTILkFAACAaZDcAgAAwDRIbgEAAGAaJLcAAAAwDZJbAAAAmAbJLQAAAEyD5BYAAACmQXILAAAA0yC5BQAAgGmQ3AIAAMA0SG4BAABgGiS3AAAAMA2SWwAAAJgGyS0AAABMw6eT2wceeEAWi8Xu1r17d9v+kydPKjU1Va1atVJYWJhSUlKUm5vrxRYDAADAm3w6uZWknj17Kjs723b76KOPbPumT5+ut99+W2vXrlVGRoaOHDmia6+91outBQAAgDcFeLsBtQkICFBMTEy17fn5+Xruuef08ssva/DgwZKklStXqkePHtq2bZsGDBjQ0E0FAACAl/n8ldv9+/crLi5OZ599tsaOHavDhw9Lknbs2KHS0lINGTLEVrZ79+5q3769MjMzvdVcAAAAeJFPX7nt37+/Vq1apW7duik7O1vz5s3TRRddpC+//FI5OTkKCgpSZGSk3WOsVqtycnJqrLe4uFjFxcW2+wUFBfXRfAAAADQwn05uhw8fbvs7ISFB/fv3V3x8vNasWaNmzZrVud4FCxZo3rx5nmgiAAAAfIjPL0uoKjIyUl27dtU333yjmJgYlZSUKC8vz65Mbm6uwzW6Vc2ePVv5+fm22/fff1+PrQYAAEBDaVTJbWFhoQ4cOKDY2Fj17dtXgYGBSk9Pt+3PysrS4cOHlZSUVGM9wcHBCg8Pt7sBAACg8fPpZQkzZ87UyJEjFR8fryNHjigtLU3+/v4aM2aMIiIiNHnyZM2YMUMtW7ZUeHi4pk6dqqSkJL4pAQAAoIny6eT2hx9+0JgxY3Ts2DFFR0frwgsv1LZt2xQdHS1JWrJkifz8/JSSkqLi4mIlJydr2bJlXm41AAAAvMViGIbh7UZ4W0FBgSIiIpSfn88SBQAAAB/kar7WqNbcAgAAADUhuQUAAIBpkNwCAADANEhuAQAAYBoktwAAADANklsAAACYBsktAAAATIPkFgAAAKZBcgsAAADTILkFAACAaZDcAgAAwDRIbgEAAGAaJLcAAAAwDZJbAAAAmAbJLQAAAEyD5BYAAACmQXILAAAA0yC5BQAAgGmQ3AIAAMA0SG4BAABgGiS3AAAAMA2SWwAAAJgGyS0AAABMg+QWAAAApkFyCwAAANMguQUAAIBpkNwCAADANEhuAQAAYBoktwAAADANklsAAACYBsktAAAATIPkFgAAAKZBcgsAAADTILkFAACAaZDcAgAAwDRIbgEAAGAaJLcAAAAwDZJbAAAAmAbJLQAAAEyD5BYAAACmQXILAAAA0yC5BQAAgGmQ3AIAAMA0SG4BAABgGiS3AAAAMA2SWwAAAJgGyS0AAABMo1EltwsXLpTFYtG0adNs206ePKnU1FS1atVKYWFhSklJUW5urvcaCQAAAK9pNMnt9u3b9cwzzyghIcFu+/Tp0/X2229r7dq1ysjI0JEjR3Tttdd6qZUAAADwpkaR3BYWFmrs2LFasWKFoqKibNvz8/P13HPPafHixRo8eLD69u2rlStX6uOPP9a2bdu82GIAAAB4Q6NIblNTUzVixAgNGTLEbvuOHTtUWlpqt7179+5q3769MjMzndZXXFysgoICuxsAAAAavwBvN6A2r776qnbu3Knt27dX25eTk6OgoCBFRkbabbdarcrJyXFa54IFCzRv3jxPNxUAAABe5tNXbr///nvdfffdeumllxQSEuKxemfPnq38/Hzb7fvvv/dY3QAAAPAen05ud+zYoaNHj6pPnz4KCAhQQECAMjIy9MQTTyggIEBWq1UlJSXKy8uze1xubq5iYmKc1hscHKzw8HC7GwAAABo/n16WcPnll2vPnj122yZOnKju3btr1qxZateunQIDA5Wenq6UlBRJUlZWlg4fPqykpCRvNBkAAABe5NPJbYsWLXTuuefabWvevLlatWpl2z558mTNmDFDLVu2VHh4uKZOnaqkpCQNGDDAG00GAACAF/l0cuuKJUuWyM/PTykpKSouLlZycrKWLVvm7WYBAADACyyGYRjeboS3FRQUKCIiQvn5+ay/BQAA8EGu5ms+/YEyAAAAwB0ktwAAADANklsAAACYBsktAAAATIPkFgAAAKZBcgsAAADTILkFAACAaZDcAgAAwDRIbgEAAGAaJLcAAAAwDZJbAAAAmAbJLQAAAEyD5BYAAACmQXILAAAA0yC5BQAAgGmQ3AIAAMA0SG4BAABgGiS3AAAAMA2SWwAAAJgGyS0AAABMg+QWAAAApkFyCwAAANMguQUAAIBpkNwCAADANEhuAQAAYBoktwAAADANklsAAACYBsktAAAATIPkFgAAAKZBcgsAAADTILkFAACAaZDcAgAAwDRIbgEAAGAaJLcAAAAwDZJbAAAAmAbJLQAAAEyD5BYAAACmQXILAAAA0yC5BQAAgGmQ3AIAAMA0SG4BAABgGiS3XrR8+XIlJCQoPDxc4eHhSkpK0oYNG2z7T548qdTUVLVq1UphYWFKSUlRbm4u8XwkXlPoI/EYM8RrWvGaQh+J1/jHTK0MGPn5+YYkIz8/v0HjvvXWW8b69euNr7/+2sjKyjLuu+8+IzAw0Pjyyy8NwzCM22+/3WjXrp2Rnp5ufPbZZ8aAAQOMgQMHEs9H4jWFPhKPMUO8phWvKfSReI13zLiar5HcGt5Lbh2Jiooynn32WSMvL88IDAw01q5da9u3b98+Q5KRmZlJPB+N542YxGvc8bwRk3jE8/WYxGvc8eorJsmtG3whuf3999+NV155xQgKCjK++uorIz093ZBk/Prrr3bl2rdvbyxevJh4PhbPGzGJ17jjeSMm8Yjn6zGJ17jj1XdMV/O1AM8vdIA79uzZo6SkJJ08eVJhYWFat26dzjnnHO3evVtBQUGKjIy0K2+1WpWTk0M8H4nnjZjEa9zxvBGTeMTz9ZjEa9zxvBXTGZLbhlZeJn33sVSYK4VZ1a3L+dq9e7fy8/P1r3/9SxMmTFBGRgbxfDWeN2ISz1TxFD9Q3bp1M3UfidfI4nkjJvFMFa9Bzmtu8Onkdvny5Vq+fLkOHTokSerZs6fmzp2r4cOHS6r49N0999yjV199VcXFxUpOTtayZctktVq92Ooa7H1LeneWVHDEtikoPE6dhz0s9b1affv21fbt2/X444/rhhtuUElJifLy8uz+28nNzVVMTAzxvBGvKfSRePUeT+FxChr2sDqfc7UkmbKPxGtE8ZpCH4nX+M9rbvLprwJr27atFi5cqB07duizzz7T4MGDNWrUKH311VeSpOnTp+vtt9/W2rVrlZGRoSNHjujaa6/1cqud2PuWtGa8/WCQpILsiu1735IklZeXq7i4WH379lVgYKDS09NtRbOysnT48GElJSURr6HjNYU+Es8r8ZpCH4nno/GaQh+J55V4Ho1ZBz595XbkyJF29x966CEtX75c27ZtU9u2bfXcc8/p5Zdf1uDBgyVJK1euVI8ePbRt2zYNGDDAG012rLys4r8cGXabZ79/UsO7BKh9hL+Or7xbL2uLtmzZoo3r31ZERIQmT56sGTNmqGWLZgoPD9fU6TOVNKC/BvTpJZWcqKjE4icFNjtVacmJingb/lJLvGl6WRkV8f7zpiKaBWjyTeM1Y8b0P+JFaOqMPyspKaniWJYUVavvVP/K3evfxo1V+je95v4FNT9VYelJyShzsX9V4jnqX8s2mnrXXRX9Oz/xVDxHAkMlw8U++n10qo/Nm512TE/rY3m55PfH/5e/l0jlpVWO6Zn0cYZatmxZEe/OO6sf06r8gyX/gD/i1da/aXrZf2tFvHfecTBmqvTvgr6nKin7XSorto9b1/5NvOlU/8KaVzyHzvrnFygFBP1xfEtdmxOV/XM4Jyr7N+DU+cUwpNKi6sfVSf8qYv6m4V0C1f7l6To+Olovr/l3Hea9vxQYcqpSt+Z9DfMiIkJTp/vavP+tYv55Yt63smrq1KkV/et7Xs3z3j+4bv2beFPN/Qto5njen2n/IiMUHhlV0b8BA5zPeUkKCJH8/Osw79fXMu/PP1WJJ+f9pIl1nPcl9TPvy8ul33+rflzr0r/mIafmfFSUwkODHM8Jqfq8P1nguf5VznnJ+bhx6bw2Q8eva6+XX33Nwbyv8tpUOQ/rKVfz6eS2qrKyMq1du1YnTpxQUlKSduzYodLSUg0ZMsRWpnv37mrfvr0yMzNrPGDFxcUqLj416QoKCuq17fru4+r/5Ug6esLQ+HW/KbvQUERwoRKsT2jj2Ga64pdVkkZoyZIl8vPzU8roq1T8u6HkTgFaNiJEmh93qpL4C6WJ60/df6yXVHTMYTOqxYtbXhHv0/+VPpWWtDHk1+akUkaNUHG5n5JHjNKyZcsqHrziMumn/+e4f83bSCeOuta/SVZdccUVklTRv6x3KuKVqXr/AkOlv2afqnDNOGn/e86OsvPj6ah/fqG2ZSx6e5r0+ctO69WfD0hH97n2HPZ6Vxs3bqzo43v3a0mbNadint7HO7ZJbXpUVPTfR6WMhc7b4E4fL75cKSkpFUt1+nXTsr777cdMVf+zRuqaXDFGj7vQv/PSK/oXVyjNj7M/plX798UaKXFsRSUH0qWXr6+1by7174Y58gsIrOjfyd+UHP979TlR6ZJ7pctmV/y95zXpeHa1Ig77968XHI+Zyv79dfKpCoqOSX/v5FLf7GMWKbvwW0UsGaQEq19FH4+/Jrt572xeSFKXodLYtafu/72z4yTbUR9jl7k+75f2l/IPO+5IRDvXz2u3xtvP+31vOe9faCvpL9+eqvDFP0nffVTL8azDvF93q7T3Taf1auy/XO/fm2tO9W9YM/ntzHHev7u/kKLiK/7+4EHp4yedt8Gd/qWkqLj094r+3ZTofM5L0oT/SB0vcn/etz5a87z/f29LPa+pqOT/vS2tvanGvrncx7EL5Ocf4Nq8v+JBadDdFX/v+qfr8/61FTXP+7TUUxXkfy89nuBS32rtX/H/nJrzf/qTigt/dTznJemcUdL1L5y6v7Cda/HOS9fGCZHO+9fLqmXrd5+qoIY8ouY+Fim78IAinr5MCef1PfVaKJ3qY+VrU+U8rCc+n9zWx6fvFixYoHnz5tVjq09T6PhXOJ4b1czh9kohISFaunSplsa97vSFyx3V4jVrJf12agCHBFi0dEQzLR3RTIruLqW+7lrF5WWuxZOk0FPbQkJCtHTcuVp6cZ5rcWpR6/Gs2r/7jthfHaqNq8/hsCnSgCscx/QAl/r44Awt/ee6ig2frpDemVl7xa72L+VeqdcV0lfrTsVryP4FB1bMiaVLpR93SCsGu1axkxO1w/61vUD64o94jvoX5ca4cSXmaWzzPvrFM4rjNF5QmFRSeCpe1T7GJUq31sO8jwg7FS8kREv/p4uWXlpYvVwduDXvH8h3vWJ3ztuDLz0VLyig4ef8iGZaessH0ll/vGOy9XHXKnd33u96yT6mN+b9wf9Kq69yrWJ35r21p/TVH/Ec9a9lmOrK5Tm/ZFHN/5TUNV7KvdJbU215RLX+xfeVznDtq13MlBVSrz/Z7bf1cenSM4rjKothGE7ec/INJSUlOnz4sO3Td88++6wyMjK0e/duTZw40e4KrCT169dPl112mR5++GGndTq6ctuuXTvl5+crPDzc851wdTKO/ZcUP9DxW47OOFqW8N3H0kt/cv4YW7x/S/HO1rtYpKDQKvXW8Pbkd5nSSykuxPujf47ecnTG0bIEl/v3RzxHAkMli6Xi79+LpfLfndcTGCod+si153D829LZF/9R72lLDU7n7O1J6cz6WPmWoySVlUplJc4fX7kswdUxWnnFx9Fbjnb1Bkn+gX+0wUHZuvav6luO5WXS7yedP7Zq2W8/lF4Y6bxspQn/keIHOX7L0VZvgBQQXPG3s2UJdemfW/PeQVlPzItq5xNPzftB9ucTt+b9H2U90T9H5xNnftwhrXZhzIz9l9R5iOvnE2fz/kz7V3Xe13ru+aOs2/PexfOJ5Nl5X/V84ta8z5BeuLr2eC7N+6rnHifLEurSP1fOJ5VOn/f7N7kWb8J/pLP61FCvgzzCEVf7Vzle6kFBQYEiIiJqzdd8/sptUFCQOnfuLMlzn74LDg5WcHBwfTbbXvxAKTyuYsG1wxcKS8X+ToNPnZyqcucKY1DzinpcineZ43gO6w11vq/TZXXvX6Ab//lXTmqX++fkeJ4uIFhSLePB1eeww6Aq9QZJCqo9vqOynuqjf+CpF4WauNq/yhOyf8CpF7HaOCrrif75+bs+NzoMcr1/fn6u12uxOC7rif7V27x3cV5IPjLv/yjr6f5VTRIciXdxzHQafCqxlVw7n9jKVpn3nuyfq+cet+e9i+cTyUfm/YX1M++dlT3T/jk7nzjjarz4ga7Pecl5G9yJ52U+/W0Jjnjz03d15ucvDau8kmw5becf94ctdG/wEa/h4nkjJvGI5+sxide443kjJvGI10B8OrmdPXu2PvzwQx06dEh79uzR7NmztWXLFo0dO9bu03ebN2/Wjh07NHHixHr99N0ZOefqioXg4bH228PjKraf48JbJ8TzXjxvxCQe8Xw9JvEadzxvxCQe8RqAT6+5nTx5stLT05Wdna2IiAglJCRo1qxZtk/fVf6IwyuvvGL36Tt3vxTY1TUcHuHgVz3q9b8c4jX+mMQjnq/HJF7jjueNmMQjXh24mq/5dHLbUBo0uQUAAIDbXM3XfHpZAgAAAOAOklsAAACYBsktAAAATIPkFgAAAKZBcgsAAADTILkFAACAaZDcAgAAwDRIbgEAAGAaJLcAAAAwDZJbAAAAmAbJLQAAAEyD5BYAAACmQXILAAAA0wjwdgN8gWEYkqSCggIvtwQAAACOVOZplXmbMyS3ko4fPy5JateunZdbAgAAgJocP35cERERTvdbjNrS3yagvLxcR44cUYsWLWSxWOo9XkFBgdq1a6fvv/9e4eHh9R6vseC4OMexcYzj4hzHxjGOi3McG8c4Lo5547gYhqHjx48rLi5Ofn7OV9Zy5VaSn5+f2rZt2+Bxw8PDmSgOcFyc49g4xnFxjmPjGMfFOY6NYxwXxxr6uNR0xbYSHygDAACAaZDcAgAAwDRIbr0gODhYaWlpCg4O9nZTfArHxTmOjWMcF+c4No5xXJzj2DjGcXHMl48LHygDAACAaXDlFgAAAKZBcgsAAADTILkFAACAaZDcAgAAwDRIbuvJ0qVL1aFDB4WEhKh///769NNPayy/du1ade/eXSEhIerVq5feeeedBmppw1iwYIEuuOACtWjRQm3atNHo0aOVlZVV42NWrVoli8VidwsJCWmgFjecBx54oFo/u3fvXuNjzD5eJKlDhw7VjovFYlFqaqrD8mYeLx9++KFGjhypuLg4WSwWvfHGG3b7DcPQ3LlzFRsbq2bNmmnIkCHav39/rfW6e57yNTUdl9LSUs2aNUu9evVS8+bNFRcXp/Hjx+vIkSM11lmX+eiLahszN910U7V+Dhs2rNZ6zTxmJDk851gsFv397393WqcZxowrr9EnT55UamqqWrVqpbCwMKWkpCg3N7fGeut6bjpTJLf14LXXXtOMGTOUlpamnTt3qnfv3kpOTtbRo0cdlv/44481ZswYTZ48Wbt27dLo0aM1evRoffnllw3c8vqTkZGh1NRUbdu2TZs2bVJpaamGDh2qEydO1Pi48PBwZWdn227fffddA7W4YfXs2dOunx999JHTsk1hvEjS9u3b7Y7Jpk2bJEnXXXed08eYdbycOHFCvXv31tKlSx3uX7RokZ544gk9/fTT+uSTT9S8eXMlJyfr5MmTTut09zzli2o6LkVFRdq5c6fmzJmjnTt36vXXX1dWVpauvvrqWut1Zz76qtrGjCQNGzbMrp+vvPJKjXWafcxIsjse2dnZev7552WxWJSSklJjvY19zLjyGj19+nS9/fbbWrt2rTIyMnTkyBFde+21NdZbl3OTRxjwuH79+hmpqam2+2VlZUZcXJyxYMECh+Wvv/56Y8SIEXbb+vfvb9x222312k5vOnr0qCHJyMjIcFpm5cqVRkRERMM1ykvS0tKM3r17u1y+KY4XwzCMu+++2+jUqZNRXl7ucH9TGS+SjHXr1tnul5eXGzExMcbf//5327a8vDwjODjYeOWVV5zW4+55ytedflwc+fTTTw1Jxnfffee0jLvzsTFwdGwmTJhgjBo1yq16muKYGTVqlDF48OAay5hxzJz+Gp2Xl2cEBgYaa9eutZXZt2+fIcnIzMx0WEddz02ewJVbDyspKdGOHTs0ZMgQ2zY/Pz8NGTJEmZmZDh+TmZlpV16SkpOTnZY3g/z8fElSy5YtayxXWFio+Ph4tWvXTqNGjdJXX33VEM1rcPv371dcXJzOPvtsjR07VocPH3ZatimOl5KSEr344ouaNGmSLBaL03JNZbxUdfDgQeXk5NiNiYiICPXv39/pmKjLecoM8vPzZbFYFBkZWWM5d+ZjY7Zlyxa1adNG3bp105QpU3Ts2DGnZZvimMnNzdX69es1efLkWsuabcyc/hq9Y8cOlZaW2j3/3bt3V/v27Z0+/3U5N3kKya2H/fzzzyorK5PVarXbbrValZOT4/AxOTk5bpVv7MrLyzVt2jQNGjRI5557rtNy3bp10/PPP68333xTL774osrLyzVw4ED98MMPDdja+te/f3+tWrVK7777rpYvX66DBw/qoosu0vHjxx2Wb2rjRZLeeOMN5eXl6aabbnJapqmMl9NVPu/ujIm6nKcau5MnT2rWrFkaM2aMwsPDnZZzdz42VsOGDdMLL7yg9PR0Pfzww8rIyNDw4cNVVlbmsHxTHDOrV69WixYtan3r3WxjxtFrdE5OjoKCgqr9Y1hbblNZxtXHeEpAvdYOOJCamqovv/yy1jVJSUlJSkpKst0fOHCgevTooWeeeUZ/+9vf6ruZDWb48OG2vxMSEtS/f3/Fx8drzZo1Ll0xaAqee+45DR8+XHFxcU7LNJXxAveVlpbq+uuvl2EYWr58eY1lm8p8vPHGG21/9+rVSwkJCerUqZO2bNmiyy+/3Ist8x3PP/+8xo4dW+sHU802Zlx9jfZlXLn1sNatW8vf37/aJwhzc3MVExPj8DExMTFulW/M7rzzTv3nP//R5s2b1bZtW7ceGxgYqMTERH3zzTf11DrfEBkZqa5duzrtZ1MaL5L03Xff6f3339fNN9/s1uOaynipfN7dGRN1OU81VpWJ7XfffadNmzbVeNXWkdrmo1mcffbZat26tdN+NqUxI0n//e9/lZWV5fZ5R2rcY8bZa3RMTIxKSkqUl5dnV7623KayjKuP8RSSWw8LCgpS3759lZ6ebttWXl6u9PR0u6tKVSUlJdmVl6RNmzY5Ld8YGYahO++8U+vWrdMHH3ygjh07ul1HWVmZ9uzZo9jY2Hpooe8oLCzUgQMHnPazKYyXqlauXKk2bdpoxIgRbj2uqYyXjh07KiYmxm5MFBQU6JNPPnE6JupynmqMKhPb/fv36/3331erVq3crqO2+WgWP/zwg44dO+a0n01lzFR67rnn1LdvX/Xu3dvtxzbGMVPba3Tfvn0VGBho9/xnZWXp8OHDTp//upybPKZeP67WRL366qtGcHCwsWrVKmPv3r3GrbfeakRGRho5OTmGYRjGuHHjjHvvvddWfuvWrUZAQIDxyCOPGPv27TPS0tKMwMBAY8+ePd7qgsdNmTLFiIiIMLZs2WJkZ2fbbkVFRbYypx+XefPmGRs3bjQOHDhg7Nixw7jxxhuNkJAQ46uvvvJGF+rNPffcY2zZssU4ePCgsXXrVmPIkCFG69atjaNHjxqG0TTHS6WysjKjffv2xqxZs6rta0rj5fjx48auXbuMXbt2GZKMxYsXG7t27bJ96n/hwoVGZGSk8eabbxpffPGFMWrUKKNjx47Gb7/9Zqtj8ODBxpNPPmm7X9t5qjGo6biUlJQYV199tdG2bVtj9+7ddued4uJiWx2nH5fa5mNjUdOxOX78uDFz5kwjMzPTOHjwoPH+++8bffr0Mbp06WKcPHnSVkdTGzOV8vPzjdDQUGP58uUO6zDjmHHlNfr222832rdvb3zwwQfGZ599ZiQlJRlJSUl29XTr1s14/fXXbfddOTfVB5LbevLkk08a7du3N4KCgox+/foZ27Zts+275JJLjAkTJtiVX7NmjdG1a1cjKCjI6Nmzp7F+/foGbnH9kuTwtnLlSluZ04/LtGnTbMfQarUaV155pbFz586Gb3w9u+GGG4zY2FgjKCjIOOuss4wbbrjB+Oabb2z7m+J4qbRx40ZDkpGVlVVtX1MaL5s3b3Y4fyr7X15ebsyZM8ewWq1GcHCwcfnll1c7ZvHx8UZaWprdtprOU41BTcfl4MGDTs87mzdvttVx+nGpbT42FjUdm6KiImPo0KFGdHS0ERgYaMTHxxu33HJLtSS1qY2ZSs8884zRrFkzIy8vz2EdZhwzrrxG//bbb8Ydd9xhREVFGaGhocY111xjZGdnV6un6mNcOTfVB8sfjQEAAAAaPdbcAgAAwDRIbgEAAGAaJLcAAAAwDZJbAAAAmAbJLQAAAEyD5BYAAACmQXILAAAA0yC5BQAvuemmmzR69GhvN6POOnTooMcee8zbzQAAO/yIAwDUA4vFUuP+tLQ0TZ8+XYZhKDIysmEa5WE//fSTmjdvrtDQUEkVfV63bl2jTtgBNH4B3m4AAJhRdna27e/XXntNc+fOVVZWlm1bWFiYwsLCvNE0j4mOjvZ2EwCgGpYlAEA9iImJsd0iIiJksVjstoWFhVVblnDppZdq6tSpmjZtmqKiomS1WrVixQqdOHFCEydOVIsWLdS5c2dt2LDBLtaXX36p4cOHKywsTFarVePGjdPPP//stG0PPPCAzjvvPLttjz32mDp06GC7X9m2Rx55RLGxsWrVqpVSU1NVWlpqK1N1WULlY6+55hpZLBa7ugCgIZHcAoAPWb16tVq3bq1PP/1UU6dO1ZQpU3Tddddp4MCB2rlzp4YOHapx48apqKhIkpSXl6fBgwcrMTFRn332md59913l5ubq+uuvP+O2bN68WQcOHNDmzZu1evVqrVq1SqtWrXJYdvv27ZKklStXKjs723YfABoayS0A+JDevXvr/vvvV5cuXTR79myFhISodevWuuWWW9SlSxfNnTtXx44d0xdffCFJeuqpp5SYmKj58+ere/fuSkxM1PPPP6/Nmzfr66+/PqO2REVF6amnnlL37t111VVXacSIEUpPT3dYtnKJQmRkpGJiYliyAMBrWHMLAD4kISHB9re/v79atWqlXr162bZZrVZJ0tGjRyVJn3/+uTZv3uxw/e6BAwfUtWvXOrelZ8+e8vf3t92PjY3Vnj176lwfADQEklsA8CGBgYF29y0Wi922ym9hKC8vlyQVFhZq5MiRevjhh6vVFRsb6zCGn5+fTv+inKpraWtqS2VcAPBVJLcA0Ij16dNH//73v9WhQwcFBLh2So+OjlZOTo4Mw7Aly7t37z7jtgQGBqqsrOyM6wGAM8GaWwBoxFJTU/XLL79ozJgx2r59uw4cOKCNGzdq4sSJThPNSy+9VD/99JMWLVqkAwcOaOnSpdW+gaEuOnTooPT0dOXk5OjXX3894/oAoC5IbgGgEYuLi9PWrVtVVlamoUOHqlevXpo2bZoiIyPl5+f4FN+jRw8tW7ZMS5cuVe/evfXpp59q5syZZ9yWRx99VJs2bVK7du2UmJh4xvUBQF3wC2UAAAAwDa7cAgAAwDRIbgEAAGAaJLcAAAAwDZJbAAAAmAbJLQAAAEyD5BYAAACmQXILAAAA0yC5BQAAgGmQ3AIAAMA0SG4BAABgGiS3AAAAMA2SWwAAAJjG/wew1/RsxwzFtwAAAABJRU5ErkJggg==",
+                        "image/png": "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5s2aNm1avWXNNmZOf43es2ePysrK7P7+iYmJio+Pd/r3b8i5yVNIbj3s559/Vnl5uaKiouy2R0VFKTc31+FzcnNz3Srf0lVUVGjGjBkaMmSIzjvvPKflevTooeeee05vvPGGXnjhBVVUVGjw4MH64YcfmrG1TW/gwIFas2aN3n77ba1cuVKHDh3SJZdcouPHjzss39rGiyS9/vrrys/P10033eS0TGsZL6er+ru7MyYacp5q6YqLizV79mxNmDBBoaGhTsu5Ox9bqhEjRuj5559XWlqaFi9erPT0dI0cOVLl5eUOy7fGMbN27VqdccYZ9b71brYx4+g1Ojc3V1artdY/hvXlNlVlXH2OpwQ0ae2AA6mpqfr888/rXZOUlJSkpKQk2+PBgwerZ8+eevrpp/Xf//3fTd3MZjNy5Ejb/T59+mjgwIFKSEjQ+vXrXbpi0Bo8++yzGjlypGJjY52WaS3jBe4rKyvT+PHjZRiGVq5cWWfZ1jIfb7zxRtv93r17q0+fPurWrZt27typK6+80ost8x3PPfecJk6cWO8HU802Zlx9jfZlXLn1sI4dO8rf37/WJwjz8vIUHR3t8DnR0dFulW/J7rrrLv373//Wjh071LlzZ7eeGxgYqH79+umbb75potb5hvDwcJ1zzjlO+9maxoskHT58WO+8845uueUWt57XWsZL1d/dnTHRkPNUS1WV2B4+fFjbt2+v86qtI/XNR7M466yz1LFjR6f9bE1jRpLef/99ZWVluX3ekVr2mHH2Gh0dHa3S0lLl5+fbla8vt6kq4+pzPIXk1sOsVqsGDBigtLQ027aKigqlpaXZXVWqKSkpya68JG3fvt1p+ZbIMAzddddd2rhxo95991117drV7TrKy8u1f/9+xcTENEELfceJEyd08OBBp/1sDeOlptWrV6tTp04aNWqUW89rLeOla9euio6OthsThYWF+vjjj52OiYacp1qiqsT2wIEDeuedd9ShQwe366hvPprFDz/8oGPHjjntZ2sZM1WeffZZDRgwQH379nX7uS1xzNT3Gj1gwAAFBgba/f2zsrJ05MgRp3//hpybPKZJP67WSr388stGUFCQsWbNGuPLL780brvtNiM8PNzIzc01DMMwJk2aZPzlL3+xlf/www+NgIAA4+9//7vx1VdfGfPnzzcCAwON/fv3e6sLHnfHHXcYYWFhxs6dO42cnBzbraioyFbm9OPy0EMPGVu3bjUOHjxo7Nmzx7jxxhuN4OBg44svvvBGF5rMvffea+zcudM4dOiQ8eGHHxrDhg0zOnbsaBw9etQwjNY5XqqUl5cb8fHxxuzZs2vta03j5fjx48a+ffuMffv2GZKMpUuXGvv27bN96n/RokVGeHi48cYbbxifffaZMWbMGKNr167GqVOnbHUMHTrUePLJJ22P6ztPtQR1HZfS0lLj2muvNTp37mx8+umnduedkpISWx2nH5f65mNLUdexOX78uHHfffcZGRkZxqFDh4x33nnH6N+/v9G9e3ejuLjYVkdrGzNVCgoKjLZt2xorV650WIcZx4wrr9G33367ER8fb7z77rvGJ598YiQlJRlJSUl29fTo0cN47bXXbI9dOTc1BZLbJvLkk08a8fHxhtVqNS666CJj165dtn2XXXaZMWXKFLvy69evN8455xzDarUavXr1MjZv3tzMLW5akhzeVq9ebStz+nGZMWOG7RhGRUUZV199tbF3797mb3wTu+GGG4yYmBjDarUaZ555pnHDDTcY33zzjW1/axwvVbZu3WpIMrKysmrta03jZceOHQ7nT1X/KyoqjLlz5xpRUVFGUFCQceWVV9Y6ZgkJCcb8+fPtttV1nmoJ6jouhw4dcnre2bFjh62O049LffOxpajr2BQVFRnDhw83IiMjjcDAQCMhIcG49dZbayWprW3MVHn66aeNNm3aGPn5+Q7rMOOYceU1+tSpU8add95pREREGG3btjWuu+46Iycnp1Y9NZ/jyrmpKVh+bwwAAADQ4rHmFgAAAKZBcgsAAADTILkFAACAaZDcAgAAwDRIbgEAAGAaJLcAAAAwDZJbAAAAmAbJLQB4yU033aSxY8d6uxkN1qVLFz322GPebgYA2OFHHACgCVgsljr3z58/XzNnzpRhGAoPD2+eRnnYTz/9pHbt2qlt27aSKvu8cePGFp2wA2j5ArzdAAAwo5ycHNv9V155RfPmzVNWVpZtW0hIiEJCQrzRNI+JjIz0dhMAoBaWJQBAE4iOjrbdwsLCZLFY7LaFhITUWpZw+eWXa/r06ZoxY4YiIiIUFRWlVatW6eTJk5o6darOOOMMnX322dqyZYtdrM8//1wjR45USEiIoqKiNGnSJP38889O2/bggw/q/PPPt9v22GOPqUuXLrbHVW37+9//rpiYGHXo0EGpqakqKyuzlam5LKHqudddd50sFotdXQDQnEhuAcCHrF27Vh07dtTu3bs1ffp03XHHHbr++us1ePBg7d27V8OHD9ekSZNUVFQkScrPz9fQoUPVr18/ffLJJ3r77beVl5en8ePHN7otO3bs0MGDB7Vjxw6tXbtWa9as0Zo1axyWzczMlCStXr1aOTk5tscA0NxIbgHAh/Tt21cPPPCAunfvrjlz5ig4OFgdO3bUrbfequ7du2vevHk6duyYPvvsM0nSU089pX79+mnBggVKTExUv3799Nxzz2nHjh36+uuvG9WWiIgIPfXUU0pMTNQ111yjUaNGKS0tzWHZqiUK4eHhio6OZskCAK9hzS0A+JA+ffrY7vv7+6tDhw7q3bu3bVtUVJQk6ejRo5Kk//znP9qxY4fD9bsHDx7UOeec0+C29OrVS/7+/rbHMTEx2r9/f4PrA4DmQHILAD4kMDDQ7rHFYrHbVvUtDBUVFZKkEydOaPTo0Vq8eHGtumJiYhzG8PPz0+lflFNzLW1dbamKCwC+iuQWAFqw/v3769VXX1WXLl0UEODaKT0yMlK5ubkyDMOWLH/66aeNbktgYKDKy8sbXQ8ANAZrbgGgBUtNTdUvv/yiCRMmKDMzUwcPHtTWrVs1depUp4nm5Zdfrp9++klLlizRwYMHtXz58lrfwNAQXbp0UVpamnJzc/Xrr782uj4AaAiSWwBowWJjY/Xhhx+qvLxcw4cPV+/evTVjxgyFh4fLz8/xKb5nz55asWKFli9frr59+2r37t267777Gt2WRx99VNu3b1dcXJz69evX6PoAoCH4hTIAAACYBlduAQAAYBoktwAAADANklsAAACYBsktAAAATIPkFgAAAKZBcgsAAADTILkFAACAaZDcAgAAwDRIbgEAAGAaJLcAAAAwDZJbAAAAmAbJLQAAAEzj/wN8MMPtriCu6QAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 800x600 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
```

### Comparing `asdm-0.0.2/ASDM/ASDM.py` & `asdm-0.0.3/ASDM/ASDM.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
             'DELAY1': r'DELAY1(?=\()',
             'DELAY3': r'DELAY3(?=\()',
             'SMTH1': r'SMTH1(?=\()',
             'SMTH3': r'SMTH3(?=\()',
             'STEP': r'STEP(?=\()',
             'HISTORY': r'HISTORY(?=\()',
             'LOOKUP': r'LOOKUP(?=\()',
+            'SUM': r'SUM(?=\()',
         }
 
         self.names = {
             'ABSOLUTENAME': r'"[\s\S]*?"',
             'NAME': r'[a-zA-Z0-9_\?]*',
         }
 
@@ -226,14 +227,19 @@
                 'operand':['FUNC']
             },
             'LOOKUP__LPAREN__FUNC__COMMA__FUNC__RPAREN':{
                 'token':['FUNC', 'LOOKUP'],
                 'operator':['LOOKUP'],
                 'operand':['FUNC']
             },
+            'SUM__LPAREN__FUNC__RPAREN':{
+                'token':['FUNC', 'SUM'],
+                'operator':['SUM'],
+                'operand':['FUNC']
+            }
         }
         
         self.patterns_logic = {
             ### Logic ###
 
             'FUNC__GT__FUNC':{
                 'token':['FUNC', 'GT'],
@@ -569,20 +575,20 @@
                 return a * b
             except TypeError as e:
                 if type(a) is dict and type(b) is dict:
                     o = dict()
                     for k in a:
                         o[k] = a[k] * b[k]
                     return o
-                elif type(a) is dict and type(b) in [int, float]:
+                elif type(a) is dict and type(b) in [int, float, np.float_]:
                     o = dict()
                     for k in a:
                         o[k] = a[k] * b
                     return o
-                elif type(a) in [int, float] and type(b) is dict:
+                elif type(a) in [int, float, np.float_] and type(b) is dict:
                     o = dict()
                     for k in b:
                         o[k] = a * b[k]
                     return o
                 else:
                     raise e
 
@@ -592,20 +598,20 @@
             except TypeError as e:
                 if type(a) is dict and type(b) is dict:
                     # print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a/b', a, b)
                     o = dict()
                     for k in a:
                         o[k] = a[k] / b[k]
                     return o
-                elif type(a) is dict and type(b) in [int, float]:
+                elif type(a) is dict and type(b) in [int, float, np.float_]:
                     o = dict()
                     for k in a:
                         o[k] = a[k] / b
                     return o
-                elif type(a) in [int, float] and type(b) is dict:
+                elif type(a) in [int, float, np.float_] and type(b) is dict:
                     o = dict()
                     for k in b:
                         o[k] = a / b[k]
                     return o
                 else:
                     raise e
         
@@ -615,20 +621,20 @@
             except TypeError as e:
                 if type(a) is dict and type(b) is dict:
                     # print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a//b', a, b)
                     o = dict()
                     for k in a:
                         o[k] = a[k] // b[k]
                     return o
-                elif type(a) is dict and type(b) in [int, float]:
+                elif type(a) is dict and type(b) in [int, float, np.float_]:
                     o = dict()
                     for k in a:
                         o[k] = a[k] // b
                     return o
-                elif type(a) in [int, float] and type(b) is dict:
+                elif type(a) in [int, float, np.float_] and type(b) is dict:
                     o = dict()
                     for k in b:
                         o[k] = a // b[k]
                     return o
                 else:
                     raise e
                 
@@ -638,20 +644,20 @@
             except TypeError as e:
                 if type(a) is dict and type(b) is dict:
                     # print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a % b', a, b)
                     o = dict()
                     for k in a:
                         o[k] = a[k] % b[k]
                     return o
-                elif type(a) is dict and type(b) in [int, float]:
+                elif type(a) is dict and type(b) in [int, float, np.float_]:
                     o = dict()
                     for k in a:
                         o[k] = a[k] % b
                     return o
-                elif type(a) in [int, float] and type(b) is dict:
+                elif type(a) in [int, float, np.float_] and type(b) is dict:
                     o = dict()
                     for k in b:
                         o[k] = a % b[k]
                     return o
                 else:
                     raise e
 
@@ -704,394 +710,395 @@
             'DELAY1',
             'DELAY3',
             'HISTORY',
             'SMTH1',
             'SMTH3',
         ]
 
+        self.array_related_functions = [ # they take variable name as argument, not its value
+            'SUM',
+        ]
+
         self.lookup_functions = [
             'LOOKUP'
         ]
 
         self.custom_functions = {}
         self.time_expr_register = {}
         
         self.id_level = 0
 
         self.HEAD = "SOLVER"
 
-    def calculate_node(self, parsed_equation, node_id='root', subscript=None, verbose=False, var_name=''):
+    def calculate_node(self, parsed_equation, node_id='root', subscript=None, verbose=False, var_name=''):        
         self.id_level += 1
 
         if verbose:
             print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'processing node {} on subscript {}:'.format(node_id, subscript))
-        #     if type(parsed_equation) is dict:
-        #         for k, p in parsed_equation.items():
-        #             print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', k, p.nodes(data=True))
-        #     else:
-        #         print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', parsed_equation.nodes(data=True))
         
         if type(parsed_equation) is dict:  
             raise Exception('Parsed equation should not be a dict. var:', var_name)
-            # # This section is not active; only kept for potential future reference
-            # # if verbose:
-            # #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'type of parsed_equation: dict')
-            # value = dict()
-            # for sub, sub_equaton in parsed_equation.items():
-            #     if verbose:
-            #         print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'sub', sub)
-            #     value[sub] = self.calculate_node(parsed_equation=sub_equaton, node_id='root', subscript=sub, verbose=verbose)
-            # if verbose:
-            #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v1 Subscripted equation:', value)
-        else:
+
+        # if verbose:
+        #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'type of parsed_equation: graph')
+        if node_id == 'root':
+            node_id = list(parsed_equation.successors('root'))[0]
+        node = parsed_equation.nodes[node_id]
+        if verbose:
+            print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'node:', node_id, node)
+        operator = node['operator']
+        operands = node['operands']
+        if operator[0] == 'IS':
             # if verbose:
-            #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'type of parsed_equation: graph')
-            if node_id == 'root':
-                node_id = list(parsed_equation.successors('root'))[0]
-            node = parsed_equation.nodes[node_id]
+            #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'oprt1')
+            #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'o1')
+            value = np.float64(operands[0][1])
             if verbose:
-                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'node:', node_id, node)
-            operator = node['operator']
-            operands = node['operands']
-            if operator[0] == 'IS':
-                # if verbose:
-                #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'oprt1')
-                #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'o1')
-                value = np.float64(operands[0][1])
-                if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v2 IS:', value)
-            elif operator[0] == 'EQUALS':
-                if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'operator v3', operator)
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'operands v3', operands)
-                if operands[0][0] == 'NAME':
-                    if subscript:
-                        value = self.name_space[operands[0][1]]
-                        if type(value) is dict:
-                            value = value[subscript]
-                            if verbose:
-                                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v3.1.1', value)
-                        else:
-                            if verbose:
-                                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v3.1.2', value)
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v2 IS:', value)
+        elif operator[0] == 'EQUALS':
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'operator v3', operator)
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'operands v3', operands)
+            if operands[0][0] == 'NAME':
+                if subscript:
+                    value = self.name_space[operands[0][1]]
+                    if type(value) is dict:
+                        value = value[subscript]
+                        if verbose:
+                            print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v3.1.1', value)
                     else:
-                        value = self.name_space[operands[0][1]]
                         if verbose:
-                            print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v3.1.3', value, operands)
-                    if verbose:
-                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v3.1 Name:', value)
-                elif operands[0][0] == 'FUNC':
+                            print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v3.1.2', value)
+                else:
+                    value = self.name_space[operands[0][1]]
                     if verbose:
-                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'o3')
-                    value = self.calculate_node(parsed_equation=parsed_equation, node_id=node_id, subscript=subscript, verbose=verbose)
+                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v3.1.3', value, operands)
+                if verbose:
+                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v3.1 Name:', value)
+            elif operands[0][0] == 'FUNC':
+                if verbose:
+                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'o3')
+                value = self.calculate_node(parsed_equation=parsed_equation, node_id=node_id, subscript=subscript, verbose=verbose)
+                if verbose:
+                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v3.2 Func:', value)
+            else:
+                if verbose:
+                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'o4')
+                raise Exception("Type of oprand not implemented: {}".format(operands[0][0]))
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v3 Equals:', value)
+        
+        elif operator[0] == 'SPAREN': # TODO this part is too dynamic, therefore can be slow.
+            var_name = operands[0][1]
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1', subscript)
+            if len(operands) == 1: # only var_name; no subscript is specified
+                if verbose:
+                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.1')
+                # this could be 
+                # (1) this variable (var_name) is not subscripted therefore the only value of it should be used;
+                # (2) this variable (var_name) is subscripted in the same way as the variable using it (a contextual info is needed and provided in the arg subscript)
+                if subscript:
                     if verbose:
-                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v3.2 Func:', value)
+                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.1.1')
+                    value = self.name_space[var_name][subscript] 
                 else:
                     if verbose:
-                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'o4')
-                    raise Exception()
+                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.1.2')
+                    value = self.name_space[var_name]
                 if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v3 Equals:', value)
-            
-            elif operator[0] == 'SPAREN': # TODO this part is too dynamic, therefore can be slow. Need to resolve this when compiling.
-                var_name = operands[0][1]
+                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v4.1 Sparen without sub:', value)
+            else: # there are explicitly specified subscripts in oprands like a[b]
                 if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1', var_name, subscript)
-                if len(operands) == 1: # only var_name; no subscript is specified
+                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.2', 'subscript from operands:', operands[1:], 'subscript from context:', subscript)
+                # prioritise subscript from operands
+                try:
+                    subscript_from_operands = tuple(operand[1] for operand in operands[1:]) # use tuple to make it hashable
+                    value = self.name_space[var_name][subscript_from_operands]
                     if verbose:
-                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.1')
-                    # this could be 
-                    # (1) this variable (var_name) is not subscripted therefore the only value of it should be used;
-                    # (2) this variable (var_name) is subscripted in the same way as the variable using it (a contextual info is needed and provided in the arg subscript)
-                    if subscript:
-                        if verbose:
-                            print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.1.1')
-                        value = self.name_space[var_name][subscript] 
-                    else:
-                        if verbose:
-                            print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.1.2')
-                        value = self.name_space[var_name]
+                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.2.1')
+                except KeyError as e: # subscript in operands looks like a[Dimension_1, Element_1], inference needed
                     if verbose:
-                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v4.1 Sparen without sub:', value)
-                else: # there are explicitly specified subscripts in oprands
-                    # if verbose:
-                    #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.2')
-                    if subscript: # subscript is explicitly specified; like a[Element_1] or a[Dimension_1]
-                        if verbose:
-                            print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.2.0', subscript, self.dimension_elements)
-                        subscript_from_operands = list()
+                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.2.2')
+                    if subscript: # there's subscript in context
                         operands_containing_subscript = operands[1:]
+                        subscript_from_operands_with_replacement = list()
                         for i in range(len(operands_containing_subscript)):
                             if operands_containing_subscript[i][1] in self.dimension_elements.keys(): # it's sth like Dimension_1
                                 # if verbose:
-                                #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.2.0.1')
-                                subscript_from_operands.append(subscript[i]) # take the element from arg subscript in the same position to replace Dimension_1
+                                #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.2.2.1')
+                                subscript_from_operands_with_replacement.append(subscript[i]) # take the element from context subscript in the same position to replace Dimension_1
                             else: # it's sth like Element_1
                                 # if verbose:
-                                #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.2.0.2')
-                                subscript_from_operands.append(operands_containing_subscript[i][1]) # add to list directly
-                        subscript_from_operands = tuple(subscript_from_operands)
-                        # if verbose:
-                        #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.2.1', subscript_from_operands)
-                        value = self.name_space[var_name][subscript_from_operands] # try if subscript is Element_1
-
-                    else: # subscript is not explicitly specified
-                        # if verbose:
-                        #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.2.2')
-                        # like a[Dimension1] -> Which element of Dimension1 to use, 
-                        # depends on the other variable.
-
-                        subscript = tuple(operand[1] for operand in operands[1:]) # use tuple to make it hashable
+                                #     print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.2.2.2')
+                                subscript_from_operands_with_replacement.append(operands_containing_subscript[i][1]) # add to list directly
+                        subscript_from_operands_with_replacement = tuple(subscript_from_operands_with_replacement)
                         if verbose:
-                            print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'subscript of interest', subscript)
-                        value = self.name_space[var_name][subscript]
-                    if verbose:
-                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v4.2 Sparen with sub:', value)
-            
-            elif operator[0] == 'PAREN':
-                value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], verbose=verbose)
+                            print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'a1.2.2', subscript_from_operands_with_replacement)
+                        value = self.name_space[var_name][subscript_from_operands_with_replacement] # try if subscript is Element_1
+                    else: # there's no subscript in context
+                        raise e
+                        
                 if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v6 Paren:', value)
+                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v4.2 Sparen with sub:', value)
+        
+        elif operator[0] == 'PAREN':
+            value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], verbose=verbose)
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v6 Paren:', value)
 
-            elif operator[0] in self.built_in_functions.keys(): # plus, minus, con, etc.
-                if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'operator v7 Built-in operator:', operator, operands)
-                func_name = operator[0]
-                function = self.built_in_functions[func_name]
-                oprds = []
-                for operand in operands:
-                    if verbose:
-                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'oprd', operand)
-                    v = self.calculate_node(parsed_equation=parsed_equation, node_id=operand[2], subscript=subscript, verbose=verbose)
-                    if verbose:
-                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'value', v)
-                    oprds.append(v)
-                if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'oprds', oprds)
-                value = function(*oprds)
+        elif operator[0] in self.built_in_functions.keys(): # plus, minus, con, etc.
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'operator v7 Built-in operator:', operator, operands)
+            func_name = operator[0]
+            function = self.built_in_functions[func_name]
+            oprds = []
+            for operand in operands:
                 if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v7 Built-in operation:', value)
-            
-            elif operator[0] in self.custom_functions.keys(): # graph functions
+                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v7.1', 'oprd', operand)
+                v = self.calculate_node(parsed_equation=parsed_equation, node_id=operand[2], subscript=subscript, verbose=verbose)
                 if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'custom func operator', operator)
-                func_name = operator[0]
-                function = self.custom_functions[func_name]
-                oprds = []
-                for operand in operands:
-                    if verbose:
-                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'oprd', operand)
-                    v = self.calculate_node(parsed_equation=parsed_equation, node_id=operand[2], verbose=verbose)
-                    if verbose:
-                        print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'value', v)
-                    oprds.append(v)
+                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v7.2', 'value', v, subscript)
+                oprds.append(v)
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v7.3', 'oprds', oprds)
+            value = function(*oprds)
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v7 Built-in operation:', value)
+        
+        elif operator[0] in self.custom_functions.keys(): # graph functions
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'custom func operator', operator)
+            func_name = operator[0]
+            function = self.custom_functions[func_name]
+            oprds = []
+            for operand in operands:
                 if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'oprds', oprds)
-                value = function(*oprds)
+                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'oprd', operand)
+                v = self.calculate_node(parsed_equation=parsed_equation, node_id=operand[2], verbose=verbose)
                 if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v8 GraphFunc:', value)
+                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'value', v)
+                oprds.append(v)
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'oprds', oprds)
+            value = function(*oprds)
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v8 GraphFunc:', value)
 
-            elif operator[0] in self.time_related_functions: # init, delay, etc
-                if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'time-related func. operator:', operator, 'operands:', operands)
-                func_name = operator[0]
-                if func_name == 'INIT':
-                    if tuple(operands[0]) in self.time_expr_register.keys():
-                        value = self.time_expr_register[tuple(operands[0])]
-                    else:
-                        value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], verbose=verbose)
-                        self.time_expr_register[tuple(operands[0])] = value
-                elif func_name == 'DELAY':
-                    # expr value
-                    expr_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], verbose=verbose)
-                    if tuple(operands[0]) in self.time_expr_register.keys():
-                        self.time_expr_register[tuple(operands[0])].append(expr_value)
-                    else:
-                        self.time_expr_register[tuple(operands[0])] = [expr_value]
-                    
-                    # init value
-                    if len(operands) == 2: # there's no initial value specified -> use the delyed expr's initial value
-                        init_value = self.time_expr_register[tuple(operands[0])][0]
-                    elif len(operands) == 3: # there's an initial value specified
-                        init_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[2][2], verbose=verbose)
-                    else:
-                        raise Exception("Invalid initial value for DELAY in operands {}".format(operands))
+        elif operator[0] in self.time_related_functions: # init, delay, etc
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'time-related func. operator:', operator, 'operands:', operands)
+            func_name = operator[0]
+            if func_name == 'INIT':
+                if tuple(operands[0]) in self.time_expr_register.keys():
+                    value = self.time_expr_register[tuple(operands[0])]
+                else:
+                    value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], subscript=subscript, verbose=verbose)
+                    self.time_expr_register[tuple(operands[0])] = value
+            elif func_name == 'DELAY':
+                # expr value
+                expr_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], subscript=subscript, verbose=verbose)
+                if tuple(operands[0]) in self.time_expr_register.keys():
+                    self.time_expr_register[tuple(operands[0])].append(expr_value)
+                else:
+                    self.time_expr_register[tuple(operands[0])] = [expr_value]
+                
+                # init value
+                if len(operands) == 2: # there's no initial value specified -> use the delayed expr's initial value
+                    init_value = self.time_expr_register[tuple(operands[0])][0]
+                elif len(operands) == 3: # there's an initial value specified
+                    init_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[2][2], subscript=subscript, verbose=verbose)
+                else:
+                    raise Exception("Invalid initial value for DELAY in operands {}".format(operands))
 
-                    # delay time
-                    delay_time = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[1][2], verbose=verbose)
-                    if delay_time > (self.sim_specs['current_time'] - self.sim_specs['initial_time']): # (- initial_time) because simulation might not start from time 0
-                        value = init_value
-                    else:
-                        delay_steps = delay_time / self.sim_specs['dt']
-                        value = self.time_expr_register[tuple(operands[0])][-int(delay_steps+1)]
-                elif func_name == 'DELAY1':
-                    # args values
-                    order = 1
-                    expr_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], verbose=verbose)
-                    delay_time = self.calculate_node(parsed_equation=parsed_equation, node_id= operands[1][2], verbose=verbose)
-
-                    if len(operands) == 3:
-                        init_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[2][2], verbose=verbose)
-                    elif len(operands) == 2:
-                        init_value = expr_value
-                    else:
-                        raise Exception('Invalid number of args for DELAY1.')
-                    
-                    # register
-                    if tuple(operands[0]) not in self.time_expr_register.keys():
-                        self.time_expr_register[tuple(operands[0])] = list()
-                        for i in range(order):
-                            self.time_expr_register[tuple(operands[0])].append(delay_time/order*init_value)
-                    # outflows
-                    outflows = list()
+                # delay time
+                delay_time = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[1][2], subscript=subscript, verbose=verbose)
+                if delay_time > (self.sim_specs['current_time'] - self.sim_specs['initial_time']): # (- initial_time) because simulation might not start from time 0
+                    value = init_value
+                else:
+                    delay_steps = delay_time / self.sim_specs['dt']
+                    value = self.time_expr_register[tuple(operands[0])][-int(delay_steps+1)]
+            elif func_name == 'DELAY1':
+                # args values
+                order = 1
+                expr_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], subscript=subscript, verbose=verbose)
+                delay_time = self.calculate_node(parsed_equation=parsed_equation, node_id= operands[1][2], subscript=subscript, verbose=verbose)
+
+                if len(operands) == 3:
+                    init_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[2][2], subscript=subscript, verbose=verbose)
+                elif len(operands) == 2:
+                    init_value = expr_value
+                else:
+                    raise Exception('Invalid number of args for DELAY1.')
+                
+                # register
+                if tuple(operands[0]) not in self.time_expr_register.keys():
+                    self.time_expr_register[tuple(operands[0])] = list()
                     for i in range(order):
-                        outflows.append(self.time_expr_register[tuple(operands[0])][i]/(delay_time/order) * self.sim_specs['dt'])
-                        self.time_expr_register[tuple(operands[0])][i] -= outflows[i]
-                    # inflows
-                    self.time_expr_register[tuple(operands[0])][0] += expr_value * self.sim_specs['dt']
-                    for i in range(1, order):
-                        self.time_expr_register[tuple(operands[0])][i] += outflows[i-1]
-
-                    return outflows[-1] / self.sim_specs['dt']
-
-                elif func_name == 'DELAY3':
-                    # arg values
-                    order = 3
-                    expr_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], verbose=verbose)
-                    delay_time = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[1][2], verbose=verbose)
-                    if len(operands) == 3:
-                        init_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[2][2], verbose=verbose)
-                    elif len(operands) == 2:
-                        init_value = expr_value
-                    else:
-                        raise Exception('Invalid number of args for SMTH3.')
-                    
-                    # register
-                    if tuple(operands[0]) not in self.time_expr_register.keys():
-                        self.time_expr_register[tuple(operands[0])] = list()
-                        for i in range(order):
-                            self.time_expr_register[tuple(operands[0])].append(delay_time/order*init_value)
-                    # outflows
-                    outflows = list()
+                        self.time_expr_register[tuple(operands[0])].append(delay_time/order*init_value)
+                # outflows
+                outflows = list()
+                for i in range(order):
+                    outflows.append(self.time_expr_register[tuple(operands[0])][i]/(delay_time/order) * self.sim_specs['dt'])
+                    self.time_expr_register[tuple(operands[0])][i] -= outflows[i]
+                # inflows
+                self.time_expr_register[tuple(operands[0])][0] += expr_value * self.sim_specs['dt']
+                for i in range(1, order):
+                    self.time_expr_register[tuple(operands[0])][i] += outflows[i-1]
+
+                return outflows[-1] / self.sim_specs['dt']
+
+            elif func_name == 'DELAY3':
+                # arg values
+                order = 3
+                expr_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], subscript=subscript, verbose=verbose)
+                delay_time = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[1][2], subscript=subscript, verbose=verbose)
+                if len(operands) == 3:
+                    init_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[2][2], subscript=subscript, verbose=verbose)
+                elif len(operands) == 2:
+                    init_value = expr_value
+                else:
+                    raise Exception('Invalid number of args for SMTH3.')
+                
+                # register
+                if tuple(operands[0]) not in self.time_expr_register.keys():
+                    self.time_expr_register[tuple(operands[0])] = list()
                     for i in range(order):
-                        outflows.append(self.time_expr_register[tuple(operands[0])][i]/(delay_time/order) * self.sim_specs['dt'])
-                        self.time_expr_register[tuple(operands[0])][i] -= outflows[i]
-                    # inflows
-                    self.time_expr_register[tuple(operands[0])][0] += expr_value * self.sim_specs['dt']
-                    for i in range(1, order):
-                        self.time_expr_register[tuple(operands[0])][i] += outflows[i-1]
-
-                    return outflows[-1] / self.sim_specs['dt']
-
-                elif func_name == 'HISTORY':
-                    # expr value
-                    expr_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], verbose=verbose)
-                    if tuple(operands[0]) in self.time_expr_register.keys():
-                        self.time_expr_register[tuple(operands[0])].append(expr_value)
-                    else:
-                        self.time_expr_register[tuple(operands[0])] = [expr_value]
-                    
-                    # historical time
-                    historical_time = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[1][2], verbose=verbose)
-                    if historical_time > self.sim_specs['current_time']:
-                        value = 0
-                    else:
-                        historical_steps = (historical_time - self.sim_specs['initial_time']) / self.sim_specs['dt']
-                        value = self.time_expr_register[tuple(operands[0])][int(historical_steps)]
-                elif func_name == 'SMTH1':
-                    # arg values
-                    order = 1
-                    expr_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], verbose=verbose)
-                    smth_time = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[1][2], verbose=verbose)
-                    if len(operands) == 3:
-                        init_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[2][2], verbose=verbose)
-                    elif len(operands) == 2:
-                        init_value = expr_value
-                    else:
-                        raise Exception('Invalid number of args for SMTH1.')
-                    
-                    # register
-                    if tuple(operands[0]) not in self.time_expr_register.keys():
-                        self.time_expr_register[tuple(operands[0])] = list()
-                        for i in range(order):
-                            self.time_expr_register[tuple(operands[0])].append(smth_time/order*init_value)
-                    # outflows
-                    outflows = list()
+                        self.time_expr_register[tuple(operands[0])].append(delay_time/order*init_value)
+                # outflows
+                outflows = list()
+                for i in range(order):
+                    outflows.append(self.time_expr_register[tuple(operands[0])][i]/(delay_time/order) * self.sim_specs['dt'])
+                    self.time_expr_register[tuple(operands[0])][i] -= outflows[i]
+                # inflows
+                self.time_expr_register[tuple(operands[0])][0] += expr_value * self.sim_specs['dt']
+                for i in range(1, order):
+                    self.time_expr_register[tuple(operands[0])][i] += outflows[i-1]
+
+                return outflows[-1] / self.sim_specs['dt']
+
+            elif func_name == 'HISTORY':
+                # expr value
+                expr_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], subscript=subscript, verbose=verbose)
+                if tuple(operands[0]) in self.time_expr_register.keys():
+                    self.time_expr_register[tuple(operands[0])].append(expr_value)
+                else:
+                    self.time_expr_register[tuple(operands[0])] = [expr_value]
+                
+                # historical time
+                historical_time = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[1][2], subscript=subscript, verbose=verbose)
+                if historical_time > self.sim_specs['current_time'] or historical_time < self.sim_specs['initial_time']:
+                    value = 0
+                else:
+                    historical_steps = (historical_time - self.sim_specs['initial_time']) / self.sim_specs['dt']
+                    value = self.time_expr_register[tuple(operands[0])][int(historical_steps)]
+            elif func_name == 'SMTH1':
+                # arg values
+                order = 1
+                expr_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], subscript=subscript, verbose=verbose)
+                if type(expr_value) is dict:
+                    if subscript is not None:
+                        expr_value = expr_value[subscript]
+                    else:
+                        raise Exception('Invalid subscript.')
+                smth_time = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[1][2], subscript=subscript, verbose=verbose)
+                if len(operands) == 3:
+                    init_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[2][2], subscript=subscript, verbose=verbose)
+                elif len(operands) == 2:
+                    init_value = expr_value
+                else:
+                    raise Exception('Invalid number of args for SMTH1.')
+                
+                # register
+                if tuple(operands[0]) not in self.time_expr_register.keys():
+                    self.time_expr_register[tuple(operands[0])] = list()
                     for i in range(order):
-                        outflows.append(self.time_expr_register[tuple(operands[0])][i]/(smth_time/order) * self.sim_specs['dt'])
-                        self.time_expr_register[tuple(operands[0])][i] -= outflows[i]
-                    # inflows
-                    self.time_expr_register[tuple(operands[0])][0] += expr_value * self.sim_specs['dt']
-                    for i in range(1, order):
-                        self.time_expr_register[tuple(operands[0])][i] += outflows[i-1]
-
-                    return outflows[-1] / self.sim_specs['dt']
-
-                elif func_name == 'SMTH3':
-                    # arg values
-                    order = 3
-                    expr_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], verbose=verbose)
-                    smth_time = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[1][2], verbose=verbose)
-                    if len(operands) == 3:
-                        init_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[2][2], verbose=verbose)
-                    elif len(operands) == 2:
-                        init_value = expr_value
-                    else:
-                        raise Exception('Invalid number of args for SMTH3.')
-                    
-                    # register
-                    if tuple(operands[0]) not in self.time_expr_register.keys():
-                        self.time_expr_register[tuple(operands[0])] = list()
-                        for i in range(order):
-                            self.time_expr_register[tuple(operands[0])].append(smth_time/order*init_value)
-                    # outflows
-                    outflows = list()
+                        self.time_expr_register[tuple(operands[0])].append(smth_time/order*init_value)
+                # outflows
+                outflows = list()
+                for i in range(order):
+                    outflows.append(self.time_expr_register[tuple(operands[0])][i]/(smth_time/order) * self.sim_specs['dt'])
+                    self.time_expr_register[tuple(operands[0])][i] -= outflows[i]
+                # inflows
+                self.time_expr_register[tuple(operands[0])][0] += expr_value * self.sim_specs['dt']
+                for i in range(1, order):
+                    self.time_expr_register[tuple(operands[0])][i] += outflows[i-1]
+
+                return outflows[-1] / self.sim_specs['dt']
+
+            elif func_name == 'SMTH3':
+                # arg values
+                order = 3
+                expr_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[0][2], subscript=subscript, verbose=verbose)
+                if type(expr_value) is dict:
+                    if subscript is not None:
+                        expr_value = expr_value[subscript]
+                    else:
+                        raise Exception('Invalid subscript.')
+                smth_time = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[1][2], subscript=subscript, verbose=verbose)
+                if len(operands) == 3:
+                    init_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[2][2], subscript=subscript, verbose=verbose)
+                elif len(operands) == 2:
+                    init_value = expr_value
+                else:
+                    raise Exception('Invalid number of args for SMTH3.')
+                
+                # register
+                if tuple(operands[0]) not in self.time_expr_register.keys():
+                    self.time_expr_register[tuple(operands[0])] = list()
                     for i in range(order):
-                        outflows.append(self.time_expr_register[tuple(operands[0])][i]/(smth_time/order) * self.sim_specs['dt'])
-                        self.time_expr_register[tuple(operands[0])][i] -= outflows[i]
-                    # inflows
-                    self.time_expr_register[tuple(operands[0])][0] += expr_value * self.sim_specs['dt']
-                    for i in range(1, order):
-                        self.time_expr_register[tuple(operands[0])][i] += outflows[i-1]
+                        self.time_expr_register[tuple(operands[0])].append(smth_time/order*init_value)
+                # outflows
+                outflows = list()
+                for i in range(order):
+                    outflows.append(self.time_expr_register[tuple(operands[0])][i]/(smth_time/order) * self.sim_specs['dt'])
+                    self.time_expr_register[tuple(operands[0])][i] -= outflows[i]
+                # inflows
+                self.time_expr_register[tuple(operands[0])][0] += expr_value * self.sim_specs['dt']
+                for i in range(1, order):
+                    self.time_expr_register[tuple(operands[0])][i] += outflows[i-1]
 
-                    return outflows[-1] / self.sim_specs['dt']
-                else:
-                    raise Exception('Unknown time-related operator {}'.format(operator[0]))
-                if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v9 Time-related Func:', value)
-            elif operator[0] in self.lookup_functions: # LOOKUP
-                if verbose:
-                    print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'Lookup func. operator:', operator, 'operands:', operands)
-                func_name = operator[0]
-                if func_name == 'LOOKUP':
-                    look_up_func_node = operands[0][2]
-                    look_up_func_name = parsed_equation.nodes[look_up_func_node]['operands'][0][1]
-                    look_up_func = self.graph_functions[look_up_func_name]
-                    input_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[1][2], verbose=verbose)
-                    value = look_up_func(input_value)
-                else:
-                    raise Exception('Unknown Lookup function {}'.format(operator[0]))
+                return outflows[-1] / self.sim_specs['dt']
             else:
-                raise Exception('Unknown operator {}'.format(operator[0]))
+                raise Exception('Unknown time-related operator {}'.format(operator[0]))
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v9 Time-related Func:', value)
+        elif operator[0] in self.array_related_functions: # Array-RELATED
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'array-related func. operator:', operator, 'operands:', operands)
+            func_name = operator[0]
+            if func_name == 'SUM':
+                arrayed_var_name = parsed_equation.nodes[operands[0][2]]['operands'][0][1]
+                sum_array = 0
+                for _, sub_val in self.name_space[arrayed_var_name].items():
+                    sum_array += sub_val
+                value = sum_array
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'v10 Array-related Func:', value)
+        elif operator[0] in self.lookup_functions: # LOOKUP
+            if verbose:
+                print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'Lookup func. operator:', operator, 'operands:', operands)
+            func_name = operator[0]
+            if func_name == 'LOOKUP':
+                look_up_func_node = operands[0][2]
+                look_up_func_name = parsed_equation.nodes[look_up_func_node]['operands'][0][1]
+                look_up_func = self.graph_functions[look_up_func_name]
+                input_value = self.calculate_node(parsed_equation=parsed_equation, node_id=operands[1][2], verbose=verbose)
+                value = look_up_func(input_value)
+            else:
+                raise Exception('Unknown Lookup function {}'.format(operator[0]))
+        else:
+            raise Exception('Unknown operator {}'.format(operator[0]))
         
         self.id_level -= 1
         
         if verbose:
             print('\t'*self.id_level+self.HEAD+' [ '+var_name+' ] ', 'value for {} {}'.format(node_id, subscript), value)
 
-        if subscript is None:
-            if type(value) is dict:
-                raise Exception('Value cannot be dict if subscript is None. Var: {}'.format(var_name))
-            else:
-                return value
-        else:
-            if type(value) is dict:
-                return value[subscript]
-            else:
-                return value
+        return value
 
 
 class GraphFunc(object):
     def __init__(self, yscale, ypts, xscale=None, xpts=None):
         self.yscale = yscale
         self.ypts = ypts
         self.eqn = None
@@ -1180,14 +1187,43 @@
 
 
 class Stock(object):
     def __init__(self):
         self.initialised = False
 
 
+class DataFeeder(object):
+    def __init__(self, data, from_time=0, data_dt=1):
+        """
+        data: a list
+
+        """
+        self.from_time =from_time
+        self.time_data = dict()
+        time = self.from_time
+        for d in data:
+            self.time_data[time] = d
+            time += data_dt
+        # print(self.time_data)
+        self.last_success_time = None
+
+    def __call__(self, current_time): # make a datafeeder callable
+        try:
+            d = self.time_data[current_time]
+            self.last_success_time = current_time
+        except KeyError:
+            if current_time < self.from_time:
+                raise Exception("Current time < external data starting time.")
+            elif current_time > list(self.time_data.keys())[-1]:
+                raise Exception("Current time > external data ending time.")
+            else:
+                d = self.time_data[self.last_success_time]
+        return(np.float64(d))
+
+
 class Structure(object):
     # equations
     def __init__(self, from_xmile=None):
         # Debug
         self.HEAD = 'ENGINE'
         self.debug_level = 0
 
@@ -1340,27 +1376,24 @@
                     ypts = [float(t) for t in gf.find('ypts').text.split(',')]
 
                     equation = GraphFunc(yscale=yscale, ypts=ypts, xscale=xscale, xpts=xpts)
                     return equation
 
                 # create var subscripted equation
                 def subscripted_equation(var):
-                    # print('Reading variable from XMILE: {}'.format(var.get('name')))
                     if var.find('dimensions'):
-                        self.var_dimensions[var.get('name')] = list()
-                        # print('Processing XMILE subscripted definition for:', var.get('name'))
+                        self.var_dimensions[self.name_handler(var.get('name'))] = list()
                         var_dimensions = var.find('dimensions').findAll('dim')
                         # print('Found dimensions {}:'.format(var), var_dimensions)
 
                         var_dims = dict()
                         for dimension in var_dimensions:
-                            name = dimension.get('name')
-                            self.var_dimensions[var.get('name')].append(name)
-                            # print('dim name:', name)
-                            var_dims[name] = dims[name]
+                            dim_name = dimension.get('name')
+                            self.var_dimensions[self.name_handler(var.get('name'))].append(dim_name)
+                            var_dims[dim_name] = dims[dim_name]
                         
                         var_subscripted_eqn = dict()
                         var_elements = var.findAll('element')
                         if len(var_elements) != 0:
                             for var_element in var_elements:
 
                                 element_combination_text = var_element.get('subscript') # something like "1, First"
@@ -1387,25 +1420,24 @@
                             elif var.find('gf'):
                                 equation = read_graph_func(var)
                                 equation.eqn = var.find('eqn').text
                             elif var.find('eqn'):
                                 var_equation = var.find('eqn').text
                                 equation = var_equation
                             else:
-                                raise Exception('No meaningful definition found for variable {}'.format(var.get('name')))
+                                raise Exception('No meaningful definition found for variable {}'.format(self.name_handler(var.get('name'))))
                             
                             # fetch lists of elements and generate elements trings
                             element_combinations = product(*list(var_dims.values()))
 
                             for ect in element_combinations:
                                 var_subscripted_eqn[ect] =equation
                         return(var_subscripted_eqn)
                     else:
-                        self.var_dimensions[var.get('name')] = None
-                        # print('Processing XMILE definition for:', var.get('name'))
+                        self.var_dimensions[self.name_handler(var.get('name'))] = None
                         var_subscripted_eqn = dict()
                         if var.find('conveyor'):
                             equation = var.find('eqn').text
                             length = var.find('len').text
                             equation = Conveyor(length, equation)
                         elif var.find('gf'):
                             equation = read_graph_func(var)
@@ -1570,17 +1602,23 @@
             parsed_equation_val = self.parser.parse(equation_init_value)
 
             return [ # using list to store [len_eqn, val_eqn]. Don't use {'len':xxx, 'val':xxx} to avoid confusion with subscripted equation.
                 parsed_equation_len, 
                 parsed_equation_val
                 ]
 
-        else:
+        elif type(equation) is DataFeeder:
+            return equation
+
+        elif type(equation) in [str, int, float, np.int_, np.float_]:
             parsed_equation = self.parser.parse(equation)
             return parsed_equation
+
+        else:
+            raise Exception('Unsupported equation {} type {}'.format(equation, type(equation)))
     
     def parse_0(self, equations, parsed_equations, verbose=False):
         for var, equation in equations.items():
             if verbose:
                 print(self.HEAD, "Parsing:", var)
                 print(self.HEAD, "    Eqn:", equation)
             
@@ -1598,295 +1636,332 @@
 
         self.parse_0(self.stock_equations, self.stock_equations_parsed, verbose=verbose)
         self.parse_0(self.flow_equations, self.flow_equations_parsed, verbose=verbose)
         self.parse_0(self.aux_equations, self.aux_equations_parsed, verbose=verbose)
         
     def is_dependent(self, var1, var2):
         # determine if var2 depends on var1, i.e., var1 --> var2 or var1 appears in var2's equation
-        dependent = False
+        
+        def is_dependent_sub(var1, parsed_equation_var2, dependent=False):
+            leafs = [x for x in parsed_equation_var2.nodes() if parsed_equation_var2.out_degree(x)==0]
+            for leaf in leafs:
+                if parsed_equation_var2.nodes[leaf]['operator'][0] in ['EQUALS', 'SPAREN']:
+                    operands = parsed_equation_var2.nodes[leaf]['operands']
+                    if operands[0][0] == 'NUMBER': # if 'NUMBER' then pass, as numbers (e.g. 100) do not have a node
+                        pass
+                    elif operands[0][0] == 'NAME': # this refers to a variable like 'a'
+                        var_dependent = operands[0][1]
+                        if var_dependent == var1:
+                            dependent = True
+                            break
+                    elif operands[0][0] == 'FUNC': # this refers to a subscripted variable like 'a[ele1]'
+                        # need to find that 'SPAREN' node
+                        var_dependent_node_id = operands[0][2]
+                        var_dependent = parsed_equation_var2.nodes[var_dependent_node_id]['operands'][0][1]
+                        if var_dependent == var1:
+                            dependent = True
+                            break
+            return dependent
+        
         parsed_equation_var2 = (self.stock_equations_parsed | self.flow_equations_parsed | self.aux_equations_parsed)[var2]
-        leafs = [x for x in parsed_equation_var2.nodes() if parsed_equation_var2.out_degree(x)==0]
-        for leaf in leafs:
-            if parsed_equation_var2.nodes[leaf]['operator'][0] in ['EQUALS', 'SPAREN']:
-                operands = parsed_equation_var2.nodes[leaf]['operands']
-                if operands[0][0] == 'NUMBER': # if 'NUMBER' then pass, as numbers (e.g. 100) do not have a node
-                    pass
-                elif operands[0][0] == 'NAME': # this refers to a variable like 'a'
-                    var_dependent = operands[0][1]
-                    if var_dependent == var1:
-                        dependent = True
-                        break
-                elif operands[0][0] == 'FUNC': # this refers to a subscripted variable like 'a[ele1]'
-                    # need to find that 'SPAREN' node
-                    var_dependent_node_id = operands[0][2]
-                    var_dependent = parsed_equation_var2.nodes[var_dependent_node_id]['operands'][0][1]
-                    if var_dependent == var1:
-                        dependent = True
-                        break
-        return dependent
+        if type(parsed_equation_var2) is dict:
+            for _, sub_eqn in parsed_equation_var2.items():
+                dependent = is_dependent_sub(var1, sub_eqn)
+                if dependent:
+                    return True
+            return False
+        else:
+            return is_dependent_sub(var1, parsed_equation_var2)
 
-    def calculate_dependents(self, parsed_equation):
+    def calculate_dependents(self, parsed_equation, verbose=False):
         leafs = [x for x in parsed_equation.nodes() if parsed_equation.out_degree(x)==0]
         for leaf in leafs:
             # print('i4.1')
             if parsed_equation.nodes[leaf]['operator'][0] in ['EQUALS', 'SPAREN']:
                 operands = parsed_equation.nodes[leaf]['operands']
                 # print('i5', operands)
                 if operands[0][0] == 'NUMBER': # if 'NUMBER' then pass, as numbers (e.g. 100) do not have a node
                     # print('i5.0') 
                     pass
                 elif operands[0][0] == 'NAME': # this refers to a variable like 'a'
                     # print('i5.1', operands[0][0])
                     var_dependent = operands[0][1]
                     # print('i5.2', var_dependent)
-                    self.calculate_variable_dynamic(var=var_dependent)
+                    self.calculate_variable_dynamic(var=var_dependent, verbose=verbose)
                 elif operands[0][0] == 'FUNC': # this refers to a subscripted variable like 'a[ele1]'
                     # print('i5.3')
                     # need to find that 'SPAREN' node
                     var_dependent_node_id = operands[0][2]
                     var_dependent = parsed_equation.nodes[var_dependent_node_id]['operands'][0][1]
                     # print('var_dependent2', var_dependent)
-                    self.calculate_variable_dynamic(var=var_dependent)
+                    self.calculate_variable_dynamic(var=var_dependent, verbose=verbose)
     
     def calculate_variable_dynamic(self, var, subscript=None, verbose=False, leak_frac=False, conveyor_init=False, conveyor_len=False):
         # print("\nEngine Calculating: {:<15} on subscript {}".format(var, subscript), '\n', 'name_space:', self.name_space, '\n', 'flow_effects', self.stock_shadow_values)
-
+        # print("Engine Calculating: {:<15} on subscript {}".format(var, subscript))
+        # debug
         if var == 'TIME':
             return
+        
+        if subscript is not None:
+            parsed_equation = (self.stock_equations_parsed | self.flow_equations_parsed | self.aux_equations_parsed)[var][subscript]
         else:
-            if subscript is not None:
-                parsed_equation = (self.stock_equations_parsed | self.flow_equations_parsed | self.aux_equations_parsed)[var][subscript]
-            else:
-                parsed_equation = (self.stock_equations_parsed | self.flow_equations_parsed | self.aux_equations_parsed)[var]
-            
-            # proceed to the 'real' calculation
-            # A: var is a Conveyor
-            if var in self.conveyors:
-                # print('Calculating Conveyor {}'.format(var))
-                if not (conveyor_init or conveyor_len):
-                    if not self.conveyors[var]['conveyor'].is_initialized:
-                        # print('Initialising {}'.format(var))
-                        # when initialising, equation of the conveyor needs to be evaluated, setting flag conveyor_len to True 
-                        self.calculate_variable_dynamic(var=var, subscript=subscript, verbose=verbose, conveyor_len=True)
-                        conveyor_length = self.conveyors[var]['len']
-                        length_steps = int(conveyor_length/self.sim_specs['dt'])
-                        
-                        # when initialising, equation of the conveyor needs to be evaluated, setting flag conveyor_init to True 
-                        self.calculate_variable_dynamic(var=var, subscript=subscript, verbose=verbose, conveyor_init=True)
-                        conveyor_init_value = self.conveyors[var]['val']
-                        
-                        leak_flows = self.conveyors[var]['leakflow']
-                        if len(leak_flows) == 0:
-                            leak_fraction = 0
-                        else:
-                            for leak_flow in leak_flows.keys():
-                                self.calculate_variable_dynamic(var=leak_flow, subscript=subscript, verbose=verbose, leak_frac=True)
-                                leak_fraction = self.conveyors[var]['leakflow'][leak_flow] # TODO multiple leakflows
-                        self.conveyors[var]['conveyor'].initialize(length_steps, conveyor_init_value, leak_fraction)
-                        
-                        # put initialised conveyor value to name_space
-                        value = self.conveyors[var]['conveyor'].level()
-                        self.name_space[var] = value
+            parsed_equation = (self.stock_equations_parsed | self.flow_equations_parsed | self.aux_equations_parsed)[var]
+        
+        # DataFeeder - external data
+        if type(parsed_equation) is DataFeeder:
+            if var not in self.name_space:
+                self.name_space[var] = parsed_equation(self.sim_specs['current_time'])
+
+        # A: var is a Conveyor
+        if var in self.conveyors:
+            # print('Calculating Conveyor {}'.format(var))
+            if not (conveyor_init or conveyor_len):
+                if not self.conveyors[var]['conveyor'].is_initialized:
+                    # print('Initialising {}'.format(var))
+                    # when initialising, equation of the conveyor needs to be evaluated, setting flag conveyor_len to True 
+                    self.calculate_variable_dynamic(var=var, subscript=subscript, verbose=verbose, conveyor_len=True)
+                    conveyor_length = self.conveyors[var]['len']
+                    length_steps = int(conveyor_length/self.sim_specs['dt'])
                     
-                    if var not in self.stock_shadow_values:
-                        # print("Updatting {} and its outflows".format(var))
-                        # print("    Name space1:", self.name_space)
-                        # leak
-                        for leak_flow, leak_fraction in self.conveyors[var]['leakflow'].items():
-                            if leak_flow not in self.name_space: 
-                                # print('    Calculating leakflow {} for {}'.format(leak_flow, var))
-                                leaked_value = self.conveyors[var]['conveyor'].leak_linear()
-                                self.name_space[leak_flow] = leaked_value / self.sim_specs['dt'] # TODO: we should also consider when leak flows are subscripted
-                        # out
-                        for outputflow in self.conveyors[var]['outputflow']:
-                            if outputflow not in self.name_space:
-                                # print('    Calculating outflow {} for {}'.format(outputflow, var))
-                                outflow_value = self.conveyors[var]['conveyor'].outflow()
-                                self.name_space[outputflow] = outflow_value / self.sim_specs['dt']
-                        # print("    Name space2:", self.name_space)
-                        self.stock_shadow_values[var] = self.conveyors[var]['conveyor'].level()
-
-                elif conveyor_len:
-                    # print('Calculating LEN for {}'.format(var))
-                    # it is the intitial value of the conveyoer
-                    parsed_equation = self.stock_equations_parsed[var][0]
-                    self.calculate_dependents(parsed_equation=parsed_equation)
-                    self.conveyors[var]['len'] = self.solver.calculate_node(parsed_equation=parsed_equation, verbose=verbose, var_name=var)
-                
-                elif conveyor_init:
-                    # print('Calculating INIT VAL for {}'.format(var))
-                    # it is the intitial value of the conveyoer
-                    parsed_equation = self.stock_equations_parsed[var][1]
-                    self.calculate_dependents(parsed_equation=parsed_equation)
-                    self.conveyors[var]['val'] = self.solver.calculate_node(parsed_equation=parsed_equation, verbose=verbose, var_name=var)
-            
-            # B: var is a normal stock
-            elif var not in self.conveyors and var in self.stocks:
-                if not self.stocks[var].initialised:
-                    # print('Stock {} not initialised'.format(var))
-                    if type(parsed_equation) is dict:
-                        for k, sub_parsed_equation in parsed_equation.items():
-                            # self.calculate_variable_dynamic(var=var, subscript=k)
-                            self.calculate_dependents(parsed_equation=sub_parsed_equation)
-                            value = self.solver.calculate_node(parsed_equation=sub_parsed_equation, subscript=k, verbose=verbose, var_name=var)
-                            if var not in self.name_space:
-                                self.name_space[var] = dict()
-                            self.name_space[var][k] = value
-                    else:
-                        self.calculate_dependents(parsed_equation=parsed_equation)
-                        value = self.solver.calculate_node(parsed_equation=parsed_equation, subscript=subscript, verbose=verbose, var_name=var)
-                        self.name_space[var] = value
-                    self.stocks[var].initialised = True
+                    # when initialising, equation of the conveyor needs to be evaluated, setting flag conveyor_init to True 
+                    self.calculate_variable_dynamic(var=var, subscript=subscript, verbose=verbose, conveyor_init=True)
+                    conveyor_init_value = self.conveyors[var]['val']
                     
-                # if the stock's shadow value has not been calculated for this dt:
+                    leak_flows = self.conveyors[var]['leakflow']
+                    if len(leak_flows) == 0:
+                        leak_fraction = 0
+                    else:
+                        for leak_flow in leak_flows.keys():
+                            self.calculate_variable_dynamic(var=leak_flow, subscript=subscript, verbose=verbose, leak_frac=True)
+                            leak_fraction = self.conveyors[var]['leakflow'][leak_flow] # TODO multiple leakflows
+                    self.conveyors[var]['conveyor'].initialize(length_steps, conveyor_init_value, leak_fraction)
+                    
+                    # put initialised conveyor value to name_space
+                    value = self.conveyors[var]['conveyor'].level()
+                    self.name_space[var] = value
+                
                 if var not in self.stock_shadow_values:
-                    # load stock's value from last dt from name_space
-                    self.stock_shadow_values[var] = deepcopy(self.name_space[var])
-                    if var in self.stock_flows: # some stocks are not connected to any flow
-                        if 'in' in self.stock_flows[var]:
-                            in_flows = self.stock_flows[var]['in']
-                            for in_flow in in_flows:
-                                if in_flow not in self.name_space:
-                                    self.calculate_variable_dynamic(var=in_flow, subscript=subscript, verbose=verbose)
-                                if var in self.stock_non_negative:
-                                    if type(self.name_space[in_flow]) is not dict:
-                                        if self.stock_shadow_values[var] + self.name_space[in_flow] * self.sim_specs['dt'] < 0:
-                                            self.name_space[in_flow] = self.stock_shadow_values[var] * -1 / self.sim_specs['dt']
-                                            self.stock_shadow_values[var] = 0
-                                        else:
-                                            self.stock_shadow_values[var] += self.name_space[in_flow] * self.sim_specs['dt']
+                    # print("Updatting {} and its outflows".format(var))
+                    # print("    Name space1:", self.name_space)
+                    # leak
+                    for leak_flow, leak_fraction in self.conveyors[var]['leakflow'].items():
+                        if leak_flow not in self.name_space: 
+                            # print('    Calculating leakflow {} for {}'.format(leak_flow, var))
+                            leaked_value = self.conveyors[var]['conveyor'].leak_linear()
+                            self.name_space[leak_flow] = leaked_value / self.sim_specs['dt'] # TODO: we should also consider when leak flows are subscripted
+                    # out
+                    for outputflow in self.conveyors[var]['outputflow']:
+                        if outputflow not in self.name_space:
+                            # print('    Calculating outflow {} for {}'.format(outputflow, var))
+                            outflow_value = self.conveyors[var]['conveyor'].outflow()
+                            self.name_space[outputflow] = outflow_value / self.sim_specs['dt']
+                    # print("    Name space2:", self.name_space)
+                    self.stock_shadow_values[var] = self.conveyors[var]['conveyor'].level()
+
+            elif conveyor_len:
+                # print('Calculating LEN for {}'.format(var))
+                # it is the intitial value of the conveyoer
+                parsed_equation = self.stock_equations_parsed[var][0]
+                self.calculate_dependents(parsed_equation=parsed_equation, verbose=verbose)
+                self.conveyors[var]['len'] = self.solver.calculate_node(parsed_equation=parsed_equation, verbose=verbose, var_name=var)
+            
+            elif conveyor_init:
+                # print('Calculating INIT VAL for {}'.format(var))
+                # it is the intitial value of the conveyoer
+                parsed_equation = self.stock_equations_parsed[var][1]
+                self.calculate_dependents(parsed_equation=parsed_equation, verbose=verbose)
+                self.conveyors[var]['val'] = self.solver.calculate_node(parsed_equation=parsed_equation, verbose=verbose, var_name=var)
+        
+        # B: var is a normal stock
+        elif var not in self.conveyors and var in self.stocks:
+            if not self.stocks[var].initialised:
+                # print('Stock {} not initialised'.format(var))
+                if type(parsed_equation) is dict:
+                    for sub, sub_parsed_equation in parsed_equation.items():
+                        self.calculate_dependents(parsed_equation=sub_parsed_equation, verbose=verbose)
+                        value = self.solver.calculate_node(parsed_equation=sub_parsed_equation, subscript=sub, verbose=verbose, var_name=var)
+                        if var not in self.name_space:
+                            self.name_space[var] = dict()
+                        self.name_space[var][sub] = value
+                elif var in self.var_dimensions and self.var_dimensions[var] is not None: # The variable is subscripted but all elements uses the same equation
+                    self.calculate_dependents(parsed_equation=parsed_equation, verbose=verbose)
+                    for sub in self.dimension_elements[self.var_dimensions[var]]:
+                        value = self.solver.calculate_node(parsed_equation=parsed_equation, subscript=sub, verbose=verbose, var_name=var)
+                        if var not in self.name_space:
+                            self.name_space[var] = dict()
+                        self.name_space[var][sub] = value
+                else: # The variable is not subscripted
+                    self.calculate_dependents(parsed_equation=parsed_equation, verbose=verbose)
+                    value = self.solver.calculate_node(parsed_equation=parsed_equation, subscript=subscript, verbose=verbose, var_name=var)
+                    self.name_space[var] = value
+                self.stocks[var].initialised = True
+                
+            # if the stock's shadow value has not been calculated for this dt:
+            if var not in self.stock_shadow_values:
+                # load stock's value from last dt from name_space
+                self.stock_shadow_values[var] = deepcopy(self.name_space[var])
+                if var in self.stock_flows: # some stocks are not connected to any flow
+                    if 'in' in self.stock_flows[var]:
+                        in_flows = self.stock_flows[var]['in']
+                        for in_flow in in_flows:
+                            if in_flow not in self.name_space:
+                                self.calculate_variable_dynamic(var=in_flow, subscript=subscript, verbose=verbose)
+                            if var in self.stock_non_negative:
+                                if type(self.name_space[in_flow]) is not dict:
+                                    if self.stock_shadow_values[var] + self.name_space[in_flow] * self.sim_specs['dt'] < 0:
+                                        self.name_space[in_flow] = self.stock_shadow_values[var] * -1 / self.sim_specs['dt']
+                                        self.stock_shadow_values[var] = 0
                                     else:
-                                        for sub, subval in self.name_space[in_flow].items():
-                                            if self.stock_shadow_values[var][sub] + subval * self.sim_specs['dt'] < 0:
-                                                self.name_space[in_flow][sub] = self.stock_shadow_values[var][sub] * -1 / self.sim_specs['dt']
-                                                self.stock_shadow_values[var][sub] = 0
-                                            else:
-                                                self.stock_shadow_values[var][sub] += subval * self.sim_specs['dt']
-                                    
-                                else:
-                                    if type(self.name_space[in_flow]) is not dict:
                                         self.stock_shadow_values[var] += self.name_space[in_flow] * self.sim_specs['dt']
-                                    else:
-                                        for sub, subval in self.name_space[in_flow].items():
-                                            self.stock_shadow_values[var][sub] += subval * self.sim_specs['dt']
-                        if 'out' in self.stock_flows[var]:
-                            out_flows = self.stock_flows[var]['out']
-                            
-                            # outflow prioritisation
-                            # rule 1: first added first
-                            # rule 2: dependents ranked higher
-                            if len(out_flows) > 1:
-                                for i in range(len(out_flows)-1, 0, -1):
-                                    for j in range(i):
-                                        if self.is_dependent(out_flows[j+1], out_flows[j]):
-                                            temp = out_flows[j+1]
-                                            out_flows[j+1] = out_flows[j]
-                                            out_flows[j] = temp
-
-                            for out_flow in out_flows:
-                                if out_flow not in self.name_space:
-                                    self.calculate_variable_dynamic(var=out_flow, subscript=subscript, verbose=verbose)
-                                if var in self.stock_non_negative:
-                                    if type(self.name_space[out_flow]) is not dict:
-                                        if self.stock_shadow_values[var] - self.name_space[out_flow] * self.sim_specs['dt'] < 0:
-                                            self.name_space[out_flow] = self.stock_shadow_values[var] / self.sim_specs['dt']
-                                            self.stock_shadow_values[var] = 0
+                                else:
+                                    for sub, subval in self.name_space[in_flow].items():
+                                        if self.stock_shadow_values[var][sub] + subval * self.sim_specs['dt'] < 0:
+                                            self.name_space[in_flow][sub] = self.stock_shadow_values[var][sub] * -1 / self.sim_specs['dt']
+                                            self.stock_shadow_values[var][sub] = 0
                                         else:
-                                            self.stock_shadow_values[var] -= self.name_space[out_flow] * self.sim_specs['dt']
-                                    else:
-                                        for sub, subval in self.name_space[out_flow].items():
-                                            if self.stock_shadow_values[var][sub] - subval * self.sim_specs['dt'] < 0:
-                                                self.name_space[out_flow][sub] = self.stock_shadow_values[var][sub] / self.sim_specs['dt']
-                                                self.stock_shadow_values[var][sub] = 0
-                                            else:
-                                                self.stock_shadow_values[var][sub] -= subval * self.sim_specs['dt']
+                                            self.stock_shadow_values[var][sub] += subval * self.sim_specs['dt']
+                                
+                            else:
+                                if type(self.name_space[in_flow]) is not dict:
+                                    self.stock_shadow_values[var] += self.name_space[in_flow] * self.sim_specs['dt']
                                 else:
-                                    if type(self.name_space[out_flow]) is not dict:
-                                        self.stock_shadow_values[var] -= self.name_space[out_flow] * self.sim_specs['dt']
+                                    for sub, subval in self.name_space[in_flow].items():
+                                        self.stock_shadow_values[var][sub] += subval * self.sim_specs['dt']
+                    if 'out' in self.stock_flows[var]:
+                        out_flows = self.stock_flows[var]['out']
+                        
+                        # outflow prioritisation
+                        # rule 1: first added first
+                        # rule 2: dependents ranked higher
+                        if len(out_flows) > 1:
+                            for i in range(len(out_flows)-1, 0, -1):
+                                for j in range(i):
+                                    if self.is_dependent(out_flows[j+1], out_flows[j]):
+                                        temp = out_flows[j+1]
+                                        out_flows[j+1] = out_flows[j]
+                                        out_flows[j] = temp
+
+                        for out_flow in out_flows:
+                            if out_flow not in self.name_space:
+                                self.calculate_variable_dynamic(var=out_flow, subscript=subscript, verbose=verbose)
+                            if var in self.stock_non_negative:
+                                if type(self.name_space[out_flow]) is not dict:
+                                    if self.stock_shadow_values[var] - self.name_space[out_flow] * self.sim_specs['dt'] < 0:
+                                        self.name_space[out_flow] = self.stock_shadow_values[var] / self.sim_specs['dt']
+                                        self.stock_shadow_values[var] = 0
                                     else:
-                                        for sub, subval in self.name_space[out_flow].items():
-                                            self.stock_shadow_values[var][sub] -= self.name_space[out_flow][sub] * self.sim_specs['dt']
-                    else: # for those stocks without flows connected:
-                        pass
-                
-                # if the stock's shadow value has been updated, do nothing as the real value is already in name_space
-                else:
+                                        self.stock_shadow_values[var] -= self.name_space[out_flow] * self.sim_specs['dt']
+                                else:
+                                    for sub, subval in self.name_space[out_flow].items():
+                                        if self.stock_shadow_values[var][sub] - subval * self.sim_specs['dt'] < 0:
+                                            self.name_space[out_flow][sub] = self.stock_shadow_values[var][sub] / self.sim_specs['dt']
+                                            self.stock_shadow_values[var][sub] = 0
+                                        else:
+                                            self.stock_shadow_values[var][sub] -= subval * self.sim_specs['dt']
+                            else:
+                                if type(self.name_space[out_flow]) is not dict:
+                                    self.stock_shadow_values[var] -= self.name_space[out_flow] * self.sim_specs['dt']
+                                else:
+                                    for sub, subval in self.name_space[out_flow].items():
+                                        self.stock_shadow_values[var][sub] -= self.name_space[out_flow][sub] * self.sim_specs['dt']
+                else: # for those stocks without flows connected:
                     pass
             
-            # C: var is a flow
-            elif var in self.flow_equations:
-                # var is a leakflow. In this case the conveyor needs to be initialised
-                if var in self.leak_conveyors:
-                    if not leak_frac:
-                        # if mode is not 'leak_frac', something other than the conveyor is requiring the leak_flow; 
-                        # then it is the real value of the leak flow that is requested.
-                        # then conveyor needs to be calculated. Otherwise it is the conveyor that requires it 
-                        if var not in self.name_space: # the leak_flow is not calculated, which means the conveyor has not been initialised
-                            self.calculate_variable_dynamic(var=self.leak_conveyors[var], subscript=subscript)
-                    else:
-                        # it is the value of the leak_fraction (a percentage) that is requested.    
-                        # leak_fraction is calculated using leakflow's equation. 
-                        parsed_equation = self.flow_equations_parsed[var]
-                        self.calculate_dependents(parsed_equation=parsed_equation)
-                        self.conveyors[self.leak_conveyors[var]]['leakflow'][var] = self.solver.calculate_node(parsed_equation=parsed_equation, verbose=verbose, var_name=var)
-
-                elif var in self.outflow_conveyors:
-                    # requiring an outflow's value triggers the calculation of its connected conveyor
-                    if var not in self.name_space: # the outflow is not calculated, which means the conveyor has not been initialised
-                        self.calculate_variable_dynamic(var=self.outflow_conveyors[var], subscript=subscript)
-                        
-                elif var in self.flow_equations:
-                    if var not in self.name_space:
-                        if type(parsed_equation) is dict:
-                            for k, sub_parsed_equaton in parsed_equation.items():
-                                # self.calculate_variable_dynamic(var=var, subscript=k)
-                                self.calculate_dependents(parsed_equation=sub_parsed_equaton)
-                                value = self.solver.calculate_node(parsed_equation=sub_parsed_equaton, subscript=k, verbose=verbose, var_name=var)
-                                
-                                # control flow positivity by itself
-                                if self.flow_positivity[var] is True:
-                                    if value < 0:
-                                        value = 0
-                                if var not in self.name_space:
-                                    self.name_space[var] = dict()
-                                self.name_space[var][k] = value
-                        else:
-                            self.calculate_dependents(parsed_equation=parsed_equation)
-                            value = self.solver.calculate_node(parsed_equation=parsed_equation, subscript=subscript, verbose=verbose, var_name=var)
-
+            # if the stock's shadow value has been updated, do nothing as the real value is already in name_space
+            else:
+                pass
+        
+        # C: var is a flow
+        elif var in self.flow_equations:
+            # var is a leakflow. In this case the conveyor needs to be initialised
+            if var in self.leak_conveyors:
+                if not leak_frac:
+                    # if mode is not 'leak_frac', something other than the conveyor is requiring the leak_flow; 
+                    # then it is the real value of the leak flow that is requested.
+                    # then conveyor needs to be calculated. Otherwise it is the conveyor that requires it 
+                    if var not in self.name_space: # the leak_flow is not calculated, which means the conveyor has not been initialised
+                        self.calculate_variable_dynamic(var=self.leak_conveyors[var], subscript=subscript)
+                else:
+                    # it is the value of the leak_fraction (a percentage) that is requested.    
+                    # leak_fraction is calculated using leakflow's equation. 
+                    parsed_equation = self.flow_equations_parsed[var]
+                    self.calculate_dependents(parsed_equation=parsed_equation, verbose=verbose)
+                    self.conveyors[self.leak_conveyors[var]]['leakflow'][var] = self.solver.calculate_node(parsed_equation=parsed_equation, verbose=verbose, var_name=var)
+
+            elif var in self.outflow_conveyors:
+                # requiring an outflow's value triggers the calculation of its connected conveyor
+                if var not in self.name_space: # the outflow is not calculated, which means the conveyor has not been initialised
+                    self.calculate_variable_dynamic(var=self.outflow_conveyors[var], subscript=subscript)
+                    
+            elif var in self.flow_equations: # var is a normal flow
+                if var not in self.name_space:
+                    if type(parsed_equation) is dict:
+                        for sub, sub_parsed_equaton in parsed_equation.items():
+                            self.calculate_dependents(parsed_equation=sub_parsed_equaton, verbose=verbose)
+                            value = self.solver.calculate_node(parsed_equation=sub_parsed_equaton, subscript=sub, verbose=verbose, var_name=var)
+                            
                             # control flow positivity by itself
                             if self.flow_positivity[var] is True:
                                 if value < 0:
                                     value = 0
-                            
-                            self.name_space[var] = value
-                    else:
-                        pass
-            
-            # D: var is an auxiliary
-            elif var in self.aux_equations:
-                if var not in self.name_space:
-                    if type(parsed_equation) is dict:
-                        for k, sub_parsed_equation in parsed_equation.items():
-                            # self.calculate_variable_dynamic(var=var, subscript=k)
-                            self.calculate_dependents(parsed_equation=sub_parsed_equation)
-                            value = self.solver.calculate_node(parsed_equation=sub_parsed_equation, subscript=k, verbose=verbose, var_name=var)
                             if var not in self.name_space:
                                 self.name_space[var] = dict()
-                            self.name_space[var][k] = value
+                            self.name_space[var][sub] = value
+                    elif var in self.var_dimensions and self.var_dimensions[var] is not None: # The variable is subscripted but all elements uses the same equation
+                        self.calculate_dependents(parsed_equation=parsed_equation, verbose=verbose)
+                        for sub in self.dimension_elements[self.var_dimensions[var]]:
+                            value = self.solver.calculate_node(parsed_equation=parsed_equation, subscript=sub, verbose=verbose, var_name=var)
+                            # control flow positivity by itself
+                            if self.flow_positivity[var] is True:
+                                if value < 0:
+                                    value = 0
+                            if var not in self.name_space:
+                                self.name_space[var] = dict()
+                            self.name_space[var][sub] = value
                     else:
-                        self.calculate_dependents(parsed_equation=parsed_equation)
+                        self.calculate_dependents(parsed_equation=parsed_equation, verbose=verbose)
                         value = self.solver.calculate_node(parsed_equation=parsed_equation, subscript=subscript, verbose=verbose, var_name=var)
+
+                        # control flow positivity by itself
+                        if self.flow_positivity[var] is True:
+                            if value < 0:
+                                value = 0
+                        
                         self.name_space[var] = value
-                            
                 else:
                     pass
-            
+        
+        # D: var is an auxiliary
+        elif var in self.aux_equations:
+            if var not in self.name_space:
+                if type(parsed_equation) is dict:
+                    for sub, sub_parsed_equation in parsed_equation.items():
+                        self.calculate_dependents(parsed_equation=sub_parsed_equation, verbose=verbose)
+                        value = self.solver.calculate_node(parsed_equation=sub_parsed_equation, subscript=sub, verbose=verbose, var_name=var)
+                        if var not in self.name_space:
+                            self.name_space[var] = dict()
+                        self.name_space[var][sub] = value
+                elif var in self.var_dimensions and self.var_dimensions[var] is not None: # The variable is subscripted but all elements uses the same equation
+                    self.calculate_dependents(parsed_equation=parsed_equation, verbose=verbose)
+                    for sub in self.dimension_elements[self.var_dimensions[var]]:
+                        value = self.solver.calculate_node(parsed_equation=parsed_equation, subscript=sub, verbose=verbose, var_name=var)
+                        if var not in self.name_space:
+                            self.name_space[var] = dict()
+                        self.name_space[var][sub] = value
+                else:
+                    self.calculate_dependents(parsed_equation=parsed_equation, verbose=verbose)
+                    value = self.solver.calculate_node(parsed_equation=parsed_equation, subscript=subscript, verbose=verbose, var_name=var)
+                    self.name_space[var] = value
+                        
             else:
-                raise Exception("Undefined var: {}".format(var))
+                pass
+        
+        else:
+            raise Exception("Undefined var: {}".format(var))
 
     def calculate_variables_dynamic(self, verbose=False):
         for var in (self.stock_equations_parsed | self.aux_equations_parsed | self.flow_equations_parsed).keys():
             self.calculate_variable_dynamic(var=var, verbose=verbose)
     
     def update_conveyors(self):
         for conveyor_name, conveyor in self.conveyors.items(): # Stock is a Conveyor
@@ -1897,19 +1972,21 @@
                     for flow in flows:
                         total_flow_effect += self.name_space[flow]
 
             # in
             conveyor['conveyor'].inflow(total_flow_effect * self.sim_specs['dt'])
             self.stock_shadow_values[conveyor_name] = conveyor['conveyor'].level()
             
-    def simulate(self, time=None, dt=None, dynamic=True, verbose=False, debug_against=None):
+    def simulate(self, time=None, dt=None, dynamic=True, verbose=False, debug_against=False):
         if debug_against is not None:
-            import pandas as pd
             if debug_against is True:
+                import pandas as pd
                 self.df_debug_against = pd.read_csv('stella.csv')
+            elif debug_against is False:
+                pass
             else:
                 self.df_debug_against = pd.read_csv(debug_against)
 
         self.parse(verbose=verbose)
 
         if time is None:
             time = self.sim_specs['simulation_time']
```

### Comparing `asdm-0.0.2/ASDM/Diagrams/ASDM.excalidraw` & `asdm-0.0.3/ASDM/Diagrams/ASDM.excalidraw`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/ASDM/Diagrams/EngineOOP.excalidraw` & `asdm-0.0.3/ASDM/Diagrams/EngineOOP.excalidraw`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/ASDM/Diagrams/Parser1.png` & `asdm-0.0.3/ASDM/Diagrams/Parser1.png`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/ASDM/Diagrams/Parser2.png` & `asdm-0.0.3/ASDM/Diagrams/Parser2.png`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/ASDM/MCMC.py` & `asdm-0.0.3/ASDM/Inference/MCMC.py`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/ASDM/Optimizer.py` & `asdm-0.0.3/ASDM/Inference/Optimizer.py`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/ASDM/Parser.excalidraw` & `asdm-0.0.3/ASDM/Diagrams/Parser.excalidraw`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/ASDM/Payoff.py` & `asdm-0.0.3/ASDM/Inference/Payoff.py`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/ASDM/Probability.py` & `asdm-0.0.3/ASDM/Inference/Probability.py`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/ASDM/Utilities.py` & `asdm-0.0.3/ASDM/Utilities.py`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/ASDM/test_Behaviour.py` & `asdm-0.0.3/tests/test_Behaviour.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import traceback
 import logging
 import pathlib
 import pandas as pd
 import numpy as np
-from ASDM import Structure
+from ASDM.ASDM import Structure
 
 ### Load the tests and outcomes ###
 
 # Run this script at the project's root directory
-path_tests = pathlib.Path('./BuiltinTestModels')
-path_test_results = pathlib.Path('./BuiltinTestModels/Stella_outcomes')
+path_tests = pathlib.Path('./BuiltInTestModels')
+path_test_results = pathlib.Path('./BuiltInTestModels/Stella_outcomes')
 tests = list()
 outcomes = list()
 for t in path_tests.iterdir():
     if t.suffix == '.stmx':
         tests.append(t)
         o = path_test_results/(t.stem+'.csv')
         if o.is_file():
```

### Comparing `asdm-0.0.2/ASDM/test_Engine.py` & `asdm-0.0.3/tests/test_Engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ASDM import Structure
+from ASDM.ASDM import Structure
 
 
 if __name__ == '__main__':
 
     #### Test Models ###
 
     # model = Structure(from_xmile='BuiltinTestModels/Basic_math.stmx')
@@ -16,14 +16,16 @@
     # model = Structure(from_xmile='BuiltinTestModels/Goal_gap.stmx')
     # model = Structure(from_xmile='BuiltinTestModels/Time_unit.stmx')
 
     # model = Structure(from_xmile='BuiltinTestModels/Goal_gap_array.stmx')
     # model = Structure(from_xmile='BuiltinTestModels/Array_parallel_reference.stmx')
     # model = Structure(from_xmile='BuiltinTestModels/Array_cross_reference.stmx')
     # model = Structure(from_xmile='BuiltinTestModels/Array_cross_reference_inference.stmx')
+    # model = Structure(from_xmile='BuiltinTestModels/array_SUM.stmx')
+    # model = Structure(from_xmile='BuiltinTestModels/array_in_function.stmx')
     
     # model = Structure(from_xmile='BuiltInTestModels/Built_in_vars.stmx')
     
     # model = Structure(from_xmile='BuiltInTestModels/Logic.stmx')
     # model = Structure(from_xmile='BuiltInTestModels/IF_THEN_ELSE.stmx')
     
     # model = Structure(from_xmile='BuiltInTestModels/Graph_function.stmx')
@@ -39,30 +41,26 @@
     # model = Structure(from_xmile='BuiltInTestModels/Conveyor.stmx')
     # model = Structure(from_xmile='BuiltInTestModels/Conveyor_leakage.stmx')
     # model = Structure(from_xmile='BuiltInTestModels/Conveyor_leakage1.stmx')
     # model = Structure(from_xmile='BuiltInTestModels/Conveyor_leakage2.stmx')
     # model = Structure(from_xmile='BuiltInTestModels/Conveyor_initialisation.stmx')
 
     ### Production Models ###
-
-    model = Structure(from_xmile='TestModels/Elective Recovery Model.stmx')
-    # model=Structure(from_xmile='TestModels/2022_07_14 no milk without meat.stmx')
-    # model=Structure(from_xmile='TestModels/TempTest1.stmx')
+    
 
     ### Controls ###
 
     # Dynamic simulation
-    model.simulate(debug_against=True, verbose=False)
+    model.simulate(debug_against=False, verbose=True)
     model.summary()
-
     ### Simulation inspections ###
 
     model.export_simulation_result(to_csv=True)
-    # r = model.export_simulation_result(format='df', to_csv=False)
-    # print(r)
+    r = model.export_simulation_result(format='df', to_csv=False)
+    print(r)
 
     # vars_to_view = [
     #     '13wk_wait_for_urgent_treatment', 
     # #     'Negative_test_results', 
     # #     'COVID_modified_percent_urgent', 
     # #     'Undergoing_diagnostic_tests',
     # #     'Positive_test_results_urgent',
```

### Comparing `asdm-0.0.2/ASDM/test_MultipleRuns.py` & `asdm-0.0.3/tests/test_MultipleRuns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ASDM import Structure
+from ASDM.ASDM import Structure
 
 class Infection(Structure):
     def __init__(self):
         super(Infection, self).__init__()
         self.add_stock("Infected", 100, in_flows=['IncreaseRate'])
         self.add_flow(
             name='IncreaseRate',
```

### Comparing `asdm-0.0.2/ASDM/test_Parser.py` & `asdm-0.0.3/tests/test_Parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ASDM import Parser
+from ASDM.ASDM import Parser
 
 if __name__ == '__main__':
 
     string_0a = 'a'
     string_1a = 'a+b-c'
     string_1b = 'a+b-2'
     string_2a = 'a*b'
```

### Comparing `asdm-0.0.2/ASDM/test_Solver.py` & `asdm-0.0.3/tests/test_Solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ASDM import Parser, Solver
+from ASDM.ASDM import Parser, Solver
 
 
 if __name__ == '__main__':
 
     name_space= {
         'a': 1,
         'b': 2,
```

### Comparing `asdm-0.0.2/LICENSE` & `asdm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/PKG-INFO` & `asdm-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asdm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Agile System Dynamics Engine
 Author-email: Wang Zhao <wang.zhao@strath.ac.uk>, Matt Stammers <matt@reallyusefulmodels.com>
 License: MIT License
         
         Copyright (c) 2022 W.Zh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,49 +54,40 @@
 
 We recommend that you use pip to install asdm but if you do wish to develop it further pipenv instructions are provided. 
 
 ## Tutorial Notebooks
 
 We use a series of Jupyter Notebooks to provide functionality guidance for the users.
 
-1. [SD Modelling](./1-SD_modelling.ipynb)
+1. [SD Modelling](https://github.com/wzh1895/ASDM/blob/main/Demo_SD_modelling.ipynb)
 
 - Creating an SD model from scratch
   - Adding stocks, flows, auxiliaries
   - Support for nonlinear functions (MIN, MAX, etc.)
   - Support for stochastic functions (random binomial trial, etc.)
 - Running simulations
 - Exporting and examing simulation outcomes
 - Displaying simulation outcomes as graph
 
-2. [Model Calibration](./2-SD_model_calibration.ipynb) [STILL IN DEVELOPMENT]
-
-- Estimating SD model parameters using Markov Chain Monte Carlo (MCMC)
-  - Support for MLE (maximum likelihood) and MAP (maximum a posteriori) approach
-  - Support for different modellings of payoff (squared error, Poisson, etc.) that are used in the likelihood function
-  - Support for different sampling methods (Slice, Metropolis, NUTS, Hamiltonian, etc.), enabled by [PyMC3](https://docs.pymc.io/en/v3/)
-- Diagnostic analyses of MCMC samples, enabled by [Arviz](https://arviz-devs.github.io/arviz/)
-  - Trace plot
-  - Autocorrelation plot
-- Comparison between Historical data and simulation data
-
-3. More to come...
-
 ## Why ASDM?
 
 Acknowledging that there are a number of SD tools that enable simulating SD models in a Python environment (see [PySD](https://github.com/JamesPHoughton/pysd) and [venpy](https://github.com/pbreach/venpy.git)), we build ASDM to bring the capability of **structure modelling** to the Python SD community. ASDM allows users to create an SD model from scratch and edit model structure as needed. With a native Python implementation of stock-and-flow structure, ASDM allows building SD models without software like [Vensim](https://vensim.com/) and [Stella](https://www.iseesystems.com/store/products/stella-architect.aspx).
 
 The long-term goal ASDM intends to achieve is an approach for **data-informed structure modelling** where data can be used to finetune SD model structure automatically. This is both an extension of data-informed SD model parameter estimation, and an innovative way to discover feedback structures from data.
 
 ## Limitations
 
 The main drawback at the moment is that we have not been working a lot on **translating Vensim/Stella models** into the format that ASDM uses, although [PySD](https://github.com/JamesPHoughton/pysd) has proved this fully doable. This functionality is in our development roadmap.
 
 We have neither been working a lot on **the speed of simulation**. Although simulating large SD models given mordern computer specs would not be extremely time-consuming, in tasks involing Monte Carlo simulation (such as parameter estimation) the speed of running a model can matter a lot more. Acceleration is in our development roadmap too.
 
+## Docs
+
+Full docs are incoming
+
 ## Licence
 
 ASDM is made public under the MIT licence.
 
 ## Authors
 **Wang Zhao**  
 PhD candidate at University of Strathclyde, UK
```

### Comparing `asdm-0.0.2/Pipfile` & `asdm-0.0.3/Pipfile`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 lxml = "==4.9.1"
 beautifulsoup4 = "==4.11.1"
 tqdm = "==4.64.0"
 ipywidgets = "==7.6.5"
 openpyxl = "==3.0.10"
 ipykernel = "==6.22.0"
 asdm = "==0.0.1"
+requests_toolbelt = "==1.0.0"
 
 [dev-packages]
 setuptools = "==67.7.1"
 setuptools-scm = "==7.1.0"
 twine = "==4.0.2"
 build = "==0.10.0"
```

### Comparing `asdm-0.0.2/Pipfile.lock` & `asdm-0.0.3/Pipfile.lock`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9871396974885845%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'ef1971ee524b57c5aac3e78102f78a0043cfd015b973a6e22e4f29691b6bfc88'}}",*

 * * "'default'": "{'requests-toolbelt': OrderedDict([('hashes', "*

 * *              "['sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6', "*

 * *              "'sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06']), "*

 * *              "('index', 'pypi'), ('version', '==1.0.0')])}",*

 * * "'develop'": "{'requests-toolbelt': {'index': 'pypi', delete: ['markers']}}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "a8f5bfc56459d34355888737f56bd7a6f9439348d528e36a536633e4b2fda66c"
+            "sha256": "ef1971ee524b57c5aac3e78102f78a0043cfd015b973a6e22e4f29691b6bfc88"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_full_version": "3.9.0",
             "python_version": "3.9"
         },
         "sources": [
@@ -1639,14 +1639,22 @@
             "hashes": [
                 "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
                 "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.30.0"
         },
+        "requests-toolbelt": {
+            "hashes": [
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
+            ],
+            "index": "pypi",
+            "version": "==1.0.0"
+        },
         "rfc3339-validator": {
             "hashes": [
                 "sha256:138a2abdf93304ad60530167e51d2dfb9549521a836871b88d7f4695d0022f6b",
                 "sha256:24f6ec1eda14ef823da9e36ec7113124b39c04d50a4d3d3a3c2859577e7791fa"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==0.1.4"
@@ -2210,15 +2218,15 @@
             "version": "==2.30.0"
         },
         "requests-toolbelt": {
             "hashes": [
                 "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
                 "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "index": "pypi",
             "version": "==1.0.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
```

### Comparing `asdm-0.0.2/README.md` & `asdm-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,49 +20,40 @@
 
 We recommend that you use pip to install asdm but if you do wish to develop it further pipenv instructions are provided. 
 
 ## Tutorial Notebooks
 
 We use a series of Jupyter Notebooks to provide functionality guidance for the users.
 
-1. [SD Modelling](./1-SD_modelling.ipynb)
+1. [SD Modelling](https://github.com/wzh1895/ASDM/blob/main/Demo_SD_modelling.ipynb)
 
 - Creating an SD model from scratch
   - Adding stocks, flows, auxiliaries
   - Support for nonlinear functions (MIN, MAX, etc.)
   - Support for stochastic functions (random binomial trial, etc.)
 - Running simulations
 - Exporting and examing simulation outcomes
 - Displaying simulation outcomes as graph
 
-2. [Model Calibration](./2-SD_model_calibration.ipynb) [STILL IN DEVELOPMENT]
-
-- Estimating SD model parameters using Markov Chain Monte Carlo (MCMC)
-  - Support for MLE (maximum likelihood) and MAP (maximum a posteriori) approach
-  - Support for different modellings of payoff (squared error, Poisson, etc.) that are used in the likelihood function
-  - Support for different sampling methods (Slice, Metropolis, NUTS, Hamiltonian, etc.), enabled by [PyMC3](https://docs.pymc.io/en/v3/)
-- Diagnostic analyses of MCMC samples, enabled by [Arviz](https://arviz-devs.github.io/arviz/)
-  - Trace plot
-  - Autocorrelation plot
-- Comparison between Historical data and simulation data
-
-3. More to come...
-
 ## Why ASDM?
 
 Acknowledging that there are a number of SD tools that enable simulating SD models in a Python environment (see [PySD](https://github.com/JamesPHoughton/pysd) and [venpy](https://github.com/pbreach/venpy.git)), we build ASDM to bring the capability of **structure modelling** to the Python SD community. ASDM allows users to create an SD model from scratch and edit model structure as needed. With a native Python implementation of stock-and-flow structure, ASDM allows building SD models without software like [Vensim](https://vensim.com/) and [Stella](https://www.iseesystems.com/store/products/stella-architect.aspx).
 
 The long-term goal ASDM intends to achieve is an approach for **data-informed structure modelling** where data can be used to finetune SD model structure automatically. This is both an extension of data-informed SD model parameter estimation, and an innovative way to discover feedback structures from data.
 
 ## Limitations
 
 The main drawback at the moment is that we have not been working a lot on **translating Vensim/Stella models** into the format that ASDM uses, although [PySD](https://github.com/JamesPHoughton/pysd) has proved this fully doable. This functionality is in our development roadmap.
 
 We have neither been working a lot on **the speed of simulation**. Although simulating large SD models given mordern computer specs would not be extremely time-consuming, in tasks involing Monte Carlo simulation (such as parameter estimation) the speed of running a model can matter a lot more. Acceleration is in our development roadmap too.
 
+## Docs
+
+Full docs are incoming
+
 ## Licence
 
 ASDM is made public under the MIT licence.
 
 ## Authors
 **Wang Zhao**  
 PhD candidate at University of Strathclyde, UK
```

### Comparing `asdm-0.0.2/apps/ERM/3-From_XMILE.ipynb` & `asdm-0.0.3/apps/ERM/3-From_XMILE.ipynb`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/apps/ERM/ERM_ASDM_app.py` & `asdm-0.0.3/apps/ERM/ERM_ASDM_app.py`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/apps/ERM/Elective Recovery Model.stmx` & `asdm-0.0.3/apps/ERM/Elective Recovery Model.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/apps/ERM/Elective Recovery Model.xlsx` & `asdm-0.0.3/apps/ERM/Elective Recovery Model.xlsx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/apps/ERM/Elective_Recovery_Model.PNG` & `asdm-0.0.3/apps/ERM/Elective_Recovery_Model.PNG`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/apps/Goal_Gap/Goal_gap_model.png` & `asdm-0.0.3/apps/Goal_Gap/Goal_gap_model.png`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/apps/Goal_Gap/Revised_Goal_Gap.py` & `asdm-0.0.3/apps/Goal_Gap/Revised_Goal_Gap.py`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/apps/Goal_Gap/Revised_Goal_Gap.stmx` & `asdm-0.0.3/apps/Goal_Gap/Revised_Goal_Gap.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/apps/Goal_Gap/goal_gap.py` & `asdm-0.0.3/apps/Goal_Gap/goal_gap.py`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/apps/Smoking_Cessation/ASDM/Engine.py` & `asdm-0.0.3/tests/Discarded/EngineArrays.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,50 +41,40 @@
         elif element_type == 'variable':
             self.variable_id += 1
             return 'variable_' + str(self.variable_id)
         elif element_type == 'parameter':
             self.parameter_id += 1
             return 'parameter_' + str(self.parameter_id)
 
-# class Data(object):
-#     def __init__(self, data_source):
-#         """
-#         data_source: a DataFrame structure
+class Data(object):
+    def __init__(self, data_source):
+        """
+        data_source: a DataFrame structure
 
-#         """
-#         self.ts = data_source # we plan to convert more types of data_source to time_series
+        """
+        self.ts = data_source # we plan to convert more types of data_source to time_series
 
 
 class DataFeeder(object):
-    def __init__(self, data, from_time=0, data_dt=1):
+    def __init__(self, data, from_step=1):
         """
-        data: a list
+        data: a Data object
 
         """
-        self.from_time =from_time
-        self.time_data = dict()
-        time = self.from_time
-        for d in data:
-            self.time_data[time] = d
-            time += data_dt
-        # print(self.time_data)
-        self.last_success_time = None
+        self.ts_enumerator = enumerate(data.ts.values)
+        self.from_step = from_step
+        # self.n = 1
+
+    def __call__(self, current_step): # make a datafeeder callable
+        if current_step >= self.from_step:
+            ix, dp = next(self.ts_enumerator)
 
-    def __call__(self, current_time): # make a datafeeder callable
-        try:
-            d = self.time_data[current_time]
-            self.last_success_time = current_time
-        except KeyError:
-            if current_time < self.from_time:
-                raise Exception("Current time < external data starting time.")
-            elif current_time > list(self.time_data.keys())[-1]:
-                raise Exception("Current time > external data ending time.")
-            else:
-                d = self.time_data[self.last_success_time]
-        return(float(d))
+            return(float(dp))
+        else:
+            return None
 
 
 class ExtFunc(object):
     def __init__(self, external_function, arguments=None):
         """
         external_function: a function that takes an input and returns an output
         *args: arguments from within the model for that external_function
@@ -111,20 +101,14 @@
         
         from scipy.interpolate import interp1d
 
         self.xpts = np.linspace(self.xscale[0], self.xscale[1], num=len(self.ypts))
         self.interp_func = interp1d(self.xpts, self.ypts, kind='linear')
 
     def __call__(self, input):
-        # TODO implement other out-of-bounds contingencies
-        if input < self.xscale[0]:
-            input = self.xscale[0]
-        if input > self.xscale[1]:
-            input = self.xscale[1]
-        
         return self.interp_func(input)
 
 
 class Conveyor(object):
     def __init__(self, length, eqn):
         self.length_time_units = length
         self.equation = eqn
@@ -213,21 +197,18 @@
             self.MULTIPLICATION,
             self.RBINOM,
             self.DELAY1,
             self.INIT
         ]
 
         self.custom_functions = {
-            'MAX': max,
-            'MIN': min,
             'rbinom': self.rbinom,
             'delay1': self.delay1,
             'delay': self.delay,
-            'DELAY': self.delay,
-            'STEP': self.step
+            'DELAY': self.delay
             # 'init': self.init
         }
 
         self.time_related_functions = {
             'init': self.init,
             'INIT': self.init,  # Stella uses capital INIT
             'delay': self.delay,
@@ -251,34 +232,31 @@
 
         self.sfd = nx.DiGraph()
         self.__uid_manager = UidManager()
         self.__name_manager = NameManager()
         self.__uid_element_name = dict()
         self.__time_slice_values = dict() # a time-slice of name values
         self.__name_values = dict() # centralised simulation data manager
-        self.__built_in_variables = {'TIME':list()}
+        self.__built_in_variables = dict()
         self.__expression_values = dict() # centralised data manager for init(expression)
-        # self.__name_external_data = dict() # centralised external data manager
+        self.__name_external_data = dict() # centralised external data manager
         
         # Specify if subscript is used
         self.subscripts = subscripts
-        self.var_dimensions = dict()
 
         # Define cumulative registers for time-related functions, such as delays
         self.delay_registers = dict()
         
         self.initial_time = 0
         self.current_time = self.initial_time
         self.current_step = 1 # object-wise global indicator for current simulation step. start from 1 (values after the 1st step)
         self.dt = 0.25
         self.simulation_time = 25
         self.time_units = 'Weeks'
 
-        self.verbose = False
-
         # Initialisation indicator
         self.is_initialised = False
 
         # If the model is based on an XMILE file
         if from_xmile is not None:
             from pathlib import Path
             xmile_path = Path(from_xmile)
@@ -351,23 +329,21 @@
                     equation = GraphFunc(xscale, yscale, ypts)
                     return equation
 
                 # create var subscripted equation
                 def subscripted_equation(var):
                     # print('Reading variable from XMILE: {}'.format(var.get('name')))
                     if var.find('dimensions'):
-                        self.var_dimensions[var.get('name')] = list()
                         # print('Processing XMILE subscripted definition for:', var.get('name'))
                         var_dimensions = var.find('dimensions').findAll('dim')
                         # print('Found dimensions {}:'.format(var), var_dimensions)
 
                         var_dims = dict()
                         for dimension in var_dimensions:
                             name = dimension.get('name')
-                            self.var_dimensions[var.get('name')].append(name)
                             # print(dimension)
                             # print(name)
                             var_dims[name] = dims[name]
                         var_subscripted_eqn = dict()
 
                         var_elements = var.findAll('element')
                         if len(var_elements) != 0:
@@ -408,15 +384,14 @@
                             element_combination_texts = ['__cmm__'.join(cmb) for cmb in element_combinations]
                             # print('ec', element_combination_texts)
 
                             for ect in element_combination_texts:
                                 var_subscripted_eqn[ect] =equation
                         return(var_subscripted_eqn)
                     else:
-                        self.var_dimensions[var.get('name')] = ['nodimension']
                         # print('Processing XMILE definition for:', var.get('name'))
                         var_subscripted_eqn = dict()
                         if var.find('conveyor'):
                             equation = var.find('eqn').text
                             length = var.find('len').text
                             equation = Conveyor(length, equation)
                         elif var.find('gf'):
@@ -505,23 +480,14 @@
         for arg in args:
             product = product * float(arg)
         return product
     
     def rbinom(self, n, p):
         return stats.binom.rvs(int(n), p, size=1)[0]
     
-    def step(self, stp, time):
-        # print('step:', stp, time)
-        if self.current_time >= time:
-            # print('step out:', stp)
-            return stp
-        else:
-            # print('step out:', 0)
-            return 0
-
     def delay(self, subscript, input, delay_time, initial_value=None):
         delay_time = float(delay_time)
         try:
             output = self.__name_values[self.current_time-delay_time][input][subscript]
             # print(input, 'aa')
         except KeyError: # current time < delay time
             if initial_value is not None: # initial value is supplied
@@ -560,21 +526,14 @@
         return output
 
     def init(self, subscript, var):
         # print('calculating init', var)
         # case 1: var is a variable in the model
         if var in self.sfd.nodes:
             v = self.__name_values[self.initial_time][var][subscript]
-        elif '__ele1__' in var and var.split('__ele1__')[0] in self.sfd.nodes:
-            print('init case1.2')
-            var_name = var.split('__ele1__')[0]
-            var_subscript = var.split('__ele1__')[1].split('__ele2__')[0]
-            v = self.__name_values[self.initial_time][var_name][var_subscript]
-            if v is None:
-                v = self.calculate_experiment(var_name, var_subscript)
         # case 2: var is an expression
         else:
             if var in self.__expression_values.keys():
                 v = self.__expression_values[var]
             else:
                 equation = var
                 value = None
@@ -696,22 +655,17 @@
                 return str(equation[1])
 
     def __add_element(self, element_name, element_type, flow_from=None, flow_to=None, x=0, y=0, equation=None, points=None, external=False, non_negative=False, leak=None):
         uid = self.__uid_manager.get_new_uid()
 
         # construct subscripted equation indexer
         # the 1st column stores the equation{function or initial value}, indexed by subscripts
-        if type(equation) is DataFeeder:  # wrap external data into DataFeeder
-            equation = {'nosubscript': equation}
-            external = True
-
-        # when equation is manually specified without explicit subscript, e.g., 1, 2+1, etc.
-        if type(equation) is not dict:
-            equation = {'nosubscript': equation}
-        
+        if type(equation) is Data:  # wrap external data into DataFeeder
+            equation = DataFeeder(equation)
+
         # create a name_values binding for its simulation data
         v_dict = dict()
         for k in equation.keys():
             v_dict[k] = None
         self.__time_slice_values[element_name] = v_dict
 
         # create a node in the SFD graph
@@ -813,18 +767,15 @@
         Get the coordinate of a specified variable
         :param name:
         :return: coordinate of the variable in a tuple
         """
         return self.sfd.nodes[name]['pos']
 
     # Simulate a structure based on a certain set of parameters
-    def simulate(self, simulation_time=None, dt=None, progress_bar=False, verbose=False):
-        self.verbose = verbose
-        if self.verbose:
-            print('Starting simulation...')
+    def simulate(self, simulation_time=None, dt=None):
         if simulation_time is not None:
             self.simulation_time = simulation_time
         if dt is not None:
             self.dt = dt
         total_steps = int(self.simulation_time / self.dt)
         
         # have a dict for all visited (calculated) variables (F/V/P) in this model
@@ -838,15 +789,15 @@
             self.__built_in_variables['TIME'].append(self.initial_time) # initialization of stocks might require TIME
             self.init_stocks()
         else:
             self.update_stocks(self.dt)
         
         # Step 2
         from tqdm import tnrange
-        for _ in tnrange(total_steps, disable=not progress_bar):
+        for _ in tnrange(total_steps):
             self.update_states()
             self.current_step += 1  # update current_step counter
             self.current_time += self.dt
             self.__built_in_variables['TIME'].append(self.current_time)
             self.__name_values[self.current_time] = deepcopy(self.__time_slice_values)
 
             self.visited = dict()
@@ -856,16 +807,15 @@
         # Step 3
 
         self.update_states()
         
     def init_stocks(self):
         self.__name_values[self.current_time] = deepcopy(self.__time_slice_values)
         for element in self.get_all_certain_type(['stock']):
-            if self.verbose:
-                print('Initializing stock: {}'.format(element))
+            print('Initializing stock: {}'.format(element))
             # for ix in self.sfd.nodes[element]['equation'].sub_index:
             for ix in self.sfd.nodes[element]['equation'].keys():
                 equation = self.sfd.nodes[element]['equation'][ix]
                 # print('EQU', equation)
 
                 # if the stock is a conveyor, extract its equation
                 is_conveyor = False
@@ -887,27 +837,27 @@
                             if self.sfd.nodes[e]['leak']:
                                 if self.sfd.nodes[e]['flow_from'] == element:
                                     leak_fraction_eqn = self.sfd.nodes[e]['equation'][ix]
                                     leak_fraction = self.calculate_experiment(leak_fraction_eqn, ix)
                     conveyor.initialize(length, value, leak_fraction)
 
         # set is_initialised flag to True
-        if self.verbose:
-            print('All stocks initialised.')
+        print('All stocks initialised.')
         self.is_initialised = True
 
     def update_stocks(self, dt):
         # have a dictionary for flows and their values in this default_dt, to be added to or subtracted from stocks
         flows_dt = dict()
 
         # find all flows in the model
         for element in self.get_all_certain_type('flow'):  # loop through all flows in this SFD,
             flows_dt[element] = dict()  # make a position for it in the dict of flows_dt, initializing it with 0
 
-        # calculate flow values for this dt
+
+        # calculate flows
         for flow in flows_dt.keys():
             for ix in self.sfd.nodes[flow]['equation'].keys():
                 flows_dt[flow][ix] = dt * self.__name_values[self.current_time-self.dt][flow][ix]
 
         # calculating changes in stocks
         # have a dictionary of affected stocks and their changes, since one flow could affect 2 stocks.
         affected_stocks = dict()
@@ -1054,61 +1004,49 @@
         
         for element in self.get_all_certain_type(['auxiliary']):
             if element not in self.visited.keys():
                 for ix in self.sfd.nodes[element]['equation'].keys():
                     # if ix not in self.visited[element].keys():
                     self.calculate_experiment(element, ix)
 
-    def process_expression(self, expression, intended_subscripts=None):
-        # print(self.n_indentation*'\t' + 'PE0 processING expression:', expression, 'with intended subs:', intended_subscripts)
-        # print(self.n_indentation*'\t' + 'split', intended_subscripts)
-        if intended_subscripts is not None:
-            intended_subscripts = intended_subscripts.split('__cmm__')
-        
+    @staticmethod
+    def process_expression(expression):
         expression_1 = expression
         while '[' in expression_1:
             expression_1_a, expression_1_b = expression_1.split('[', 1)
             expression_1_b, expression_1_c = expression_1_b.split(']', 1)
             expression_1_b = expression_1_b.replace(' ', '').replace(',', '__cmm__')
-            
-            # Dynamically resolve collective reference such as a[Dimension1]
-            if intended_subscripts is not None:
-                subscripts = expression_1_b.split('__cmm__')
-                for i in range(len(subscripts)):
-                    if subscripts[i] in self.subscripts.keys(): # a[Dimension1] instead of a[Element1]
-                        subscripts[i] = intended_subscripts[i] # dynamically replace Dimension1 by Element1
-                expression_1_b = '__cmm__'.join(subscripts)
-
             expression_1 = expression_1_a + '__ele1__' + expression_1_b + '__ele2__' + expression_1_c
         expression = expression_1
-        # print(self.n_indentation*'\t' + 'PE1 processED equation:', expression)
+        # print('processed equation:', expression)
         return expression
     
     @staticmethod
     def process_subscript(subscript):
         subscript = subscript.replace(',', '__cmm__').replace(' ', '')
         return subscript
 
     
     def calculate_experiment(self, expression, subscript):
         self.n_indentation += 1
-        if self.verbose:
-            print(self.n_indentation*'\t' + 'processing expression of {} on subscript {}:'.format(expression, subscript))
+        # print(self.n_indentation*'\t' + 'processing expression:', expression)
 
         # check if the expression contains '[]' - cross reference of arrays
         if type(expression) is str and '[' in expression:
             # print('process a')
             expression = self.process_expression(expression)
             # print('process expression with subscripts:', expression)
-        
-        elif type(expression) is str and '__ele1__' in expression:
+            # expression = expression.replace('[', '__ele1__').replace(']', '__ele2__').replace(',', '__cmm__')
+
+        # check if the expression is abc__ele1__subscript__ele2__
+        if type(expression) is str and '__ele1__' in expression:
             # print('process b')
-            expression, subscript = expression.split('__ele1__')
-            subscript = subscript.split('__ele2__')[0]
-            # print('process b:', expression, subscript)
+            expression, subscript = expression.split('__ele1__', 1)
+            subscript, remaining = subscript.split('__ele2__', 1)
+            # print('process b', expression, subscript, remaining)
 
         # check if this value has been calculated and stored in buffer
         # when initialising stock values, there's no 'self.visited' yet
         if expression in self.visited.keys():
             # print('calc a')
             # print(self.visited[expression])
             if subscript in self.visited[expression].keys():
@@ -1163,46 +1101,40 @@
         # expression is the name of a leaking flow
         elif expression in self.sfd.nodes and self.sfd.nodes[expression]['leak']:
             if not self.is_initialised: # it's currently in the process of init_stocks, no leaks have been calculated
                 self.n_indentation -= 1
                 return 0 # leaks are currently all 0
 
         else:  # calculation is needed
-            # print(self.n_indentation*'\t' + 'calc h:', expression, 'SUB:', subscript)
+            # print(self.n_indentation*'\t' + 'calc h:', expression, subscript)
             if expression in self.sfd.nodes: # careful - outflows from conveyors have eqn 0 but should not be dealt with here
                 # print(self.n_indentation*'\t' + 'calc h1:', self.sfd.nodes[expression]['equation'])
-                # print(self.n_indentation*'\t' + 'retriving:', list(self.sfd.nodes[expression]['equation'].keys()))
                 if subscript in self.sfd.nodes[expression]['equation'].keys():
                     # print(self.n_indentation*'\t' + 'calc h1.1')
                     equation = self.sfd.nodes[expression]['equation'][subscript]
                 else:
                     # print(self.n_indentation*'\t' + 'calc h1.2')
                     equation = self.sfd.nodes[expression]['equation']['nosubscript']
             else:
                 equation = expression
 
             # replace abc[subscript] -> abc__ele1__subscript__ele2__
             if type(equation) is str:
-                equation = self.process_expression(equation, intended_subscripts=subscript)
+                equation = self.process_expression(equation)
             
             # pre-process expression to match Python syntax
             # replace '=' with '=='
             if type(equation) is str:
                 reg = "(?<!(<|>|=))=(?!(<|>|=))"
                 equation = re.sub(reg, "==", equation)
             
             value = None
 
             while type(value) not in [int, float, np.int64, bool]: # if value has not become a number (taking care of the numpy data types)
                 
-                # check if the expression is an external DataFeeder
-                if type(equation) is DataFeeder:
-                    # print('calc df')
-                    equation = equation(self.current_time)
-
                 # check if the variable is a graph function which has an additonal layer that transforms the equation outcome
                 if type(equation) is GraphFunc:
                     # print('calc h0')
                     input = self.calculate_experiment(equation.eqn, subscript)
                     equation = equation(input)
                 
                 # check if this is a conditional statement
@@ -1267,50 +1199,41 @@
                         equation = 'True'
                     else:
                         equation = 'False'
 
                 # check if there are time-related functions in the equation
                 elif type(equation) is str and re.findall(r"(\w+)[(].+[)]", str(equation)):
                     func_names = re.findall(r"(\w+)[(].+[)]", str(equation))
-                    # print(self.n_indentation*'\t'+'calc h3')
+                    # print('calc h3')
                     for func_name in func_names:
-                        # print(self.n_indentation*'\t'+'calc h3.0', func_name)
+                        # print(0, equation)
+                        # print('calc h3 0', func_name)
                         if func_name in self.time_related_functions.keys():
                             func_args = re.findall(r"\w+[(](.+)[)]", str(equation))
-                            # print(self.n_indentation*'\t'+'calc h3.0.0',func_args)
+                            # print('1',func_args)
                             func_args_split = func_args[0].split(",")
-                            # print(self.n_indentation*'\t'+'calc h3.0.1',func_names[0], func_args_split)
+                            # print('2',func_names[0], func_args_split)
 
                             # pass args to the corresponding time-related function
                             func_args_full = [subscript] + func_args_split
                             func_value = self.time_related_functions[func_names[0]](*func_args_full)
                             
                             # replace the init() parts in the equation with their values
                             func_value_str = str(func_value)
                             func_str = func_name+'('+func_args[0]+')'
                             equation = equation.replace(func_str, func_value_str) # in case init() is a part of an equation, substitue init() with its value
-                            # print(self.n_indentation*'\t'+'calc h3.0.2', equation)
-
-                # # check if the expression is abc__ele1__subscript__ele2__
-                # elif type(expression) is str and '__ele1__' in expression:
-                #     print('process b')
-                #     expression, subscript = expression.split('__ele1__', 1)
-                #     subscript, remaining = subscript.split('__ele2__', 1)
-                #     print('process b', expression, subscript, remaining)
-
-                # if type(equation) is str and '[' in equation:
-                #     equation = self.process_expression(equation)
+                            # print('3', equation)
 
                 '''
                 Until here, all we want to have is an modified equation suitable for evaluation.
                 '''
 
                 try:
                     # print(self.n_indentation*'\t' + 'eval:', equation)
-                    value = eval(str(equation), self.custom_functions) # TODO: 'Beds' in 'TimeToAddBeds' got replaced by the value of var 'Beds'. Fix needed
+                    value = eval(str(equation), self.custom_functions)
                     # print(self.n_indentation*'\t'+'Evaluated {} = {}'.format(equation, value))
 
                 except NameError as e:
                     s = e.args[0]
                     p = s.split("'")[1]
                     # print(self.n_indentation*'\t'+'NameError {} for equation: {}'.format(p,equation))
                     val = self.calculate_experiment(p, subscript)
@@ -1323,64 +1246,49 @@
                     raise e
             
             if expression in self.sfd.nodes:
 
                 # Noted 21/8/2022: This is not OK. Positive check of non-negative stocks should be performed when updating the stock, not calculating flows. -10->[0]-10-> is legitimate but not pass here.
                 # non-negative control of flows
                 if self.sfd.nodes[expression]['element_type'] == 'flow':
-                    # when flow is not bi-flow, i.e., cannot go negative
                     if self.sfd.nodes[expression]['non_negative']:
                         if value < 0:
                             # print('Flow {} is non-negative but is going under 0 to {}.'.format(expression, value))
                             value = 0
-                    # check if flow is constrained by the stock it is drawing from; this is not perfect - if 2 flows f1, f2 are drawing from the same stock, f2 is constrained by s-f1, not just s
-                    if self.sfd.nodes[expression]['flow_from'] is not None:
-                        stock_flow_from_level = self.__name_values[self.current_time][self.sfd.nodes[expression]['flow_from']][subscript]
-                        if value > stock_flow_from_level:
-                            value = stock_flow_from_level
-
+                
                 # leak flows have eqn but it's not for value, but for leak fraction. Check before register
                 if self.sfd.nodes[expression]['leak']:
                     pass
-                # register calculated values to __name_values
                 else:
-                    if 'nosubscript' in self.sfd.nodes[expression]['equation'].keys(): # A variable is not subscripted but is used to calculate a subscripted variable
-                        self.__name_values[self.current_time][expression]['nosubscript'] = value
-                    else:
-                        self.__name_values[self.current_time][expression][subscript] = value
+                    self.__name_values[self.current_time][expression][subscript] = value
 
                 try:  # when initialising stock values, there's no 'self.visited' yet
                     # print('calc updating vidited', expression, subscript, value)
                     if expression in self.sfd.nodes: # only register those that are variable names in the model
                         if expression not in self.visited.keys():
                             self.visited[expression] = dict()
                         if subscript not in self.visited[expression].keys():
                             self.visited[expression][subscript] = value
                 except AttributeError:
                     pass
             
-            if self.verbose:
-                print(self.n_indentation*'\t'+'calc-ed value:'+str(value))
-            
             self.n_indentation -= 1
             return value
 
 
     def clear_last_run(self):
         """
         Clear values for all nodes
         :return:
         """
         self.current_step = 1
         self.current_time = self.initial_time
 
-        # for name in self.__name_values.keys():
-        #     self.__name_values[name] = dict()
-
-        self.__name_values = dict()
+        for name in self.__name_values.keys():
+            self.__name_values[name] = dict()
         
         self.__built_in_variables['TIME'] = list()
         
         # reset delay_registers
         self.delay_registers = dict()
 
         # reset is_initialised flag
@@ -1493,25 +1401,19 @@
         """
         # step 1: if not stock, remove all incoming connectors into this variable (node)
         #         if stock, just reset it's (initial) value
         # step 2: replace the equation of this variable in the graph representation
         # step 3: confirm connectors based on the new equation (only when the new equation is a function not a number
         # print("Engine: Replacing equation of {}".format(name))
         
-        if new_equation is None:
-        #     new_equation_parsed = self.text_to_equation(new_equation)
-        # else:
+        if new_equation is not None:
+            new_equation_parsed = self.text_to_equation(new_equation)
+        else:
             raise Exception("New equation for replacing could not be None.")
         
-        # step 0: consider DataFeeder
-        if type(new_equation) is DataFeeder:
-            self.sfd.nodes[name]['equation']['nosubscript'] = new_equation
-            self.sfd.nodes[name]['external'] = True
-            return
-
         # step 1:
         if self.sfd.nodes[name]['element_type'] != 'stock':
             to_remove = list()
             for u, v in self.sfd.in_edges(name):
                 # print("In_edge found:", u, v)
                 to_remove.append((u, v))
             self.sfd.remove_edges_from(to_remove)
@@ -1535,20 +1437,20 @@
                 subscript_elements.append(elements)
             subscripts = pd.MultiIndex.from_product(subscript_elements, subscript_names)
         
         for ix in subscripts:
             self.sfd.nodes[name]['equation'][ix] = new_equation
         
             # step 3:
-            # if type(new_equation) not in [int, float]:
-            #     # If new equation (parsed list) does not starts with a number, 
-            #     # it's not a constant value, but a function
-            #     if type(new_equation) is not str:
-            #         self.__add_function_dependencies(name, new_equation, ix)
-            #         # print("Engine: New edges created.")
+            if type(new_equation_parsed[0]) not in [int, float]:
+                # If new equation (parsed list) does not starts with a number, 
+                # it's not a constant value, but a function
+                if type(new_equation_parsed) is not str:
+                    self.__add_function_dependencies(name, new_equation_parsed, ix)
+                    # print("Engine: New edges created.")
 
     def remove_element(self, name):
         """
         Delete an element
         :param name:
         :return:
         """
@@ -1559,33 +1461,24 @@
         self.sfd.remove_edge(from_element, to_element)
 
     # Reset a structure
     def reset_a_structure(self):
         self.sfd.clear()
 
     # Return a behavior
-    def get_element_simulation_result(self, name):
-        full_result = dict()
-        for time, values in self.__name_values.items():
-            time_result = dict()
-            time_result[self.time_units] = time
-            name_output = name.replace('_', ' ')
-            if name_output[0].isdigit():
-                name_output = '"{}"'.format(name_output)
-            
-            for ix in self.__name_values[time][name].keys():
-                if ix == 'nosubscript':
-                    time_result[name_output] = values[name]['nosubscript']
-                else:
-                    time_result[name_output+'[{}]'.format(ix.replace('__cmm__', ', ').replace('_', ' '))] = values[name][ix]
-            full_result[time] = time_result
-        # return full_result
-        df_full_result = pd.DataFrame.from_dict(full_result).transpose()
-        df_full_result.set_index(self.time_units, inplace=True)
-        return df_full_result[name]
+    def get_element_simulation_result(self, name, subscripts=None):
+        if subscripts is None:
+            subscripts = self.__name_values[name].keys()
+        result = self.__name_values[name]
+        result_dict = dict()
+        for ix in subscripts:
+            result_dict[ix] = result[ix]  # return a list of values; not a pandas DataFrame
+        if len(result_dict) == 1:
+            result_dict = next(iter(result_dict.values()))
+        return result_dict
 
     # Return all simulation results as a pandas DataFrame
     def export_simulation_result(self):
         full_result = dict()
         for time, values in self.__name_values.items():
             # time_result = pd.DataFrame(index=None)
             time_result = dict()
@@ -1597,15 +1490,15 @@
                 if node_output[0].isdigit():
                     node_output = '"{}"'.format(node_output)
                 
                 for ix in self.__name_values[time][node].keys():
                     if ix == 'nosubscript':
                         time_result[node_output] = values[node]['nosubscript']
                     else:
-                        time_result[node_output+'[{}]'.format(ix.replace('__cmm__', ', ').replace('_', ' '))] = values[node][ix]
+                        time_result[node_output+'[{}]'.format(ix.replace('_', ' '))] = values[node][ix]
             full_result[time] = time_result
         df_full_result = pd.DataFrame.from_dict(full_result).transpose()
         df_full_result.set_index(self.time_units, inplace=True)
         return df_full_result
 
     # Draw results
     def display_results(self, variables=None, dpi=100, rtn=False):
```

### Comparing `asdm-0.0.2/apps/Smoking_Cessation/smoking_cessation.py` & `asdm-0.0.3/apps/Smoking_Cessation/smoking_cessation.py`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/asdm.egg-info/PKG-INFO` & `asdm-0.0.3/asdm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asdm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Agile System Dynamics Engine
 Author-email: Wang Zhao <wang.zhao@strath.ac.uk>, Matt Stammers <matt@reallyusefulmodels.com>
 License: MIT License
         
         Copyright (c) 2022 W.Zh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,49 +54,40 @@
 
 We recommend that you use pip to install asdm but if you do wish to develop it further pipenv instructions are provided. 
 
 ## Tutorial Notebooks
 
 We use a series of Jupyter Notebooks to provide functionality guidance for the users.
 
-1. [SD Modelling](./1-SD_modelling.ipynb)
+1. [SD Modelling](https://github.com/wzh1895/ASDM/blob/main/Demo_SD_modelling.ipynb)
 
 - Creating an SD model from scratch
   - Adding stocks, flows, auxiliaries
   - Support for nonlinear functions (MIN, MAX, etc.)
   - Support for stochastic functions (random binomial trial, etc.)
 - Running simulations
 - Exporting and examing simulation outcomes
 - Displaying simulation outcomes as graph
 
-2. [Model Calibration](./2-SD_model_calibration.ipynb) [STILL IN DEVELOPMENT]
-
-- Estimating SD model parameters using Markov Chain Monte Carlo (MCMC)
-  - Support for MLE (maximum likelihood) and MAP (maximum a posteriori) approach
-  - Support for different modellings of payoff (squared error, Poisson, etc.) that are used in the likelihood function
-  - Support for different sampling methods (Slice, Metropolis, NUTS, Hamiltonian, etc.), enabled by [PyMC3](https://docs.pymc.io/en/v3/)
-- Diagnostic analyses of MCMC samples, enabled by [Arviz](https://arviz-devs.github.io/arviz/)
-  - Trace plot
-  - Autocorrelation plot
-- Comparison between Historical data and simulation data
-
-3. More to come...
-
 ## Why ASDM?
 
 Acknowledging that there are a number of SD tools that enable simulating SD models in a Python environment (see [PySD](https://github.com/JamesPHoughton/pysd) and [venpy](https://github.com/pbreach/venpy.git)), we build ASDM to bring the capability of **structure modelling** to the Python SD community. ASDM allows users to create an SD model from scratch and edit model structure as needed. With a native Python implementation of stock-and-flow structure, ASDM allows building SD models without software like [Vensim](https://vensim.com/) and [Stella](https://www.iseesystems.com/store/products/stella-architect.aspx).
 
 The long-term goal ASDM intends to achieve is an approach for **data-informed structure modelling** where data can be used to finetune SD model structure automatically. This is both an extension of data-informed SD model parameter estimation, and an innovative way to discover feedback structures from data.
 
 ## Limitations
 
 The main drawback at the moment is that we have not been working a lot on **translating Vensim/Stella models** into the format that ASDM uses, although [PySD](https://github.com/JamesPHoughton/pysd) has proved this fully doable. This functionality is in our development roadmap.
 
 We have neither been working a lot on **the speed of simulation**. Although simulating large SD models given mordern computer specs would not be extremely time-consuming, in tasks involing Monte Carlo simulation (such as parameter estimation) the speed of running a model can matter a lot more. Acceleration is in our development roadmap too.
 
+## Docs
+
+Full docs are incoming
+
 ## Licence
 
 ASDM is made public under the MIT licence.
 
 ## Authors
 **Wang Zhao**  
 PhD candidate at University of Strathclyde, UK
```

### Comparing `asdm-0.0.2/asdm.egg-info/SOURCES.txt` & `asdm-0.0.3/asdm.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,55 @@
 .gitignore
-1-SD_modelling.ipynb
-ASDM.code-workspace
+Demo_SD_modelling.ipynb
 LICENSE
 Pipfile
 Pipfile.lock
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 ASDM/ASDM.py
-ASDM/MCMC.py
-ASDM/Optimizer.py
-ASDM/Parser.excalidraw
-ASDM/Parser_XMILE.py
-ASDM/Payoff.py
-ASDM/Probability.py
-ASDM/SpeedComparison.py
 ASDM/Utilities.py
 ASDM/__init__.py
-ASDM/test_Behaviour.py
-ASDM/test_Engine.py
-ASDM/test_MultipleRuns.py
-ASDM/test_Parser.py
-ASDM/test_Solver.py
 ASDM/Diagrams/ASDM.excalidraw
 ASDM/Diagrams/EngineOOP.excalidraw
+ASDM/Diagrams/Parser.excalidraw
 ASDM/Diagrams/Parser1.png
 ASDM/Diagrams/Parser2.png
+ASDM/Inference/MCMC.py
+ASDM/Inference/Optimizer.py
+ASDM/Inference/Payoff.py
+ASDM/Inference/Probability.py
+ASDM/Inference/__init__.py
 apps/ERM/3-From_XMILE.ipynb
 apps/ERM/ERM_ASDM_app.py
 apps/ERM/Elective Recovery Model.stmx
 apps/ERM/Elective Recovery Model.xlsx
 apps/ERM/Elective_Recovery_Model.PNG
 apps/Goal_Gap/Goal_gap_model.png
 apps/Goal_Gap/Revised_Goal_Gap.py
 apps/Goal_Gap/Revised_Goal_Gap.stmx
 apps/Goal_Gap/goal_gap.py
 apps/Smoking_Cessation/smoking_cessation.py
-apps/Smoking_Cessation/ASDM/Engine.py
-apps/Smoking_Cessation/ASDM/MCMC.py
-apps/Smoking_Cessation/ASDM/Optimizer.py
-apps/Smoking_Cessation/ASDM/Parser_XMILE.py
-apps/Smoking_Cessation/ASDM/Payoff.py
-apps/Smoking_Cessation/ASDM/Probability.py
-apps/Smoking_Cessation/ASDM/Utilities.py
-apps/Smoking_Cessation/ASDM/__init__.py
-apps/Smoking_Cessation/ASDM/Diagrams/ASDM.excalidraw
 asdm.egg-info/PKG-INFO
 asdm.egg-info/SOURCES.txt
 asdm.egg-info/dependency_links.txt
 asdm.egg-info/requires.txt
 asdm.egg-info/top_level.txt
 assets/images/Goal_gap_model.png
 assets/images/Infection_model.png
 assets/images/Simplified_patient_flow_model.png
-notebooks/0-Performance_comparison.ipynb
-notebooks/2-SD_model_calibration.ipynb
-notebooks/ValidateOutcome.ipynb
-tests/__init__.py
+notebooks/ValidateSimuOutcomes.ipynb
 tests/run_tests.py
-tests/test_goal_gap_model.py
+tests/test_Behaviour.py
+tests/test_Engine.py
+tests/test_Externals.py
+tests/test_MultipleRuns.py
+tests/test_Parser.py
+tests/test_Solver.py
 tests/BuiltInTestModels/Array_cross_reference.stmx
 tests/BuiltInTestModels/Array_cross_reference_inference.stmx
 tests/BuiltInTestModels/Array_parallel_reference.stmx
 tests/BuiltInTestModels/Basic_math.stmx
 tests/BuiltInTestModels/Built_in_vars.stmx
 tests/BuiltInTestModels/Conveyor.stmx
 tests/BuiltInTestModels/Conveyor_initialisation.stmx
@@ -80,15 +66,14 @@
 tests/BuiltInTestModels/INIT.stmx
 tests/BuiltInTestModels/Isolated_var.stmx
 tests/BuiltInTestModels/LOOKUP.stmx
 tests/BuiltInTestModels/Logic.stmx
 tests/BuiltInTestModels/MOD.stmx
 tests/BuiltInTestModels/MOD_arrayed.stmx
 tests/BuiltInTestModels/Min_Max.stmx
-tests/BuiltInTestModels/Modules.stmx
 tests/BuiltInTestModels/Non-negative_stocks.stmx
 tests/BuiltInTestModels/Non-negative_stocks_with_flows.stmx
 tests/BuiltInTestModels/Smooth.stmx
 tests/BuiltInTestModels/Time_related_functions.stmx
 tests/BuiltInTestModels/Time_unit.stmx
 tests/BuiltInTestModels/Stella_outcomes/Array_cross_reference.csv
 tests/BuiltInTestModels/Stella_outcomes/Array_cross_reference_inference.csv
@@ -115,8 +100,18 @@
 tests/BuiltInTestModels/Stella_outcomes/MOD_arrayed.csv
 tests/BuiltInTestModels/Stella_outcomes/Min_Max.csv
 tests/BuiltInTestModels/Stella_outcomes/Modules.csv
 tests/BuiltInTestModels/Stella_outcomes/Non-negative_stocks.csv
 tests/BuiltInTestModels/Stella_outcomes/Non-negative_stocks_with_flows.csv
 tests/BuiltInTestModels/Stella_outcomes/Smooth.csv
 tests/BuiltInTestModels/Stella_outcomes/Time_related_functions.csv
-tests/BuiltInTestModels/Stella_outcomes/Time_unit.csv
+tests/BuiltInTestModels/Stella_outcomes/Time_unit.csv
+tests/Discarded/EngineArrays.py
+tests/Discarded/EngineArraysTest.ipynb
+tests/Discarded/EngineArraysTest.py
+tests/Discarded/EngineNew0.py
+tests/Discarded/EngineNew1.py
+tests/Discarded/EngineNew2.py
+tests/Discarded/EngineOOP.py
+tests/Discarded/EngineStatic.py
+tests/Discarded/Var.py
+tests/Discarded/sly_example.py
```

### Comparing `asdm-0.0.2/assets/images/Goal_gap_model.png` & `asdm-0.0.3/assets/images/Goal_gap_model.png`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/assets/images/Infection_model.png` & `asdm-0.0.3/assets/images/Infection_model.png`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/assets/images/Simplified_patient_flow_model.png` & `asdm-0.0.3/assets/images/Simplified_patient_flow_model.png`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/pyproject.toml` & `asdm-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/requirements.txt` & `asdm-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Array_cross_reference.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Array_cross_reference.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Array_cross_reference_inference.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Array_cross_reference_inference.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Array_parallel_reference.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Array_parallel_reference.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Basic_math.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Basic_math.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Built_in_vars.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Built_in_vars.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Conveyor.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Conveyor.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Conveyor_initialisation.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Conveyor_initialisation.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Conveyor_leakage.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Conveyor_leakage.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Conveyor_leakage1.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Conveyor_leakage1.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Conveyor_leakage2.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Conveyor_leakage2.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Delays.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Delays.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Delays2.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Delays2.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Goal_gap.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Goal_gap.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Goal_gap_array.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Goal_gap_array.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Graph_function.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Graph_function.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/History.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/History.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/IF_THEN_ELSE.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/IF_THEN_ELSE.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/INIT.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/INIT.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Isolated_var.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Isolated_var.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/LOOKUP.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/LOOKUP.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Logic.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Logic.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/MOD.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/MOD.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/MOD_arrayed.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/MOD_arrayed.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Min_Max.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Min_Max.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Modules.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Non-negative_stocks_with_flows.stmx`

 * *Files 13% similar despite different names*

#### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Modules.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Non-negative_stocks_with_flows.stmx`

```diff
@@ -1,45 +1,124 @@
 <?xml version="1.0" encoding="utf-8"?>
 <xmile xmlns="http://docs.oasis-open.org/xmile/ns/XMILE/v1.0" xmlns:isee="http://iseesystems.com/XMILE" version="1.0">
   <header>
-    <smile version="1.0" namespace="std, isee" uses_submodels=""/>
-    <name>Modules</name>
-    <uuid>304ce7c7-1293-4c1f-bb56-f696378a7d3d</uuid>
+    <smile version="1.0" namespace="std, isee"/>
+    <name>Non-negative_stocks_with_flows</name>
+    <uuid>537894ae-ccc9-463b-b0ee-a643f5e1cbb8</uuid>
     <vendor>isee systems, inc.</vendor>
     <product version="2.0" isee:build_number="2176" isee:saved_by_v1="true" lang="en">Stella Professional</product>
   </header>
-  <sim_specs isee:sim_duration="0.5" isee:simulation_delay="0.125" isee:restore_on_start="false" method="Euler" time_units="Months" isee:instantaneous_flows="false" isee:loop_scores="true" isee:loop_exhaustive_allowed="1000">
+  <sim_specs isee:sim_duration="1.5" isee:simulation_delay="0.214286" isee:restore_on_start="false" method="Euler" time_units="Months" isee:instantaneous_flows="false" isee:loop_scores="false" isee:loop_exhaustive_allowed="1000">
     <start>1</start>
-    <stop>5</stop>
-    <dt reciprocal="true">4</dt>
+    <stop>8</stop>
+    <dt reciprocal="true">1</dt>
   </sim_specs>
-  <isee:prefs show_module_prefix="true" live_update_on_drag="true" show_restore_buttons="false" layer="model" interface_scale_ui="true" interface_max_page_width="10000" interface_max_page_height="10000" interface_min_page_width="0" interface_min_page_height="0" rerun_on_structure_change="false" saved_runs="5" keep="false" rifp="true"/>
+  <isee:prefs show_module_prefix="true" live_update_on_drag="true" show_restore_buttons="false" layer="model" interface_scale_ui="true" interface_max_page_width="10000" interface_max_page_height="10000" interface_min_page_width="0" interface_min_page_height="0" rerun_on_structure_change="false" saved_runs="1" keep="false" rifp="true"/>
   <isee:multiplayer_settings include_chat="true" allow_observers="false" advance_time_increment="1" observer_start_page="home_page" enabled="false"/>
   <isee:time_formats default_format="Builtin">
     <isee:time_format name="Builtin" type="adaptive"/>
   </isee:time_formats>
   <default_format/>
   <data>
     <export resource="/Users/jonker/Library/CloudStorage/OneDrive-UniversityofStrathclyde/ASDM/stella.csv" interval="DT" precomputed="false" isee:format="numbers">
       <all/>
     </export>
   </data>
   <model_units/>
   <model>
     <variables>
-      <aux name="a">
-        <eqn>1</eqn>
+      <stock name="Stock 1">
+        <eqn>OutFlow_1+OutFlow_2-20</eqn>
+        <inflow>InFlow</inflow>
+        <outflow>OutFlow_1</outflow>
+        <outflow>OutFlow_2</outflow>
+        <non_negative/>
+      </stock>
+      <flow name="OutFlow 1">
+        <eqn>50</eqn>
+        <non_negative/>
+      </flow>
+      <flow name="InFlow">
+        <eqn>30</eqn>
+        <non_negative/>
+      </flow>
+      <flow name="OutFlow 2">
+        <eqn>10</eqn>
+        <non_negative/>
+      </flow>
+      <aux name="Converter 1">
+        <eqn>OutFlow_1</eqn>
       </aux>
-      <module name="Module 1" isee:label="">
-        <connect to="Module_1.a" from=".a"/>
-        <connect2 to="Module_1.a" from="a"/>
-        <connect to=".b" from="Module_1.b"/>
-        <connect2 to="b" from="Module_1.b"/>
-      </module>
-      <aux name="b" access="input"/>
+      <aux name="Converter 2">
+        <eqn>OutFlow_2</eqn>
+      </aux>
+      <aux name="Converter 3">
+        <eqn>Stock_1</eqn>
+      </aux>
+      <stock name="Stock 2">
+        <eqn>0</eqn>
+        <inflow>InFlow2</inflow>
+        <non_negative/>
+      </stock>
+      <flow name="InFlow2">
+        <eqn>-3</eqn>
+        <non_negative/>
+      </flow>
+      <stock name="Stock 3">
+        <eqn>20</eqn>
+        <outflow>Flow_1</outflow>
+        <outflow>Flow_2</outflow>
+        <non_negative/>
+      </stock>
+      <stock name="Stock 4">
+        <eqn>20</eqn>
+        <outflow>Flow_3</outflow>
+        <outflow>Flow_4</outflow>
+        <non_negative/>
+      </stock>
+      <flow name="Flow 1">
+        <eqn>15</eqn>
+        <non_negative/>
+      </flow>
+      <flow name="Flow 2">
+        <eqn>15</eqn>
+        <non_negative/>
+      </flow>
+      <flow name="Flow 3">
+        <eqn>15</eqn>
+        <non_negative/>
+      </flow>
+      <flow name="Flow 4">
+        <eqn>15</eqn>
+        <non_negative/>
+      </flow>
+      <stock name="Stock 5">
+        <eqn>20</eqn>
+        <inflow>Flow_5</inflow>
+        <outflow>Flow_6</outflow>
+        <outflow>Flow_7</outflow>
+        <outflow>Flow_8</outflow>
+        <non_negative/>
+      </stock>
+      <flow name="Flow 5">
+        <eqn>20</eqn>
+        <non_negative/>
+      </flow>
+      <flow name="Flow 6">
+        <eqn>10</eqn>
+        <non_negative/>
+      </flow>
+      <flow name="Flow 7">
+        <eqn>20</eqn>
+        <non_negative/>
+      </flow>
+      <flow name="Flow 8">
+        <eqn>30</eqn>
+        <non_negative/>
+      </flow>
     </variables>
     <views>
       <style color="black" background="white" font_style="normal" font_weight="normal" text_decoration="none" text_align="center" vertical_text_align="center" font_color="black" font_family="Arial" font_size="10pt" padding="2" border_color="black" border_width="thin" border_style="none">
         <text_box color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt"/>
         <isee:loop_indicator color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt"/>
         <numeric_display color="blue" background="white" font_size="9pt" isee:transparent="false"/>
         <graph color="black" background="white" font_size="12pt" axis_color="#666666" grid_color="#C8C8C8" isee:graph_area_color="white" legend_position="bottom" isee:transparent="false" isee:hide_border="false" axis_title_font_style="normal" axis_title_font_weight="normal" axis_title_text_decoration="none" axis_title_text_align="center" axis_title_vertical_text_align="center" axis_title_font_color="black" axis_title_font_family="Arial" axis_title_font_size="12pt" axis_title_text_padding="2" axis_title_text_border_color="black" axis_title_text_border_width="thin" axis_title_text_border_style="none" axis_label_font_style="normal" axis_label_font_weight="normal" axis_label_text_decoration="none" axis_label_text_align="center" axis_label_vertical_text_align="center" axis_label_font_color="black" axis_label_font_family="Arial" axis_label_font_size="9pt" axis_label_text_padding="2" axis_label_text_border_color="black" axis_label_text_border_width="thin" axis_label_text_border_style="none">
@@ -78,15 +157,15 @@
         <isee:animation_object color="black" background="white" font_size="12pt"/>
         <isee:navigation_widget color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt" border_color="#999999" border_width="thin" border_style="solid" item_spacing="6" appearance="tabs" corner_radius="4" selected_item_color="black" selected_item_background="white" item_background="#DDDDDD"/>
         <isee:shape color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt" border_width="thin" border_style="solid" opacity="1" transparent_background="true"/>
         <isee:selector color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt"/>
         <isee:iframe color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt" border_width="thin" border_style="solid"/>
         <isee:financial_table color="black" background="#E0E0E0" text_align="right" font_size="12pt" auto_fit="true" first_column_width="250" other_column_width="100" header_font_style="normal" header_font_weight="bold" header_text_decoration="none" header_text_align="center" header_vertical_text_align="center" header_font_color="black" header_font_family="Arial" header_font_size="14pt" header_text_padding="2" header_text_border_color="black" header_text_border_width="thin" header_text_border_style="none"/>
       </style>
-      <view isee:show_pages="false" background="white" page_width="818" page_height="571" isee:popup_graphs_are_comparative="true" isee:enable_non_negative_highlights="false" type="stock_flow">
+      <view isee:show_pages="false" background="white" page_width="818" page_height="571" isee:page_cols="2" isee:page_rows="3" isee:scroll_x="281" isee:scroll_y="408" isee:popup_graphs_are_comparative="true" isee:enable_non_negative_highlights="false" type="stock_flow">
         <style color="black" background="white" font_style="normal" font_weight="normal" text_decoration="none" text_align="center" vertical_text_align="center" font_color="black" font_family="Arial" font_size="10pt" padding="2" border_color="black" border_width="thin" border_style="none">
           <stock color="blue" background="white" font_color="blue" font_size="9pt" label_side="top">
             <shape type="rectangle" width="45" height="35"/>
           </stock>
           <flow color="blue" background="white" font_color="blue" font_size="9pt" label_side="bottom"/>
           <isee:placeholder color="#228B22" background="white" font_color="#228B22" font_size="9pt" label_side="bottom"/>
           <module color="blue" background="white" font_color="blue" font_size="9pt" label_side="top">
@@ -115,72 +194,135 @@
               <isee:series_style color="#F586FF" thickness="1" pen_style="dotted"/>
               <isee:series_style color="black" thickness="1" pen_style="dashed"/>
               <isee:series_style color="#C8C8C8" thickness="1"/>
             </isee:series_styles>
           </graph>
           <table color="black" background="#E0E0E0" text_align="right" font_size="12pt" orientation="vertical" wrap_text="false" isee:auto_fit="true" isee:use_alternate_row_colors="false" isee:unlimited_table_length="false" blank_column_width="80" column_width="160" interval="1" report_balances="beginning" report_flows="instantaneous" header_font_style="normal" header_font_weight="normal" header_text_decoration="none" header_text_align="center" header_vertical_text_align="center" header_font_color="black" header_font_family="Arial" header_font_size="12pt" header_text_padding="2" header_text_border_color="black" header_text_border_width="thin" header_text_border_style="none"/>
         </style>
-        <aux x="270" y="223" name="a"/>
-        <module x="426" y="254.5" name="Module 1"/>
-        <connector uid="1" angle="17.8787">
-          <from>a</from>
-          <to>Module_1</to>
+        <stock x="363" y="174" name="Stock 1"/>
+        <flow x="468.75" y="174" name="OutFlow 1">
+          <pts>
+            <pt x="385.5" y="174"/>
+            <pt x="576" y="174"/>
+          </pts>
+        </flow>
+        <flow x="255.25" y="174" name="InFlow">
+          <pts>
+            <pt x="170" y="174"/>
+            <pt x="340.5" y="174"/>
+          </pts>
+        </flow>
+        <flow x="364" y="261.75" name="OutFlow 2">
+          <pts>
+            <pt x="364" y="191.5"/>
+            <pt x="364" y="353"/>
+          </pts>
+        </flow>
+        <aux x="549" y="99" name="Converter 1"/>
+        <connector uid="1" angle="72.646">
+          <from>OutFlow_1</from>
+          <to>Converter_1</to>
         </connector>
-        <aux font_style="italic" font_weight="bold" x="284" y="326" name="b"/>
-        <connector uid="2" angle="188.945">
-          <from>Module_1</from>
-          <to>b</to>
+        <aux x="464" y="332" name="Converter 2"/>
+        <connector uid="2" angle="4.49258">
+          <from>OutFlow_2</from>
+          <to>Converter_2</to>
         </connector>
-      </view>
-    </views>
-  </model>
-  <model name="Module_1">
-    <variables>
-      <aux name="a" access="input"/>
-      <aux name="b" access="output">
-        <eqn>2</eqn>
-      </aux>
-    </variables>
-    <views>
-      <view isee:show_pages="false" background="white" page_width="818" page_height="571" isee:popup_graphs_are_comparative="true" isee:enable_non_negative_highlights="false" type="stock_flow">
-        <style color="black" background="white" font_style="normal" font_weight="normal" text_decoration="none" text_align="center" vertical_text_align="center" font_color="black" font_family="Arial" font_size="10pt" padding="2" border_color="black" border_width="thin" border_style="none">
-          <stock color="blue" background="white" font_color="blue" font_size="9pt" label_side="top">
-            <shape type="rectangle" width="45" height="35"/>
-          </stock>
-          <flow color="blue" background="white" font_color="blue" font_size="9pt" label_side="bottom"/>
-          <isee:placeholder color="#228B22" background="white" font_color="#228B22" font_size="9pt" label_side="bottom"/>
-          <module color="blue" background="white" font_color="blue" font_size="9pt" label_side="top">
-            <shape type="rectangle" width="55" height="45"/>
-          </module>
-          <aux color="blue" background="white" font_color="blue" font_size="9pt" label_side="bottom">
-            <shape type="circle" radius="18"/>
-          </aux>
-          <group color="red" background="white" font_color="red" font_size="9pt"/>
-          <connector color="#FF007F" background="white" font_color="#FF007F" font_size="9pt" isee:thickness="1"/>
-          <text_box color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt"/>
-          <isee:loop_indicator color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt"/>
-          <numeric_display color="blue" background="white" font_size="9pt" isee:transparent="false"/>
-          <graph color="black" background="white" font_size="12pt" axis_color="#666666" grid_color="#C8C8C8" isee:graph_area_color="white" legend_position="bottom" isee:transparent="false" isee:hide_border="false" axis_title_font_style="normal" axis_title_font_weight="normal" axis_title_text_decoration="none" axis_title_text_align="center" axis_title_vertical_text_align="center" axis_title_font_color="black" axis_title_font_family="Arial" axis_title_font_size="12pt" axis_title_text_padding="2" axis_title_text_border_color="black" axis_title_text_border_width="thin" axis_title_text_border_style="none" axis_label_font_style="normal" axis_label_font_weight="normal" axis_label_text_decoration="none" axis_label_text_align="center" axis_label_vertical_text_align="center" axis_label_font_color="black" axis_label_font_family="Arial" axis_label_font_size="9pt" axis_label_text_padding="2" axis_label_text_border_color="black" axis_label_text_border_width="thin" axis_label_text_border_style="none">
-            <isee:series_styles>
-              <isee:series_style color="blue" thickness="1"/>
-              <isee:series_style color="red" thickness="1" pen_style="dot_dashed"/>
-              <isee:series_style color="fuchsia" thickness="1" pen_style="dotted"/>
-              <isee:series_style color="#008F44" thickness="1" pen_style="dashed"/>
-              <isee:series_style color="#FF7F00" thickness="1"/>
-              <isee:series_style color="#7F00FF" thickness="1" pen_style="dot_dashed"/>
-              <isee:series_style color="#0CA0FF" thickness="1" pen_style="dotted"/>
-              <isee:series_style color="lime" thickness="1" pen_style="dashed"/>
-              <isee:series_style color="#FF007F" thickness="1"/>
-              <isee:series_style color="aqua" thickness="1" pen_style="dot_dashed"/>
-              <isee:series_style color="#F586FF" thickness="1" pen_style="dotted"/>
-              <isee:series_style color="black" thickness="1" pen_style="dashed"/>
-              <isee:series_style color="#C8C8C8" thickness="1"/>
-            </isee:series_styles>
+        <stacked_container uid="3" x="200.75" y="425" width="557" height="418">
+          <graph width="557" height="418" type="time_series" isee:points_only="false" show_grid="false" include_units_in_legend="false" plot_numbers="false" isee:label_pie_slices="false" num_x_grid_lines="0" num_y_grid_lines="0" num_x_labels="8" num_y_labels="11" isee:fill_intensity="0.1" isee:allow_zero_axis="true" left_axis_multi_scale="false" left_axis_auto_scale="true" left_include_units="true" right_axis_multi_scale="false" right_axis_auto_scale="true" right_include_units="true">
+            <plot color="blue" isee:keep_zero_visible="true" pen_width="1" index="0" show_y_axis="true">
+              <entity name="InFlow"/>
+            </plot>
+            <plot color="red" pen_style="dot_dashed" isee:keep_zero_visible="true" pen_width="1" index="1" show_y_axis="true">
+              <entity name="OutFlow_1"/>
+            </plot>
+            <plot color="fuchsia" pen_style="dotted" isee:keep_zero_visible="true" pen_width="1" index="2" show_y_axis="true">
+              <entity name="OutFlow_2"/>
+            </plot>
+            <plot color="#008F44" pen_style="dashed" isee:keep_zero_visible="true" pen_width="1" index="3" show_y_axis="true">
+              <entity name="Stock_1"/>
+            </plot>
           </graph>
-          <table color="black" background="#E0E0E0" text_align="right" font_size="12pt" orientation="vertical" wrap_text="false" isee:auto_fit="true" isee:use_alternate_row_colors="false" isee:unlimited_table_length="false" blank_column_width="80" column_width="160" interval="1" report_balances="beginning" report_flows="instantaneous" header_font_style="normal" header_font_weight="normal" header_text_decoration="none" header_text_align="center" header_vertical_text_align="center" header_font_color="black" header_font_family="Arial" header_font_size="12pt" header_text_padding="2" header_text_border_color="black" header_text_border_width="thin" header_text_border_style="none"/>
-        </style>
-        <aux font_style="italic" font_weight="bold" x="538" y="339" name="a"/>
-        <aux x="538" y="416" name="b"/>
+        </stacked_container>
+        <aux x="317" y="59" name="Converter 3"/>
+        <connector uid="4" angle="135.644">
+          <from>Stock_1</from>
+          <to>Converter_3</to>
+        </connector>
+        <stacked_container uid="5" x="851" y="233">
+          <graph width="350" height="250" type="time_series" isee:points_only="false" show_grid="false" include_units_in_legend="false" plot_numbers="false" isee:label_pie_slices="false" num_x_grid_lines="0" num_y_grid_lines="0" num_x_labels="5" num_y_labels="3" isee:fill_intensity="0.1" isee:allow_zero_axis="true" left_axis_multi_scale="false" left_axis_auto_scale="true" left_include_units="true" right_axis_multi_scale="false" right_axis_auto_scale="true" right_include_units="true">
+            <plot color="blue" isee:keep_zero_visible="true" pen_width="1" index="0" show_y_axis="true">
+              <entity name="Stock_1"/>
+            </plot>
+            <plot color="red" pen_style="dot_dashed" isee:keep_zero_visible="true" pen_width="1" index="1" show_y_axis="true">
+              <entity name="Converter_3"/>
+            </plot>
+          </graph>
+        </stacked_container>
+        <stock x="1019" y="516" name="Stock 2"/>
+        <flow x="923.25" y="519" name="InFlow2">
+          <pts>
+            <pt x="850" y="519"/>
+            <pt x="996.5" y="519"/>
+          </pts>
+        </flow>
+        <text_box uid="6" x="844" y="440.5" width="189" height="32">When the input is negative</text_box>
+        <text_box uid="7" x="209" y="892" width="237" height="30">Comparison: order of adding flows</text_box>
+        <stock x="290" y="995" name="Stock 3"/>
+        <stock x="653.5" y="995" name="Stock 4"/>
+        <flow x="361.25" y="995" name="Flow 1">
+          <pts>
+            <pt x="312.5" y="995"/>
+            <pt x="434" y="995"/>
+          </pts>
+        </flow>
+        <flow x="289" y="1051.75" name="Flow 2">
+          <pts>
+            <pt x="289" y="1012.5"/>
+            <pt x="289" y="1112"/>
+          </pts>
+        </flow>
+        <flow x="653.5" y="1057.25" name="Flow 3">
+          <pts>
+            <pt x="653.5" y="1012.5"/>
+            <pt x="653.5" y="1123"/>
+          </pts>
+        </flow>
+        <flow x="732" y="993" name="Flow 4">
+          <pts>
+            <pt x="676" y="993"/>
+            <pt x="812" y="993"/>
+          </pts>
+        </flow>
+        <text_box uid="8" x="359" y="950" width="114" height="18">added first - got 15</text_box>
+        <text_box uid="9" x="319" y="1042.75" width="136" height="18">added second - got 5</text_box>
+        <text_box uid="10" x="672" y="1054" width="114" height="18">added first - got 15</text_box>
+        <text_box uid="11" x="655" y="941.75" width="136" height="18">added second - got 5</text_box>
+        <stock x="932.25" y="968" width="142" height="37" name="Stock 5"/>
+        <flow x="968" y="915.5" name="Flow 5">
+          <pts>
+            <pt x="968" y="863"/>
+            <pt x="968" y="968"/>
+          </pts>
+        </flow>
+        <flow x="954" y="1053.5" name="Flow 6">
+          <pts>
+            <pt x="954" y="1005"/>
+            <pt x="954" y="1123"/>
+          </pts>
+        </flow>
+        <flow x="995" y="1054" name="Flow 7">
+          <pts>
+            <pt x="995" y="1005"/>
+            <pt x="995" y="1124"/>
+          </pts>
+        </flow>
+        <flow x="1043" y="1054" name="Flow 8">
+          <pts>
+            <pt x="1043" y="1005"/>
+            <pt x="1043" y="1124"/>
+          </pts>
+        </flow>
       </view>
     </views>
   </model>
 </xmile>
```

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Non-negative_stocks.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Non-negative_stocks.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Non-negative_stocks_with_flows.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Smooth.stmx`

 * *Files 14% similar despite different names*

#### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Non-negative_stocks_with_flows.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Smooth.stmx`

```diff
@@ -1,20 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <xmile xmlns="http://docs.oasis-open.org/xmile/ns/XMILE/v1.0" xmlns:isee="http://iseesystems.com/XMILE" version="1.0">
   <header>
     <smile version="1.0" namespace="std, isee"/>
-    <name>Non-negative_stocks_with_flows</name>
-    <uuid>537894ae-ccc9-463b-b0ee-a643f5e1cbb8</uuid>
+    <name>Smooth</name>
+    <uuid>39f62f55-44ee-4a01-bfd0-b83cd9607464</uuid>
     <vendor>isee systems, inc.</vendor>
     <product version="2.0" isee:build_number="2176" isee:saved_by_v1="true" lang="en">Stella Professional</product>
   </header>
-  <sim_specs isee:sim_duration="1.5" isee:simulation_delay="0.214286" isee:restore_on_start="false" method="Euler" time_units="Months" isee:instantaneous_flows="false" isee:loop_scores="false" isee:loop_exhaustive_allowed="1000">
-    <start>1</start>
-    <stop>8</stop>
-    <dt reciprocal="true">1</dt>
+  <sim_specs isee:sim_duration="0.5" isee:simulation_delay="0.0714286" isee:restore_on_start="false" method="Euler" time_units="Months" isee:instantaneous_flows="false" isee:loop_scores="true" isee:loop_exhaustive_allowed="1000">
+    <start>0</start>
+    <stop>7</stop>
+    <dt reciprocal="true">4</dt>
   </sim_specs>
   <isee:prefs show_module_prefix="true" live_update_on_drag="true" show_restore_buttons="false" layer="model" interface_scale_ui="true" interface_max_page_width="10000" interface_max_page_height="10000" interface_min_page_width="0" interface_min_page_height="0" rerun_on_structure_change="false" saved_runs="1" keep="false" rifp="true"/>
   <isee:multiplayer_settings include_chat="true" allow_observers="false" advance_time_increment="1" observer_start_page="home_page" enabled="false"/>
   <isee:time_formats default_format="Builtin">
     <isee:time_format name="Builtin" type="adaptive"/>
   </isee:time_formats>
   <default_format/>
@@ -22,103 +22,80 @@
     <export resource="/Users/jonker/Library/CloudStorage/OneDrive-UniversityofStrathclyde/ASDM/stella.csv" interval="DT" precomputed="false" isee:format="numbers">
       <all/>
     </export>
   </data>
   <model_units/>
   <model>
     <variables>
+      <aux name="Source">
+        <eqn>1+STEP(2, 2)</eqn>
+      </aux>
+      <aux name="a">
+        <eqn>SMTH1(Source,  smth_time,   init_val)</eqn>
+      </aux>
+      <aux name="b">
+        <eqn>SMTH3(Source,  smth_time,   init_val)</eqn>
+      </aux>
+      <aux name="smth time">
+        <eqn>5</eqn>
+      </aux>
+      <flow name="Flow 1">
+        <eqn>Source</eqn>
+        <non_negative/>
+      </flow>
       <stock name="Stock 1">
-        <eqn>OutFlow_1+OutFlow_2-20</eqn>
-        <inflow>InFlow</inflow>
-        <outflow>OutFlow_1</outflow>
-        <outflow>OutFlow_2</outflow>
+        <eqn>init_val*smth_time</eqn>
+        <inflow>Flow_1</inflow>
+        <outflow>Flow_a</outflow>
         <non_negative/>
       </stock>
-      <flow name="OutFlow 1">
-        <eqn>50</eqn>
-        <non_negative/>
-      </flow>
-      <flow name="InFlow">
-        <eqn>30</eqn>
+      <flow name="Flow a">
+        <eqn>Stock_1/smth_time</eqn>
         <non_negative/>
       </flow>
-      <flow name="OutFlow 2">
-        <eqn>10</eqn>
+      <aux name="init val">
+        <eqn>1</eqn>
+      </aux>
+      <flow name="Flow 2">
+        <eqn>Source</eqn>
         <non_negative/>
       </flow>
-      <aux name="Converter 1">
-        <eqn>OutFlow_1</eqn>
-      </aux>
-      <aux name="Converter 2">
-        <eqn>OutFlow_2</eqn>
-      </aux>
-      <aux name="Converter 3">
-        <eqn>Stock_1</eqn>
-      </aux>
       <stock name="Stock 2">
-        <eqn>0</eqn>
-        <inflow>InFlow2</inflow>
+        <eqn>smth_time/3*init_val</eqn>
+        <inflow>Flow_2</inflow>
+        <outflow>Flow_3</outflow>
         <non_negative/>
       </stock>
-      <flow name="InFlow2">
-        <eqn>-3</eqn>
-        <non_negative/>
-      </flow>
       <stock name="Stock 3">
-        <eqn>20</eqn>
-        <outflow>Flow_1</outflow>
-        <outflow>Flow_2</outflow>
+        <eqn>smth_time/3*init_val</eqn>
+        <inflow>Flow_3</inflow>
+        <outflow>Flow_4</outflow>
         <non_negative/>
       </stock>
       <stock name="Stock 4">
-        <eqn>20</eqn>
-        <outflow>Flow_3</outflow>
-        <outflow>Flow_4</outflow>
+        <eqn>smth_time/3*init_val</eqn>
+        <inflow>Flow_4</inflow>
+        <outflow>Flow_b</outflow>
         <non_negative/>
       </stock>
-      <flow name="Flow 1">
-        <eqn>15</eqn>
-        <non_negative/>
-      </flow>
-      <flow name="Flow 2">
-        <eqn>15</eqn>
-        <non_negative/>
-      </flow>
       <flow name="Flow 3">
-        <eqn>15</eqn>
+        <eqn>Stock_2/(smth_time/3)</eqn>
         <non_negative/>
       </flow>
       <flow name="Flow 4">
-        <eqn>15</eqn>
-        <non_negative/>
-      </flow>
-      <stock name="Stock 5">
-        <eqn>20</eqn>
-        <inflow>Flow_5</inflow>
-        <outflow>Flow_6</outflow>
-        <outflow>Flow_7</outflow>
-        <outflow>Flow_8</outflow>
-        <non_negative/>
-      </stock>
-      <flow name="Flow 5">
-        <eqn>20</eqn>
-        <non_negative/>
-      </flow>
-      <flow name="Flow 6">
-        <eqn>10</eqn>
+        <eqn>Stock_3/(smth_time/3)</eqn>
         <non_negative/>
       </flow>
-      <flow name="Flow 7">
-        <eqn>20</eqn>
-        <non_negative/>
-      </flow>
-      <flow name="Flow 8">
-        <eqn>30</eqn>
+      <flow name="Flow b">
+        <eqn>Stock_4/(smth_time/3)</eqn>
         <non_negative/>
       </flow>
+      <aux name="c">
+        <eqn>SMTH1(Source,  smth_time)</eqn>
+      </aux>
     </variables>
     <views>
       <style color="black" background="white" font_style="normal" font_weight="normal" text_decoration="none" text_align="center" vertical_text_align="center" font_color="black" font_family="Arial" font_size="10pt" padding="2" border_color="black" border_width="thin" border_style="none">
         <text_box color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt"/>
         <isee:loop_indicator color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt"/>
         <numeric_display color="blue" background="white" font_size="9pt" isee:transparent="false"/>
         <graph color="black" background="white" font_size="12pt" axis_color="#666666" grid_color="#C8C8C8" isee:graph_area_color="white" legend_position="bottom" isee:transparent="false" isee:hide_border="false" axis_title_font_style="normal" axis_title_font_weight="normal" axis_title_text_decoration="none" axis_title_text_align="center" axis_title_vertical_text_align="center" axis_title_font_color="black" axis_title_font_family="Arial" axis_title_font_size="12pt" axis_title_text_padding="2" axis_title_text_border_color="black" axis_title_text_border_width="thin" axis_title_text_border_style="none" axis_label_font_style="normal" axis_label_font_weight="normal" axis_label_text_decoration="none" axis_label_text_align="center" axis_label_vertical_text_align="center" axis_label_font_color="black" axis_label_font_family="Arial" axis_label_font_size="9pt" axis_label_text_padding="2" axis_label_text_border_color="black" axis_label_text_border_width="thin" axis_label_text_border_style="none">
@@ -157,15 +134,15 @@
         <isee:animation_object color="black" background="white" font_size="12pt"/>
         <isee:navigation_widget color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt" border_color="#999999" border_width="thin" border_style="solid" item_spacing="6" appearance="tabs" corner_radius="4" selected_item_color="black" selected_item_background="white" item_background="#DDDDDD"/>
         <isee:shape color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt" border_width="thin" border_style="solid" opacity="1" transparent_background="true"/>
         <isee:selector color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt"/>
         <isee:iframe color="black" background="white" text_align="left" vertical_text_align="top" font_size="12pt" border_width="thin" border_style="solid"/>
         <isee:financial_table color="black" background="#E0E0E0" text_align="right" font_size="12pt" auto_fit="true" first_column_width="250" other_column_width="100" header_font_style="normal" header_font_weight="bold" header_text_decoration="none" header_text_align="center" header_vertical_text_align="center" header_font_color="black" header_font_family="Arial" header_font_size="14pt" header_text_padding="2" header_text_border_color="black" header_text_border_width="thin" header_text_border_style="none"/>
       </style>
-      <view isee:show_pages="false" background="white" page_width="818" page_height="571" isee:page_cols="2" isee:page_rows="3" isee:scroll_x="281" isee:scroll_y="408" isee:popup_graphs_are_comparative="true" isee:enable_non_negative_highlights="false" type="stock_flow">
+      <view isee:show_pages="false" background="white" page_width="818" page_height="571" isee:page_cols="2" isee:page_rows="2" zoom="80" isee:popup_graphs_are_comparative="true" isee:enable_non_negative_highlights="false" type="stock_flow">
         <style color="black" background="white" font_style="normal" font_weight="normal" text_decoration="none" text_align="center" vertical_text_align="center" font_color="black" font_family="Arial" font_size="10pt" padding="2" border_color="black" border_width="thin" border_style="none">
           <stock color="blue" background="white" font_color="blue" font_size="9pt" label_side="top">
             <shape type="rectangle" width="45" height="35"/>
           </stock>
           <flow color="blue" background="white" font_color="blue" font_size="9pt" label_side="bottom"/>
           <isee:placeholder color="#228B22" background="white" font_color="#228B22" font_size="9pt" label_side="bottom"/>
           <module color="blue" background="white" font_color="blue" font_size="9pt" label_side="top">
@@ -194,135 +171,163 @@
               <isee:series_style color="#F586FF" thickness="1" pen_style="dotted"/>
               <isee:series_style color="black" thickness="1" pen_style="dashed"/>
               <isee:series_style color="#C8C8C8" thickness="1"/>
             </isee:series_styles>
           </graph>
           <table color="black" background="#E0E0E0" text_align="right" font_size="12pt" orientation="vertical" wrap_text="false" isee:auto_fit="true" isee:use_alternate_row_colors="false" isee:unlimited_table_length="false" blank_column_width="80" column_width="160" interval="1" report_balances="beginning" report_flows="instantaneous" header_font_style="normal" header_font_weight="normal" header_text_decoration="none" header_text_align="center" header_vertical_text_align="center" header_font_color="black" header_font_family="Arial" header_font_size="12pt" header_text_padding="2" header_text_border_color="black" header_text_border_width="thin" header_text_border_style="none"/>
         </style>
-        <stock x="363" y="174" name="Stock 1"/>
-        <flow x="468.75" y="174" name="OutFlow 1">
-          <pts>
-            <pt x="385.5" y="174"/>
-            <pt x="576" y="174"/>
-          </pts>
-        </flow>
-        <flow x="255.25" y="174" name="InFlow">
+        <stacked_container uid="1" x="705.5" y="203.5" width="504" height="173">
+          <graph width="504" height="173" type="time_series" isee:points_only="false" show_grid="false" include_units_in_legend="false" plot_numbers="false" isee:label_pie_slices="false" num_x_grid_lines="0" num_y_grid_lines="0" num_x_labels="5" num_y_labels="8" isee:fill_intensity="0.1" isee:allow_zero_axis="true" left_axis_multi_scale="false" left_axis_auto_scale="true" left_include_units="true" right_axis_multi_scale="false" right_axis_auto_scale="true" right_include_units="true">
+            <plot color="blue" isee:keep_zero_visible="true" pen_width="1" index="0" show_y_axis="true">
+              <entity name="Source"/>
+            </plot>
+          </graph>
+        </stacked_container>
+        <aux x="129" y="384.25" name="Source"/>
+        <aux x="303" y="298.25" name="a"/>
+        <aux x="303" y="384.25" name="b"/>
+        <connector uid="2" angle="38.4181">
+          <from>Source</from>
+          <to>a</to>
+        </connector>
+        <connector uid="3" angle="16.1892">
+          <from>Source</from>
+          <to>b</to>
+        </connector>
+        <aux x="212" y="450.25" name="smth time"/>
+        <connector uid="4" angle="77.6609">
+          <from>smth_time</from>
+          <to>a</to>
+        </connector>
+        <connector uid="5" angle="35.9524">
+          <from>smth_time</from>
+          <to>b</to>
+        </connector>
+        <flow x="130.75" y="552.25" name="Flow 1">
           <pts>
-            <pt x="170" y="174"/>
-            <pt x="340.5" y="174"/>
+            <pt x="65" y="552.25"/>
+            <pt x="196.5" y="552.25"/>
           </pts>
         </flow>
-        <flow x="364" y="261.75" name="OutFlow 2">
+        <stock x="219" y="556.25" name="Stock 1"/>
+        <flow x="287.25" y="556.25" name="Flow a">
           <pts>
-            <pt x="364" y="191.5"/>
-            <pt x="364" y="353"/>
+            <pt x="241.5" y="556.25"/>
+            <pt x="357" y="556.25"/>
           </pts>
         </flow>
-        <aux x="549" y="99" name="Converter 1"/>
-        <connector uid="1" angle="72.646">
-          <from>OutFlow_1</from>
-          <to>Converter_1</to>
-        </connector>
-        <aux x="464" y="332" name="Converter 2"/>
-        <connector uid="2" angle="4.49258">
-          <from>OutFlow_2</from>
-          <to>Converter_2</to>
+        <connector uid="6" angle="10.7843">
+          <from>smth_time</from>
+          <to>Flow_a</to>
+        </connector>
+        <connector uid="7" angle="270.597">
+          <from>Source</from>
+          <to>Flow_1</to>
         </connector>
-        <stacked_container uid="3" x="200.75" y="425" width="557" height="418">
-          <graph width="557" height="418" type="time_series" isee:points_only="false" show_grid="false" include_units_in_legend="false" plot_numbers="false" isee:label_pie_slices="false" num_x_grid_lines="0" num_y_grid_lines="0" num_x_labels="8" num_y_labels="11" isee:fill_intensity="0.1" isee:allow_zero_axis="true" left_axis_multi_scale="false" left_axis_auto_scale="true" left_include_units="true" right_axis_multi_scale="false" right_axis_auto_scale="true" right_include_units="true">
+        <connector uid="8" angle="45">
+          <from>Stock_1</from>
+          <to>Flow_a</to>
+        </connector>
+        <stacked_container uid="9" x="705.5" y="376.5" width="504" height="173">
+          <graph width="504" height="173" type="time_series" isee:points_only="false" show_grid="false" include_units_in_legend="false" plot_numbers="false" isee:label_pie_slices="false" num_x_grid_lines="0" num_y_grid_lines="0" num_x_labels="5" num_y_labels="8" isee:fill_intensity="0.1" isee:allow_zero_axis="true" left_axis_multi_scale="false" left_axis_auto_scale="true" left_include_units="true" right_axis_multi_scale="false" right_axis_auto_scale="true" right_include_units="true">
             <plot color="blue" isee:keep_zero_visible="true" pen_width="1" index="0" show_y_axis="true">
-              <entity name="InFlow"/>
+              <entity name="a"/>
             </plot>
             <plot color="red" pen_style="dot_dashed" isee:keep_zero_visible="true" pen_width="1" index="1" show_y_axis="true">
-              <entity name="OutFlow_1"/>
-            </plot>
-            <plot color="fuchsia" pen_style="dotted" isee:keep_zero_visible="true" pen_width="1" index="2" show_y_axis="true">
-              <entity name="OutFlow_2"/>
-            </plot>
-            <plot color="#008F44" pen_style="dashed" isee:keep_zero_visible="true" pen_width="1" index="3" show_y_axis="true">
-              <entity name="Stock_1"/>
+              <entity name="Flow_a"/>
             </plot>
           </graph>
         </stacked_container>
-        <aux x="317" y="59" name="Converter 3"/>
-        <connector uid="4" angle="135.644">
-          <from>Stock_1</from>
-          <to>Converter_3</to>
-        </connector>
-        <stacked_container uid="5" x="851" y="233">
-          <graph width="350" height="250" type="time_series" isee:points_only="false" show_grid="false" include_units_in_legend="false" plot_numbers="false" isee:label_pie_slices="false" num_x_grid_lines="0" num_y_grid_lines="0" num_x_labels="5" num_y_labels="3" isee:fill_intensity="0.1" isee:allow_zero_axis="true" left_axis_multi_scale="false" left_axis_auto_scale="true" left_include_units="true" right_axis_multi_scale="false" right_axis_auto_scale="true" right_include_units="true">
+        <stacked_container uid="10" x="705.5" y="549.5" width="504" height="173">
+          <graph width="504" height="173" type="time_series" isee:points_only="false" show_grid="false" include_units_in_legend="false" plot_numbers="false" isee:label_pie_slices="false" num_x_grid_lines="0" num_y_grid_lines="0" num_x_labels="5" num_y_labels="8" isee:fill_intensity="0.1" isee:allow_zero_axis="true" left_axis_multi_scale="false" left_axis_auto_scale="true" left_include_units="true" right_axis_multi_scale="false" right_axis_auto_scale="true" right_include_units="true">
             <plot color="blue" isee:keep_zero_visible="true" pen_width="1" index="0" show_y_axis="true">
-              <entity name="Stock_1"/>
+              <entity name="b"/>
             </plot>
             <plot color="red" pen_style="dot_dashed" isee:keep_zero_visible="true" pen_width="1" index="1" show_y_axis="true">
-              <entity name="Converter_3"/>
+              <entity name="Flow_b"/>
             </plot>
           </graph>
         </stacked_container>
-        <stock x="1019" y="516" name="Stock 2"/>
-        <flow x="923.25" y="519" name="InFlow2">
-          <pts>
-            <pt x="850" y="519"/>
-            <pt x="996.5" y="519"/>
-          </pts>
-        </flow>
-        <text_box uid="6" x="844" y="440.5" width="189" height="32">When the input is negative</text_box>
-        <text_box uid="7" x="209" y="892" width="237" height="30">Comparison: order of adding flows</text_box>
-        <stock x="290" y="995" name="Stock 3"/>
-        <stock x="653.5" y="995" name="Stock 4"/>
-        <flow x="361.25" y="995" name="Flow 1">
-          <pts>
-            <pt x="312.5" y="995"/>
-            <pt x="434" y="995"/>
-          </pts>
-        </flow>
-        <flow x="289" y="1051.75" name="Flow 2">
-          <pts>
-            <pt x="289" y="1012.5"/>
-            <pt x="289" y="1112"/>
-          </pts>
-        </flow>
-        <flow x="653.5" y="1057.25" name="Flow 3">
-          <pts>
-            <pt x="653.5" y="1012.5"/>
-            <pt x="653.5" y="1123"/>
-          </pts>
-        </flow>
-        <flow x="732" y="993" name="Flow 4">
-          <pts>
-            <pt x="676" y="993"/>
-            <pt x="812" y="993"/>
-          </pts>
-        </flow>
-        <text_box uid="8" x="359" y="950" width="114" height="18">added first - got 15</text_box>
-        <text_box uid="9" x="319" y="1042.75" width="136" height="18">added second - got 5</text_box>
-        <text_box uid="10" x="672" y="1054" width="114" height="18">added first - got 15</text_box>
-        <text_box uid="11" x="655" y="941.75" width="136" height="18">added second - got 5</text_box>
-        <stock x="932.25" y="968" width="142" height="37" name="Stock 5"/>
-        <flow x="968" y="915.5" name="Flow 5">
+        <aux x="435" y="414.25" name="init val"/>
+        <connector uid="11" angle="138.691">
+          <from>init_val</from>
+          <to>a</to>
+        </connector>
+        <connector uid="12" angle="177.879">
+          <from>init_val</from>
+          <to>b</to>
+        </connector>
+        <flow x="210.75" y="701.25" name="Flow 2">
           <pts>
-            <pt x="968" y="863"/>
-            <pt x="968" y="968"/>
+            <pt x="155" y="701.25"/>
+            <pt x="266.5" y="701.25"/>
           </pts>
         </flow>
-        <flow x="954" y="1053.5" name="Flow 6">
+        <stock x="289" y="701.25" name="Stock 2"/>
+        <stock x="396.75" y="701.25" name="Stock 3"/>
+        <stock x="511" y="701.25" name="Stock 4"/>
+        <flow x="336.875" y="701.25" name="Flow 3">
           <pts>
-            <pt x="954" y="1005"/>
-            <pt x="954" y="1123"/>
+            <pt x="311.5" y="701.25"/>
+            <pt x="374.25" y="701.25"/>
           </pts>
         </flow>
-        <flow x="995" y="1054" name="Flow 7">
+        <flow x="447.875" y="701.25" name="Flow 4">
           <pts>
-            <pt x="995" y="1005"/>
-            <pt x="995" y="1124"/>
+            <pt x="419.25" y="701.25"/>
+            <pt x="488.5" y="701.25"/>
           </pts>
         </flow>
-        <flow x="1043" y="1054" name="Flow 8">
+        <flow x="569.25" y="702.25" name="Flow b">
           <pts>
-            <pt x="1043" y="1005"/>
-            <pt x="1043" y="1124"/>
+            <pt x="533.5" y="702.25"/>
+            <pt x="629" y="702.25"/>
           </pts>
         </flow>
+        <connector uid="13" angle="284.461">
+          <from>Source</from>
+          <to>Flow_2</to>
+        </connector>
+        <connector uid="14" angle="53.1301">
+          <from>Stock_2</from>
+          <to>Flow_3</to>
+        </connector>
+        <connector uid="15" angle="49.0078">
+          <from>Stock_3</from>
+          <to>Flow_4</to>
+        </connector>
+        <connector uid="16" angle="48.9909">
+          <from>Stock_4</from>
+          <to>Flow_b</to>
+        </connector>
+        <connector uid="17" angle="312.357">
+          <from>smth_time</from>
+          <to>Flow_3</to>
+        </connector>
+        <connector uid="18" angle="328.57">
+          <from>smth_time</from>
+          <to>Flow_4</to>
+        </connector>
+        <connector uid="19" angle="350.134">
+          <from>smth_time</from>
+          <to>Flow_b</to>
+        </connector>
+        <aux x="310" y="218.75" name="c"/>
+        <connector uid="20" angle="86.2414">
+          <from>Source</from>
+          <to>c</to>
+        </connector>
+        <connector uid="21" angle="82.606">
+          <from>smth_time</from>
+          <to>c</to>
+        </connector>
+        <stacked_container uid="22" x="456.875" y="17.25" width="504" height="173">
+          <graph width="504" height="173" type="time_series" isee:points_only="false" show_grid="false" include_units_in_legend="false" plot_numbers="false" isee:label_pie_slices="false" num_x_grid_lines="0" num_y_grid_lines="0" num_x_labels="5" num_y_labels="8" isee:fill_intensity="0.1" isee:allow_zero_axis="true" left_axis_multi_scale="false" left_axis_auto_scale="true" left_include_units="true" right_axis_multi_scale="false" right_axis_auto_scale="true" right_include_units="true">
+            <plot color="blue" isee:keep_zero_visible="true" pen_width="1" index="0" show_y_axis="true">
+              <entity name="c"/>
+            </plot>
+          </graph>
+        </stacked_container>
       </view>
     </views>
   </model>
 </xmile>
```

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Array_cross_reference.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Array_cross_reference.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Conveyor_leakage.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Conveyor_leakage.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Conveyor_leakage1.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Conveyor_leakage1.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Conveyor_leakage2.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Conveyor_leakage2.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Delays.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Delays.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Goal_gap.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Goal_gap.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Goal_gap_array.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Goal_gap_array.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Graph_function.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Graph_function.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/INIT.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/INIT.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/LOOKUP.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/LOOKUP.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/MOD.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/MOD.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Min_Max.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Min_Max.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Non-negative_stocks_with_flows.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Non-negative_stocks_with_flows.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Stella_outcomes/Smooth.csv` & `asdm-0.0.3/tests/BuiltInTestModels/Stella_outcomes/Smooth.csv`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Time_related_functions.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Time_related_functions.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/BuiltInTestModels/Time_unit.stmx` & `asdm-0.0.3/tests/BuiltInTestModels/Time_unit.stmx`

 * *Files identical despite different names*

### Comparing `asdm-0.0.2/tests/run_tests.py` & `asdm-0.0.3/tests/run_tests.py`

 * *Files identical despite different names*

