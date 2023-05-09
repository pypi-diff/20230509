# Comparing `tmp/mercury-robust-0.0.1.tar.gz` & `tmp/mercury-robust-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-robust-0.0.1.tar", last modified: Mon Apr  3 15:10:08 2023, max compression
+gzip compressed data, was "mercury-robust-0.0.2.tar", last modified: Tue May  9 09:01:08 2023, max compression
```

## Comparing `mercury-robust-0.0.1.tar` & `mercury-robust-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:10:08.045032 mercury-robust-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-03 15:10:08.045032 mercury-robust-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:10:08.037032 mercury-robust-0.0.1/mercury/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:10:08.041032 mercury-robust-0.0.1/mercury/robust/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/_base_batch_drift_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/_category_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/_chi2_drift_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/_drift_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/_histogram_distance_drift_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/_label_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/_linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/_tree_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/_treeselector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/basetests.py
--rw-r--r--   0 runner    (1001) docker     (123)    50428 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/data_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    50006 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/model_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/mercury/robust/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:10:08.041032 mercury-robust-0.0.1/mercury_robust.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-03 15:10:08.000000 mercury-robust-0.0.1/mercury_robust.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-03 15:10:08.000000 mercury-robust-0.0.1/mercury_robust.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 15:10:08.000000 mercury-robust-0.0.1/mercury_robust.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-03 15:10:08.000000 mercury-robust-0.0.1/mercury_robust.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-03 15:10:08.000000 mercury-robust-0.0.1/mercury_robust.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 15:10:08.045032 mercury-robust-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:10:08.045032 mercury-robust-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/tests/test_basetests.py
--rw-r--r--   0 runner    (1001) docker     (123)    28586 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/tests/test_data_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    33015 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/tests/test_model_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-03 15:09:54.000000 mercury-robust-0.0.1/tests/test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:01:08.467048 mercury-robust-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-09 09:01:08.467048 mercury-robust-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:01:08.463048 mercury-robust-0.0.2/mercury/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:01:08.463048 mercury-robust-0.0.2/mercury/robust/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/_category_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/_label_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/_tree_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/_treeselector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/basetests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50444 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/data_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59316 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/model_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:01:08.467048 mercury-robust-0.0.2/mercury_robust.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-09 09:01:08.000000 mercury-robust-0.0.2/mercury_robust.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-09 09:01:08.000000 mercury-robust-0.0.2/mercury_robust.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:01:08.000000 mercury-robust-0.0.2/mercury_robust.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 09:01:08.000000 mercury-robust-0.0.2/mercury_robust.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 09:01:08.000000 mercury-robust-0.0.2/mercury_robust.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:01:08.467048 mercury-robust-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:01:08.467048 mercury-robust-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/tests/test_basetests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28586 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/tests/test_data_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35938 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/tests/test_model_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/tests/test_suite.py
```

### Comparing `mercury-robust-0.0.1/LICENSE` & `mercury-robust-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.1/mercury/robust/_category_struct.py` & `mercury-robust-0.0.2/mercury/robust/_category_struct.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.1/mercury/robust/_label_cleaning.py` & `mercury-robust-0.0.2/mercury/robust/_label_cleaning.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.1/mercury/robust/_linalg.py` & `mercury-robust-0.0.2/mercury/robust/_linalg.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.1/mercury/robust/_tree_analysis.py` & `mercury-robust-0.0.2/mercury/robust/_tree_analysis.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.1/mercury/robust/_treeselector.py` & `mercury-robust-0.0.2/mercury/robust/_treeselector.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.1/mercury/robust/basetests.py` & `mercury-robust-0.0.2/mercury/robust/basetests.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.1/mercury/robust/data_tests.py` & `mercury-robust-0.0.2/mercury/robust/data_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,16 +217,16 @@
     def run(self, *args, **kwargs):
         """
         Runs the test.
 
         Raises:
             FailedTestError if any drift is detected
         """
