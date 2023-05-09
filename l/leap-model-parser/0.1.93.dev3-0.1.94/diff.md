# Comparing `tmp/leap_model_parser-0.1.93.dev3.tar.gz` & `tmp/leap_model_parser-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_model_parser-0.1.93.dev3.tar", max compression
+gzip compressed data, was "leap_model_parser-0.1.94.tar", max compression
```

## Comparing `leap_model_parser-0.1.93.dev3.tar` & `leap_model_parser-0.1.94.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2022-02-10 15:52:31.114426 leap_model_parser-0.1.93.dev3/LICENSE
--rw-r--r--   0        0        0       68 2022-02-13 12:20:32.223194 leap_model_parser-0.1.93.dev3/README.md
--rw-r--r--   0        0        0      132 2022-05-26 14:22:41.518359 leap_model_parser-0.1.93.dev3/leap_model_parser/__init__.py
--rw-r--r--   0        0        0        0 2022-02-10 15:52:31.865328 leap_model_parser-0.1.93.dev3/leap_model_parser/contract/__init__.py
--rw-r--r--   0        0        0      691 2023-03-06 12:05:13.379795 leap_model_parser-0.1.93.dev3/leap_model_parser/contract/importmodelresponse.py
--rw-r--r--   0        0        0    44142 2023-05-02 07:42:26.775061 leap_model_parser-0.1.93.dev3/leap_model_parser/contract/nodedata.py
--rw-r--r--   0        0        0   421621 2023-05-02 07:42:26.773903 leap_model_parser-0.1.93.dev3/leap_model_parser/contract/ui_components.json
--rw-r--r--   0        0        0    15485 2023-04-02 14:14:25.101809 leap_model_parser-0.1.93.dev3/leap_model_parser/keras_json_model_import.py
--rw-r--r--   0        0        0     6766 2023-03-29 10:33:06.573801 leap_model_parser-0.1.93.dev3/leap_model_parser/model_parser.py
--rw-r--r--   0        0        0        0 2022-05-26 14:22:41.520554 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-05-26 14:22:41.520732 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/layerpedia/__init__.py
--rw-r--r--   0        0        0     9291 2022-05-26 14:22:41.520971 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/layerpedia/layerpedia.py
--rw-r--r--   0        0        0        1 2022-05-26 14:22:41.521197 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/tlinspection/__init__.py
--rw-r--r--   0        0        0     2786 2022-05-26 14:22:41.521396 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/tlinspection/leapinspection.py
--rw-r--r--   0        0        0      111 2022-05-26 14:22:41.521654 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/__init__.py
--rw-r--r--   0        0        0     3035 2022-05-26 14:22:41.521847 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/generatenodedata.py
--rw-r--r--   0        0        0     5799 2022-06-13 10:57:06.739900 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
--rw-r--r--   0        0        0    19604 2023-04-30 15:00:43.099004 leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/ui_components_config.yaml
--rw-r--r--   0        0        0     1072 2023-05-07 07:07:38.837689 leap_model_parser-0.1.93.dev3/pyproject.toml
--rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 leap_model_parser-0.1.93.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-07-18 07:29:48.936891 leap_model_parser-0.1.94/LICENSE
+-rw-r--r--   0        0        0       68 2022-07-18 07:29:48.936891 leap_model_parser-0.1.94/README.md
+-rw-r--r--   0        0        0      132 2022-07-18 07:29:48.936891 leap_model_parser-0.1.94/leap_model_parser/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.94/leap_model_parser/contract/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-04 06:58:15.124228 leap_model_parser-0.1.94/leap_model_parser/contract/importmodelresponse.py
+-rw-r--r--   0        0        0    43326 2023-05-08 06:06:56.507686 leap_model_parser-0.1.94/leap_model_parser/contract/nodedata.py
+-rw-r--r--   0        0        0   416303 2023-05-08 06:04:30.540347 leap_model_parser-0.1.94/leap_model_parser/contract/ui_components.json
+-rw-r--r--   0        0        0    15485 2023-04-04 06:58:15.124228 leap_model_parser-0.1.94/leap_model_parser/keras_json_model_import.py
+-rw-r--r--   0        0        0     6766 2023-04-04 06:58:15.124228 leap_model_parser-0.1.94/leap_model_parser/model_parser.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.94/leap_model_parser/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.940891 leap_model_parser-0.1.94/leap_model_parser/utils/layerpedia/__init__.py
+-rw-r--r--   0        0        0     9291 2022-07-18 07:29:48.940891 leap_model_parser-0.1.94/leap_model_parser/utils/layerpedia/layerpedia.py
+-rw-r--r--   0        0        0        1 2022-07-18 07:29:48.940891 leap_model_parser-0.1.94/leap_model_parser/utils/tlinspection/__init__.py
+-rw-r--r--   0        0        0     2804 2023-05-08 06:00:02.429640 leap_model_parser-0.1.94/leap_model_parser/utils/tlinspection/leapinspection.py
+-rw-r--r--   0        0        0      111 2022-07-18 07:29:48.940891 leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/__init__.py
+-rw-r--r--   0        0        0     3035 2022-07-18 07:29:48.940891 leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/generatenodedata.py
+-rw-r--r--   0        0        0     6768 2023-05-08 06:06:56.515687 leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
+-rw-r--r--   0        0        0    19604 2023-04-04 06:58:15.124228 leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/ui_components_config.yaml
+-rw-r--r--   0        0        0     1052 2023-05-09 06:05:22.198667 leap_model_parser-0.1.94/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 leap_model_parser-0.1.94/PKG-INFO
```

### Comparing `leap_model_parser-0.1.93.dev3/LICENSE` & `leap_model_parser-0.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev3/leap_model_parser/contract/importmodelresponse.py` & `leap_model_parser-0.1.94/leap_model_parser/contract/importmodelresponse.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev3/leap_model_parser/contract/nodedata.py` & `leap_model_parser-0.1.94/leap_model_parser/contract/nodedata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Union
-from typing import List
 from dataclasses import dataclass
