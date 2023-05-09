# Comparing `tmp/nexora-0.0.1.tar.gz` & `tmp/nexora-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexora-0.0.1.tar", last modified: Fri May  5 14:01:38 2023, max compression
+gzip compressed data, was "nexora-0.0.2.tar", last modified: Tue May  9 14:44:37 2023, max compression
```

## Comparing `nexora-0.0.1.tar` & `nexora-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-05 14:01:38.628374 nexora-0.0.1/
--rw-r--r--   0 alicabukel   (501) staff       (20)    11357 2023-05-04 08:59:14.000000 nexora-0.0.1/LICENSE
--rw-r--r--   0 alicabukel   (501) staff       (20)     1508 2023-05-05 14:01:38.628620 nexora-0.0.1/PKG-INFO
--rw-r--r--   0 alicabukel   (501) staff       (20)     1207 2023-05-05 01:47:02.000000 nexora-0.0.1/README.md
--rw-r--r--   0 alicabukel   (501) staff       (20)      122 2023-05-04 09:39:11.000000 nexora-0.0.1/pyproject.toml
--rw-r--r--   0 alicabukel   (501) staff       (20)      672 2023-05-05 14:01:38.629520 nexora-0.0.1/setup.cfg
--rw-r--r--   0 alicabukel   (501) staff       (20)      403 2023-05-05 00:23:02.000000 nexora-0.0.1/setup.py
-drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-05 14:01:38.600457 nexora-0.0.1/src/
-drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-05 14:01:38.618140 nexora-0.0.1/src/nexora/
--rw-r--r--   0 alicabukel   (501) staff       (20)       54 2023-05-05 00:17:53.000000 nexora-0.0.1/src/nexora/__init__.py
--rw-r--r--   0 alicabukel   (501) staff       (20)      331 2023-05-04 23:40:22.000000 nexora-0.0.1/src/nexora/api.py
--rw-r--r--   0 alicabukel   (501) staff       (20)    12280 2023-05-05 12:54:05.000000 nexora-0.0.1/src/nexora/autotuna.py
--rw-r--r--   0 alicabukel   (501) staff       (20)    25357 2023-05-05 02:08:04.000000 nexora-0.0.1/src/nexora/boruta.py
-drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-05 14:01:38.627418 nexora-0.0.1/src/nexora/cli/
--rw-r--r--   0 alicabukel   (501) staff       (20)      305 2023-05-04 22:38:26.000000 nexora-0.0.1/src/nexora/cli/__init__.py
--rw-r--r--   0 alicabukel   (501) staff       (20)      996 2023-05-04 23:33:02.000000 nexora-0.0.1/src/nexora/cli/autotuna.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     1738 2023-05-05 14:01:12.000000 nexora-0.0.1/src/nexora/cli/explain.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     1108 2023-05-05 14:00:52.000000 nexora-0.0.1/src/nexora/cli/monitor.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     1181 2023-05-04 23:41:39.000000 nexora-0.0.1/src/nexora/cli/predict.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     1499 2023-05-04 23:33:34.000000 nexora-0.0.1/src/nexora/cli/serve.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     4482 2023-05-05 02:13:19.000000 nexora-0.0.1/src/nexora/cli/train.py
--rw-r--r--   0 alicabukel   (501) staff       (20)       43 2023-05-04 21:27:39.000000 nexora-0.0.1/src/nexora/config.ini
--rw-r--r--   0 alicabukel   (501) staff       (20)      185 2023-05-04 22:07:14.000000 nexora-0.0.1/src/nexora/config.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     1386 2023-05-05 00:54:20.000000 nexora-0.0.1/src/nexora/enums.py
--rw-r--r--   0 alicabukel   (501) staff       (20)      429 2023-05-05 00:12:11.000000 nexora-0.0.1/src/nexora/logger.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     3293 2023-05-05 03:37:14.000000 nexora-0.0.1/src/nexora/metrics.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     2474 2023-05-05 01:31:21.000000 nexora-0.0.1/src/nexora/params.py
--rw-r--r--   0 alicabukel   (501) staff       (20)     4244 2023-05-05 01:55:15.000000 nexora-0.0.1/src/nexora/predict.py
--rw-r--r--   0 alicabukel   (501) staff       (20)      485 2023-05-05 02:12:05.000000 nexora-0.0.1/src/nexora/schemas.py
--rw-r--r--   0 alicabukel   (501) staff       (20)    16090 2023-05-05 13:18:52.000000 nexora-0.0.1/src/nexora/utils.py
-drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-05 14:01:38.621501 nexora-0.0.1/src/nexora.egg-info/
--rw-r--r--   0 alicabukel   (501) staff       (20)     1508 2023-05-05 14:01:38.000000 nexora-0.0.1/src/nexora.egg-info/PKG-INFO
--rw-r--r--   0 alicabukel   (501) staff       (20)      713 2023-05-05 14:01:38.000000 nexora-0.0.1/src/nexora.egg-info/SOURCES.txt
--rw-r--r--   0 alicabukel   (501) staff       (20)        1 2023-05-05 14:01:38.000000 nexora-0.0.1/src/nexora.egg-info/dependency_links.txt
--rw-r--r--   0 alicabukel   (501) staff       (20)       52 2023-05-05 14:01:38.000000 nexora-0.0.1/src/nexora.egg-info/entry_points.txt
--rw-r--r--   0 alicabukel   (501) staff       (20)      234 2023-05-05 14:01:38.000000 nexora-0.0.1/src/nexora.egg-info/requires.txt
--rw-r--r--   0 alicabukel   (501) staff       (20)        7 2023-05-05 14:01:38.000000 nexora-0.0.1/src/nexora.egg-info/top_level.txt
+drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-09 14:44:37.650276 nexora-0.0.2/
+-rw-r--r--   0 alicabukel   (501) staff       (20)    11357 2023-05-04 08:59:14.000000 nexora-0.0.2/LICENSE
+-rw-r--r--   0 alicabukel   (501) staff       (20)      349 2023-05-09 14:44:37.650428 nexora-0.0.2/PKG-INFO
+-rw-r--r--   0 alicabukel   (501) staff       (20)       45 2023-05-09 14:29:35.000000 nexora-0.0.2/README.md
+drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-09 14:44:37.645803 nexora-0.0.2/nexora/
+-rw-r--r--   0 alicabukel   (501) staff       (20)       54 2023-05-09 14:43:59.000000 nexora-0.0.2/nexora/__init__.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)      331 2023-05-04 23:40:22.000000 nexora-0.0.2/nexora/api.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)    13108 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/autotuna.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)    25293 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/boruta.py
+drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-09 14:44:37.648229 nexora-0.0.2/nexora/cli/
+-rw-r--r--   0 alicabukel   (501) staff       (20)      305 2023-05-06 21:12:06.000000 nexora-0.0.2/nexora/cli/__init__.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     1227 2023-05-09 14:29:36.000000 nexora-0.0.2/nexora/cli/autotuna.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     2361 2023-05-09 14:33:32.000000 nexora-0.0.2/nexora/cli/explain.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     1122 2023-05-09 14:29:36.000000 nexora-0.0.2/nexora/cli/monitor.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     1332 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/cli/predict.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     1668 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/cli/serve.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     5648 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/cli/train.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)      181 2023-05-06 13:16:06.000000 nexora-0.0.2/nexora/config.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     1444 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/enums.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)      391 2023-05-09 14:33:55.000000 nexora-0.0.2/nexora/logger.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     3374 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/metrics.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     2644 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/params.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)     4763 2023-05-09 14:29:37.000000 nexora-0.0.2/nexora/predict.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)      504 2023-05-09 11:12:34.000000 nexora-0.0.2/nexora/schemas.py
+-rw-r--r--   0 alicabukel   (501) staff       (20)    18458 2023-05-09 14:34:09.000000 nexora-0.0.2/nexora/utils.py
+drwxr-xr-x   0 alicabukel   (501) staff       (20)        0 2023-05-09 14:44:37.649973 nexora-0.0.2/nexora.egg-info/
+-rw-r--r--   0 alicabukel   (501) staff       (20)      349 2023-05-09 14:44:37.000000 nexora-0.0.2/nexora.egg-info/PKG-INFO
+-rw-r--r--   0 alicabukel   (501) staff       (20)      629 2023-05-09 14:44:37.000000 nexora-0.0.2/nexora.egg-info/SOURCES.txt
+-rw-r--r--   0 alicabukel   (501) staff       (20)        1 2023-05-09 14:44:37.000000 nexora-0.0.2/nexora.egg-info/dependency_links.txt
+-rw-r--r--   0 alicabukel   (501) staff       (20)       52 2023-05-09 14:44:37.000000 nexora-0.0.2/nexora.egg-info/entry_points.txt
+-rw-r--r--   0 alicabukel   (501) staff       (20)      234 2023-05-09 14:44:37.000000 nexora-0.0.2/nexora.egg-info/requires.txt
+-rw-r--r--   0 alicabukel   (501) staff       (20)        7 2023-05-09 14:44:37.000000 nexora-0.0.2/nexora.egg-info/top_level.txt
+-rw-r--r--   0 alicabukel   (501) staff       (20)      122 2023-05-04 09:39:11.000000 nexora-0.0.2/pyproject.toml
+-rw-r--r--   0 alicabukel   (501) staff       (20)      972 2023-05-09 14:44:37.650951 nexora-0.0.2/setup.cfg
+-rw-r--r--   0 alicabukel   (501) staff       (20)      398 2023-05-09 11:29:03.000000 nexora-0.0.2/setup.py
```

### Comparing `nexora-0.0.1/LICENSE` & `nexora-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nexora-0.0.1/src/nexora/autotuna.py` & `nexora-0.0.2/nexora/autotuna.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 @dataclass
 class AutoTuna:
     # required arguments
     train_filename: str
     output: str
     algo: str
