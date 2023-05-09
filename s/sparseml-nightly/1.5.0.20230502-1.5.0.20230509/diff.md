# Comparing `tmp/sparseml_nightly-1.5.0.20230502-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.5.0.20230509-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,370 +1,370 @@
-Zip file size: 947049 bytes, number of entries: 368
--rw-rw-r--  2.0 unx     1413 b- defN 23-May-02 03:01 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-May-02 03:01 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-May-02 03:01 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-May-02 03:01 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-May-02 03:01 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-May-02 03:01 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17631 b- defN 23-May-02 03:01 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-May-02 03:01 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-May-02 03:01 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-May-02 03:01 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-May-02 03:01 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-May-02 03:01 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-May-02 03:01 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-May-02 03:01 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-May-02 03:01 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-May-02 03:01 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     4751 b- defN 23-May-02 03:01 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2252 b- defN 23-May-02 03:01 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-May-02 03:01 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-May-02 03:01 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-May-02 03:01 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-May-02 03:01 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-May-02 03:01 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-May-02 03:01 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-May-02 03:01 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-May-02 03:01 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-May-02 03:01 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-May-02 03:01 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-May-02 03:01 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-May-02 03:01 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-May-02 03:01 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4470 b- defN 23-May-02 03:01 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4571 b- defN 23-May-02 03:01 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-May-02 03:01 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-May-02 03:01 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-May-02 03:01 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-May-02 03:01 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-May-02 03:01 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-May-02 03:01 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-May-02 03:01 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-May-02 03:01 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-May-02 03:01 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      730 b- defN 23-May-02 03:01 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx     8704 b- defN 23-May-02 03:01 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-May-02 03:01 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-May-02 03:01 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-May-02 03:01 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-May-02 03:01 sparseml/framework/info.py
--rw-rw-r--  2.0 unx      970 b- defN 23-May-02 03:01 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-May-02 03:01 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-May-02 03:01 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-May-02 03:01 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-May-02 03:01 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-May-02 03:01 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-May-02 03:01 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-May-02 03:01 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-May-02 03:01 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-May-02 03:01 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-May-02 03:01 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-May-02 03:01 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-May-02 03:01 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-May-02 03:01 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-May-02 03:01 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-May-02 03:01 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-May-02 03:01 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-May-02 03:01 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-May-02 03:01 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-May-02 03:01 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-May-02 03:01 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-May-02 03:01 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-May-02 03:01 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-May-02 03:01 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-May-02 03:01 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-May-02 03:01 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-May-02 03:01 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-May-02 03:01 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-May-02 03:01 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-May-02 03:01 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-May-02 03:01 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-May-02 03:01 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-May-02 03:01 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-May-02 03:01 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-May-02 03:01 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-May-02 03:01 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-May-02 03:01 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-May-02 03:01 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-May-02 03:01 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-May-02 03:01 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-May-02 03:01 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-May-02 03:01 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-May-02 03:01 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13274 b- defN 23-May-02 03:01 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19634 b- defN 23-May-02 03:01 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-May-02 03:01 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-May-02 03:01 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14520 b- defN 23-May-02 03:01 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-May-02 03:01 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4514 b- defN 23-May-02 03:01 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-May-02 03:01 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-May-02 03:01 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-May-02 03:01 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-May-02 03:01 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-May-02 03:01 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13002 b- defN 23-May-02 03:01 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    16407 b- defN 23-May-02 03:01 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-May-02 03:01 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    41529 b- defN 23-May-02 03:01 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-May-02 03:01 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31586 b- defN 23-May-02 03:01 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-May-02 03:01 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      734 b- defN 23-May-02 03:01 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3694 b- defN 23-May-02 03:01 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-May-02 03:01 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-May-02 03:01 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-May-02 03:01 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-May-02 03:01 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-May-02 03:01 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-May-02 03:01 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-May-02 03:01 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-May-02 03:01 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     1848 b- defN 23-May-02 03:01 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6173 b- defN 23-May-02 03:01 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-May-02 03:01 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10826 b- defN 23-May-02 03:01 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     2814 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-May-02 03:01 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-May-02 03:01 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-May-02 03:01 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-May-02 03:01 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-May-02 03:01 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-May-02 03:01 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-May-02 03:01 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-May-02 03:01 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-May-02 03:01 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-May-02 03:01 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-May-02 03:01 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    20912 b- defN 23-May-02 03:01 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-May-02 03:01 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-May-02 03:01 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-May-02 03:01 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-May-02 03:01 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-May-02 03:01 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-May-02 03:01 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-May-02 03:01 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-May-02 03:01 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-May-02 03:01 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-May-02 03:01 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-May-02 03:01 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-May-02 03:01 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-May-02 03:01 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-May-02 03:01 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-May-02 03:01 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-May-02 03:01 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-May-02 03:01 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-May-02 03:01 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-May-02 03:01 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-May-02 03:01 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-May-02 03:01 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-May-02 03:01 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-May-02 03:01 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-May-02 03:01 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-May-02 03:01 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-May-02 03:01 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-May-02 03:01 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-May-02 03:01 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-May-02 03:01 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-May-02 03:01 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-May-02 03:01 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-May-02 03:01 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-May-02 03:01 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-May-02 03:01 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-May-02 03:01 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-May-02 03:01 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-May-02 03:01 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-May-02 03:01 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-May-02 03:01 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-May-02 03:01 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-May-02 03:01 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-May-02 03:01 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26253 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17591 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    69959 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-May-02 03:01 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      744 b- defN 23-May-02 03:01 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-May-02 03:01 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-May-02 03:01 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-May-02 03:01 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    40790 b- defN 23-May-02 03:01 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-May-02 03:01 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-May-02 03:01 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-May-02 03:01 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-May-02 03:01 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-May-02 03:01 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-May-02 03:01 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31056 b- defN 23-May-02 03:01 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    39284 b- defN 23-May-02 03:01 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-May-02 03:01 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-May-02 03:01 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-May-02 03:01 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-May-02 03:01 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-May-02 03:01 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-May-02 03:01 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-May-02 03:01 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-May-02 03:01 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-May-02 03:01 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-May-02 03:01 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-May-02 03:01 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-May-02 03:01 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-May-02 03:01 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-May-02 03:01 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-May-02 03:01 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-May-02 03:01 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-May-02 03:01 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-May-02 03:01 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-May-02 03:01 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-May-02 03:01 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-May-02 03:01 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-May-02 03:01 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-May-02 03:01 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-May-02 03:01 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-May-02 03:01 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-May-02 03:01 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx      987 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-May-02 03:01 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     4390 b- defN 23-May-02 03:01 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    19721 b- defN 23-May-02 03:01 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30936 b- defN 23-May-02 03:01 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36738 b- defN 23-May-02 03:01 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40358 b- defN 23-May-02 03:01 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34464 b- defN 23-May-02 03:01 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-May-02 03:01 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-May-02 03:01 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    43756 b- defN 23-May-02 03:01 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-May-02 03:01 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-May-02 03:01 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-May-02 03:01 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-May-02 03:01 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    15797 b- defN 23-May-02 03:01 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-May-02 03:01 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-May-02 03:01 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26321 b- defN 23-May-02 03:01 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-May-02 03:01 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-May-02 03:01 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-May-02 03:01 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-May-02 03:01 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-May-02 03:01 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-May-02 03:01 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-May-02 03:01 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-May-02 03:01 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-May-02 03:01 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-May-02 03:01 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-May-02 03:01 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-May-02 03:01 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-May-02 03:01 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-May-02 03:01 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-May-02 03:01 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     3266 b- defN 23-May-02 03:01 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-May-02 03:01 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-May-02 03:01 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-May-02 03:01 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx      958 b- defN 23-May-02 03:01 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5781 b- defN 23-May-02 03:01 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2502 b- defN 23-May-02 03:01 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-May-02 03:01 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7194 b- defN 23-May-02 03:01 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    33979 b- defN 23-May-02 03:01 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2666 b- defN 23-May-02 03:01 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8196 b- defN 23-May-02 03:01 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-May-02 03:01 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6298 b- defN 23-May-02 03:01 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     4041 b- defN 23-May-02 03:01 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-May-02 03:03 sparseml_nightly-1.5.0.20230502.dist-info/LICENSE
--rw-rw-r--  2.0 unx    20659 b- defN 23-May-02 03:03 sparseml_nightly-1.5.0.20230502.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-May-02 03:03 sparseml_nightly-1.5.0.20230502.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-May-02 03:03 sparseml_nightly-1.5.0.20230502.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2372 b- defN 23-May-02 03:03 sparseml_nightly-1.5.0.20230502.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-May-02 03:03 sparseml_nightly-1.5.0.20230502.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    36575 b- defN 23-May-02 03:04 sparseml_nightly-1.5.0.20230502.dist-info/RECORD
-368 files, 3426770 bytes uncompressed, 887841 bytes compressed:  74.1%
+Zip file size: 945872 bytes, number of entries: 368
+-rw-rw-r--  2.0 unx     1413 b- defN 23-May-09 03:01 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-May-09 03:01 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-May-09 03:01 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-May-09 03:01 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-May-09 03:01 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-May-09 03:01 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17631 b- defN 23-May-09 03:01 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-May-09 03:01 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-May-09 03:01 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-May-09 03:01 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-May-09 03:01 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-May-09 03:01 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-May-09 03:01 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-May-09 03:01 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-May-09 03:01 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-May-09 03:01 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     4751 b- defN 23-May-09 03:01 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2252 b- defN 23-May-09 03:01 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-May-09 03:01 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-May-09 03:01 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     3866 b- defN 23-May-09 03:01 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-May-09 03:01 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-May-09 03:01 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-May-09 03:01 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-May-09 03:01 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-May-09 03:01 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-May-09 03:01 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-May-09 03:01 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-May-09 03:01 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-May-09 03:01 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-May-09 03:01 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     4470 b- defN 23-May-09 03:01 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4571 b- defN 23-May-09 03:01 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-May-09 03:01 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-May-09 03:01 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-May-09 03:01 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-May-09 03:01 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-May-09 03:01 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-May-09 03:01 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-May-09 03:01 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-May-09 03:01 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-May-09 03:01 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-May-09 03:01 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx     8704 b- defN 23-May-09 03:01 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-May-09 03:01 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-May-09 03:01 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-May-09 03:01 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-May-09 03:01 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx      970 b- defN 23-May-09 03:01 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-May-09 03:01 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-May-09 03:01 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-May-09 03:01 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-May-09 03:01 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-May-09 03:01 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-May-09 03:01 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-May-09 03:01 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-May-09 03:01 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-May-09 03:01 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-May-09 03:01 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-May-09 03:01 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-May-09 03:01 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-May-09 03:01 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-May-09 03:01 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-May-09 03:01 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-May-09 03:01 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-May-09 03:01 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-May-09 03:01 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-May-09 03:01 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-May-09 03:01 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-May-09 03:01 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-May-09 03:01 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-May-09 03:01 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-May-09 03:01 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-May-09 03:01 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-May-09 03:01 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-May-09 03:01 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-May-09 03:01 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-May-09 03:01 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-May-09 03:01 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-May-09 03:01 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-May-09 03:01 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-May-09 03:01 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-May-09 03:01 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-May-09 03:01 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-May-09 03:01 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-May-09 03:01 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-May-09 03:01 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-May-09 03:01 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-May-09 03:01 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-May-09 03:01 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-May-09 03:01 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13274 b- defN 23-May-09 03:01 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19634 b- defN 23-May-09 03:01 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-May-09 03:01 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-May-09 03:01 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14520 b- defN 23-May-09 03:01 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-May-09 03:01 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4514 b- defN 23-May-09 03:01 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-May-09 03:01 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-May-09 03:01 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-May-09 03:01 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-May-09 03:01 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-May-09 03:01 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13002 b- defN 23-May-09 03:01 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    16407 b- defN 23-May-09 03:01 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-May-09 03:01 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    41529 b- defN 23-May-09 03:01 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-May-09 03:01 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31586 b- defN 23-May-09 03:01 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-May-09 03:01 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      734 b- defN 23-May-09 03:01 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3694 b- defN 23-May-09 03:01 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-May-09 03:01 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-May-09 03:01 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-May-09 03:01 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-May-09 03:01 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-May-09 03:01 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-May-09 03:01 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-May-09 03:01 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-May-09 03:01 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     1848 b- defN 23-May-09 03:01 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6173 b- defN 23-May-09 03:01 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-May-09 03:01 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10826 b- defN 23-May-09 03:01 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     2814 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-May-09 03:01 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-May-09 03:01 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    20912 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-May-09 03:01 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-May-09 03:01 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-May-09 03:01 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-May-09 03:01 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-May-09 03:01 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-May-09 03:01 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-May-09 03:01 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-May-09 03:01 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-May-09 03:01 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-May-09 03:01 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-May-09 03:01 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-May-09 03:01 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-May-09 03:01 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-May-09 03:01 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-May-09 03:01 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-May-09 03:01 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-May-09 03:01 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-May-09 03:01 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-May-09 03:01 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-May-09 03:01 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-May-09 03:01 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-May-09 03:01 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-May-09 03:01 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-May-09 03:01 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-May-09 03:01 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-May-09 03:01 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-May-09 03:01 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-May-09 03:01 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-May-09 03:01 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-May-09 03:01 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-May-09 03:01 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-May-09 03:01 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26253 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17591 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    69959 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      744 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    41409 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-May-09 03:01 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-May-09 03:01 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-May-09 03:01 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-May-09 03:01 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31056 b- defN 23-May-09 03:01 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    39284 b- defN 23-May-09 03:01 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-May-09 03:01 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-May-09 03:01 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-May-09 03:01 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-May-09 03:01 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-May-09 03:01 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-May-09 03:01 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-May-09 03:01 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-May-09 03:01 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-May-09 03:01 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-May-09 03:01 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-May-09 03:01 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-May-09 03:01 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-May-09 03:01 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-May-09 03:01 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-May-09 03:01 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-May-09 03:01 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-May-09 03:01 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-May-09 03:01 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-May-09 03:01 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-May-09 03:01 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-May-09 03:01 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-May-09 03:01 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-May-09 03:01 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-May-09 03:01 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-May-09 03:01 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-May-09 03:01 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx      987 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-May-09 03:01 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    19731 b- defN 23-May-09 03:01 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30936 b- defN 23-May-09 03:01 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36738 b- defN 23-May-09 03:01 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40480 b- defN 23-May-09 03:01 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34530 b- defN 23-May-09 03:01 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-May-09 03:01 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-May-09 03:01 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    43756 b- defN 23-May-09 03:01 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-May-09 03:01 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-May-09 03:01 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-May-09 03:01 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-May-09 03:01 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    15797 b- defN 23-May-09 03:01 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-May-09 03:01 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-May-09 03:01 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26321 b- defN 23-May-09 03:01 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-May-09 03:01 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-May-09 03:01 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-May-09 03:01 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-May-09 03:01 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-May-09 03:01 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-May-09 03:01 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-May-09 03:01 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-May-09 03:01 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-May-09 03:01 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-May-09 03:01 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-May-09 03:01 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-May-09 03:01 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-May-09 03:01 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-May-09 03:01 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-May-09 03:01 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1245 b- defN 23-May-09 03:01 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-May-09 03:01 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-May-09 03:01 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-May-09 03:01 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx      958 b- defN 23-May-09 03:01 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5781 b- defN 23-May-09 03:01 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-May-09 03:01 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-May-09 03:01 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7194 b- defN 23-May-09 03:01 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    34223 b- defN 23-May-09 03:01 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2666 b- defN 23-May-09 03:01 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-May-09 03:01 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-May-09 03:01 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6288 b- defN 23-May-09 03:01 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-May-09 03:01 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21295 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2372 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    36575 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/RECORD
+368 files, 3423373 bytes uncompressed, 886664 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1077,29 +1077,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230502.dist-info/LICENSE
+Filename: sparseml_nightly-1.5.0.20230509.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230502.dist-info/METADATA
+Filename: sparseml_nightly-1.5.0.20230509.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230502.dist-info/NOTICE
+Filename: sparseml_nightly-1.5.0.20230509.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230502.dist-info/WHEEL
+Filename: sparseml_nightly-1.5.0.20230509.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230502.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.5.0.20230509.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230502.dist-info/top_level.txt
+Filename: sparseml_nightly-1.5.0.20230509.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230502.dist-info/RECORD
+Filename: sparseml_nightly-1.5.0.20230509.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/pytorch/torchvision/train.py