+from typing import List
+from typing import Union
 from enum import Enum
 
 
 class ActivationsEnum(Enum):
     relu = "relu"
     softmax = "softmax"
     selu = "selu"
@@ -117,15 +117,14 @@
     GlobalAveragePooling1D = "GlobalAveragePooling1D"
     GlobalAveragePooling2D = "GlobalAveragePooling2D"
     GlobalAveragePooling3D = "GlobalAveragePooling3D"
     GlobalMaxPooling1D = "GlobalMaxPooling1D"
     GlobalMaxPooling2D = "GlobalMaxPooling2D"
     GlobalMaxPooling3D = "GlobalMaxPooling3D"
     GroupNormalization = "GroupNormalization"
-    Identity = "Identity"
     IntegerLookup = "IntegerLookup"
     LSTM = "LSTM"
     LSTMCell = "LSTMCell"
     LSTMCellV1 = "LSTMCellV1"
     LSTMCellV2 = "LSTMCellV2"
     LSTMV1 = "LSTMV1"
     LSTMV2 = "LSTMV2"
@@ -191,26 +190,25 @@
     MeanAbsoluteError = "MeanAbsoluteError"
     MeanAbsolutePercentageError = "MeanAbsolutePercentageError"
     MeanSquaredError = "MeanSquaredError"
     MeanSquaredLogarithmicError = "MeanSquaredLogarithmicError"
     Poisson = "Poisson"
     SquaredHinge = "SquaredHinge"
     Adadelta = "Adadelta"
-    Adafactor = "Adafactor"
     Adagrad = "Adagrad"
     Adam = "Adam"
-    AdamW = "AdamW"
     Adamax = "Adamax"
     Ftrl = "Ftrl"
     Nadam = "Nadam"
     RMSprop = "RMSprop"
     SGD = "SGD"
     OnnxAbs = "OnnxAbs"
     OnnxErf = "OnnxErf"
     OnnxHardSigmoid = "OnnxHardSigmoid"
+    OnnxLSTM = "OnnxLSTM"
     OnnxReduceMean = "OnnxReduceMean"
     OnnxSqrt = "OnnxSqrt"
     Dataset = "Dataset"
     Input = "Input"
     RepresentationBlock = "RepresentationBlock"
     GroundTruth = "GroundTruth"
     CustomLayer = "CustomLayer"
@@ -298,15 +296,14 @@
     gamma_initializer: InitializersEnum
     moving_mean_initializer: InitializersEnum
     moving_variance_initializer: InitializersEnum
     beta_regularizer: RegularizerEnum
     gamma_regularizer: RegularizerEnum
     beta_constraint: ConstraintEnum
     gamma_constraint: ConstraintEnum
-    synchronized: bool
     type: NodeType
 
 
 @dataclass
 class Bidirectional:
     merge_mode: str
     weights: List[int]
@@ -694,15 +691,14 @@
     output_dim: int
     embeddings_initializer: str
     embeddings_regularizer: RegularizerEnum
     activity_regularizer: RegularizerEnum
     embeddings_constraint: ConstraintEnum
     mask_zero: bool
     input_length: List[int]
-    sparse: bool
     type: NodeType
 
 
 @dataclass
 class Flatten:
     type: NodeType
 
@@ -915,22 +911,14 @@
     gamma_regularizer: RegularizerEnum
     beta_constraint: ConstraintEnum
     gamma_constraint: ConstraintEnum
     type: NodeType
 
 
 @dataclass
-class Identity:
-    trainable: bool
-    dtype: List[int]
-    dynamic: bool
-    type: NodeType
-
-
-@dataclass
 class IntegerLookup:
     max_tokens: List[int]
     num_oov_indices: int
     mask_token: List[int]
     oov_token: int
     vocabulary: List[int]
     vocabulary_dtype: str
@@ -1272,15 +1260,15 @@
     scale: List[int]
     trainable: bool
     type: NodeType
 
 
 @dataclass
 class RandomHeight:
-    factor: float
+    factor: List[int]
     interpolation: str
     seed: List[int]
     type: NodeType
 
 
 @dataclass
 class RandomRotation:
@@ -1301,23 +1289,23 @@
     seed: List[int]
     fill_value: float
     type: NodeType
 
 
 @dataclass
 class RandomWidth:
-    factor: float
+    factor: List[int]
     interpolation: str
     seed: List[int]
     type: NodeType
 
 
 @dataclass
 class RandomZoom:
-    height_factor: float
+    height_factor: List[int]
     width_factor: List[int]
     fill_mode: str
     interpolation: str
     seed: List[int]
     fill_value: float
     type: NodeType
 
@@ -1677,33 +1665,14 @@
     ema_momentum: float
     ema_overwrite_frequency: List[int]
     jit_compile: bool
     type: NodeType
 
 
 @dataclass
-class Adafactor:
-    learning_rate: float
-    beta_2_decay: float
-    epsilon_1: float
-    epsilon_2: float
-    clip_threshold: float
-    relative_step: bool
-    weight_decay: List[int]
-    clipnorm: List[int]
-    clipvalue: List[int]
-    global_clipnorm: List[int]
-    use_ema: bool
-    ema_momentum: float
-    ema_overwrite_frequency: List[int]
-    jit_compile: bool
-    type: NodeType
-
-
-@dataclass
 class Adagrad:
     learning_rate: float
     initial_accumulator_value: float
     epsilon: float
     weight_decay: List[int]
     clipnorm: List[int]
     clipvalue: List[int]
@@ -1730,32 +1699,14 @@
     ema_momentum: float
     ema_overwrite_frequency: List[int]
     jit_compile: bool
     type: NodeType
 
 
 @dataclass
-class AdamW:
-    learning_rate: float
-    weight_decay: float
-    beta_1: float
-    beta_2: float
-    epsilon: float
-    amsgrad: bool
-    clipnorm: List[int]
-    clipvalue: List[int]
-    global_clipnorm: List[int]
-    use_ema: bool
-    ema_momentum: float
-    ema_overwrite_frequency: List[int]
-    jit_compile: bool
-    type: NodeType
-
-
-@dataclass
 class Adamax:
     learning_rate: float
     beta_1: float
     beta_2: float
     epsilon: float
     weight_decay: List[int]
     clipnorm: List[int]
@@ -1824,14 +1775,15 @@
 
 
 @dataclass
 class SGD:
     learning_rate: float
     momentum: float
     nesterov: bool
+    amsgrad: bool
     weight_decay: List[int]
     clipnorm: List[int]
     clipvalue: List[int]
     global_clipnorm: List[int]
     use_ema: bool
     ema_momentum: float
     ema_overwrite_frequency: List[int]
@@ -1853,14 +1805,22 @@
 class OnnxHardSigmoid:
     alpha: float
     beta: float
     type: NodeType
 
 
 @dataclass
+class OnnxLSTM:
+    units: int
+    return_sequences: bool
+    return_lstm_state: bool
+    type: NodeType
+
+
+@dataclass
 class OnnxReduceMean:
     axes: List[int]
     keepdims: bool
     type: NodeType
 
 
 @dataclass