-    
+
+    objective: Optional[str] = "loss"
     # optional arguments
     test_filename: Optional[str] = None
     task: Optional[str] = None
     idx: Optional[str] = "id"
     targets: Optional[List[str]] = None
     features: Optional[List[str]] = None
     categorical_features: Optional[List[str]] = None
@@ -36,15 +37,17 @@
     num_trials: Optional[int] = 1000
     time_limit: Optional[int] = None
     fast: Optional[bool] = False
     fs: Optional[int] = 0
 
     def __post_init__(self):
         if os.path.exists(self.output):
-            raise Exception("Output directory already exists. Please specify some other directory.")
+            raise Exception(
+                "Output directory already exists. Please specify some other directory."
+            )
         os.makedirs(self.output, exist_ok=True)
         logger.info(f"Output directory: {self.output}")
 
         if self.targets is None:
             logger.warning("No target columns specified. Will default to `target`.")
             self.targets = ["target"]
 
@@ -56,27 +59,38 @@
         if "kfold" in train_df.columns:
             self.num_folds = len(np.unique(train_df["kfold"]))
             logger.info("Using `kfold` for folds from training data")
             return train_df
 
         logger.info("Creating folds")
         train_df["kfold"] = -1
-        if problem_type in (ProblemType.binary_classification, ProblemType.multi_class_classification):
+        if problem_type in (
+            ProblemType.binary_classification,
+            ProblemType.multi_class_classification,
+        ):
             y = train_df[self.targets].values
-            kf = StratifiedKFold(n_splits=self.num_folds, shuffle=True, random_state=self.seed)
+            kf = StratifiedKFold(
+                n_splits=self.num_folds, shuffle=True, random_state=self.seed
+            )
             for fold, (_, valid_indicies) in enumerate(kf.split(X=train_df, y=y)):
                 train_df.loc[valid_indicies, "kfold"] = fold
         elif problem_type == ProblemType.single_column_regression:
             y = train_df[self.targets].values
             num_bins = int(np.floor(1 + np.log2(len(train_df))))
             if num_bins > 10:
                 num_bins = 10
-            kf = StratifiedKFold(n_splits=self.num_folds, shuffle=True, random_state=self.seed)
-            train_df["bins"] = pd.cut(train_df[self.targets].values.ravel(), bins=num_bins, labels=False)
-            for fold, (_, valid_indicies) in enumerate(kf.split(X=train_df, y=train_df.bins.values)):
+            kf = StratifiedKFold(
+                n_splits=self.num_folds, shuffle=True, random_state=self.seed
+            )
+            train_df["bins"] = pd.cut(
+                train_df[self.targets].values.ravel(), bins=num_bins, labels=False
+            )
+            for fold, (_, valid_indicies) in enumerate(
+                kf.split(X=train_df, y=train_df.bins.values)
+            ):
                 train_df.loc[valid_indicies, "kfold"] = fold
             train_df = train_df.drop("bins", axis=1)
         elif problem_type == ProblemType.multi_column_regression:
             y = train_df[self.targets].values
             kf = KFold(n_splits=self.num_folds, shuffle=True, random_state=self.seed)
             for fold, (_, valid_indicies) in enumerate(kf.split(X=train_df, y=y)):
                 train_df.loc[valid_indicies, "kfold"] = fold
@@ -135,15 +149,17 @@
             elif target_type == "binary":
                 problem_type = ProblemType.binary_classification
             elif target_type == "multiclass":
                 problem_type = ProblemType.multi_class_classification
             elif target_type == "multilabel-indicator":
                 problem_type = ProblemType.multi_label_classification
             else:
-                raise Exception("Unable to infer `problem_type`. Please provide `classification` or `regression`")
+                raise Exception(
+                    "Unable to infer `problem_type`. Please provide `classification` or `regression`"
+                )
         logger.info(f"Problem type: {problem_type.name}")
         return problem_type
 
     def _inject_idxumn(self, df):
         if self.idx not in df.columns:
             df[self.idx] = np.arange(len(df))
         return df
@@ -165,15 +181,18 @@
         ignore_columns = [self.idx, "kfold"] + self.targets
 
         if self.features is None:
             self.features = list(train_df.columns)
             self.features = [x for x in self.features if x not in ignore_columns]
 
         # encode target(s)
-        if problem_type in [ProblemType.binary_classification, ProblemType.multi_class_classification]:
+        if problem_type in [
+            ProblemType.binary_classification,
+            ProblemType.multi_class_classification,
+        ]:
             logger.info("Encoding target(s)")
             target_encoder = LabelEncoder()
             target_encoder.fit(
                 train_df[self.targets].values.reshape(
                     -1,
                 )
             )
@@ -202,24 +221,38 @@
         categorical_encoders = {}
         for fold in range(self.num_folds):
             fold_train = train_df[train_df.kfold != fold].reset_index(drop=True)
             fold_valid = train_df[train_df.kfold == fold].reset_index(drop=True)
             if self.test_filename is not None:
                 test_fold = test_df.copy(deep=True)
             if len(categorical_features) > 0:
-                ord_encoder = OrdinalEncoder(handle_unknown="use_encoded_value", unknown_value=np.nan)
-                fold_train[categorical_features] = ord_encoder.fit_transform(fold_train[categorical_features].values)
-                fold_valid[categorical_features] = ord_encoder.transform(fold_valid[categorical_features].values)
+                ord_encoder = OrdinalEncoder(
+                    handle_unknown="use_encoded_value", unknown_value=np.nan
+                )
+                fold_train[categorical_features] = ord_encoder.fit_transform(
+                    fold_train[categorical_features].values
+                )
+                fold_valid[categorical_features] = ord_encoder.transform(
+                    fold_valid[categorical_features].values
+                )
                 if self.test_filename is not None:
-                    test_fold[categorical_features] = ord_encoder.transform(test_fold[categorical_features].values)
+                    test_fold[categorical_features] = ord_encoder.transform(
+                        test_fold[categorical_features].values
+                    )
                 categorical_encoders[fold] = ord_encoder
-            fold_train.to_feather(os.path.join(self.output, f"train_fold_{fold}.feather"))
-            fold_valid.to_feather(os.path.join(self.output, f"valid_fold_{fold}.feather"))
+            fold_train.to_feather(
+                os.path.join(self.output, f"train_fold_{fold}.feather")
+            )
+            fold_valid.to_feather(
+                os.path.join(self.output, f"valid_fold_{fold}.feather")
+            )
             if self.test_filename is not None:
-                test_fold.to_feather(os.path.join(self.output, f"test_fold_{fold}.feather"))
+                test_fold.to_feather(
+                    os.path.join(self.output, f"test_fold_{fold}.feather")
+                )
 
         # save config
         model_config = {}
         model_config["idx"] = self.idx
         model_config["features"] = self.features
         model_config["categorical_features"] = categorical_features
         model_config["train_filename"] = self.train_filename
@@ -230,16 +263,17 @@
         model_config["targets"] = self.targets
         model_config["use_gpu"] = self.use_gpu
         model_config["num_folds"] = self.num_folds
         model_config["seed"] = self.seed
         model_config["num_trials"] = self.num_trials
         model_config["time_limit"] = self.time_limit
         model_config["fast"] = self.fast
-        model_config['algo'] = self.algo
-        model_config['fs'] = self.fs
+        model_config["algo"] = self.algo
+        model_config["fs"] = self.fs
+        model_config["objective"] = self.objective
 
         self.model_config = ModelConfig(**model_config)
         logger.info(f"Model config: {self.model_config}")
         logger.info("Saving model config")
         joblib.dump(self.model_config, f"{self.output}/atuna.config")
 
         # save encoders
@@ -247,25 +281,31 @@
         joblib.dump(categorical_encoders, f"{self.output}/atuna.categorical_encoders")
         joblib.dump(target_encoder, f"{self.output}/atuna.target_encoder")
 
     def train(self):
         self._process_data()
 
         if self.model_config.fs == 1:
-            logger.info('Feature Importance Step')
+            logger.info("Feature Importance Step")
             selected_features = select_features(self.model_config)
             self.model_config.features = selected_features
-            logger.info('Features updated with selected features')
+            logger.info("Features updated with selected features")
             logger.info(selected_features)
 
         best_params = train_model(self.model_config)
-        
-        logger.info(f'Best params: {best_params}')
-        with open(os.path.join(self.model_config.output, 'best_params.json'), 'w') as f:
+
+        logger.info(f"Best params: {best_params}")
+        with open(os.path.join(self.model_config.output, "best_params.json"), "w") as f:
             json.dump(best_params, f)
-        
+
+        selected_features_dict = {f: f for f in self.model_config.features}
+        with open(
+            os.path.join(self.model_config.output, "selected_features.json"), "w"
+        ) as f:
+            json.dump(selected_features_dict, f)
+
         logger.info("Training complete")
         self.predict(best_params)
 
     def predict(self, best_params):
         logger.info("Creating OOF and test predictions")
         predict_model(self.model_config, best_params)