```diff
@@ -263,14 +263,16 @@
         random_erase_prob = getattr(args, "random_erase", 0.0)
         ra_magnitude = args.ra_magnitude
         augmix_severity = args.augmix_severity
         dataset = torchvision.datasets.ImageFolder(
             traindir,
             presets.ClassificationPresetTrain(
                 crop_size=train_crop_size,
+                mean=args.rgb_mean,
+                std=args.rgb_std,
                 interpolation=interpolation,
                 auto_augment_policy=auto_augment_policy,
                 random_erase_prob=random_erase_prob,
                 ra_magnitude=ra_magnitude,
                 augmix_severity=augmix_severity,
             ),
         )
@@ -285,14 +287,16 @@
     if args.cache_dataset and os.path.exists(cache_path):
         # Attention, as the transforms are also cached!
         _LOGGER.info(f"Loading dataset_test from {cache_path}")
         dataset_test, _ = torch.load(cache_path)
     else:
         preprocessing = presets.ClassificationPresetEval(
             crop_size=val_crop_size,
+            mean=args.rgb_mean,
+            std=args.rgb_std,
             resize_size=val_resize_size,
             interpolation=interpolation,
         )
 
         dataset_test = torchvision.datasets.ImageFolder(
             valdir,
             preprocessing,
@@ -1208,14 +1212,34 @@
     type=str,
     help=(
         "The architecture key for teacher image classification model; "
         "example: `resnet50`, `mobilenet`. "
         "Note: Will be read from the checkpoint if not specified"
     ),
 )
+@click.option(
+    "--rgb-mean",
+    nargs=3,
+    default=(0.485, 0.456, 0.406),
+    type=float,
+    help=(
+        "RGB mean values used to shift input RGB values; "
+        "Note: Will use ImageNet values if not specified."
+    ),
+)
+@click.option(
+    "--rgb-std",
+    default=(0.229, 0.224, 0.225),
+    nargs=3,
+    type=float,
+    help=(
+        "RGB standard-deviation values used to normalize input RGB values; "
+        "Note: Will use ImageNet values if not specified."
+    ),
+)
 @click.pass_context
 def cli(ctx, **kwargs):
     """
     PyTorch classification training
     """
     if len(ctx.args) > 0:
         raise ValueError(_ARGUMENTS_ERROR.format(ctx.args))
```