-        from mercury.robust._histogram_distance_drift_detector import HistogramDistanceDrift
-        from mercury.robust._chi2_drift_detector import Chi2Drift
+        from mercury.monitoring.drift.histogram_distance_drift_detector import HistogramDistanceDrift
+        from mercury.monitoring.drift.chi2_drift_detector import Chi2Drift
 
         super().run(*args, **kwargs)
 
         schema_ref = self.schema_ref
 
         # Test numerical features with HistogramDistance
         featnames = schema_ref.continuous_feats + schema_ref.discrete_feats
@@ -586,15 +586,15 @@
         threshold (float): threshold to specify the percentage of noisy labels from which the test will fail. Default value is 0.4
         text_col (str): column containing the text. Only has to be specified when using a text dataset.
         preprocessor (Union[TransformerMixin, BaseEstimator]): Optional preprocessor for the features. If not specified, it will
             create a preprocessor with OneHotEncoder to encode categorical features in case of tabular data
             (text_col not specified) or a CountVectorizer to encode text in case of a text dataset(text_col specified)
         ignore_feats (List[str]): features that will not be used in the algorithm to detect noisy labels.
         calculate_idx_issues (bool): whether to calculate also the index of samples with label issues. If True, the idx will be
-            available in `idx_issues_` attribute. Default value is False.
+            available in `idx_issues_` attribute. Default value is True.
         label_issues_args (dict): arguments for the algorithm to detect noisy labels. You can check documentation from
             `_label_cleaning.get_label_issues` to see all available arguments.
         schema_custom_feature_map: Internally, this test generates a DataSchema object. In case you find it makes
                                    wrong feature type assignations to your features you can pass here a dictionary which
                                    specify the feature type of the columns you want to fix. (See DataSchema. `force_types`
                                    parameter for more info on this).
         dataset_schema: Pre built schema. This argument is complementary to `schema_custom_feature_map`. In case you want to
@@ -624,15 +624,15 @@
     def __init__(self,
                  base_dataset: "pandas.DataFrame",  # noqa: F821
                  label_name: str,
                  threshold: float = None,
                  text_col: str = None,
                  preprocessor: Union["TransformerMixin", "BaseEstimator"] = None,  # noqa: F821
                  ignore_feats: List[str] = None,
-                 calculate_idx_issues: bool = False,
+                 calculate_idx_issues: bool = True,
                  label_issues_args: dict = None,
                  name: str = None,
                  schema_custom_feature_map: Dict[str, FeatType] = None,
                  dataset_schema: DataSchema = None,
                  *args: Any, **kwargs: Any):
         super().__init__(base_dataset, name, *args, **kwargs)
```

### Comparing `mercury-robust-0.0.1/mercury/robust/model_tests.py` & `mercury-robust-0.0.2/mercury/robust/model_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import warnings
 import numpy as np
 import pandas as pd
 import sklearn
 from sklearn.pipeline import Pipeline
 from sklearn.compose import ColumnTransformer
 from sklearn.preprocessing import OneHotEncoder, StandardScaler
 from sklearn.linear_model import LogisticRegression, LinearRegression
@@ -13,15 +12,15 @@
 import copy
 from typing import Union, Callable, List, Dict
 from mercury.robust.basetests import RobustModelTest, TaskInferrer
 from mercury.robust.errors import FailedTestError
 
 from mercury.dataschema.feature import FeatType
 from mercury.dataschema import DataSchema