```

### Comparing `nexora-0.0.1/src/nexora/boruta.py` & `nexora-0.0.2/nexora/boruta.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,18 +116,18 @@
 
     early_stopping : bool, default = False
         Whether to use early stopping to terminate the selection process
         before reaching `max_iter` iterations if the algorithm cannot
         confirm a tentative feature for `n_iter_no_change` iterations.
         Will speed up the process at a cost of a possibility of a
         worse result.
-        
+
     n_iter_no_change : int, default = 20
         Ignored if `early_stopping` is False. The maximum amount of
-        iterations without confirming a tentative feature. 
+        iterations without confirming a tentative feature.
 
     Attributes
     ----------
 
     n_features_ : int
         The number of selected features.
 
@@ -145,70 +145,80 @@
         The feature ranking, such that ``ranking_[i]`` corresponds to the
         ranking position of the i-th feature. Selected (i.e., estimated
         best) features are assigned rank 1 and tentative features are assigned
         rank 2.
 
     importance_history_ : array-like, shape [n_features, n_iters]
 
-        The calculated importance values for each feature across all iterations.  
+        The calculated importance values for each feature across all iterations.
 
     Examples
     --------
-    
+
     import pandas as pd
     from sklearn.ensemble import RandomForestClassifier
     from boruta import BorutaPy
-    
+
     # load X and y
     # NOTE BorutaPy accepts numpy arrays only, hence the .values attribute
     X = pd.read_csv('examples/test_X.csv', index_col=0).values
     y = pd.read_csv('examples/test_y.csv', header=None, index_col=0).values
     y = y.ravel()
-    
+
     # define random forest classifier, with utilising all cores and
     # sampling in proportion to y labels
     rf = RandomForestClassifier(n_jobs=-1, class_weight='balanced', max_depth=5)
-    
+
     # define Boruta feature selection method
     feat_selector = BorutaPy(rf, n_estimators='auto', verbose=2, random_state=1)
-    
+
     # find all relevant features - 5 features should be selected
     feat_selector.fit(X, y)
-    
+
     # check selected features - first 5 features are selected
     feat_selector.support_
-    
+
     # check ranking of features
     feat_selector.ranking_
-    
+
     # call transform() on X to filter it down to selected features
     X_filtered = feat_selector.transform(X)
 
     References
     ----------
 
     [1] Kursa M., Rudnicki W., "Feature Selection with the Boruta Package"
         Journal of Statistical Software, Vol. 36, Issue 11, Sep 2010
     """
 
-    def __init__(self, estimator, n_estimators=1000, perc=100, alpha=0.05,
-                 two_step=True, max_iter=100, random_state=None, verbose=0,
-                 early_stopping=False, n_iter_no_change=20):
+    def __init__(
+        self,
+        estimator,
+        n_estimators=1000,
+        perc=100,
+        alpha=0.05,
+        two_step=True,
+        max_iter=100,
+        random_state=None,
+        verbose=0,
+        early_stopping=False,
+        n_iter_no_change=20,
+    ):
         self.estimator = estimator
         self.n_estimators = n_estimators
         self.perc = perc
         self.alpha = alpha
         self.two_step = two_step
         self.max_iter = max_iter
         self.random_state = random_state
         self.verbose = verbose
         self.early_stopping = early_stopping
         self.n_iter_no_change = n_iter_no_change
-        self.__version__ = '0.3'
-        self._is_lightgbm = 'lightgbm' in str(type(self.estimator))
+        self.__version__ = "0.3"
+        self._is_lightgbm = "lightgbm" in str(type(self.estimator))
 
     def fit(self, X, y):
         """
         Fits the Boruta feature selection with the provided estimator.
 
         Parameters
         ----------
@@ -228,15 +238,15 @@
         Parameters
         ----------
         X : array-like, shape = [n_samples, n_features]
             The training input samples.
 
         weak: boolean, default = False
             If set to true, the tentative features are also used to reduce X.
-        
+
         return_df : boolean, default = False
             If ``X`` if a pandas dataframe and this parameter is set to True,
             the transformed data will also be a dataframe.
 
         Returns
         -------
         X : array-like, shape = [n_samples, n_features_]
@@ -275,41 +285,39 @@
         self._fit(X, y)
         return self._transform(X, weak, return_df)
 
     def _validate_pandas_input(self, arg):
         try:
             return arg.values
         except AttributeError:
-            raise ValueError(
-                "input needs to be a numpy array or pandas data frame."
-            )
+            raise ValueError("input needs to be a numpy array or pandas data frame.")
 
     def _fit(self, X, y):
         # check input params
         self._check_params(X, y)
 
         if not isinstance(X, np.ndarray):
-            X = self._validate_pandas_input(X) 
+            X = self._validate_pandas_input(X)
         if not isinstance(y, np.ndarray):
             y = self._validate_pandas_input(y)
 
         self.random_state = check_random_state(self.random_state)
-        
+
         early_stopping = False
         if self.early_stopping:
             if self.n_iter_no_change >= self.max_iter:
                 if self.verbose > 0:
                     print(
                         f"n_iter_no_change is bigger or equal to max_iter"
                         f"({self.n_iter_no_change} >= {self.max_iter}), "
                         f"early stopping will not be used."
                     )
             else:
                 early_stopping = True
-        
+
         # setup variables for Boruta
         n_sample, n_feat = X.shape
         _iter = 1
         # early stopping vars
         _same_iters = 1
         _last_dec_reg = None
         # holds the decision about each feature:
@@ -321,29 +329,31 @@
         # the best of the shadow features
         hit_reg = np.zeros(n_feat, dtype=int)
         # these record the history of the iterations
         imp_history = np.zeros(n_feat, dtype=float)
         sha_max_history = []
 
         # set n_estimators
-        if self.n_estimators != 'auto':
+        if self.n_estimators != "auto":
             self.estimator.set_params(n_estimators=self.n_estimators)
 
         # main feature selection loop
         while np.any(dec_reg == 0) and _iter < self.max_iter:
             # find optimal number of trees and depth
-            if self.n_estimators == 'auto':
+            if self.n_estimators == "auto":
                 # number of features that aren't rejected
                 not_rejected = np.where(dec_reg >= 0)[0].shape[0]
                 n_tree = self._get_tree_num(not_rejected)
                 self.estimator.set_params(n_estimators=n_tree)
 
             # make sure we start with a new tree in each iteration
             if self._is_lightgbm:
-                self.estimator.set_params(random_state=self.random_state.randint(0, 10000))
+                self.estimator.set_params(
+                    random_state=self.random_state.randint(0, 10000)
+                )
             else:
                 self.estimator.set_params(random_state=self.random_state)
 
             # add shadow attributes, shuffle them and train estimator, get imps
             cur_imp = self._add_shadows_get_imps(X, y, dec_reg)
 
             # get the threshold of shadow importances we will use for rejection
@@ -361,15 +371,15 @@
             dec_reg = self._do_tests(dec_reg, hit_reg, _iter)
 
             # print out confirmed features
             if self.verbose > 0 and _iter < self.max_iter:
                 self._print_results(dec_reg, _iter, 0)
             if _iter < self.max_iter:
                 _iter += 1