## sparseml/transformers/__init__.py

```diff
@@ -16,119 +16,28 @@
 Tools for integrating SparseML with transformers training flows
 """
 
 # flake8: noqa
 
 import logging as _logging
 
-import pkg_resources
 from sparseml.analytics import sparseml_analytics as _analytics
 
 
 _analytics.send_event("python__transformers__init")
 
-_EXPECTED_VERSION = "4.23.1"
-
 
 _LOGGER = _logging.getLogger(__name__)
-_NM_TRANSFORMERS_TAR_TEMPLATE = (
-    "https://github.com/neuralmagic/transformers/releases/download/"
-    "{version}/transformers-4.23.1-py3-none-any.whl"
-)
-_NM_TRANSFORMERS_NIGHTLY = _NM_TRANSFORMERS_TAR_TEMPLATE.format(version="nightly")
-
-
-def _install_transformers_and_deps():
-
-    import subprocess as _subprocess
-    import sys as _sys
-
-    import sparseml as _sparseml
-
-    nm_transformers_release = (
-        "nightly" if not _sparseml.is_release else f"v{_sparseml.version_major_minor}"
-    )
-    transformers_requirement = _NM_TRANSFORMERS_TAR_TEMPLATE.format(
-        version=nm_transformers_release
-    )
-    try:
-        _subprocess.check_call(
-            [
-                _sys.executable,
-                "-m",
-                "pip",
-                "install",
-                transformers_requirement,
-                "datasets<=1.18.4",
-                "scikit-learn",
-                "seqeval",
-            ]
-        )
-
-        import transformers as _transformers
-
-        _LOGGER.info("sparseml-transformers and dependencies successfully installed")
-    except Exception:
-        raise ValueError(
-            "Unable to install and import sparseml-transformers dependencies check "
-            "that transformers is installed, if not, install via "
-            f"`pip install {_NM_TRANSFORMERS_NIGHTLY}`"
-        )
 
 
 def _check_transformers_install():
-    transformers_version = next(
-        (
-            pkg.version
-            for pkg in pkg_resources.working_set
-            if pkg.project_name.lower() == "transformers"
-        ),
-        None,
-    )
-
-    # Either no transformers install is found or wrong version installed
-    if transformers_version != _EXPECTED_VERSION:
-        import os
-
-        if os.getenv("NM_NO_AUTOINSTALL_TRANSFORMERS", False):
-            _LOGGER.warning(
-                "Unable to import, skipping auto installation "
-                "due to NM_NO_AUTOINSTALL_TRANSFORMERS"
-            )
-            # skip any further checks
-            return
-        else:
-            _LOGGER.warning(
-                f"sparseml-transformers v{_EXPECTED_VERSION} installation not "
-                f"detected. Installing  sparseml-transformers v{_EXPECTED_VERSION} "
-                "dependencies if transformers is already  installed in the "
-                "environment, it will be overwritten. Set  environment variable "
-                "NM_NO_AUTOINSTALL_TRANSFORMERS to disable"
-            )
-            _install_transformers_and_deps()
-
-    else:
-        import transformers as _transformers
-
-        # Edge case where user has expected version of transformers installed, but
-        # not the nm integrated one
-        if not _transformers.NM_INTEGRATED:
-            _install_transformers_and_deps()
-            raise RuntimeError(
-                "Installed transformers package has been overwritten with "
-                "sparseml-transformers. Stopping process as this is likely to cause "
-                "import issues. Please re-run command"
-            )
-
-    # re check import after potential install
-    try:
-        import transformers as _transformers
+    # check for NM integration in transformers version
+    import transformers as _transformers
 
-        assert _transformers.NM_INTEGRATED
-    except Exception:
+    if not _transformers.NM_INTEGRATED:
         _LOGGER.warning(
             "the neuralmagic fork of transformers may not be installed. it can be "
             "installed via "
             f"`pip install {_NM_TRANSFORMERS_NIGHTLY}`"
         )
```