-from ._drift_simulation import BatchDriftGenerator
+from mercury.monitoring.drift.drift_simulation import BatchDriftGenerator
 from ._tree_analysis import SkLearnTreeCoverageAnalyzer, SkLearnTreeEnsembleCoverageAnalyzer
 
 
 
 class ModelReproducibilityTest(RobustModelTest):
     """
     This test checks if the training of a model is reproducible. It does so by training the model two times
@@ -903,14 +902,15 @@
 
     Example:
         ```python
         >>> testing_dataset = pd.DataFrame(...)
         >>> rf = RandomForestClassifier().fit(train_data)
         >>> test = TreeCoverageTest(
         ...    rf,
+        ...    testing_dataset,
         ...    threshold_coverage=.8
         ...    name="My Tree Coverage Test"
         ... )
         >>> test.run()  # The test will fail if the obtained coverage is less than 80%
         ```
     """
 
@@ -968,8 +968,215 @@
         coverage = self._analyzer.get_percent_coverage()
         self.coverage = coverage
 
         if coverage < self.threshold_coverage:
             raise FailedTestError(f"Achieved a coverage of {coverage} while the minimum required was {self.threshold_coverage}")
 
     def info(self) -> dict:
-        return {'coverage': self.coverage}
+        return {'coverage': self.coverage}
+    
+class FeatureCheckerTest(RobustModelTest):
+    """
+    This model robustness test checks if training the models using less columns in the dataframe can achieve identical results.
+    To do so, it uses the variable importance taken from the model itself or estimated using a mercury.explainability explainer
+    (ShuffleImportanceExplainer). It does a small number of attempts at removing unimportant variables and "fails if it succeeds",
+    since success implies that a smaller, therefore more efficient, dataset should be used instead. The purpose of this test is
+    not to find that optimal dataset. That can be achieved by removing the columns identified as unimportant and iterating.
+
+    **NOTE**: This class will retrain (fit) the model several times resulting in the model being altered as a side effect. Make
+    copies of your model before using this tool. This tool is intended as a diagnostic tool.
+
+    Args:
+        model: The model being evaluated. The model is assumed to comply to a minimalistic sklearn-like interface. More precisely:
+            1. It must have a fit() method that works on the dataset and the dataset with some columns removed. It is important that each
+            time the method fit() is called the model is trained from scratch (ie does not perform incremental training).
+            2. It must have a predict() method that works on the dataset and returns a vector that is accepted by the evaluation function.
+            3. If the argument `importance` is used, it must have an attribute with that name containing a list of (value, column_name)
+            tuples which is consistent with many sklearn models.
+            Alternatively, you can provide a function that creates a model or pipeline. This is useful in models or pipelines where
+            removing columns from a dataframe raises an error because it expects the removed column. In this case, the interface of
+            the function is model_fn(dataframe, model_args), where dataframe is the input pandas dataframe with the features already
+            removed and model_fn_args is a dictionary with optional parameters that can be passed to the function. Importantly,
+            this function just needs to create the model (unfitted) instance, but not to perform the training
+        model_fn_args: if you are using a function in `model` parameter, you can use this argument to provide arguments to that function.
+        train: The pandas dataset used for training the model, possibly with some columns removed.
+        target: The name of the target variable predicted by the model which must be one columns in the train dataset.
+        test: If given, a separate dataset with identical column structure used for the evaluation parts. Otherwise, the train dataset
+            will be used instead.
+        importance: If given, the name of a property in the model is updated by a fit() call. It must contain the importance of the
+            columns as a list of (value, column_name) tuples. Otherwise, the importance of the variables will be estimated using a
+            mercury.explainer ShuffleImportanceExplainer.
+        eval: If given, an evaluation function that defines what "identical" results are. The function must accept two vectors returned
+            by model.predict() and return some positive value that is smaller than `tolerance` if "identical". Otherwise a sum of squared
+            differences will be used instead.
+        tolerance: A real value to be compared with the result of the evaluation function. Note that the purpose of the test is finding
+            unimportant variables. Therefore, the test will fail when the result (named as `loss`) is smaller than the tolerance, meaning
+            the model could work "identically" well with less variables. When the test fails, you can see the value returned by the `eval`
+            function in the RuntimeError message displayed as `loss`.
+        num_tries: The total number of column removal tries the test should do before passing. This value times `remove_num` must be
+            smaller than the number of columns (Y excluded).
+        remove_num: The number of columns removed at each try.
+        name: A name for the test. If not used, it will take the name of the class.
+
+    Example:
+        ```python
+        >>> from mercury.robust.model_tests import FeatureCheckerTest
+        >>> test = FeatureCheckerTest(
+        >>>     model=model,
+        >>>     train=df_train,
+        >>>     target="label_col",
+        >>>     test=df_test,
+        >>>     num_tries=len(df_train.columns)-1,
+        >>>     remove_num=1,
+        >>>     tolerance=len(df_test)*0.01
+        >>> )
+        >>> test.run()
+        ```
+    """
+
+    def __init__(
+        self,
+        model: Union["Estimator", Callable],  # noqa: F821
+        train: pd.DataFrame,
+        target: str,
+        test: pd.DataFrame = None,
+        model_fn_args: dict = None,
+        importance: str = None,
+        eval: Callable = None,
+        tolerance: float = 1e-3,
+        num_tries: int = 3,
+        remove_num: int = 1,
+        name: str = None
+    ):
+        super().__init__(model, name)
+        self.model_fn_args = model_fn_args
+        self.train = train
+        self.target = target
+        self.test = test if test is not None else train
+        self.importance = importance
+        self.eval = eval
+        self.remove_num = remove_num
+        self.num_tries = num_tries
+        self.tolerance = tolerance
+        self.losses = {}
+
+    def info(self):
+        return self.losses
+
+    def _get_least_important(self, N):
+
+        names = []
+
+        if self.importance is None:
+
+            try:
+                from mercury.explainability.explainers import ShuffleImportanceExplainer
+            except:
+                raise ImportError(
+                    'Install mercury-explainability to use the FeatureCheckerTest with this type of model'
+                )
+
+            def model_inference_function(data, target):
+                assert target == self.target
+
+                X = data.loc[:, data.columns != self.target]
+                Y = data.loc[:, self.target]
+                Yh = self.fitted_model.predict(X)
+
+                if self.eval is None:
+                    return sum((Y - Yh) ** 2)
+
+                return self.eval(Y, Yh)
+
+            explainer = ShuffleImportanceExplainer(model_inference_function)
+
+            explanation = explainer.explain(self.test, target=self.target)
+
+            for name, _ in sorted(explanation.get_importances(), key=lambda x: x[1]):
+                names.append(name)
+                N -= 1
+                if N == 0:
+                    break
+
+            return names
+
+        try:
+            importance = getattr(self.model, self.importance)
+
+        except AttributeError:
+            return names
+
+        finally:
+            columns = self.test.columns[self.test.columns != self.target]
+            if len(columns) != len(importance):
+                return names
+
+            for _, name in sorted(zip(importance, columns)):
+                names.append(name)
+                N -= 1
+                if N == 0:
+                    break
+
+            return names
+
+    def run(self, *args, **kwargs):
+        """
+        Runs the test.
+
+        Raises:
+            `FailedTestError` with a descriptive message if any of the attempts fail.
+        """
+
+        super().run(*args, **kwargs)
+
+        N = self.remove_num * self.num_tries
+
+        X_train = self.train.loc[:, self.train.columns != self.target]
+        Y_train = self.train.loc[:, self.target]
+
+        # Fit model with all the features
+        self._fit_model(X_train, Y_train)
+
+        X_test = self.test.loc[:, self.test.columns != self.target]
+        Y_hat = self.fitted_model.predict(X_test)
+
+        remove = self._get_least_important(N)
+
+        if len(remove) != N:
+            raise RuntimeError(
+                "Wrong arguments. Not enough columns for remove_num*num_tries."
+            )
+
+        for t in range(self.num_tries):
+            exclude = remove[0:self.remove_num]
+            remove = remove[self.remove_num:]
+
+            exclude.append(self.target)
+
+            x_cols = [c for c in self.train.columns if c not in exclude]
+
+            X_alt_train = self.train.loc[:, x_cols]
+
+            # Fit model with the removed features
+            self._fit_model(X_alt_train, Y_train)
+
+            X_alt_test = self.test.loc[:, x_cols]
+            Y_alt_hat = self.fitted_model.predict(X_alt_test)
+
+            if self.eval is None:
+                loss = sum((Y_hat - Y_alt_hat) ** 2)
+            else:
+                loss = self.eval(Y_hat, Y_alt_hat)
+            self.losses[", ".join(exclude[:-1])] = loss
+
+            if loss < self.tolerance:
+                raise FailedTestError(
+                    "Test failed. A model fitted removing columns [%s] is identical within tolerance %.3f (loss = %.3f)"
+                    % (", ".join(exclude[:-1]), self.tolerance, loss)
+                )
+
+    def _fit_model(self, X, Y):
+        if callable(self.model):
+            self.fitted_model = self.model(X, self.model_fn_args)
+            self.fitted_model.fit(X, Y)
+        else:
+            self.fitted_model = self.model.fit(X, Y)
```

### Comparing `mercury-robust-0.0.1/mercury/robust/suite.py` & `mercury-robust-0.0.2/mercury/robust/suite.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.1/mercury_robust.egg-info/SOURCES.txt` & `mercury-robust-0.0.2/mercury_robust.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 mercury/robust/__init__.py
-mercury/robust/_base_batch_drift_detector.py
 mercury/robust/_category_struct.py