-                
+
             # early stopping
             if early_stopping:
                 if _last_dec_reg is not None and (_last_dec_reg == dec_reg).all():
                     _same_iters += 1
                     if self.verbose > 0:
                         print(
                             f"Early stopping: {_same_iters} out "
@@ -383,16 +393,15 @@
 
         # we automatically apply R package's rough fix for tentative ones
         confirmed = np.where(dec_reg == 1)[0]
         tentative = np.where(dec_reg == 0)[0]
         # ignore the first row of zeros
         tentative_median = np.median(imp_history[1:, tentative], axis=0)
         # which tentative to keep
-        tentative_confirmed = np.where(tentative_median
-                                       > np.median(sha_max_history))[0]
+        tentative_confirmed = np.where(tentative_median > np.median(sha_max_history))[0]
         tentative = tentative[tentative_confirmed]
 
         # basic result variables
         self.n_features_ = confirmed.shape[0]
         self.support_ = np.zeros(n_feat, dtype=bool)
         self.support_[confirmed] = 1
         self.support_weak_ = np.zeros(n_feat, dtype=bool)
@@ -407,26 +416,26 @@
         # all rejected features are sorted by importance history
         not_selected = np.setdiff1d(np.arange(n_feat), selected)
         # large importance values should rank higher = lower ranks -> *(-1)
         imp_history_rejected = imp_history[1:, not_selected] * -1
 
         # update rank for not_selected features
         if not_selected.shape[0] > 0:
-                # calculate ranks in each iteration, then median of ranks across feats
-                iter_ranks = self._nanrankdata(imp_history_rejected, axis=1)
-                rank_medians = np.nanmedian(iter_ranks, axis=0)
-                ranks = self._nanrankdata(rank_medians, axis=0)
-
-                # set smallest rank to 3 if there are tentative feats
-                if tentative.shape[0] > 0:
-                    ranks = ranks - np.min(ranks) + 3
-                else:
-                    # and 2 otherwise
-                    ranks = ranks - np.min(ranks) + 2
-                self.ranking_[not_selected] = ranks
+            # calculate ranks in each iteration, then median of ranks across feats
+            iter_ranks = self._nanrankdata(imp_history_rejected, axis=1)
+            rank_medians = np.nanmedian(iter_ranks, axis=0)
+            ranks = self._nanrankdata(rank_medians, axis=0)
+
+            # set smallest rank to 3 if there are tentative feats
+            if tentative.shape[0] > 0:
+                ranks = ranks - np.min(ranks) + 3
+            else:
+                # and 2 otherwise
+                ranks = ranks - np.min(ranks) + 2
+            self.ranking_[not_selected] = ranks
         else:
             # all are selected, thus we set feature supports to True
             self.support_ = np.ones(n_feat, dtype=bool)
 
         self.importance_history_ = imp_history
 
         # notify user
@@ -435,15 +444,15 @@
         return self
 
     def _transform(self, X, weak=False, return_df=False):
         # sanity check
         try:
             self.ranking_
         except AttributeError:
-            raise ValueError('You need to call the fit(X, y) method first.')
+            raise ValueError("You need to call the fit(X, y) method first.")
 
         if weak:
             indices = self.support_ + self.support_weak_
         else:
             indices = self.support_
 
         if return_df:
@@ -451,55 +460,59 @@
         else:
             X = X[:, indices]
         return X
 
     def _get_tree_num(self, n_feat):
         depth = None
         try:
-            depth = self.estimator.get_params()['max_depth']
+            depth = self.estimator.get_params()["max_depth"]
         except KeyError:
             warnings.warn(
                 "The estimator does not have a max_depth property, as a result "
                 " the number of trees to use cannot be estimated automatically."
             )
         if depth == None:
             depth = 10
         # how many times a feature should be considered on average
         f_repr = 100
         # n_feat * 2 because the training matrix is extended with n shadow features
-        multi = ((n_feat * 2) / (np.sqrt(n_feat * 2) * depth))
+        multi = (n_feat * 2) / (np.sqrt(n_feat * 2) * depth)
         n_estimators = int(multi * f_repr)
         return n_estimators
 
     def _get_imp(self, X, y):
         try:
             self.estimator.fit(X, y)
         except Exception as e:
-            raise ValueError('Please check your X and y variable. The provided '
-                             'estimator cannot be fitted to your data.\n' + str(e))
+            raise ValueError(
+                "Please check your X and y variable. The provided "
+                "estimator cannot be fitted to your data.\n" + str(e)
+            )
         try:
             imp = self.estimator.feature_importances_
         except Exception:
-            raise ValueError('Only methods with feature_importance_ attribute '
-                             'are currently supported in BorutaPy.')
+            raise ValueError(
+                "Only methods with feature_importance_ attribute "
+                "are currently supported in BorutaPy."
+            )
         return imp
 
     def _get_shuffle(self, seq):
         self.random_state.shuffle(seq)
         return seq
 
     def _add_shadows_get_imps(self, X, y, dec_reg):
         # find features that are tentative still
         x_cur_ind = np.where(dec_reg >= 0)[0]
         x_cur = np.copy(X[:, x_cur_ind])
         x_cur_w = x_cur.shape[1]
         # deep copy the matrix for the shadow matrix
         x_sha = np.copy(x_cur)
         # make sure there's at least 5 columns in the shadow matrix for
-        while (x_sha.shape[1] < 5):
+        while x_sha.shape[1] < 5:
             x_sha = np.hstack((x_sha, x_sha))
         # shuffle xSha
         x_sha = np.apply_along_axis(self._get_shuffle, 0, x_sha)
         # get importance of the merged matrix
         imp = self._get_imp(np.hstack((x_cur, x_sha)), y)
         # separate importances of real and shadow features
         imp_sha = imp[x_cur_w:]
@@ -516,16 +529,16 @@
         hit_reg[hits] += 1
         return hit_reg
 
     def _do_tests(self, dec_reg, hit_reg, _iter):
         active_features = np.where(dec_reg >= 0)[0]
         hits = hit_reg[active_features]
         # get uncorrected p values based on hit_reg
-        to_accept_ps = sp.stats.binom.sf(hits - 1, _iter, .5).flatten()
-        to_reject_ps = sp.stats.binom.cdf(hits, _iter, .5).flatten()
+        to_accept_ps = sp.stats.binom.sf(hits - 1, _iter, 0.5).flatten()
+        to_reject_ps = sp.stats.binom.cdf(hits, _iter, 0.5).flatten()
 
         if self.two_step:
             # two step multicor process
             # first we correct for testing several features in each round using FDR
             to_accept = self._fdrcorrection(to_accept_ps, alpha=self.alpha)[0]
             to_reject = self._fdrcorrection(to_reject_ps, alpha=self.alpha)[0]
 
@@ -603,35 +616,35 @@
     def _check_params(self, X, y):
         """
         Check hyperparameters as well as X and y before proceeding with fit.
         """
         # check X and y are consistent len, X is Array and y is column
         X, y = check_X_y(X, y)
         if self.perc <= 0 or self.perc > 100:
-            raise ValueError('The percentile should be between 0 and 100.')
+            raise ValueError("The percentile should be between 0 and 100.")
 
         if self.alpha <= 0 or self.alpha > 1:
-            raise ValueError('Alpha should be between 0 and 1.')
+            raise ValueError("Alpha should be between 0 and 1.")
 
     def _print_results(self, dec_reg, _iter, flag):
-        n_iter = str(_iter) + ' / ' + str(self.max_iter)
+        n_iter = str(_iter) + " / " + str(self.max_iter)
         n_confirmed = np.where(dec_reg == 1)[0].shape[0]
         n_rejected = np.where(dec_reg == -1)[0].shape[0]
-        cols = ['Iteration: ', 'Confirmed: ', 'Tentative: ', 'Rejected: ']
+        cols = ["Iteration: ", "Confirmed: ", "Tentative: ", "Rejected: "]
 
         # still in feature selection
         if flag == 0:
             n_tentative = np.where(dec_reg == 0)[0].shape[0]
             content = map(str, [n_iter, n_confirmed, n_tentative, n_rejected])
             if self.verbose == 1:
                 output = cols[0] + n_iter
             elif self.verbose > 1:
-                output = '\n'.join([x[0] + '\t' + x[1] for x in zip(cols, content)])
+                output = "\n".join([x[0] + "\t" + x[1] for x in zip(cols, content)])
 
         # Boruta finished running and tentatives have been filtered
         else:
             n_tentative = np.sum(self.support_weak_)
-            n_rejected = np.sum(~(self.support_|self.support_weak_))
+            n_rejected = np.sum(~(self.support_ | self.support_weak_))
             content = map(str, [n_iter, n_confirmed, n_tentative, n_rejected])
-            result = '\n'.join([x[0] + '\t' + x[1] for x in zip(cols, content)])
+            result = "\n".join([x[0] + "\t" + x[1] for x in zip(cols, content)])
             output = "\n\nBorutaPy finished running.\n\n" + result
         print(output)
```

### Comparing `nexora-0.0.1/src/nexora/cli/autotuna.py` & `nexora-0.0.2/nexora/cli/autotuna.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import argparse
 
 from .. import __version__
+
 from .predict import PredictAutoTunaCommand
 from .serve import ServeAutoTunaCommand
 from .train import TrainAutoTunaCommand
+from .explain import ExplainAutoTunaCommand
+from .monitor import MonitorAutoTunaCommand
 
 
 def main():
     parser = argparse.ArgumentParser(
         "AutoTuna CLI",
         usage="nexora <command> [<args>]",
         epilog="For more information about a command, run: `nexora <command> --help`",
     )
-    parser.add_argument("--version", "-v", help="Display AutoTuna version", action="store_true")
+    parser.add_argument(
+        "--version", "-v", help="Display AutoTuna version", action="store_true"
+    )
 
     commands_parser = parser.add_subparsers(help="commands")
     TrainAutoTunaCommand.register_subcommand(commands_parser)
     PredictAutoTunaCommand.register_subcommand(commands_parser)
     ServeAutoTunaCommand.register_subcommand(commands_parser)
+    ExplainAutoTunaCommand.register_subcommand(commands_parser)
+    MonitorAutoTunaCommand.register_subcommand(commands_parser)
 
     args = parser.parse_args()
 
     if args.version:
         print(__version__)
         exit(0)
```

### Comparing `nexora-0.0.1/src/nexora/cli/explain.py` & `nexora-0.0.2/nexora/cli/explain.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,73 @@
 import os
 import pandas as pd
+import json
 import joblib
 from argparse import ArgumentParser
 
 from shapash import SmartExplainer
-
 from . import BaseCommand
 
 
 def explain_autotuna_command_factory(args):
-    return ExplainAutoTunaCommand(args.model_path, args.data_path, args.config_path, args.port, args.host)
+    return ExplainAutoTunaCommand(
+        args.model_path,
+        args.data_path,
+        args.config_path,
+        args.features_path,
+        args.port,
+        args.host,
+    )
 
 
 class ExplainAutoTunaCommand(BaseCommand):
     @staticmethod
     def register_subcommand(parser: ArgumentParser):
         _parser = parser.add_parser("explain", help="Explain AutoTuna Models")
-        _parser.add_argument("--model_path", help="Path to model", required=True, type=str)
-        _parser.add_argument("--data_path", help="Path to data", required=True, type=str)
-        _parser.add_argument("--config_path", help="Path to config", required=True, type=str)
-        _parser.add_argument("--port", help="Port to serve on", default=8080, type=int, required=False)
-        _parser.add_argument("--host", help="Host to serve on", default="127.0.0.1", type=str, required=False)
+        _parser.add_argument(
+            "--model_path", help="Path to model", required=True, type=str
+        )
+        _parser.add_argument(
+            "--data_path", help="Path to data", required=True, type=str
+        )
+        _parser.add_argument(
+            "--config_path", help="Path to config", required=True, type=str
+        )
+        _parser.add_argument(
+            "--features_path", help="Path to features", required=True, type=str
+        )
+        _parser.add_argument(
+            "--port", help="Port to serve on", default=8050, type=int, required=False
+        )
+        _parser.add_argument(
+            "--host",
+            help="Host to serve on",
+            default="0.0.0.0",
+            type=str,
+            required=False,
+        )
         _parser.set_defaults(func=explain_autotuna_command_factory)
 
-    def __init__(self, model_path, data_path, config_path, port, host):
+    def __init__(self, model_path, data_path, config_path, features_path, port, host):
         self.model_path = model_path
         self.data_path = data_path
         self.config_path = config_path
+        self.features_path = features_path
         self.port = port
         self.host = host
 
     def execute(self):
         os.environ["AUTOTUNA_MODEL_PATH"] = self.model_path
         model = joblib.load(self.model_path)
-        config = joblib.load('xgb-trial-2/atuna.config')
+        config = joblib.load(self.config_path)
         df = pd.read_feather(self.data_path)
-        x=df[config.features]
-        y=df[config.targets]
-        xpl = SmartExplainer(model=model)
+        with open(self.features_path) as f:
+            features_dict = json.load(f)
+        x = df[list(features_dict.keys())]
+        y = df[config.targets]
+        xpl = SmartExplainer(
+            model=model,
+            features_dict=features_dict,
+            explainer_args={"algorithm": "tree"},
+        )
         xpl.compile(x=x, y_target=y)
-        app = xpl.run_app(title_story=config.output, host=self.host, port=self.port)
+        _ = xpl.run_app(title_story=config.output, host=self.host, port=self.port)
```

### Comparing `nexora-0.0.1/src/nexora/cli/monitor.py` & `nexora-0.0.2/nexora/cli/monitor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-import os
 from argparse import ArgumentParser
 
 import optuna_dashboard
 
 from . import BaseCommand
 
 
 def monitor_autotuna_command_factory(args):
-    return MonitorAutoTunaCommand(args.model_path, args.port, args.host, args.workers, args.debug)
+    return MonitorAutoTunaCommand(args.db_path, args.port, args.host)
 
 
 class MonitorAutoTunaCommand(BaseCommand):
     @staticmethod
     def register_subcommand(parser: ArgumentParser):
         _parser = parser.add_parser("monitor", help="Explain AutoTuna Models")
         _parser.add_argument("--db_path", help="Path to db", required=True, type=str)
-        _parser.add_argument("--port", help="Port to serve on", default=8080, type=int, required=False)
-        _parser.add_argument("--host", help="Host to serve on", default="127.0.0.1", type=str, required=False)
+        _parser.add_argument(
+            "--port", help="Port to serve on", default=8080, type=int, required=False
+        )
+        _parser.add_argument(
+            "--host",
+            help="Host to serve on",
+            default="0.0.0.0",
+            type=str,
+            required=False,
+        )
         _parser.set_defaults(func=monitor_autotuna_command_factory)
 
     def __init__(self, db_path, port, host):
         self.db_path = db_path
         self.port = port
         self.host = host
 
     def execute(self):
-        os.environ["AUTOTUNA_MODEL_PATH"] = self.model_path
-        optuna_dashboard.run_server(storage=self.db_path, host=self.host, port=self.port)
+        optuna_dashboard.run_server(
+            storage=self.db_path, host=self.host, port=self.port
+        )
```

### Comparing `nexora-0.0.1/src/nexora/cli/predict.py` & `nexora-0.0.2/nexora/cli/predict.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 from argparse import ArgumentParser
 
 from ..predict import AutoTunaPredict
 from . import BaseCommand
 
 
 def predict_autotuna_command_factory(args):
-    return PredictAutoTunaCommand(args.model_path, args.test_filename, args.out_filename)
+    return PredictAutoTunaCommand(
+        args.model_path, args.test_filename, args.out_filename
+    )
 
 
 class PredictAutoTunaCommand(BaseCommand):
     @staticmethod
     def register_subcommand(parser: ArgumentParser):
         _parser = parser.add_parser("predict", help="Make predictions on any CSV file")
-        _parser.add_argument("--model_path", help="Path to model", required=True, type=str)
-        _parser.add_argument("--test_filename", help="Path to test file", required=False, type=str, default=None)
-        _parser.add_argument("--out_filename", help="Path to output file", required=True, type=str)
+        _parser.add_argument(
+            "--model_path", help="Path to model", required=True, type=str
+        )
+        _parser.add_argument(
+            "--test_filename",
+            help="Path to test file",
+            required=False,
+            type=str,
+            default=None,
+        )
+        _parser.add_argument(
+            "--out_filename", help="Path to output file", required=True, type=str
+        )
         _parser.set_defaults(func=predict_autotuna_command_factory)
 
     def __init__(self, model_path, test_filename, out_filename):
         self.model_path = model_path
         self.test_filename = test_filename
         self.out_filename = out_filename
 
     def execute(self):
         atunap = AutoTunaPredict(model_path=self.model_path)
-        atunap.predict_file(test_filename=self.test_filename, out_filename=self.out_filename)
+        atunap.predict_file(
+            test_filename=self.test_filename, out_filename=self.out_filename
+        )
```

### Comparing `nexora-0.0.1/src/nexora/cli/serve.py` & `nexora-0.0.2/nexora/cli/serve.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,38 +3,54 @@
 
 import uvicorn
 
 from . import BaseCommand
 
 
 def serve_autotuna_command_factory(args):
-    return ServeAutoTunaCommand(args.model_path, args.port, args.host, args.workers, args.debug)
+    return ServeAutoTunaCommand(
+        args.model_path, args.port, args.host, args.workers, args.debug
+    )
 
 
 class ServeAutoTunaCommand(BaseCommand):
     @staticmethod
     def register_subcommand(parser: ArgumentParser):
         _parser = parser.add_parser("serve", help="Serve AutoTuna API")
-        _parser.add_argument("--model_path", help="Path to model", required=True, type=str)
-        _parser.add_argument("--port", help="Port to serve on", default=9999, type=int, required=False)
-        _parser.add_argument("--host", help="Host to serve on", default="127.0.0.1", type=str, required=False)
-        _parser.add_argument("--workers", help="Number of workers", default=1, type=int, required=False)
-        _parser.add_argument("--debug", help="Debug mode", action="store_true", required=False)
+        _parser.add_argument(
+            "--model_path", help="Path to model", required=True, type=str
+        )
+        _parser.add_argument(
+            "--port", help="Port to serve on", default=9999, type=int, required=False
+        )
+        _parser.add_argument(
+            "--host",
+            help="Host to serve on",
+            default="0.0.0.0",
+            type=str,
+            required=False,
+        )
+        _parser.add_argument(
+            "--workers", help="Number of workers", default=1, type=int, required=False
+        )
+        _parser.add_argument(
+            "--debug", help="Debug mode", action="store_true", required=False
+        )
         _parser.set_defaults(func=serve_autotuna_command_factory)
 
     def __init__(self, model_path, port, host, workers, debug):
         self.model_path = model_path
         self.port = port
         self.host = host
         self.workers = workers
         self.debug = debug
 
     def execute(self):
         os.environ["AUTOTUNA_MODEL_PATH"] = self.model_path
         # run app using uvicorn
         uvicorn.run(
-            "autotuna.api:app",
+            "nexora.api:app",
             host=self.host,
             port=self.port,
             debug=self.debug,
             workers=self.workers,
         )
```

### Comparing `nexora-0.0.1/src/nexora/enums.py` & `nexora-0.0.2/nexora/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,11 +39,15 @@
         elif label == "multi_column_regression":
             return ProblemType.multi_column_regression
         else:
             raise NotImplementedError
 
 
 class Algo(enum.Enum):
-    xgb = 'xgb'
-    lgbm = 'lgbm'
-    gbm = 'gbm'
-    rf = 'rf'
+    xgb = "xgb"
+    lgbm = "lgbm"
+    rf = "rf"
+
+
+class Objective(enum.Enum):
+    loss = "loss"
+    accuracy = "accuracy"
```

### Comparing `nexora-0.0.1/src/nexora/metrics.py` & `nexora-0.0.2/nexora/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,46 +11,49 @@
 @dataclass
 class Metrics:
     problem_type: ProblemType
     algo: Algo
 
     def __post_init__(self):
         if self.problem_type == ProblemType.binary_classification:
-            log_loss_key = 'logloss'
+            log_loss_key = "logloss"
             if self.algo == Algo.lgbm.value:
-                log_loss_key = 'binary_logloss'
+                log_loss_key = "binary_logloss"
             self.valid_metrics = {
                 "auc": skmetrics.roc_auc_score,
                 log_loss_key: skmetrics.log_loss,
                 "f1": skmetrics.f1_score,
                 "accuracy": skmetrics.accuracy_score,
                 "precision": skmetrics.precision_score,
                 "recall": skmetrics.recall_score,
             }
         elif self.problem_type == ProblemType.multi_class_classification:
-            log_loss_key = 'mlogloss'
+            log_loss_key = "mlogloss"
             if self.algo == Algo.lgbm.value:
-                log_loss_key = 'multi_logloss'
+                log_loss_key = "multi_logloss"
             self.valid_metrics = {
                 log_loss_key: skmetrics.log_loss,
                 "accuracy": skmetrics.accuracy_score,
                 "mlogloss": skmetrics.log_loss,
             }
-        elif self.problem_type in (ProblemType.single_column_regression, ProblemType.multi_column_regression):
+        elif self.problem_type in (
+            ProblemType.single_column_regression,
+            ProblemType.multi_column_regression,
+        ):
             self.valid_metrics = {
                 "r2": skmetrics.r2_score,
                 "mse": skmetrics.mean_squared_error,
                 "mae": skmetrics.mean_absolute_error,
                 "rmse": partial(skmetrics.mean_squared_error, squared=False),
                 "rmsle": partial(skmetrics.mean_squared_log_error, squared=False),
             }
         elif self.problem_type == ProblemType.multi_label_classification:
-            log_loss_key = 'logloss'
+            log_loss_key = "logloss"
             if self.algo == Algo.lgbm.value:
-                log_loss_key = 'binary_logloss'
+                log_loss_key = "binary_logloss"
             self.valid_metrics = {
                 log_loss_key: skmetrics.log_loss,
             }
         else:
             raise Exception("Invalid problem type")
 
     def calculate(self, y_true, y_pred):
@@ -61,15 +64,17 @@
                     metrics[metric_name] = metric_func(y_true, y_pred[:, 1])
                 elif metric_name in ["logloss", "binary_logloss"]:
                     metrics[metric_name] = metric_func(y_true, y_pred)
                 else:
                     metrics[metric_name] = metric_func(y_true, y_pred[:, 1] >= 0.5)
             elif self.problem_type == ProblemType.multi_class_classification:
                 if metric_name == "accuracy":
-                    metrics[metric_name] = metric_func(y_true, np.argmax(y_pred, axis=1))
+                    metrics[metric_name] = metric_func(
+                        y_true, np.argmax(y_pred, axis=1)
+                    )
                 else:
                     metrics[metric_name] = metric_func(y_true, y_pred)
             else:
                 if metric_name == "rmsle":
                     temp_pred = copy.deepcopy(y_pred)
                     temp_pred[temp_pred < 0] = 0
                     metrics[metric_name] = metric_func(y_true, temp_pred)
```

### Comparing `nexora-0.0.1/src/nexora/params.py` & `nexora-0.0.2/nexora/params.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,39 +6,53 @@
         params = {
             "learning_rate": trial.suggest_float("learning_rate", 1e-2, 0.25, log=True),
             "reg_lambda": trial.suggest_float("reg_lambda", 1e-8, 100.0, log=True),
             "reg_alpha": trial.suggest_float("reg_alpha", 1e-8, 100.0, log=True),
             "subsample": trial.suggest_float("subsample", 0.1, 1.0),
             "colsample_bytree": trial.suggest_float("colsample_bytree", 0.1, 1.0),
             "max_depth": trial.suggest_int("max_depth", 1, 9),
-            "early_stopping_rounds": trial.suggest_int("early_stopping_rounds", 100, 500),
-            "n_estimators": trial.suggest_categorical("n_estimators", [7000, 15000, 20000]),
+            "early_stopping_rounds": trial.suggest_int(
+                "early_stopping_rounds", 100, 500
+            ),
+            "n_estimators": trial.suggest_categorical(
+                "n_estimators", [7000, 15000, 20000]
+            ),
         }
         if model_config.use_gpu:
             params["tree_method"] = "gpu_hist"
             params["gpu_id"] = 0
             params["predictor"] = "gpu_predictor"
         else:
-            params["tree_method"] = trial.suggest_categorical("tree_method", ["exact", "approx", "hist"])
-            params["booster"] = trial.suggest_categorical("booster", ["gbtree", "gblinear"])
+            params["tree_method"] = trial.suggest_categorical(
+                "tree_method", ["exact", "approx", "hist"]
+            )
+            params["booster"] = trial.suggest_categorical(
+                "booster", ["gbtree", "gblinear"]
+            )
             if params["booster"] == "gbtree":
                 params["gamma"] = trial.suggest_float("gamma", 1e-8, 1.0, log=True)
-                params["grow_policy"] = trial.suggest_categorical("grow_policy", ["depthwise", "lossguide"])
+                params["grow_policy"] = trial.suggest_categorical(
+                    "grow_policy", ["depthwise", "lossguide"]
+                )
 
     elif model_config.algo == Algo.lgbm.value:
         params = {
-                "learning_rate": trial.suggest_float("learning_rate", 1e-2, 0.25, log=True),
-                "max_depth": trial.suggest_int("max_depth", 1, 9),
-                "early_stopping_rounds": trial.suggest_int("early_stopping_rounds", 100, 500),
-                "n_estimators": trial.suggest_categorical("n_estimators", [7000, 15000, 20000]),
-                'lambda_l1': trial.suggest_float('lambda_l1', 1e-8, 10.0, log=True),
-                'lambda_l2': trial.suggest_float('lambda_l2', 1e-8, 10.0, log=True),
-                'num_leaves': trial.suggest_int('num_leaves', 2, 256),
-                'feature_fraction': trial.suggest_float('feature_fraction', 0.4, 1.0),
-                'bagging_fraction': trial.suggest_float('bagging_fraction', 0.4, 1.0),
-                'bagging_freq': trial.suggest_int('bagging_freq', 1, 7),
-                'min_child_samples': trial.suggest_int('min_child_samples', 5, 100),
-            }
+            "learning_rate": trial.suggest_float("learning_rate", 1e-2, 0.25, log=True),
+            "max_depth": trial.suggest_int("max_depth", 1, 9),
+            "early_stopping_rounds": trial.suggest_int(
+                "early_stopping_rounds", 100, 500
+            ),
+            "n_estimators": trial.suggest_categorical(
+                "n_estimators", [7000, 15000, 20000]
+            ),
+            "lambda_l1": trial.suggest_float("lambda_l1", 1e-8, 10.0, log=True),
+            "lambda_l2": trial.suggest_float("lambda_l2", 1e-8, 10.0, log=True),
+            "num_leaves": trial.suggest_int("num_leaves", 2, 256),
+            "feature_fraction": trial.suggest_float("feature_fraction", 0.4, 1.0),
+            "bagging_fraction": trial.suggest_float("bagging_fraction", 0.4, 1.0),
+            "bagging_freq": trial.suggest_int("bagging_freq", 1, 7),
+            "min_child_samples": trial.suggest_int("min_child_samples", 5, 100),
+        }
     else:
         raise NotImplementedError
 
     return params