## sparseml/transformers/export.py

```diff
@@ -174,15 +174,15 @@
         from sparseml.transformers.token_classification import (
             DataTrainingArguments,
             get_tokenized_token_classification_dataset,
         )
 
         data_training_args = DataTrainingArguments(**data_args)
         return get_tokenized_token_classification_dataset(
-            data_args=data_training_args, tokenizer=tokenizer, model=model
+            data_args=data_training_args, tokenizer=tokenizer, model=model or config
         )
 
     if (
         task == "sequence-classification"
         or task == "glue"
         or task == "sentiment-analysis"
         or task == "text-classification"
```

## sparseml/transformers/text_classification.py

```diff
@@ -493,14 +493,15 @@
             multi_label_preds = (preds_sigmoid > threshold).astype(np.float32)
             label_to_id = _get_label_to_id(
                 data_args=data_args,
                 is_regression=is_regression,
                 label_list=label_list,
                 model=model,
                 num_labels=num_labels,
+                config=config,
             )
             id_to_label = {id_: label for label, id_ in label_to_id.items()}
 
             return multi_label_precision_recall_f1(
                 predictions=multi_label_preds,
                 targets=p.label_ids,
                 id_to_label=id_to_label,
@@ -683,15 +684,15 @@
         is_multi_label_classification,
     )
 
 
 def _get_tokenized_and_preprocessed_raw_datasets(
     config,
     data_args: DataTrainingArguments,
-    model: Module,
+    model: Optional[Module],
     raw_datasets,
     tokenizer: transformers.PreTrainedTokenizerBase,
     teacher_tokenizer=None,
     make_eval_dataset: bool = False,
     do_predict: bool = False,
     do_train: bool = False,
     main_process_func=None,
@@ -701,14 +702,15 @@
         label_column,
         label_list,
         num_labels,
         is_multi_label_classification,
     ) = _get_label_info(data_args, raw_datasets)
 
     train_dataset = predict_dataset = eval_dataset = None
+    config = model.config if model else config
     if not main_process_func:
         main_process_func = lambda desc: nullcontext(desc)  # noqa: E731
 
     # Preprocessing the datasets
     if data_args.input_column_names is not None:
         if "," in data_args.input_column_names:
             # two input columns
@@ -749,23 +751,23 @@
         # We will pad later, dynamically at batch creation, to the max sequence
         # length in each batch
         padding = False
 
     # Some models have set the order of the labels to use, so let's make sure
     # we do use it
     label_to_id = _get_label_to_id(
-        data_args, is_regression, label_list, model, num_labels
+        data_args, is_regression, label_list, model, num_labels, config=config
     )
 
     if label_to_id is not None:
-        model.config.label2id = label_to_id
-        model.config.id2label = {id: label for label, id in config.label2id.items()}
+        config.label2id = label_to_id
+        config.id2label = {id: label for label, id in config.label2id.items()}
     elif data_args.task_name is not None and not is_regression:
-        model.config.label2id = {l: i for i, l in enumerate(label_list)}
-        model.config.id2label = {id: label for label, id in config.label2id.items()}
+        config.label2id = {l: i for i, l in enumerate(label_list)}
+        config.id2label = {id: label for label, id in config.label2id.items()}
 
     max_seq_length = data_args.max_seq_length
     if max_seq_length > tokenizer.model_max_length:
         _LOGGER.warning(
             f"The max_seq_length passed ({max_seq_length}) is larger than "
             f"the maximum length for the model ({tokenizer.model_max_length}). "
             f"Using max_seq_length={tokenizer.model_max_length}."
@@ -837,23 +839,24 @@
         "train": train_dataset,
         "validation": eval_dataset,
         "test": predict_dataset,
     }
     return tokenized_datasets, raw_datasets
 
 
-def _get_label_to_id(data_args, is_regression, label_list, model, num_labels):
+def _get_label_to_id(data_args, is_regression, label_list, model, num_labels, config):
     label_to_id = None
+    config = model.config if model else config
     if (
-        model.config.label2id != PretrainedConfig(num_labels=num_labels).label2id
+        config.label2id != PretrainedConfig(num_labels=num_labels).label2id
         and data_args.task_name is not None
         and not is_regression
     ):
         # Some have all caps in their config, some don't.
-        label_name_to_id = {k.lower(): v for k, v in model.config.label2id.items()}
+        label_name_to_id = {k.lower(): v for k, v in config.label2id.items()}
         if list(sorted(label_name_to_id.keys())) == list(sorted(label_list)):
             label_to_id = {
                 i: int(label_name_to_id[label_list[i]]) for i in range(num_labels)
             }
         else:
             _LOGGER.warning(
                 "Your model seems to have been trained with labels, but they don't "
```