-mercury/robust/_chi2_drift_detector.py
-mercury/robust/_drift_simulation.py
-mercury/robust/_histogram_distance_drift_detector.py
 mercury/robust/_label_cleaning.py
 mercury/robust/_linalg.py
-mercury/robust/_metrics.py
 mercury/robust/_tree_analysis.py
 mercury/robust/_treeselector.py
 mercury/robust/basetests.py
 mercury/robust/data_tests.py
 mercury/robust/errors.py
 mercury/robust/model_tests.py
 mercury/robust/suite.py
```

### Comparing `mercury-robust-0.0.1/pyproject.toml` & `mercury-robust-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mercury-robust"
 license = {file = "LICENSE.txt"}
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Mercury Team", email="mercury.group@bbva.com" },
 ]
 description = "Mercury's robust is a library to perform robust testing on models and/or datasets.."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,24 +19,26 @@
 ]
 dependencies = [
   'matplotlib>=3.0.2',
   'pandas>=0.24.2',
   'scikit-learn>=0.23.1',
   'seaborn',
   'mercury-dataschema',
+  'mercury-monitoring',
   'psutil',
   'cleanlab'
 ]
 
 [project.optional-dependencies]
 dev = [
   'tensorflow<2.11',
   'pytest',
   'flake8',
   'xgboost',
+  'mercury-explainability'
 ]
 doc = [
   'mkdocs',
   'mkdocstrings[python]',
   'mkdocs-material',
   'mkdocs-minify-plugin==0.5.0',
   'mkdocs-exclude',
```

### Comparing `mercury-robust-0.0.1/tests/test_basetests.py` & `mercury-robust-0.0.2/tests/test_basetests.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.1/tests/test_data_tests.py` & `mercury-robust-0.0.2/tests/test_data_tests.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.1/tests/test_model_tests.py` & `mercury-robust-0.0.2/tests/test_model_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from mercury.robust.model_tests import (
     ModelReproducibilityTest,
     ModelSimplicityChecker,
     DriftPredictionsResistanceTest,
     ClassificationInvarianceTest,
     TreeCoverageTest,
-    DriftMetricResistanceTest
+    DriftMetricResistanceTest,
+    FeatureCheckerTest
 )
 from mercury.robust.errors import FailedTestError
 
 
 @pytest.fixture(scope="module")
 def datasets():
     tips = sns.load_dataset("tips")
@@ -1029,7 +1030,95 @@
         drift_args = drift_args_1,
         tolerance= 1.0,
         Y = y,
         task='invalid'
     )
     with pytest.raises(ValueError):
         test.run()