@@ -1955,22 +1915,22 @@
     props: Union[Activation, ActivityRegularization, Add, AdditiveAttention, AlphaDropout, Average, AveragePooling1D, 
                  AveragePooling2D, AveragePooling3D, BatchNormalization, Bidirectional, CategoryEncoding, CenterCrop, 
                  Concatenate, Conv1D, Conv1DTranspose, Conv2D, Conv2DTranspose, Conv3D, Conv3DTranspose, ConvLSTM1D, 
                  ConvLSTM2D, ConvLSTM3D, Cropping1D, Cropping2D, Cropping3D, CuDNNGRU, CuDNNLSTM, Dense, 
                  DepthwiseConv1D, DepthwiseConv2D, Discretization, Dot, Dropout, ELU, Embedding, Flatten, GRU, GRUCell, 
                  GRUCellV1, GRUCellV2, GRUV1, GRUV2, GaussianDropout, GaussianNoise, GlobalAveragePooling1D, 
                  GlobalAveragePooling2D, GlobalAveragePooling3D, GlobalMaxPooling1D, GlobalMaxPooling2D, 
-                 GlobalMaxPooling3D, GroupNormalization, Identity, IntegerLookup, LSTM, LSTMCell, LSTMCellV1, 
-                 LSTMCellV2, LSTMV1, LSTMV2, LayerNormalization, LeakyReLU, LocallyConnected1D, LocallyConnected2D, 
-                 Masking, MaxPooling1D, MaxPooling2D, MaxPooling3D, Maximum, Minimum, MultiHeadAttention, Multiply, 
-                 Normalization, PReLU, Permute, RandomBrightness, RandomContrast, RandomCrop, RandomFlip, 
-                 RandomFourierFeatures, RandomHeight, RandomRotation, RandomTranslation, RandomWidth, RandomZoom, ReLU, 
-                 RepeatVector, Reshape, Resizing, SeparableConv1D, SeparableConv2D, SimpleRNN, SimpleRNNCell, Softmax, 
-                 SpatialDropout1D, SpatialDropout2D, SpatialDropout3D, StringLookup, Subtract, SyncBatchNormalization, 
-                 TextVectorization, ThresholdedReLU, TimeDistributed, UnitNormalization, UpSampling1D, UpSampling2D, 
-                 UpSampling3D, ZeroPadding1D, ZeroPadding2D, ZeroPadding3D, BinaryCrossentropy, BinaryFocalCrossentropy, 
+                 GlobalMaxPooling3D, GroupNormalization, IntegerLookup, LSTM, LSTMCell, LSTMCellV1, LSTMCellV2, LSTMV1, 
+                 LSTMV2, LayerNormalization, LeakyReLU, LocallyConnected1D, LocallyConnected2D, Masking, MaxPooling1D, 
+                 MaxPooling2D, MaxPooling3D, Maximum, Minimum, MultiHeadAttention, Multiply, Normalization, PReLU, 
+                 Permute, RandomBrightness, RandomContrast, RandomCrop, RandomFlip, RandomFourierFeatures, RandomHeight, 
+                 RandomRotation, RandomTranslation, RandomWidth, RandomZoom, ReLU, RepeatVector, Reshape, Resizing, 
+                 SeparableConv1D, SeparableConv2D, SimpleRNN, SimpleRNNCell, Softmax, SpatialDropout1D, 
+                 SpatialDropout2D, SpatialDropout3D, StringLookup, Subtract, SyncBatchNormalization, TextVectorization, 
+                 ThresholdedReLU, TimeDistributed, UnitNormalization, UpSampling1D, UpSampling2D, UpSampling3D, 
+                 ZeroPadding1D, ZeroPadding2D, ZeroPadding3D, BinaryCrossentropy, BinaryFocalCrossentropy, 
                  CategoricalCrossentropy, CategoricalHinge, CosineSimilarity, Hinge, Huber, KLDivergence, LogCosh, 
                  MeanAbsoluteError, MeanAbsolutePercentageError, MeanSquaredError, MeanSquaredLogarithmicError, Poisson, 
-                 SquaredHinge, Adadelta, Adafactor, Adagrad, Adam, AdamW, Adamax, Ftrl, Nadam, RMSprop, SGD, OnnxAbs, 
-                 OnnxErf, OnnxHardSigmoid, OnnxReduceMean, OnnxSqrt, Dataset, Input, RepresentationBlock, GroundTruth, 
+                 SquaredHinge, Adadelta, Adagrad, Adam, Adamax, Ftrl, Nadam, RMSprop, SGD, OnnxAbs, OnnxErf, 
+                 OnnxHardSigmoid, OnnxLSTM, OnnxReduceMean, OnnxSqrt, Dataset, Input, RepresentationBlock, GroundTruth, 
                  CustomLayer, CustomLoss, Visualizer, Metric, Lambda, TFOpLambda, SlicingOpLambda, Repeat, Variable, 
                  Gather, FixedDropout]