## sparseml/transformers/token_classification.py

```diff
@@ -724,50 +724,51 @@
     return tokenized_dataset
 
 
 def _get_tokenized_dataset(
     data_args: DataTrainingArguments,
     label_list: List,
     labels_are_int: bool,
-    model: Module,
+    model: Module,  # model config object can be passed in as well
     num_labels: int,
     raw_datasets: Union[Dataset, DatasetDict, IterableDatasetDict, IterableDataset],
     tokenizer: transformers.PreTrainedTokenizerBase,
     text_column_name: str,
     label_column_name: str,
     label_to_id: Dict[Any, Any],
     do_train: bool,
     do_eval: bool,
     main_process_func,
     do_predict: bool = False,
 ) -> Dict[str, Any]:
     train_dataset = predict_dataset = eval_dataset = None
+    config = model.config if isinstance(model, Module) else model
     # Model has labels -> use them.
-    if model.config.label2id != PretrainedConfig(num_labels=num_labels).label2id:
-        if list(sorted(model.config.label2id.keys())) == list(sorted(label_list)):
+    if config.label2id != PretrainedConfig(num_labels=num_labels).label2id:
+        if list(sorted(config.label2id.keys())) == list(sorted(label_list)):
             # Reorganize `label_list` to match the ordering of the model.
             if labels_are_int:
                 label_to_id = {
-                    i: int(model.config.label2id[l]) for i, l in enumerate(label_list)
+                    i: int(config.label2id[l]) for i, l in enumerate(label_list)
                 }
-                label_list = [model.config.id2label[i] for i in range(num_labels)]
+                label_list = [config.id2label[i] for i in range(num_labels)]
             else:
-                label_list = [model.config.id2label[i] for i in range(num_labels)]
+                label_list = [config.id2label[i] for i in range(num_labels)]
                 label_to_id = {l: i for i, l in enumerate(label_list)}
         else:
             _LOGGER.warning(
                 "Your model seems to have been trained with labels, but they don't "
                 "match the dataset: ",
-                f"model labels: {list(sorted(model.config.label2id.keys()))}, dataset "
+                f"model labels: {list(sorted(config.label2id.keys()))}, dataset "
                 f"labels: {list(sorted(label_list))}."
                 "\nIgnoring the model labels as a result.",
             )
     # Set the correspondences label/ID inside the model config
-    model.config.label2id = {l: i for i, l in enumerate(label_list)}
-    model.config.id2label = {i: l for i, l in enumerate(label_list)}
+    config.label2id = {l: i for i, l in enumerate(label_list)}
+    config.id2label = {i: l for i, l in enumerate(label_list)}
     # Map that sends B-Xxx label to its I-Xxx counterpart
     b_to_i_label = []
     for idx, label in enumerate(label_list):
         if isinstance(label, str) and (
             label.startswith("B-") and label.replace("B-", "I-") in label_list
         ):
             b_to_i_label.append(label_list.index(label.replace("B-", "I-")))
```

## sparseml/yolov5/__init__.py