+
+def test_feature_checker_test():
+    df = pd.read_csv('%s/csv/test_twt.csv' % pathlib.Path(__file__).parent.resolve(), sep = '\t')
+
+    train, test = train_test_split(df, test_size = 0.2)
+
+    X_train = train.loc[:, train.columns != 'Y']
+    Y_train = train.loc[:, 'Y']
+
+    rf = RandomForestClassifier()
+    rf.fit(X_train, Y_train)
+
+    fct = FeatureCheckerTest(rf, train, 'Y', tolerance = 100)
+    with pytest.raises(FailedTestError):
+        fct.run()
+
+    fct = FeatureCheckerTest(rf, train, 'Y', test, tolerance = 100)
+    with pytest.raises(FailedTestError):
+        fct.run()
+
+    def eval_fun(Y_obs, Y_hat):
+        return sum((Y_obs - Y_hat)**2)
+
+    fct = FeatureCheckerTest(rf, train, 'Y', test, eval = eval_fun, tolerance = 100)
+    with pytest.raises(FailedTestError):
+        fct.run()
+
+    fct = FeatureCheckerTest(rf, train, 'Y', test, importance = 'feature_importances_', tolerance = 100)
+    with pytest.raises(FailedTestError):
+        fct.run()
+
+    fct = FeatureCheckerTest(rf, train, 'Y', test, importance = 'feature_importances_', eval = eval_fun, tolerance = 100, remove_num = 2, num_tries = 1)
+    with pytest.raises(FailedTestError):
+        fct.run()
+
+
+def test_feature_checker_test_model_function():
+
+    # Create Dataset
+    X, y = make_classification(200, n_features=5, n_informative=5, n_redundant=0)
+    df = pd.DataFrame(X, columns=["x1", "x2", "x3", "x4", "x5"])
+    df["x6"] = np.random.choice(["cat_0", "cat_1", "cat_2"], size=len(df)) # make categorical feature feature
+    df["y"] = y
+    df_train, df_test = train_test_split(df, test_size = 0.2)
+
+    # Define function to create the model (pipeline)
+    def create_pipeline_fn(X, model_args):
+
+        num_feats = [f for f in model_args['num_feats'] if f in X.columns]
+        cat_feats = [f for f in model_args['cat_feats'] if f in X.columns]
+
+        numeric_transformer = Pipeline(steps=[("scaler", StandardScaler())])
+        categorical_transformer = Pipeline(steps=[("ohe", OneHotEncoder(handle_unknown="ignore"))])
+
+        preprocessor = ColumnTransformer(
+            transformers=[
+                ("num", numeric_transformer, num_feats),
+                ("cat", categorical_transformer, cat_feats),
+            ], remainder='drop'
+        )
+
+        pipeline = Pipeline(
+            steps=[
+                ("preprocessor", preprocessor),
+                ("classifier", DecisionTreeClassifier())
+            ]
+        )
+        
+        return pipeline
+
+    # Create and run test
+    num_feats = ["x1", "x2", "x3", "x4", "x5"]
+    cat_feats = ["x6"]
+    model_fn_args = {
+        'num_feats': num_feats,
+        'cat_feats': cat_feats
+    }
+    test = FeatureCheckerTest(
+        model=create_pipeline_fn,
+        train=df_train,
+        target="y",
+        test=df_test,
+        tolerance=-1,
+        num_tries=3,
+        remove_num=1,
+        model_fn_args = model_fn_args,
+    )
+    test.run()
```

### Comparing `mercury-robust-0.0.1/tests/test_suite.py` & `mercury-robust-0.0.2/tests/test_suite.py`

 * *Files identical despite different names*