```

### Comparing `leap_model_parser-0.1.93.dev3/leap_model_parser/contract/ui_components.json` & `leap_model_parser-0.1.94/leap_model_parser/contract/ui_components.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9734356499981499%*

 * *Differences: {'124': "{'parents': {insert: [(2, 'optimizer_experimental')]}}",*

 * * '125': "{'parents': {insert: [(2, 'optimizer_experimental')]}}",*

 * * '126': "{'parents': {insert: [(2, 'optimizer_experimental')]}}",*

 * * '127': "{'parents': {insert: [(2, 'optimizer_experimental')]}}",*

 * * '128': "{'parents': {insert: [(2, 'optimizer_experimental')]}}",*

 * * '129': "{'parents': {insert: [(2, 'optimizer_experimental')]}}",*

 * * '130': "{'parents': {insert: [(2, 'optimizer_experimental')]}}",*

 * * '131': "{'parents': {insert: [(2, 'optimizer_expe […]*

```diff
@@ -722,20 +722,14 @@
                 "values": [
                     "MaxNorm",
                     "MinMaxNorm",
                     "NonNeg",
                     "RadialConstraint",
                     "UnitNorm"
                 ]
-            },
-            {
-                "default_val": false,
-                "isdefault": true,
-                "name": "synchronized",
-                "type": "bool"
             }
         ],
         "receptive_fields_func": "IdentityReceptiveFieldsFunc",
         "shape_calc": [
             "IdentityFunc"
         ],
         "type": "Layer"
@@ -4740,20 +4734,14 @@
                 "type": "bool"
             },
             {
                 "default_val": null,
                 "isdefault": true,
                 "name": "input_length",
                 "type": "NoneType"
-            },
-            {
-                "default_val": false,
-                "isdefault": true,
-                "name": "sparse",
-                "type": "bool"
             }
         ],
         "receptive_fields_func": "EmptyReceptiveFieldsFunc",
         "shape_calc": [
             "EmbeddingShapeFunc"
         ],
         "type": "Layer"
@@ -6836,74 +6824,14 @@
                 }
             ]
         },
         "menu_sections": [
             "Layer",
             "Core"
         ],
-        "name": "Identity",
-        "options": null,
-        "outputs_data": {
-            "outputs": [
-                {
-                    "name": "feature_map"
-                }
-            ]
-        },
-        "parents": [
-            "keras",
-            "layers",
-            "core",
-            "identity"
-        ],
-        "properties": [
-            {
-                "default_val": true,
-                "isdefault": true,
-                "name": "trainable",
-                "type": "bool"
-            },
-            {
-                "default_val": null,
-                "isdefault": true,
-                "name": "dtype",
-                "type": "NoneType"
-            },
-            {
-                "default_val": false,
-                "isdefault": true,
-                "name": "dynamic",
-                "type": "bool"
-            }
-        ],
-        "receptive_fields_func": "EmptyReceptiveFieldsFunc",
-        "shape_calc": [
-            "IdentityFunc"
-        ],
-        "type": "Layer"
-    },
-    {
-        "inputs_data": {
-            "add_input_by_drag": false,
-            "inputs": [
-                {
-                    "approval_connection": [
-                        "Input",
-                        "Dataset",
-                        "Layer",
-                        "CustomLayer"
-                    ],
-                    "name": "input"
-                }
-            ]
-        },
-        "menu_sections": [
-            "Layer",
-            "Core"
-        ],
         "name": "IntegerLookup",
         "options": null,
         "outputs_data": {
             "outputs": [
                 {
                     "name": "feature_map"
                 }
@@ -10210,15 +10138,15 @@
             "image_preprocessing"
         ],
         "properties": [
             {
                 "default_val": null,
                 "isdefault": false,
                 "name": "factor",
-                "type": "float"
+                "type": "tuple"
             },
             {
                 "default_val": "bilinear",
                 "isdefault": true,
                 "name": "interpolation",
                 "type": "str"
             },
@@ -10420,15 +10348,15 @@
             "image_preprocessing"
         ],
         "properties": [
             {
                 "default_val": null,
                 "isdefault": false,
                 "name": "factor",
-                "type": "float"
+                "type": "tuple"
             },
             {
                 "default_val": "bilinear",
                 "isdefault": true,
                 "name": "interpolation",
                 "type": "str"
             },
@@ -10480,15 +10408,15 @@
             "image_preprocessing"
         ],
         "properties": [
             {
                 "default_val": null,
                 "isdefault": false,
                 "name": "height_factor",
-                "type": "float"
+                "type": "tuple"
             },
             {
                 "default_val": null,
                 "isdefault": true,
                 "name": "width_factor",
                 "type": "NoneType"
             },
@@ -13658,14 +13586,15 @@
         },
         "outputs_data": {
             "outputs": []
         },
         "parents": [
             "keras",
             "optimizers",
+            "optimizer_experimental",
             "adadelta"
         ],
         "properties": [
             {
                 "default_val": 0.001,
                 "isdefault": true,
                 "name": "learning_rate",
@@ -13746,139 +13675,26 @@
                     "name": "loss_${id}"
                 }
             ]
         },
         "menu_sections": [
             "Optimizeres"
         ],
-        "name": "Adafactor",
-        "options": null,
-        "outputs_data": {
-            "outputs": []
-        },
-        "parents": [
-            "keras",
-            "optimizers",
-            "adafactor"
-        ],
-        "properties": [
-            {
-                "default_val": 0.001,
-                "isdefault": true,
-                "name": "learning_rate",
-                "type": "float"
-            },
-            {
-                "default_val": -0.8,
-                "isdefault": true,
-                "name": "beta_2_decay",
-                "type": "float"
-            },
-            {
-                "default_val": 1e-30,
-                "isdefault": true,
-                "name": "epsilon_1",
-                "type": "float"
-            },
-            {
-                "default_val": 0.001,
-                "isdefault": true,
-                "name": "epsilon_2",
-                "type": "float"
-            },
-            {
-                "default_val": 1.0,
-                "isdefault": true,
-                "name": "clip_threshold",
-                "type": "float"
-            },
-            {
-                "default_val": true,
-                "isdefault": true,
-                "name": "relative_step",
-                "type": "bool"
-            },
-            {
-                "default_val": null,
-                "isdefault": true,
-                "name": "weight_decay",
-                "type": "NoneType"
-            },
-            {
-                "default_val": null,
-                "isdefault": true,
-                "name": "clipnorm",
-                "type": "NoneType"
-            },
-            {
-                "default_val": null,
-                "isdefault": true,
-                "name": "clipvalue",
-                "type": "NoneType"
-            },
-            {
-                "default_val": null,
-                "isdefault": true,
-                "name": "global_clipnorm",
-                "type": "NoneType"
-            },
-            {
-                "default_val": false,
-                "isdefault": true,
-                "name": "use_ema",
-                "type": "bool"
-            },
-            {
-                "default_val": 0.99,
-                "isdefault": true,
-                "name": "ema_momentum",
-                "type": "float"
-            },
-            {
-                "default_val": null,
-                "isdefault": true,
-                "name": "ema_overwrite_frequency",
-                "type": "NoneType"
-            },
-            {
-                "default_val": true,
-                "isdefault": true,
-                "name": "jit_compile",
-                "type": "bool"
-            }
-        ],
-        "type": "Optimizer"
-    },
-    {
-        "inputs_data": {
-            "add_input_by_drag": true,
-            "inputs": [
-                {
-                    "approval_connection": [
-                        "Loss",
-                        "CustomLoss"
-                    ],
-                    "name": "loss_${id}"
-                }
-            ]
-        },
-        "menu_sections": [
-            "Optimizeres"
-        ],
         "name": "Adagrad",
         "options": {
             "layer_inspection": false,
             "representation_block": false
         },
         "outputs_data": {
             "outputs": []
         },
         "parents": [
             "keras",
             "optimizers",
+            "optimizer_experimental",
             "adagrad"
         ],
         "properties": [
             {
                 "default_val": 0.001,
                 "isdefault": true,
                 "name": "learning_rate",
@@ -13970,14 +13786,15 @@
         },
         "outputs_data": {
             "outputs": []
         },
         "parents": [
             "keras",
             "optimizers",
+            "optimizer_experimental",
             "adam"
         ],
         "properties": [
             {
                 "default_val": 0.001,
                 "isdefault": true,
                 "name": "learning_rate",
@@ -14070,133 +13887,26 @@
                     "name": "loss_${id}"
                 }
             ]
         },
         "menu_sections": [
             "Optimizeres"
         ],
-        "name": "AdamW",
-        "options": null,
-        "outputs_data": {
-            "outputs": []
-        },
-        "parents": [
-            "keras",
-            "optimizers",
-            "adamw"
-        ],
-        "properties": [
-            {
-                "default_val": 0.001,
-                "isdefault": true,
-                "name": "learning_rate",
-                "type": "float"
-            },
-            {
-                "default_val": 0.004,
-                "isdefault": true,
-                "name": "weight_decay",
-                "type": "float"
-            },
-            {
-                "default_val": 0.9,
-                "isdefault": true,
-                "name": "beta_1",
-                "type": "float"
-            },
-            {
-                "default_val": 0.999,
-                "isdefault": true,
-                "name": "beta_2",
-                "type": "float"
-            },
-            {
-                "default_val": 1e-07,
-                "isdefault": true,
-                "name": "epsilon",
-                "type": "float"
-            },
-            {
-                "default_val": false,
-                "isdefault": true,
-                "name": "amsgrad",
-                "type": "bool"
-            },
-            {
-                "default_val": null,
-                "isdefault": true,
-                "name": "clipnorm",
-                "type": "NoneType"
-            },
-            {
-                "default_val": null,
-                "isdefault": true,
-                "name": "clipvalue",
-                "type": "NoneType"
-            },
-            {
-                "default_val": null,
-                "isdefault": true,
-                "name": "global_clipnorm",
-                "type": "NoneType"
-            },
-            {
-                "default_val": false,
-                "isdefault": true,
-                "name": "use_ema",
-                "type": "bool"
-            },
-            {
-                "default_val": 0.99,
-                "isdefault": true,
-                "name": "ema_momentum",
-                "type": "float"
-            },
-            {
-                "default_val": null,
-                "isdefault": true,
-                "name": "ema_overwrite_frequency",
-                "type": "NoneType"
-            },
-            {
-                "default_val": true,
-                "isdefault": true,
-                "name": "jit_compile",
-                "type": "bool"
-            }
-        ],
-        "type": "Optimizer"
-    },
-    {
-        "inputs_data": {
-            "add_input_by_drag": true,
-            "inputs": [
-                {
-                    "approval_connection": [
-                        "Loss",
-                        "CustomLoss"
-                    ],
-                    "name": "loss_${id}"
-                }
-            ]
-        },
-        "menu_sections": [
-            "Optimizeres"
-        ],
         "name": "Adamax",
         "options": {
             "layer_inspection": false,
             "representation_block": false
         },
         "outputs_data": {
             "outputs": []
         },
         "parents": [
             "keras",
             "optimizers",
+            "optimizer_experimental",
             "adamax"
         ],
         "properties": [
             {
                 "default_val": 0.001,
                 "isdefault": true,
                 "name": "learning_rate",
@@ -14294,14 +14004,15 @@
         },
         "outputs_data": {
             "outputs": []
         },
         "parents": [
             "keras",
             "optimizers",
+            "optimizer_experimental",
             "ftrl"
         ],
         "properties": [
             {
                 "default_val": 0.001,
                 "isdefault": true,
                 "name": "learning_rate",
@@ -14417,14 +14128,15 @@
         },
         "outputs_data": {
             "outputs": []
         },
         "parents": [
             "keras",
             "optimizers",
+            "optimizer_experimental",
             "nadam"
         ],
         "properties": [
             {
                 "default_val": 0.001,
                 "isdefault": true,
                 "name": "learning_rate",
@@ -14522,14 +14234,15 @@
         },
         "outputs_data": {
             "outputs": []
         },
         "parents": [
             "keras",
             "optimizers",
+            "optimizer_experimental",
             "rmsprop"
         ],
         "properties": [
             {
                 "default_val": 0.001,
                 "isdefault": true,
                 "name": "learning_rate",
@@ -14633,14 +14346,15 @@
         },
         "outputs_data": {
             "outputs": []
         },
         "parents": [
             "keras",
             "optimizers",
+            "optimizer_experimental",
             "sgd"
         ],
         "properties": [
             {
                 "default_val": 0.01,
                 "isdefault": true,
                 "name": "learning_rate",
@@ -14655,14 +14369,20 @@
             {
                 "default_val": false,
                 "isdefault": true,
                 "name": "nesterov",
                 "type": "bool"
             },
             {
+                "default_val": false,
+                "isdefault": true,
+                "name": "amsgrad",
+                "type": "bool"
+            },
+            {
                 "default_val": null,
                 "isdefault": true,
                 "name": "weight_decay",
                 "type": "NoneType"
             },
             {
                 "default_val": null,
@@ -14837,14 +14557,91 @@
             }
         ],
         "receptive_fields_func": "IdentityReceptiveFieldsFunc",
         "shape_calc": [
             "IdentityFunc"
         ],
         "type": "Layer"
+    },
+    {
+        "inputs_data": {
+            "add_input_by_drag": false,
+            "inputs": [
+                {
+                    "approval_connection": [
+                        "Input",
+                        "Dataset",
+                        "Layer",
+                        "CustomLayer"
+                    ],
+                    "name": "input"
+                },
+                {
+                    "approval_connection": [
+                        "Input",
+                        "Dataset",
+                        "Layer",
+                        "CustomLayer"
+                    ],
+                    "name": "initial_h_state"
+                },
+                {
+                    "approval_connection": [
+                        "Input",
+                        "Dataset",
+                        "Layer",
+                        "CustomLayer"
+                    ],
+                    "name": "initial_c_state"
+                }
+            ]
+        },
+        "menu_sections": [
+            "Layer",
+            "Onnx"
+        ],
+        "name": "OnnxLSTM",
+        "options": null,
+        "outputs_data": {
+            "outputs": [
+                {
+                    "name": "feature_map"
+                }
+            ]
+        },
+        "parents": [
+            "onnx2kerastl",
+            "customonnxlayer",
+            "onnxlstm"
+        ],
+        "properties": [
+            {
+                "default_val": null,
+                "isdefault": false,
+                "name": "units",
+                "type": "int"
+            },
+            {
+                "default_val": null,
+                "isdefault": false,
+                "name": "return_sequences",
+                "type": "bool"
+            },
+            {
+                "default_val": null,
+                "isdefault": false,
+                "name": "return_lstm_state",
+                "type": "bool"
+            }
+        ],
+        "receptive_fields_func": "IdentityReceptiveFieldsFunc",
+        "shape_calc": [
+            "IdentityFunc"
+        ],
+        "type": "Layer"
     },
     {
         "inputs_data": {
             "add_input_by_drag": false,
             "inputs": [
                 {
                     "approval_connection": [
```

### Comparing `leap_model_parser-0.1.93.dev3/leap_model_parser/keras_json_model_import.py` & `leap_model_parser-0.1.94/leap_model_parser/keras_json_model_import.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev3/leap_model_parser/model_parser.py` & `leap_model_parser-0.1.94/leap_model_parser/model_parser.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev3/leap_model_parser/utils/layerpedia/layerpedia.py` & `leap_model_parser-0.1.94/leap_model_parser/utils/layerpedia/layerpedia.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev3/leap_model_parser/utils/tlinspection/leapinspection.py` & `leap_model_parser-0.1.94/leap_model_parser/utils/tlinspection/leapinspection.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 classes.append(cls_dict)
 
         return classes
 
     @staticmethod
     def get_type(func, pval):
         dtype_map = {'int': ['int', 'Integer', 'number'], 'float': ['float'], 'str': ['string', 'str'],
-                     'name': ['name'], 'tuple': ["tuple", "Tuple"]}
+                     'name': ['name'], 'tuple': ["tuple", "Tuple"], 'bool': ['bool']}
         if pval.default != inspect._empty:
             return str(type(pval.default)).split('\'')[1]
         # TODO: comment out due to missing CallableMeta type in python 3.8, if an error occurs from this section consider
         # finding the right way to write this if in python 3.8
         # if isinstance(pval.annotation, CallableMeta):
         #     return Callable
         if pval.annotation is str:
```

### Comparing `leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/generatenodedata.py` & `leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/generatenodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/tensorflowinscpection.py` & `leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/tensorflowinscpection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import os
-from typing import List, Optional
+from typing import List, Optional, Callable, Any
 
 import yaml
 from leap_model_parser.utils.layerpedia.layerpedia import Layerpedia
 from leap_model_parser.utils.tlinspection.leapinspection import LeapInspect
+from copy import deepcopy
 
 
 class TensorFlowInspection(LeapInspect):
 
     def __init__(self):
         file_path = os.path.dirname(os.path.abspath(__file__))
         with open(f'{file_path}/ui_components_config.yaml') as f:
@@ -51,14 +52,32 @@
                     arg['default_val'] = override_def
             _args.append(arg)
         return _args
 
     def filter_node(self, node):
         return node['name'] in self.ignores['clsignore']
 
+    def get_filled_group_values(self, node_type: str, class_pointer: Callable[..., Any]) -> dict:
+        if node_type == 'customonnxlayer':
+            var_names = class_pointer.__dict__['call'].__code__.co_varnames
+            arg_names = var_names[1:class_pointer.__dict__['call'].__code__.co_argcount]  # remove self
+            if len(arg_names) == 1:
+                return self.group_type[node_type]
+            else:
+                config_dict = deepcopy(self.group_type[node_type])
+                inputs_list = config_dict['inputs_data']['inputs']
+                for arg in arg_names[1:]:
+                    inputs_list.append(
+                        {'name': f'{arg}',
+                         'approval_connection': ['Input', 'Dataset', 'Layer', 'CustomLayer']}
+                    )
+                return config_dict
+        else:
+            return self.group_type[node_type]
+
     def inspect_lib(self, lib):
         # TODO: extract only classes and not aliases
         classes = LeapInspect.get_classes(lib, self.ignores['lib_ignore'])
         nodes = []
         for node_cls in classes:
             if self.filter_node(node_cls):
                 continue