```diff
@@ -17,94 +17,27 @@
 """
 # flake8: noqa
 
 import logging as _logging
 
 from sparseml.analytics import sparseml_analytics as _analytics
 
-from .helpers import *
-
 
 _analytics.send_event("python__yolov5__init")
 
-try:
-    import yolov5 as _yolov5
-
-    _yolov5_import_error = None
-except Exception as _yolov5_import_err:
-    _yolov5_import_error = _yolov5_import_err
-
 _LOGGER = _logging.getLogger(__name__)
-_NM_YOLOV5_TAR_TEMPLATE = (
-    "https://github.com/neuralmagic/yolov5/releases/download/"
-    "{version}/yolov5-6.2.0-py3-none-any.whl"
-)
-_NM_YOLOV5_NIGHTLY = _NM_YOLOV5_TAR_TEMPLATE.format(version="nightly")
-
-
-def _install_yolov5_and_deps():
-
-    import subprocess as _subprocess
-    import sys as _sys
-
-    import sparseml as _sparseml
-
-    nm_yolov5_release = (
-        "nightly" if not _sparseml.is_release else f"v{_sparseml.version_major_minor}"
-    )
-
-    yolov5_requirement = _NM_YOLOV5_TAR_TEMPLATE.format(version=nm_yolov5_release)
-
-    try:
-        _subprocess.check_call(
-            [
-                _sys.executable,
-                "-m",
-                "pip",
-                "install",
-                yolov5_requirement,
-            ]
-        )
-
-        import yolov5 as _yolov5
-
-        _LOGGER.info("sparseml-yolov5 and dependencies successfully installed")
-    except Exception:
-        raise ValueError(
-            "Unable to install and import sparseml-yolov5 dependencies check "
-            "that yolov5 is installed, if not, install via "
-            f"`pip install {_NM_YOLOV5_NIGHTLY}`"
-        )
 
 
 def _check_yolov5_install():
-    if _yolov5_import_error is not None:
-        import os
-
-        if os.getenv("NM_NO_AUTOINSTALL_YOLOV5", False):
-            _LOGGER.warning(
-                "Unable to import, skipping auto installation "
-                "due to NM_NO_AUTOINSTALL_YOLOV5"
-            )
-            # skip any further checks
-            return
-        else:
-            _LOGGER.warning(
-                "sparseml-yolov5 installation not detected. Installing "
-                "sparseml-yolov5 dependencies if yolov5 is already "
-                "installed in the environment, it will be overwritten. Set "
-                "environment variable NM_NO_AUTOINSTALL_YOLOV5 to disable"
-            )
-            _install_yolov5_and_deps()
-
-    # re check import after potential install
+    # check nm-yolov5 is installed
     try:
         import yolov5 as _yolov5
     except Exception:
-        _LOGGER.warning(
-            "the neuralmagic fork of yolov5 may not be installed. it can be "
-            "installed via "
-            f"`pip install {_NM_YOLOV5_NIGHTLY}`"
+        raise ImportError(
+            "Unable to import the neuralmagic fork of yolov5 may not be installed. "
+            f"it can be installed via `pip install nn-yolov5`"
         )
 
 
 _check_yolov5_install()
+
+from .helpers import *
```

## sparseml/yolov8/trainers.py

```diff
@@ -24,14 +24,15 @@
 from typing import List, Optional
 
 import onnx
 import torch
 
 from sparseml.optim.helpers import load_recipe_yaml_str
 from sparseml.pytorch.optim.manager import ScheduledModifierManager
+from sparseml.pytorch.sparsification.quantization import skip_onnx_input_quantize
 from sparseml.pytorch.utils import ModuleExporter
 from sparseml.pytorch.utils.helpers import download_framework_model_by_recipe_type
 from sparseml.pytorch.utils.logger import LoggerManager, PythonLogger, WANDBLogger
 from sparseml.yolov8.modules import Bottleneck, Conv
 from sparseml.yolov8.utils import (
     check_coco128_segmentation,
     create_grad_sampler,
@@ -717,15 +718,21 @@
             # ultralytics-specific argument
             do_constant_folding=True,
             output_names=["output0", "output1"]
             if isinstance(self.model, SegmentationModel)
             else ["output0"],
         )
 
-        onnx.checker.check_model(os.path.join(save_dir, name))
+        complete_path = os.path.join(save_dir, name)
+        try:
+            skip_onnx_input_quantize(complete_path, complete_path)
+        except Exception:
+            pass
+
+        onnx.checker.check_model(complete_path)
         deployment_folder = exporter.create_deployment_folder(onnx_model_name=name)
         if args["export_samples"]:
             trainer_config = get_cfg(cfg=DEFAULT_SPARSEML_CONFIG_PATH)
 
             if args["dataset_path"] is not None:
                 args["data"] = data_from_dataset_path(
                     args["data"], args["dataset_path"]
```

## sparseml/yolov8/utils/export_samples.py

```diff
@@ -102,18 +102,23 @@
     )
 
     for batch in data_loader:
         file_idx = f"{exported_samples}".zfill(4)
         preprocessed_batch = preprocess(batch=batch, device=device)
         image = preprocessed_batch["img"]
 
-        # Save inputs as numpy array
-        _export_inputs(image, sample_in_dir, file_idx, save_inputs_as_uint8)
         # Save torch outputs as numpy array
         _export_torch_outputs(image, model, sample_out_dir_torch, file_idx)
+
+        # Convert input data type if needed
+        if save_inputs_as_uint8:
+            image = (255 * image).to(dtype=torch.uint8)
+
+        # Save inputs as numpy array
+        _export_inputs(image, sample_in_dir, file_idx)
         # Save onnxruntime outputs as numpy array
         _export_ort_outputs(
             image.cpu().numpy(), ort_session, sample_out_dir_ort, file_idx
         )
 
         exported_samples += 1
 
@@ -162,21 +167,17 @@
     # preds, interm_out1, interm_out2, interm_out3 = model_out
     preds, *_ = ort_outs
 
     sample_output_filename = os.path.join(sample_out_dir, f"out-{file_idx}.npz")
     numpy.savez(sample_output_filename, preds)
 
 
-def _export_inputs(
-    image: torch.Tensor, sample_in_dir: str, file_idx: str, save_inputs_as_uint8: bool
-):
+def _export_inputs(image: torch.Tensor, sample_in_dir: str, file_idx: str):
 
     sample_in = image.detach().to("cpu")
-    if save_inputs_as_uint8:
-        sample_in = (255 * sample_in).to(dtype=torch.uint8)
 
     sample_input_filename = os.path.join(sample_in_dir, f"inp-{file_idx}.npz")
     numpy.savez(sample_input_filename, sample_in)
 
 
 def _graph_has_uint8_inputs(onnx_path: str) -> bool:
     """
```

## Comparing `sparseml_nightly-1.5.0.20230502.dist-info/LICENSE` & `sparseml_nightly-1.5.0.20230509.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230502.dist-info/METADATA` & `sparseml_nightly-1.5.0.20230509.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.5.0.20230502
+Version: 1.5.0.20230509
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
@@ -95,16 +95,28 @@
 Requires-Dist: gputils ; extra == 'torch_all'
 Requires-Dist: torchvision (<=0.14,>=0.3.0) ; extra == 'torch_all'
 Requires-Dist: torchaudio (<=0.13) ; extra == 'torch_all'
 Provides-Extra: torchvision
 Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'torchvision'
 Requires-Dist: gputils ; extra == 'torchvision'
 Requires-Dist: torchvision (<=0.14,>=0.3.0) ; extra == 'torchvision'