```

### Comparing `nexora-0.0.1/src/nexora/predict.py` & `nexora-0.0.2/nexora/predict.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,19 +18,26 @@
 
 @dataclass
 class AutoTunaPredict:
     model_path: str
 
     def __post_init__(self):
         self.model_config = joblib.load(os.path.join(self.model_path, "atuna.config"))
-        self.target_encoder = joblib.load(os.path.join(self.model_path, "atuna.target_encoder"))
-        self.categorical_encoders = joblib.load(os.path.join(self.model_path, "atuna.categorical_encoders"))
+        self.target_encoder = joblib.load(
+            os.path.join(self.model_path, "atuna.target_encoder")
+        )
+        self.categorical_encoders = joblib.load(
+            os.path.join(self.model_path, "atuna.categorical_encoders")
+        )
+        with open(os.path.join(self.model_path, "selected_features.json"), "r") as f:
+            self.selected_features = list(json.load(f).keys())
+
         self.models = []
         for fold in range(self.model_config.num_folds):
-            model_ = joblib.load(os.path.join(self.model_path, f"atuna.{fold}"))
+            model_ = joblib.load(os.path.join(self.model_path, f"atuna_model.{fold}"))
             self.models.append(model_)
 
         _, self.use_predict_proba, _, _ = fetch_model_params(self.model_config)
 
     # TODO: improve schema with optional null values
     def get_prediction_schema(self):
         cat_features = self.model_config.categorical_features