@@ -74,15 +93,15 @@
             enable_bigger_input_rank = self.query_layerpedia_enable_bigger_input_rank(
                 node_cls['name'])
             if enable_bigger_input_rank:
                 node['enable_bigger_input_rank'] = enable_bigger_input_rank
             template_node = {}
             for d in [*node_cls['parents'], node['name']]:
                 if d in self.group_type:
-                    template_node = {**template_node, **self.group_type[d]}
+                    template_node = {**template_node, **self.get_filled_group_values(d, node_cls['class'])}
             node = {**template_node, **node}
             if 'hash' in node and not self.query_layerpedia_is_trainable(node_cls['name']):
                 node.pop('hash')
             nodes.append(node)
         return nodes
 
     def inspect(self, dist: str) -> List[dict]:
```

### Comparing `leap_model_parser-0.1.93.dev3/leap_model_parser/utils/uicomponents/ui_components_config.yaml` & `leap_model_parser-0.1.94/leap_model_parser/utils/uicomponents/ui_components_config.yaml`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.93.dev3/pyproject.toml` & `leap_model_parser-0.1.94/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "leap-model-parser"
-version = "0.1.93.dev3"
+version = "0.1.94"
 description = ""
 authors = ["idan <idan.yogev@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/leap-model-parser"
 homepage = "https://github.com/tensorleap/leap-model-parser"
 include = [
     "LICENSE",
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
-tensorflow = {version = "2.12.0", markers = "platform_machine  == 'x86_64'"}
-tensorflow-macos = {version = "2.12.0", markers = "platform_machine  == 'arm64'"}
+tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
+tensorflow-macos = {version = "2.11.0", markers = "platform_machine  == 'arm64'"}
 numpy = "^1.22.3"
 onnx = "1.10.1"
-onnx2kerastl = "0.0.84.dev2"
-keras-data-format-converter = "0.1.15.dev2"
-leap-model-rebuilder = "0.1.6.dev3"
+onnx2kerastl = "0.0.86"
+keras-data-format-converter = "0.1.14"
+leap-model-rebuilder = "0.1.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 mypy = "^0.941"
 grappa = "^1.0.1"
 pytest-cov = "^3.0.0"
 pytest-watch = "^4.2.0"
```