+Provides-Extra: transformers
+Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'transformers'
+Requires-Dist: gputils ; extra == 'transformers'
+Requires-Dist: nm-transformers-nightly (~=1.5.0) ; extra == 'transformers'
+Requires-Dist: datasets (<=1.18.4) ; extra == 'transformers'
+Requires-Dist: scikit-learn ; extra == 'transformers'
+Requires-Dist: seqeval ; extra == 'transformers'
 Provides-Extra: ultralytics
 Requires-Dist: ultralytics (==8.0.30) ; extra == 'ultralytics'
+Provides-Extra: yolov5
+Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'yolov5'
+Requires-Dist: gputils ; extra == 'yolov5'
+Requires-Dist: torchvision (<=0.14,>=0.3.0) ; extra == 'yolov5'
+Requires-Dist: nm-yolov5-nightly (~=1.5.0) ; extra == 'yolov5'
 
 <!--
 Copyright (c) 2021 - present / Neuralmagic, Inc. All Rights Reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

## Comparing `sparseml_nightly-1.5.0.20230502.dist-info/NOTICE` & `sparseml_nightly-1.5.0.20230509.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230502.dist-info/entry_points.txt` & `sparseml_nightly-1.5.0.20230509.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230502.dist-info/RECORD` & `sparseml_nightly-1.5.0.20230509.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 sparseml/pytorch/sparsification/training/modifier_lr.py,sha256=m_tCydo_BHiXCHMUKZu6iqKLAP24acAT8-NLjH9RIlE,24287
 sparseml/pytorch/sparsification/training/modifier_params.py,sha256=G_0eVqu0Cup8WNLFhkfPmYnKtJlNrxcJt0FcOOdq9tA,21497
 sparseml/pytorch/sparsification/training/modifier_regularizer.py,sha256=ezHbcwI8ITgq4vwkzsWXgnq_ls6NONW_D8jEN-YR7u8,6690
 sparseml/pytorch/torchvision/__init__.py,sha256=qPAYUqRxLOdwP3JCQ79MF1N1rXaULmNQLWpqH5osPzY,744
 sparseml/pytorch/torchvision/export_onnx.py,sha256=oiittOzvPEWMBpyldcfX6Yr7GQjKiKkOH4IUX-QQ718,6490
 sparseml/pytorch/torchvision/presets.py,sha256=PMRKjg4sBm6_UdhAV29wSSeOdDR6QlCzjcJbQWSenUA,2870
 sparseml/pytorch/torchvision/sampler.py,sha256=VuebeOVoQWLsafwJEeGgKQrDfF8PxzimHWFLs9odGz8,2530
-sparseml/pytorch/torchvision/train.py,sha256=YwETS0-EgjpGvs9LzKRCbGkcSHh35Mv-iOBJPGatnnM,40790
+sparseml/pytorch/torchvision/train.py,sha256=14gq2sO3_8hKdCm3S5MPA3er7ImeLcbmi1gg3ns6sBs,41409
 sparseml/pytorch/torchvision/transforms.py,sha256=_WfLKV2G9ZLt2zdpKvaHA1ricPGufVIF-lzgKaOL2Ec,7128
 sparseml/pytorch/torchvision/utils.py,sha256=weRmF78Qf9_Kgd-L7aAHERmXKoCVqUP4J8pbSZmav58,16675
 sparseml/pytorch/utils/__init__.py,sha256=WWPrEPVj8YsCZN0JemnAF5z7hOf0nL203uixlqWoAeo,1160
 sparseml/pytorch/utils/benchmarker.py,sha256=Zw1pEj7wDe4ZU_-G0JOCymdLXydN19K1QZKzPJvBp9E,9706
 sparseml/pytorch/utils/callbacks.py,sha256=1z10T8xE0IY5mcL2ARSsHDt6sDWRVF-Nq6zVf9OvD0s,2846
 sparseml/pytorch/utils/distributed.py,sha256=lJtEvgMg6LvH9iUwhveCaWNrx_t7pjn-sOW9rfYViwI,1061
 sparseml/pytorch/utils/exporter.py,sha256=KfoPciN46ZDHKgvVk7oYBR_cyZwihRPNcCm-EvPnpfg,31056
@@ -308,20 +308,20 @@
 sparseml/tensorflow_v1/utils/__init__.py,sha256=FhgTPE_G6lftVrwrOCUghTMxmi_1TbRwOX3TYJt5X7A,967
 sparseml/tensorflow_v1/utils/exporter.py,sha256=RqpSP-w21SrkA_ik9WoIWdIVAAui88AiBXxRWaDZJJs,10913
 sparseml/tensorflow_v1/utils/helpers.py,sha256=40eZgnejvIki_CdupK4V1gETAgGDE9rbEXEwuNg9ASA,996
 sparseml/tensorflow_v1/utils/loss.py,sha256=4AsXh70fjp1dDcxBUzgjjpLgndwVa1CBiMG1sYi5Was,1974
 sparseml/tensorflow_v1/utils/nets_utils.py,sha256=cOTKgw7PVPEjRVU-bvcsNLdBJGTi-A7djJaUaZQwsT4,8119
 sparseml/tensorflow_v1/utils/summary.py,sha256=A2ub7KDwzsaindIuCHa7N3cRpCU6d7QbD5uNHV-R6H8,1327
 sparseml/tensorflow_v1/utils/variable.py,sha256=6ziLaNOLnxQrSPWJ2RaINqg4w-4NK9reVJWH-weK3-k,12536
-sparseml/transformers/__init__.py,sha256=qOQrnlpoWXtpOyp7LEC5d1Xg607wvF3sU6QVfy-_Mwg,4390
-sparseml/transformers/export.py,sha256=JR5cWm0u9pZsn5EiXpJkEZrIHuVLtzSB0js84GsoGn8,19721
+sparseml/transformers/__init__.py,sha256=0nUAFFKl3q3FUyigmXeiqvhuzCFJRZNENVwsm5j2PfY,1327
+sparseml/transformers/export.py,sha256=i5_-92O7N-t0MaNOkYSuzQ87hi9_5E3KdI0BW01R0ZM,19731
 sparseml/transformers/masked_language_modeling.py,sha256=3NVCBveaLUI-BNgTqX5Pm97-apHNFVbyNUDr5z5x1cI,30936
 sparseml/transformers/question_answering.py,sha256=koobYWD4GBcGqWkW1L005QCw4huh5rbFa8rJp_wnWko,36738