@@ -47,52 +54,68 @@
         categorical_features = self.model_config.categorical_features
         final_preds = []
         test_ids = df[self.model_config.idx].values
         for fold in range(self.model_config.num_folds):
             fold_test = df.copy(deep=True)
             if len(categorical_features) > 0:
                 categorical_encoder = self.categorical_encoders[fold]
-                fold_test[categorical_features] = categorical_encoder.transform(fold_test[categorical_features].values)
+                fold_test[categorical_features] = categorical_encoder.transform(
+                    fold_test[categorical_features].values
+                )
 
-            test_features = fold_test[self.model_config.features]
+            # test_features = fold_test[self.model_config.features]
+            test_features = fold_test[self.selected_features]
 
             for col in test_features.columns:
                 if test_features[col].dtype == "object":
                     test_features[col] = test_features[col].astype(np.int64)
 
             if self.model_config.problem_type in (
                 ProblemType.multi_column_regression,
                 ProblemType.multi_label_classification,
             ):
                 test_preds_mll = []
                 for midx in range(len(self.models[fold])):
-                    if self.model_config.problem_type == ProblemType.multi_column_regression:
+                    if (
+                        self.model_config.problem_type
+                        == ProblemType.multi_column_regression
+                    ):
                         test_pred_temp = self.models[fold][midx].predict(test_features)
                     else:
-                        test_pred_temp = self.models[fold][midx].predict_proba(test_features)[:, 1]
+                        test_pred_temp = self.models[fold][midx].predict_proba(
+                            test_features
+                        )[:, 1]
                     test_preds_mll.append(test_pred_temp)
 
                 test_preds = np.column_stack(test_preds_mll)
             else:
                 if self.use_predict_proba:
                     test_preds = self.models[fold].predict_proba(test_features)
                 else:
                     test_preds = self.models[fold].predict(test_features)
 
             final_preds.append(test_preds)
 
         final_preds = np.mean(final_preds, axis=0)
         if self.target_encoder is None:
-            final_preds = pd.DataFrame(final_preds, columns=self.model_config.target_cols)
+            final_preds = pd.DataFrame(
+                final_preds, columns=self.model_config.target_cols
+            )
         else:
-            final_preds = pd.DataFrame(final_preds, columns=list(self.target_encoder.classes_))
+            final_preds = pd.DataFrame(
+                final_preds, columns=list(self.target_encoder.classes_)
+            )
         final_preds.insert(loc=0, column=self.model_config.idx, value=test_ids)
         return final_preds
 
-    def predict_single(self, sample: Dict[str, Union[str, int, float]] = None, fast_predict: bool = True):
+    def predict_single(
+        self,
+        sample: Dict[str, Union[str, int, float]] = None,
+        fast_predict: bool = True,
+    ):
         sample = json.loads(sample)
         sample_df = pd.DataFrame.from_dict(sample, orient="index").T
         sample_df[self.model_config.idx] = 0
         preds = self._predict_df(sample_df)
         preds = preds.to_dict(orient="records")[0]
         return preds
```

### Comparing `nexora-0.0.1/src/nexora/utils.py` & `nexora-0.0.2/nexora/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,32 +4,31 @@
 
 import joblib
 import numpy as np
 import optuna
 import pandas as pd
 import xgboost as xgb
 import lightgbm as lgbm
-import shap
 from sklearn.ensemble import RandomForestClassifier
 
-from .enums import ProblemType, Algo
+from .enums import ProblemType, Algo, Objective
 from .logger import logger
 from .metrics import Metrics
 from .params import get_params
 from .boruta import BorutaPy
 
 
 optuna.logging.set_verbosity(optuna.logging.INFO)
 
 
 def reduce_memory_usage(df, verbose=True):
     # NOTE: Original author of this function is unknown
     # if you know the *original author*, please let me know.
     numerics = ["int8", "int16", "int32", "int64", "float16", "float32", "float64"]
-    start_mem = df.memory_usage().sum() / 1024 ** 2
+    start_mem = df.memory_usage().sum() / 1024**2
     for col in df.columns:
         col_type = df[col].dtypes
         if col_type in numerics:
             c_min = df[col].min()
             c_max = df[col].max()
             if str(col_type)[:3] == "int":
                 if c_min > np.iinfo(np.int8).min and c_max < np.iinfo(np.int8).max:
@@ -37,21 +36,27 @@
                 elif c_min > np.iinfo(np.int16).min and c_max < np.iinfo(np.int16).max:
                     df[col] = df[col].astype(np.int16)
                 elif c_min > np.iinfo(np.int32).min and c_max < np.iinfo(np.int32).max:
                     df[col] = df[col].astype(np.int32)
                 elif c_min > np.iinfo(np.int64).min and c_max < np.iinfo(np.int64).max:
                     df[col] = df[col].astype(np.int64)
             else:
-                if c_min > np.finfo(np.float16).min and c_max < np.finfo(np.float16).max:
+                if (
+                    c_min > np.finfo(np.float16).min
+                    and c_max < np.finfo(np.float16).max
+                ):
                     df[col] = df[col].astype(np.float16)
-                elif c_min > np.finfo(np.float32).min and c_max < np.finfo(np.float32).max:
+                elif (
+                    c_min > np.finfo(np.float32).min
+                    and c_max < np.finfo(np.float32).max
+                ):
                     df[col] = df[col].astype(np.float32)
                 else:
                     df[col] = df[col].astype(np.float64)
-    end_mem = df.memory_usage().sum() / 1024 ** 2
+    end_mem = df.memory_usage().sum() / 1024**2
     if verbose:
         logger.info(
             "Mem. usage decreased to {:.2f} Mb ({:.1f}% reduction)".format(
                 end_mem, 100 * (start_mem - end_mem) / start_mem
             )
         )
     return df
@@ -60,74 +65,126 @@
 def dict_mean(dict_list):
     mean_dict = {}
     for key in dict_list[0].keys():
         mean_dict[key] = sum(d[key] for d in dict_list) / len(dict_list)
     return mean_dict
 
 
-def save_valid_predictions(final_valid_predictions, model_config, target_encoder, output_file_name):
-    final_valid_predictions = pd.DataFrame.from_dict(final_valid_predictions, orient="index").reset_index()
+def save_valid_predictions(
+    final_valid_predictions, model_config, target_encoder, output_file_name
+):
+    final_valid_predictions = pd.DataFrame.from_dict(
+        final_valid_predictions, orient="index"
+    ).reset_index()
     if target_encoder is None:
         final_valid_predictions.columns = [model_config.idx] + model_config.targets
     else:
-        final_valid_predictions.columns = [model_config.idx] + list(target_encoder.classes_)
+        final_valid_predictions.columns = [model_config.idx] + list(
+            target_encoder.classes_
+        )
 
     final_valid_predictions.to_csv(
         os.path.join(model_config.output, output_file_name),
         index=False,
     )
 
 
-def save_test_predictions(final_test_predictions, model_config, target_encoder, test_ids, output_file_name):
+def save_test_predictions(
+    final_test_predictions, model_config, target_encoder, test_ids, output_file_name
+):
     final_test_predictions = np.mean(final_test_predictions, axis=0)
     if target_encoder is None:
-        final_test_predictions = pd.DataFrame(final_test_predictions, columns=model_config.targets)
+        final_test_predictions = pd.DataFrame(
+            final_test_predictions, columns=model_config.targets
+        )
     else:
-        final_test_predictions = pd.DataFrame(final_test_predictions, columns=list(target_encoder.classes_))
+        final_test_predictions = pd.DataFrame(
+            final_test_predictions, columns=list(target_encoder.classes_)
+        )
     final_test_predictions.insert(loc=0, column=model_config.idx, value=test_ids)
     final_test_predictions.to_csv(
         os.path.join(model_config.output, output_file_name),
         index=False,
     )
 
 
 def fetch_model_params(model_config):
     if model_config.problem_type == ProblemType.binary_classification:
-        if model_config.algo == Algo.xgb.value:
-            tree_model = xgb.XGBClassifier
-            eval_metric = "logloss"
-        elif model_config.algo == Algo.lgbm.value:
-            tree_model = lgbm.LGBMClassifier
-            eval_metric = "binary_logloss"
+        if model_config.objective == Objective.loss.value:
+            if model_config.algo == Algo.xgb.value:
+                tree_model = xgb.XGBClassifier
+                eval_metric = "logloss"
+            elif model_config.algo == Algo.lgbm.value:
+                tree_model = lgbm.LGBMClassifier
+                eval_metric = "binary_logloss"
+            else:
+                raise NotImplementedError
+            use_predict_proba = True
+            direction = "minimize"
+        elif model_config.objective == Objective.accuracy.value:
+            if model_config.algo == Algo.xgb.value:
+                tree_model = xgb.XGBClassifier
+                eval_metric = "accuracy"
+            elif model_config.algo == Algo.lgbm.value:
+                tree_model = lgbm.LGBMClassifier
+                eval_metric = "accuracy"
+            else:
+                raise NotImplementedError
+            direction = "maximize"
         else:
             raise NotImplementedError
-        use_predict_proba = True
-        direction = "minimize"
     elif model_config.problem_type == ProblemType.multi_class_classification:
-        if model_config.algo == Algo.xgb.value:
-            tree_model = xgb.XGBClassifier
-            eval_metric = "mlogloss"
-        elif model_config.algo == Algo.lgbm.value:
-            tree_model = lgbm.LGBMClassifier
-            eval_metric = "multi_logloss"
+        if model_config.objective == Objective.loss.value:
+            if model_config.algo == Algo.xgb.value:
+                tree_model = xgb.XGBClassifier
+                eval_metric = "mlogloss"
+            elif model_config.algo == Algo.lgbm.value:
+                tree_model = lgbm.LGBMClassifier
+                eval_metric = "multi_logloss"
+            else:
+                raise NotImplementedError
+            use_predict_proba = True
+            direction = "minimize"
+        elif model_config.objective == Objective.accuracy.value:
+            if model_config.algo == Algo.xgb.value:
+                tree_model = xgb.XGBClassifier
+                eval_metric = "accuracy"
+            elif model_config.algo == Algo.lgbm.value:
+                tree_model = lgbm.LGBMClassifier
+                eval_metric = "accuracy"
+            else:
+                raise NotImplementedError
+            direction = "maximize"
         else:
             raise NotImplementedError
-        use_predict_proba = True
-        direction = "minimize"
     elif model_config.problem_type == ProblemType.multi_label_classification:
-        if model_config.algo == Algo.xgb.value:
-            tree_model = xgb.XGBClassifier
-            eval_metric = "logloss"
-        elif model_config.algo == Algo.lgbm.value:
-            tree_model = lgbm.LGBMClassifier
-            eval_metric = "binary_logloss"
+        if model_config.objective == Objective.loss.value:
+            if model_config.algo == Algo.xgb.value:
+                tree_model = xgb.XGBClassifier
+                eval_metric = "logloss"
+            elif model_config.algo == Algo.lgbm.value:
+                tree_model = lgbm.LGBMClassifier
+                eval_metric = "binary_logloss"
+            else:
+                raise NotImplementedError
+            use_predict_proba = True
+            direction = "minimize"
+        elif model_config.objective == Objective.accuracy.value:
+            if model_config.algo == Algo.xgb.value:
+                tree_model = xgb.XGBClassifier
+                eval_metric = "accuracy"
+            elif model_config.algo == Algo.lgbm.value:
+                tree_model = lgbm.LGBMClassifier
+                eval_metric = "accuracy"
+            else:
+                raise NotImplementedError
+            use_predict_proba = True
+            direction = "maximize"
         else:
             raise NotImplementedError
