# Comparing `tmp/digital-experiments-1.0.7.tar.gz` & `tmp/digital-experiments-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-experiments-1.0.7.tar", last modified: Thu Apr 20 10:11:53 2023, max compression
+gzip compressed data, was "digital-experiments-1.0.8.tar", last modified: Tue May  9 14:18:15 2023, max compression
```

## Comparing `digital-experiments-1.0.7.tar` & `digital-experiments-1.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:11:53.679876 digital-experiments-1.0.7/
--rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.0.7/LICENSE
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-04-20 10:11:53.679692 digital-experiments-1.0.7/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/README.md
--rw-r--r--   0 john       (504) staff       (20)     1321 2023-04-20 10:11:46.000000 digital-experiments-1.0.7/pyproject.toml
--rw-r--r--   0 john       (504) staff       (20)       38 2023-04-20 10:11:53.679928 digital-experiments-1.0.7/setup.cfg
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:11:53.673190 digital-experiments-1.0.7/src/
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:11:53.676441 digital-experiments-1.0.7/src/digital_experiments/
--rw-r--r--   0 john       (504) staff       (20)      139 2023-04-20 10:11:46.000000 digital-experiments-1.0.7/src/digital_experiments/__init__.py
--rw-r--r--   0 john       (504) staff       (20)     6219 2023-04-04 08:39:31.000000 digital-experiments-1.0.7/src/digital_experiments/backends.py
--rw-r--r--   0 john       (504) staff       (20)     1016 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/control_center.py
--rw-r--r--   0 john       (504) staff       (20)     3303 2023-04-20 10:11:29.000000 digital-experiments-1.0.7/src/digital_experiments/experiment.py
--rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/inspection.py
--rw-r--r--   0 john       (504) staff       (20)      592 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/metadata.py
--rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.0.7/src/digital_experiments/minimize.py
--rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/observation.py
--rw-r--r--   0 john       (504) staff       (20)      735 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/pretty.py
--rw-r--r--   0 john       (504) staff       (20)     2454 2023-04-20 10:03:31.000000 digital-experiments-1.0.7/src/digital_experiments/querying.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:11:53.677873 digital-experiments-1.0.7/src/digital_experiments/search/
--rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/search/skopt_suggest.py
--rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/search/space.py
--rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.0.7/src/digital_experiments/search/suggest.py
--rw-r--r--   0 john       (504) staff       (20)     3545 2023-04-04 08:55:31.000000 digital-experiments-1.0.7/src/digital_experiments/util.py
--rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/src/digital_experiments/version_control.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:11:53.677428 digital-experiments-1.0.7/src/digital_experiments.egg-info/
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-04-20 10:11:53.000000 digital-experiments-1.0.7/src/digital_experiments.egg-info/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1049 2023-04-20 10:11:53.000000 digital-experiments-1.0.7/src/digital_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 john       (504) staff       (20)        1 2023-04-20 10:11:53.000000 digital-experiments-1.0.7/src/digital_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 john       (504) staff       (20)      160 2023-04-20 10:11:53.000000 digital-experiments-1.0.7/src/digital_experiments.egg-info/requires.txt
--rw-r--r--   0 john       (504) staff       (20)       32 2023-04-20 10:11:53.000000 digital-experiments-1.0.7/src/digital_experiments.egg-info/top_level.txt
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-20 10:11:53.679380 digital-experiments-1.0.7/tests/
--rw-r--r--   0 john       (504) staff       (20)     1861 2023-03-29 16:29:55.000000 digital-experiments-1.0.7/tests/test_backends.py
--rw-r--r--   0 john       (504) staff       (20)      377 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/tests/test_control_center.py
--rw-r--r--   0 john       (504) staff       (20)      863 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/tests/test_experiment.py
--rw-r--r--   0 john       (504) staff       (20)      793 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/tests/test_metadata.py
--rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/tests/test_minimize.py
--rw-r--r--   0 john       (504) staff       (20)     1156 2023-04-20 10:06:14.000000 digital-experiments-1.0.7/tests/test_querying.py
--rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/tests/test_space.py
--rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.0.7/tests/test_suggest.py
--rw-r--r--   0 john       (504) staff       (20)      795 2023-03-29 15:42:00.000000 digital-experiments-1.0.7/tests/test_util.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-09 14:18:15.408534 digital-experiments-1.0.8/
+-rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.0.8/LICENSE
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-09 14:18:15.408363 digital-experiments-1.0.8/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/README.md
+-rw-r--r--   0 john       (504) staff       (20)     1321 2023-05-09 14:18:09.000000 digital-experiments-1.0.8/pyproject.toml
+-rw-r--r--   0 john       (504) staff       (20)       38 2023-05-09 14:18:15.408584 digital-experiments-1.0.8/setup.cfg
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-09 14:18:15.402525 digital-experiments-1.0.8/src/
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-09 14:18:15.405534 digital-experiments-1.0.8/src/digital_experiments/
+-rw-r--r--   0 john       (504) staff       (20)      139 2023-05-09 14:18:09.000000 digital-experiments-1.0.8/src/digital_experiments/__init__.py
+-rw-r--r--   0 john       (504) staff       (20)     6329 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/src/digital_experiments/backends.py
+-rw-r--r--   0 john       (504) staff       (20)     1016 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     3651 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/src/digital_experiments/experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/inspection.py
+-rw-r--r--   0 john       (504) staff       (20)      592 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/metadata.py
+-rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.0.8/src/digital_experiments/minimize.py
+-rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/observation.py
+-rw-r--r--   0 john       (504) staff       (20)      735 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/pretty.py
+-rw-r--r--   0 john       (504) staff       (20)     2581 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/src/digital_experiments/querying.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-09 14:18:15.406882 digital-experiments-1.0.8/src/digital_experiments/search/
+-rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/search/skopt_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/search/space.py
+-rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.0.8/src/digital_experiments/search/suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     3971 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/src/digital_experiments/util.py
+-rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/version_control.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-09 14:18:15.406339 digital-experiments-1.0.8/src/digital_experiments.egg-info/
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-09 14:18:15.000000 digital-experiments-1.0.8/src/digital_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1049 2023-05-09 14:18:15.000000 digital-experiments-1.0.8/src/digital_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (504) staff       (20)        1 2023-05-09 14:18:15.000000 digital-experiments-1.0.8/src/digital_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (504) staff       (20)      160 2023-05-09 14:18:15.000000 digital-experiments-1.0.8/src/digital_experiments.egg-info/requires.txt
+-rw-r--r--   0 john       (504) staff       (20)       32 2023-05-09 14:18:15.000000 digital-experiments-1.0.8/src/digital_experiments.egg-info/top_level.txt
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-09 14:18:15.408121 digital-experiments-1.0.8/tests/
+-rw-r--r--   0 john       (504) staff       (20)     1861 2023-03-29 16:29:55.000000 digital-experiments-1.0.8/tests/test_backends.py
+-rw-r--r--   0 john       (504) staff       (20)      377 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/tests/test_control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     1179 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/tests/test_experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      793 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/tests/test_metadata.py
+-rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/tests/test_minimize.py
+-rw-r--r--   0 john       (504) staff       (20)     1580 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/tests/test_querying.py
+-rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/tests/test_space.py
+-rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.0.8/tests/test_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     1407 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/tests/test_util.py
```

### Comparing `digital-experiments-1.0.7/LICENSE` & `digital-experiments-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/PKG-INFO` & `digital-experiments-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.0.7
+Version: 1.0.8
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.0.7/README.md` & `digital-experiments-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/pyproject.toml` & `digital-experiments-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digital-experiments"
-version = "1.0.7"
+version = "1.0.8"
 description = "Keep track of digital experiments."
 readme = "README.md"
 authors = [{ name = "John Gardner", email = "gardner.john97@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -41,15 +41,15 @@
     "pytest-cov",
 ]
 
 [project.urls]
 Homepage = "https://github.com/jla-gardner/digital-experiments"
 
 [tool.bumpver]
-current_version = "1.0.7"
+current_version = "1.0.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `digital-experiments-1.0.7/src/digital_experiments/backends.py` & `digital-experiments-1.0.8/src/digital_experiments/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Dict, List
 
 import pandas as pd
 import yaml
 
 from .control_center import Run
 from .observation import Observation
-from .util import exclusive_file_access, flatten, generate_id, unflatten
+from .util import dict_equality, exclusive_file_access, flatten, generate_id, unflatten
 
 __BACKENDS: Dict[str, "Backend"] = {}
 
 
 def register_backend(name: str, cls: "Backend"):
     __BACKENDS[name] = cls
     cls.name = name
@@ -102,37 +102,45 @@
         """
         assert not location.exists(), f"{location} already exists"
         location.mkdir(parents=True)
 
         # label this directory as a digital experiment
         # and store various required metadata
         HomeLabel.create_new(location, cls.name, code)
-             
+
         return cls(location)
 
     @contextlib.contextmanager
     def unique_run(self):
         id = generate_id()
         directory = self.home / Files.RUNS / id
         directory.mkdir(parents=True, exist_ok=False)
 
         run = Run(id, directory)
+
         yield run  # experiments happen while this is yielded
+
         if not any(run.directory.iterdir()):
             shutil.rmtree(run.directory)
 
     @staticmethod
     def from_existing(home: Path):
         """
         Load an existing backend from the given location.
         """
 
         label = HomeLabel.from_existing(home)
         return backend_from_type(label.backend_name)(home)
 
+    def _observation_for_(self, config):
+        for obs in self.all_observations():
+            if dict_equality(obs.config, config):
+                return obs
+        return None
+
 
 @this_is_a_backend("yaml")
 class YAMLBackend(Backend):
     @property
     def yaml_file(self):
         return self.home / "observations.yaml"
 
@@ -163,65 +171,61 @@
         return self.home / "observations.csv"
 
     def save(self, obs: Observation):
         existing_observations = self.all_observations()
         existing_observations.append(obs)
 
         df = pd.DataFrame(
-            [
-                flatten(o.as_dict(), self.SEPARATOR)
-                for o in existing_observations
-            ],
+            [flatten(o.as_dict(), self.SEPARATOR) for o in existing_observations],
         )
         with exclusive_file_access(self.csv_file):
             df.to_csv(self.csv_file, index=False)
 
     def all_observations(self) -> List[Observation]:
         if not self.csv_file.exists():
             return []
 
         with exclusive_file_access(self.csv_file):
             df = pd.read_csv(self.csv_file, dtype={"id": str})
-        
+
         return [
-            Observation(**unflatten(row, self.SEPARATOR))
-            for _, row in df.iterrows()
+            Observation(**unflatten(row, self.SEPARATOR)) for _, row in df.iterrows()
         ]
 
 
 class Files:
     LABEL = ".digital-experiment"
     RUNS = "runs"
 
 
 @dataclass
 class HomeLabel:
     """
     A class to label a directory as containing the results of a digital
     experiment.
     """
+
     backend_name: str
     code: str
 
     @classmethod
     def file_path(cls, home: Path):
         return home / Files.LABEL
 
     def save_to(self, home: Path):
         namespace = asdict(self)
 
         with open(self.file_path(home), "w") as f:
-            yaml.dump(namespace, f, default_style='|')
-    
+            yaml.dump(namespace, f, default_style="|")
+
     @classmethod
     def from_existing(cls, home: Path):
         with open(cls.file_path(home)) as f:
             namespace = yaml.safe_load(f)
 
         return cls(**namespace)
-    
+
     @classmethod
     def create_new(cls, home: Path, backend_name: str, code: str):
         label = cls(backend_name, code)
         label.save_to(home)
         return label
-
```

### Comparing `digital-experiments-1.0.7/src/digital_experiments/control_center.py` & `digital-experiments-1.0.8/src/digital_experiments/control_center.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/src/digital_experiments/experiment.py` & `digital-experiments-1.0.8/src/digital_experiments/experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,27 @@
 def experiment(
     experiment_fn=None,
     *,
     backend: str = "yaml",
     root: str = None,
     absolute_root: Union[str, Path] = None,
     verbose: bool = False,
+    cache: bool = True,
 ):
     """
     decorator to record an experiment
     """
     if experiment_fn is None:
         return partial(
-            experiment, backend=backend, root=root, absolute_root=absolute_root
+            experiment,
+            backend=backend,
+            root=root,
+            absolute_root=absolute_root,
+            verbose=verbose,
+            cache=cache,
         )
 
     # get the directory of the file where the experiment is defined
     # and where <root> should be relative to
     expmt_file = Path(experiment_fn.__code__.co_filename).parent
     if "ipykernel" in str(expmt_file):
         expmt_file = Path(".")
@@ -37,35 +43,41 @@
         final_root = expmt_file.resolve() / "experiments" / experiment_fn.__name__
     elif absolute_root:
         assert root is None, "Cannot specify both root and absolute_root"
         final_root = Path(absolute_root).resolve()
     else:
         final_root = expmt_file.resolve() / root
 
-    return Experiment(experiment_fn, backend, final_root, verbose=verbose)
+    return Experiment(experiment_fn, backend, final_root, verbose, cache)
 
 
 class Experiment:
     def __init__(
         self,
         experiment: callable,
         backend: str,
         root: Path,
         verbose: bool = False,
+        cache: bool = True,
     ):
         self._experiment = experiment
         self._backend = get_or_create_backend_for(root, code_for(experiment), backend)
         self.verbose = verbose
+        self.cache = cache
 
     def run(self, args: list, kwargs: dict):
         if not GLOBAL.should_record():
             return self._experiment(*args, **kwargs)
 
         config = complete_config(self._experiment, args, kwargs)
 
+        previous_observation = self._backend._observation_for_(config)
+        if self.cache and previous_observation is not None:
+            return previous_observation.result
+
         with self._backend.unique_run() as run, GLOBAL.recording_run(run):
             id = run.id
             if self.verbose:
                 print(
                     f"digital-experiments: Running experiment {id} with config: {config}"
                 )
             metadata, result = record_metadata(self._experiment, args, kwargs)
```

### Comparing `digital-experiments-1.0.7/src/digital_experiments/metadata.py` & `digital-experiments-1.0.8/src/digital_experiments/metadata.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/src/digital_experiments/minimize.py` & `digital-experiments-1.0.8/src/digital_experiments/minimize.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/src/digital_experiments/observation.py` & `digital-experiments-1.0.8/src/digital_experiments/observation.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/src/digital_experiments/pretty.py` & `digital-experiments-1.0.8/src/digital_experiments/pretty.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/src/digital_experiments/querying.py` & `digital-experiments-1.0.8/src/digital_experiments/querying.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 
     Returns
     -------
     pd.DataFrame
         DataFrame with the observations
     """
 
+    if len(observations) == 0:
+        warnings.warn("No observations to convert to dataframe")
+        return pd.DataFrame()
+
     dicts = [o.as_dict() for o in observations]
     config_keys = union(d["config"].keys() for d in dicts)
     result_keys = union(
         d["result"].keys() if isinstance(d["result"], dict) else [] for d in dicts
     )
 
     overlap = intersect([config_keys, result_keys])
```

### Comparing `digital-experiments-1.0.7/src/digital_experiments/search/skopt_suggest.py` & `digital-experiments-1.0.8/src/digital_experiments/search/skopt_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/src/digital_experiments/search/space.py` & `digital-experiments-1.0.8/src/digital_experiments/search/space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/src/digital_experiments/search/suggest.py` & `digital-experiments-1.0.8/src/digital_experiments/search/suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/src/digital_experiments/util.py` & `digital-experiments-1.0.8/src/digital_experiments/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,7 +145,28 @@
     relevant_kwargs = {}
     signature = inspect.signature(experiment._experiment)
     for k, v in kwargs.items():
         if k in signature.parameters:
             relevant_kwargs[k] = interpret(v, signature.parameters[k])
 
     return relevant_kwargs
+
+
+def dict_equality(d1: Dict, d2: Dict):
+    if set(d1.keys()) != set(d2.keys()):
+        return False
+
+    for k in d1.keys():
+        v1 = d1[k]
+        v2 = d2[k]
+
+        if isinstance(v1, dict):
+            if not isinstance(v2, dict):
+                return False
+            if not dict_equality(v1, v2):
+                return False
+            continue
+
+        if v1 != v2:
+            return False
+
+    return True
```

### Comparing `digital-experiments-1.0.7/src/digital_experiments/version_control.py` & `digital-experiments-1.0.8/src/digital_experiments/version_control.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/src/digital_experiments.egg-info/PKG-INFO` & `digital-experiments-1.0.8/src/digital_experiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.0.7
+Version: 1.0.8
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.0.7/src/digital_experiments.egg-info/SOURCES.txt` & `digital-experiments-1.0.8/src/digital_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/tests/test_backends.py` & `digital-experiments-1.0.8/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/tests/test_metadata.py` & `digital-experiments-1.0.8/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/tests/test_minimize.py` & `digital-experiments-1.0.8/tests/test_minimize.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/tests/test_space.py` & `digital-experiments-1.0.8/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.7/tests/test_suggest.py` & `digital-experiments-1.0.8/tests/test_suggest.py`

 * *Files identical despite different names*