-sparseml/transformers/text_classification.py,sha256=9uVAi6vGSl7rF5DHPS005lW0dxOpz2N4ZIXk5-50u8c,40358
-sparseml/transformers/token_classification.py,sha256=6BMBgmEpQvq_RoZzWhLdexQqK4oK9Iv69Qs0IOd-Qds,34464
+sparseml/transformers/text_classification.py,sha256=W1e6gOcQb1vHBdhkDaJwApgFi8n3sWNmmYuKuG7WtVQ,40480
+sparseml/transformers/token_classification.py,sha256=UL1TdVCA3cZglfQNKmiJoULaEXONI4IWpDMpDrM84Q0,34530
 sparseml/transformers/sparsification/__init__.py,sha256=22XZNePvLFXNxp5NrcUIXzjgynCZm6jvQOErpRGlQNY,833
 sparseml/transformers/sparsification/question_answering.py,sha256=FAXhtQ8MW_2ar1dix2tQ1x1RXZuSWMLHZbVHToNWwmo,19529
 sparseml/transformers/sparsification/trainer.py,sha256=g2tP2s_W8Pmpef1CuCIsMD_teRkq9ZRIppR0Uq84Mpw,43756
 sparseml/transformers/sparsification/training_args.py,sha256=gGivIDchLi__PZMNQRmzDOaQcQLkUVFystq3LaVko3Y,1890
 sparseml/transformers/utils/__init__.py,sha256=dxyg6b2XznhBzOsduHdOalgTmoX1JC32Rb4AHns6rVk,794
 sparseml/transformers/utils/helpers.py,sha256=pgxtf0ygP7qJEVPse_dGxm7UpWSJ9JVebA_ex1c8Muw,3090
 sparseml/transformers/utils/metrics.py,sha256=ciZsxgdrzlSMnyzbgKOFE3spWsKql0z82BiYFRXiVOU,2536
@@ -340,29 +340,29 @@
 sparseml/utils/datasets/imagenet.py,sha256=qAL7K6tmlfwBY7FI14wcVb-7g3Rzs4wtZIOV1kvoV0w,23366
 sparseml/utils/datasets/imagenette.py,sha256=AIxAI0wfUqu08XPJ1cG8SNUVocjoeFHVepQZDfsztFI,8967
 sparseml/utils/datasets/voc.py,sha256=CzSEnTe-KqWyOLwleame66PtYqF8vuq9EXaNgmms6u0,1009
 sparseml/yolact/COCO.sh,sha256=Q_1I3VZwS4N1e3AwOoimQH2plK2K0athUDWooWR4ZVQ,1875
 sparseml/yolact/COCO_test.sh,sha256=ZoA_h_68zM8EWF510o24_5xBaQtbJLMHenNjSzldYYc,1418
 sparseml/yolact/__init__.py,sha256=5t9V0aePHnzJBik6z1r4W_3DsSn0lKpYjl3pIuZQft0,4020
 sparseml/yolact/scripts.py,sha256=7GE3xp_B8JJpa2H-Vum6rmiOJHcChyffuno4-yteUUw,1784
-sparseml/yolov5/__init__.py,sha256=k7-HHtzMl2zdGuWrov6hIweSoohqUc_Wi_yKzV89QtQ,3266
+sparseml/yolov5/__init__.py,sha256=MiLIIDpAyJvgX8hMOjVsTfEmU5d9YoN27FIqgvSVjjk,1245
 sparseml/yolov5/helpers.py,sha256=jxzJrgKjsb0PHTeGevKICaL8iBOUzxwZXvPAyGyVE-c,4505
 sparseml/yolov5/scripts.py,sha256=rbVgQ3yNsBCk57BMVh5mKomDHql0S-PkHNGCy_qUfEg,1609
 sparseml/yolov5/yolov5.status.yaml,sha256=4GF6DClV65Qw_1b0J5Ul-B4YFHYQUj34vvqALX8sZFY,1220
 sparseml/yolov8/__init__.py,sha256=4akRvqiJRrRI9kcdXG3rqIiZLWIh7tvA-0zOI2zxO0w,958
 sparseml/yolov8/default.yaml,sha256=lWJc8dKEKS0PWG28pAntMe-kHym5PEXX21h9G-9zZhA,5781
 sparseml/yolov8/export.py,sha256=BN4KFsrYYEfpU8e7icW4rQr4uR4lioNXlY3MII9ecKw,2502
 sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
 sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
-sparseml/yolov8/trainers.py,sha256=Fk33TpRkd_P3-XyY1p3v89_zghTqOespk9QhYKJJhXU,33979
+sparseml/yolov8/trainers.py,sha256=qr6iyYvyJtpTwo0Tbch-sumgMrs7ZjwG5LSBK-ywhIQ,34223
 sparseml/yolov8/val.py,sha256=tWKRybY-ClQ3cqf-9rMZdMwHLrSuyrSFwtqGS_8siq4,2666
 sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
-sparseml/yolov8/utils/export_samples.py,sha256=YbiV_0cv_W0xrhtZLg6ActLeSRYYikrOzHz0FqJ0LII,6298
+sparseml/yolov8/utils/export_samples.py,sha256=gn7et_J-OfnCTEYP0iLXx2W-HARgxqUnHqJWHBG72KM,6288
 sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
-sparseml_nightly-1.5.0.20230502.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.5.0.20230502.dist-info/METADATA,sha256=1vz03_VUXJ-Ar3W-X2vVQTShYaU5RKUkRQI8ymTEdK4,20659
-sparseml_nightly-1.5.0.20230502.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.5.0.20230502.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.5.0.20230502.dist-info/entry_points.txt,sha256=vz4Edi7tfmTpoq62ETf5EYJWKHltDxcPz-6GlJ8iVlI,2372
-sparseml_nightly-1.5.0.20230502.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.5.0.20230502.dist-info/RECORD,,
+sparseml_nightly-1.5.0.20230509.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.5.0.20230509.dist-info/METADATA,sha256=P4Q7V5Pbt2HCwFOkWKRy2J3CSoQwmjpanfM84ISKjbM,21295
+sparseml_nightly-1.5.0.20230509.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.5.0.20230509.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.5.0.20230509.dist-info/entry_points.txt,sha256=vz4Edi7tfmTpoq62ETf5EYJWKHltDxcPz-6GlJ8iVlI,2372
+sparseml_nightly-1.5.0.20230509.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.5.0.20230509.dist-info/RECORD,,
```