-        use_predict_proba = True
-        direction = "minimize"
     elif model_config.problem_type == ProblemType.single_column_regression:
         if model_config.algo == Algo.xgb.value:
             tree_model = xgb.XGBRegressor
         elif model_config.algo == Algo.lgbm.value:
             tree_model = lgbm.LGBMRegressor
         else:
             raise NotImplementedError
@@ -162,31 +219,38 @@
     del params["early_stopping_rounds"]
 
     metrics = Metrics(model_config.problem_type, model_config.algo)
 
     scores = []
 
     for fold in range(model_config.num_folds):
-        train_feather = pd.read_feather(os.path.join(model_config.output, f"train_fold_{fold}.feather"))
-        valid_feather = pd.read_feather(os.path.join(model_config.output, f"valid_fold_{fold}.feather"))
+        train_feather = pd.read_feather(
+            os.path.join(model_config.output, f"train_fold_{fold}.feather")
+        )
+        valid_feather = pd.read_feather(
+            os.path.join(model_config.output, f"valid_fold_{fold}.feather")
+        )
         xtrain = train_feather[model_config.features]
         xvalid = valid_feather[model_config.features]
 
         ytrain = train_feather[model_config.targets].values
         yvalid = valid_feather[model_config.targets].values
 
         # train model
         model = tree_model(
             random_state=model_config.seed,
             eval_metric=eval_metric,
             use_label_encoder=False,
             **params,
         )
 
-        if model_config.problem_type in (ProblemType.multi_column_regression, ProblemType.multi_label_classification):
+        if model_config.problem_type in (
+            ProblemType.multi_column_regression,
+            ProblemType.multi_label_classification,
+        ):
             ypred = []
             models = [model] * len(model_config.targets)
             for idx, _m in enumerate(models):
                 _m.fit(
                     xtrain,
                     ytrain[:, idx],
                     early_stopping_rounds=early_stopping_rounds,
@@ -222,15 +286,17 @@
 
     mean_metrics = dict_mean(scores)
     logger.info(f"Metrics: {mean_metrics}")
     return mean_metrics[eval_metric]
 
 
 def train_model(model_config):
-    tree_model, use_predict_proba, eval_metric, direction = fetch_model_params(model_config)
+    tree_model, use_predict_proba, eval_metric, direction = fetch_model_params(
+        model_config
+    )
 
     optimize_func = partial(
         optimize,
         tree_model=tree_model,
         use_predict_proba=use_predict_proba,
         eval_metric=eval_metric,
         model_config=model_config,
@@ -238,27 +304,29 @@
     db_path = os.path.join(model_config.output, "params.db")
     study = optuna.create_study(
         direction=direction,
         study_name="autotuna",
         storage=f"sqlite:///{db_path}",
         load_if_exists=True,
     )
-    
-    logger.info('======================================================')
-    logger.info('|                                                    |')
-    logger.info('|                                                    |')
-    logger.info('|  Monitor the study                                 |')
-    logger.info('| Run the following command under the output folder: |')
-    logger.info(f'| cd  {db_path}                                     |')
-    logger.info('| optuna-dashboard sqlite:///params.db               |')
-    logger.info('|                                                    |')
-    logger.info('|                                                    |')
-    logger.info('======================================================')
 
-    study.optimize(optimize_func, n_trials=model_config.num_trials, timeout=model_config.time_limit)
+    logger.info("======================================================")
+    logger.info("|                                                    |")
+    logger.info("|                                                    |")
+    logger.info("|  Monitor the study                                 |")
+    logger.info("| Run the following command under the output folder: |")
+    logger.info(f"| cd  {db_path}                                     |")
+    logger.info("| optuna-dashboard sqlite:///params.db               |")
+    logger.info("|                                                    |")
+    logger.info("|                                                    |")
+    logger.info("======================================================")
+
+    study.optimize(
+        optimize_func, n_trials=model_config.num_trials, timeout=model_config.time_limit
+    )
     return study.best_params
 
 
 def predict_model(model_config, best_params):
 
     early_stopping_rounds = best_params["early_stopping_rounds"]
     del best_params["early_stopping_rounds"]
@@ -276,38 +344,47 @@
     final_test_predictions = []
     final_valid_predictions = {}
 
     target_encoder = joblib.load(f"{model_config.output}/atuna.target_encoder")
 
     for fold in range(model_config.num_folds):
         logger.info(f"Training and predicting for fold {fold}")
-        train_feather = pd.read_feather(os.path.join(model_config.output, f"train_fold_{fold}.feather"))
-        valid_feather = pd.read_feather(os.path.join(model_config.output, f"valid_fold_{fold}.feather"))
+        train_feather = pd.read_feather(
+            os.path.join(model_config.output, f"train_fold_{fold}.feather")
+        )
+        valid_feather = pd.read_feather(
+            os.path.join(model_config.output, f"valid_fold_{fold}.feather")
+        )
 
         xtrain = train_feather[model_config.features]
         xvalid = valid_feather[model_config.features]
 
         valid_ids = valid_feather[model_config.idx].values
 
         if model_config.test_filename is not None:
-            test_feather = pd.read_feather(os.path.join(model_config.output, f"test_fold_{fold}.feather"))
+            test_feather = pd.read_feather(
+                os.path.join(model_config.output, f"test_fold_{fold}.feather")
+            )
             xtest = test_feather[model_config.features]
             test_ids = test_feather[model_config.idx].values
 
         ytrain = train_feather[model_config.targets].values
         yvalid = valid_feather[model_config.targets].values
 
         model = tree_model(
             random_state=model_config.seed,
             eval_metric=eval_metric,
             use_label_encoder=False,
             **best_params,
         )
 
-        if model_config.problem_type in (ProblemType.multi_column_regression, ProblemType.multi_label_classification):
+        if model_config.problem_type in (
+            ProblemType.multi_column_regression,
+            ProblemType.multi_label_classification,
+        ):
             ypred = []
             test_pred = []
             trained_models = []
             for idx in range(len(model_config.targets)):
                 _m = copy.deepcopy(model)
                 _m.fit(
                     xtrain,
@@ -374,43 +451,60 @@
         # calculate metric
         metric_dict = metrics.calculate(yvalid, ypred)
         scores.append(metric_dict)
         logger.info(f"Fold {fold} done!")
 
     mean_metrics = dict_mean(scores)
     logger.info(f"Metrics: {mean_metrics}")
-    save_valid_predictions(final_valid_predictions, model_config, target_encoder, "oof_predictions.csv")
+    save_valid_predictions(
+        final_valid_predictions, model_config, target_encoder, "oof_predictions.csv"
+    )
 
     if model_config.test_filename is not None:
-        save_test_predictions(final_test_predictions, model_config, target_encoder, test_ids, "test_predictions.csv")
+        save_test_predictions(
+            final_test_predictions,
+            model_config,
+            target_encoder,
+            test_ids,
+            "test_predictions.csv",
+        )
     else:
         logger.info("No test data supplied. Only OOF predictions were generated")
 
 
 def select_features(model_config, fold=0, seed=0):
 
-    train_feather = pd.read_feather(os.path.join(model_config.output, f"train_fold_{fold}.feather"))
-    valid_feather = pd.read_feather(os.path.join(model_config.output, f"valid_fold_{fold}.feather"))
- 
-    x = pd.concat([train_feather[model_config.features], valid_feather[model_config.features]])
-    y = pd.concat([train_feather[model_config.targets], valid_feather[model_config.targets]])
-    if model_config.problem_type in [ProblemType.binary_classification, ProblemType.multi_class_classification]:
-        model = RandomForestClassifier(n_jobs=-1, class_weight=None, max_depth=7, random_state=seed)
+    train_feather = pd.read_feather(
+        os.path.join(model_config.output, f"train_fold_{fold}.feather")
+    )
+    valid_feather = pd.read_feather(
+        os.path.join(model_config.output, f"valid_fold_{fold}.feather")
+    )
+
+    x = pd.concat(
+        [train_feather[model_config.features], valid_feather[model_config.features]]
+    )
+    y = pd.concat(
+        [train_feather[model_config.targets], valid_feather[model_config.targets]]
+    )
+    if model_config.problem_type in [
+        ProblemType.binary_classification,
+        ProblemType.multi_class_classification,
+    ]:
+        model = RandomForestClassifier(
+            n_jobs=-1, class_weight=None, max_depth=7, random_state=seed
+        )
     elif model_config.problem_type in [ProblemType.multi_column_regression]:
         model = xgb.XGBRegressor(seed=seed)
     else:
         raise NotImplementedError
 
-    feat_selector = BorutaPy(model, n_estimators='auto', verbose=2, random_state=seed)
+    feat_selector = BorutaPy(model, n_estimators="auto", verbose=2, random_state=seed)
     feat_selector.fit(x.values, y.values)
     selected_features = x.columns[feat_selector.support_]
-    joblib.dump(feat_selector, 
-                os.path.join(
-                        model_config.output, 
-                        'feature_selector.joblib')
+    joblib.dump(
+        feat_selector, os.path.join(model_config.output, "atuna.feature_selection")
     )
-    # selected = x.values[:, feat_selector.support_]
-    logger.info('Feature selection is done, selected features:')
+    # selected = x.values[:, feat_selector.support_]
+    logger.info("Feature selection is done, selected features:")
     logger.info(selected_features)
     return selected_features
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