### Comparing `leap_model_parser-0.1.93.dev3/PKG-INFO` & `leap_model_parser-0.1.94/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: leap-model-parser
-Version: 0.1.93.dev3
+Version: 0.1.94
 Summary: 
 Home-page: https://github.com/tensorleap/leap-model-parser
 License: MIT
 Author: idan
 Author-email: idan.yogev@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: keras-data-format-converter (==0.1.15.dev2)
-Requires-Dist: leap-model-rebuilder (==0.1.6.dev3)
+Requires-Dist: keras-data-format-converter (==0.1.14)
+Requires-Dist: leap-model-rebuilder (==0.1.5)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: onnx (==1.10.1)
-Requires-Dist: onnx2kerastl (==0.0.84.dev2)
-Requires-Dist: tensorflow (==2.12.0) ; platform_machine == "x86_64"
-Requires-Dist: tensorflow-macos (==2.12.0) ; platform_machine == "arm64"
+Requires-Dist: onnx2kerastl (==0.0.86)
+Requires-Dist: tensorflow (==2.11.0) ; platform_machine == "x86_64"
+Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64"
 Project-URL: Repository, https://github.com/tensorleap/leap-model-parser
 Description-Content-Type: text/markdown
 
 # Tensorleap model parser
 Used to parse model to the import format
```

