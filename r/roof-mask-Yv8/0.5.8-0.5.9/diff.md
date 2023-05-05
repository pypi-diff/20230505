# Comparing `tmp/roof_mask_Yv8-0.5.8.tar.gz` & `tmp/roof_mask_Yv8-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roof_mask_Yv8-0.5.8.tar", last modified: Fri Apr 28 21:02:22 2023, max compression
+gzip compressed data, was "roof_mask_Yv8-0.5.9.tar", last modified: Fri May  5 19:35:23 2023, max compression
```

## Comparing `roof_mask_Yv8-0.5.8.tar` & `roof_mask_Yv8-0.5.9.tar`

### file list

```diff
@@ -1,303 +1,303 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:39.966410 roof_mask_Yv8-0.5.8/
--rwxrwxrwx   0 root         (0) root         (0)      149 2023-04-27 19:14:59.000000 roof_mask_Yv8-0.5.8/.gitignore
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-20 18:44:18.000000 roof_mask_Yv8-0.5.8/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      473 2023-04-28 21:02:21.955967 roof_mask_Yv8-0.5.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.015382 roof_mask_Yv8-0.5.8/detectron2/
--rwxrwxrwx   0 root         (0) root         (0)      258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.080345 roof_mask_Yv8-0.5.8/detectron2/checkpoint/
--rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/checkpoint/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    17782 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/checkpoint/c2_model_loading.py
--rwxrwxrwx   0 root         (0) root         (0)     5685 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/checkpoint/catalog.py
--rwxrwxrwx   0 root         (0) root         (0)     5258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/checkpoint/detection_checkpoint.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.145308 roof_mask_Yv8-0.5.8/detectron2/config/
--rwxrwxrwx   0 root         (0) root         (0)      599 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/config/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7890 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/config/compat.py
--rwxrwxrwx   0 root         (0) root         (0)     9211 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/config/config.py
--rwxrwxrwx   0 root         (0) root         (0)    29512 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/config/defaults.py
--rwxrwxrwx   0 root         (0) root         (0)     2719 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/config/instantiate.py
--rwxrwxrwx   0 root         (0) root         (0)    14944 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/config/lazy.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.204274 roof_mask_Yv8-0.5.8/detectron2/data/
--rwxrwxrwx   0 root         (0) root         (0)      644 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7378 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/data/benchmark.py
--rwxrwxrwx   0 root         (0) root         (0)    20605 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/data/build.py
--rwxrwxrwx   0 root         (0) root         (0)     7224 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/data/catalog.py
--rwxrwxrwx   0 root         (0) root         (0)     9164 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/data/common.py
--rwxrwxrwx   0 root         (0) root         (0)     8169 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.8/detectron2/data/dataset_mapper.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.267238 roof_mask_Yv8-0.5.8/detectron2/data/datasets/
--rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/README.md
--rwxrwxrwx   0 root         (0) root         (0)      523 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10174 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/builtin.py
--rwxrwxrwx   0 root         (0) root         (0)    21841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/builtin_meta.py
--rwxrwxrwx   0 root         (0) root         (0)    13167 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/cityscapes.py
--rwxrwxrwx   0 root         (0) root         (0)     7821 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/cityscapes_panoptic.py
--rwxrwxrwx   0 root         (0) root         (0)    23465 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/coco.py
--rwxrwxrwx   0 root         (0) root         (0)     8977 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/coco_panoptic.py
--rwxrwxrwx   0 root         (0) root         (0)     9623 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis.py
--rwxrwxrwx   0 root         (0) root         (0)   223757 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis_v0_5_categories.py
--rwxrwxrwx   0 root         (0) root         (0)   219177 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis_v1_categories.py
--rwxrwxrwx   0 root         (0) root         (0)    39414 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis_v1_category_image_count.py
--rwxrwxrwx   0 root         (0) root         (0)     3128 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/pascal_voc.py
--rwxrwxrwx   0 root         (0) root         (0)      169 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/datasets/register_coco.py
--rwxrwxrwx   0 root         (0) root         (0)    22841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/detection_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.341196 roof_mask_Yv8-0.5.8/detectron2/data/samplers/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/samplers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11789 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/samplers/distributed_sampler.py
--rwxrwxrwx   0 root         (0) root         (0)     1944 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/samplers/grouped_batch_sampler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.415153 roof_mask_Yv8-0.5.8/detectron2/data/transforms/
--rwxrwxrwx   0 root         (0) root         (0)      466 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/transforms/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14117 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/transforms/augmentation.py
--rwxrwxrwx   0 root         (0) root         (0)    23069 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/transforms/augmentation_impl.py
--rwxrwxrwx   0 root         (0) root         (0)    12629 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/data/transforms/transform.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.469122 roof_mask_Yv8-0.5.8/detectron2/engine/
--rwxrwxrwx   0 root         (0) root         (0)      340 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/engine/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    26868 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/engine/defaults.py
--rwxrwxrwx   0 root         (0) root         (0)    25497 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/engine/hooks.py
--rwxrwxrwx   0 root         (0) root         (0)     4089 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/engine/launch.py
--rwxrwxrwx   0 root         (0) root         (0)    14104 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/engine/train_loop.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.536084 roof_mask_Yv8-0.5.8/detectron2/evaluation/
--rwxrwxrwx   0 root         (0) root         (0)      671 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8369 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/cityscapes_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)    30423 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/coco_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     8156 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/evaluator.py
--rwxrwxrwx   0 root         (0) root         (0)     5078 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/fast_eval_api.py
--rwxrwxrwx   0 root         (0) root         (0)    15018 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/lvis_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     7500 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/panoptic_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)    10862 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/pascal_voc_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     7608 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/rotated_coco_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     8191 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/sem_seg_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     2614 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/evaluation/testing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.612041 roof_mask_Yv8-0.5.8/detectron2/export/
--rwxrwxrwx   0 root         (0) root         (0)      513 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/README.md
--rwxrwxrwx   0 root         (0) root         (0)      336 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9280 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/api.py
--rwxrwxrwx   0 root         (0) root         (0)    21035 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/c10.py
--rwxrwxrwx   0 root         (0) root         (0)     7803 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/caffe2_export.py
--rwxrwxrwx   0 root         (0) root         (0)     6674 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/caffe2_inference.py
--rwxrwxrwx   0 root         (0) root         (0)    17034 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/caffe2_modeling.py
--rwxrwxrwx   0 root         (0) root         (0)     5033 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/caffe2_patch.py
--rwxrwxrwx   0 root         (0) root         (0)    11807 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/flatten.py
--rwxrwxrwx   0 root         (0) root         (0)    38071 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/shared.py
--rwxrwxrwx   0 root         (0) root         (0)     5008 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/torchscript.py
--rwxrwxrwx   0 root         (0) root         (0)    11526 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/export/torchscript_patch.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.696993 roof_mask_Yv8-0.5.8/detectron2/layers/
--rwxrwxrwx   0 root         (0) root         (0)      839 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5764 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/aspp.py
--rwxrwxrwx   0 root         (0) root         (0)    12131 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/batch_norm.py
--rwxrwxrwx   0 root         (0) root         (0)     3024 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/blocks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.776947 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/
--rwxrwxrwx   0 root         (0) root         (0)      122 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.857900 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/
--rwxrwxrwx   0 root         (0) root         (0)     2870 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated.h
--rwxrwxrwx   0 root         (0) root         (0)    16031 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cpu.cpp
--rwxrwxrwx   0 root         (0) root         (0)    13876 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cuda.cu
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:40.933856 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/
--rwxrwxrwx   0 root         (0) root         (0)      988 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated.h
--rwxrwxrwx   0 root         (0) root         (0)     1090 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cpu.cpp
--rwxrwxrwx   0 root         (0) root         (0)     4454 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cuda.cu
--rwxrwxrwx   0 root         (0) root         (0)    10844 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_utils.h
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.238682 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cocoeval/
--rwxrwxrwx   0 root         (0) root         (0)    20746 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cocoeval/cocoeval.cpp
--rwxrwxrwx   0 root         (0) root         (0)     3515 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cocoeval/cocoeval.h
--rwxrwxrwx   0 root         (0) root         (0)      622 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cuda_version.cu
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.307643 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/
--rwxrwxrwx   0 root         (0) root         (0)     8384 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/deform_conv.h
--rwxrwxrwx   0 root         (0) root         (0)    31785 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/deform_conv_cuda.cu
--rwxrwxrwx   0 root         (0) root         (0)    44279 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/deform_conv_cuda_kernel.cu
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.368609 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/
--rwxrwxrwx   0 root         (0) root         (0)     1089 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/nms_rotated.h
--rwxrwxrwx   0 root         (0) root         (0)     2307 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/nms_rotated_cpu.cpp
--rwxrwxrwx   0 root         (0) root         (0)     4859 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/nms_rotated_cuda.cu
--rwxrwxrwx   0 root         (0) root         (0)     3167 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/csrc/vision.cpp
--rwxrwxrwx   0 root         (0) root         (0)    16978 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/deform_conv.py
--rwxrwxrwx   0 root         (0) root         (0)     4204 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/losses.py
--rwxrwxrwx   0 root         (0) root         (0)    10881 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/mask_ops.py
--rwxrwxrwx   0 root         (0) root         (0)     6490 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/nms.py
--rwxrwxrwx   0 root         (0) root         (0)     3098 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/roi_align.py
--rwxrwxrwx   0 root         (0) root         (0)     3302 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/roi_align_rotated.py
--rwxrwxrwx   0 root         (0) root         (0)      652 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/rotated_boxes.py
--rwxrwxrwx   0 root         (0) root         (0)      661 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/shape_spec.py
--rwxrwxrwx   0 root         (0) root         (0)     4893 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/layers/wrappers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.416581 roof_mask_Yv8-0.5.8/detectron2/modeling/
--rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15443 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/anchor_generator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.485541 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/
--rwxrwxrwx   0 root         (0) root         (0)      475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1543 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/backbone.py
--rwxrwxrwx   0 root         (0) root         (0)     1015 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/build.py
--rwxrwxrwx   0 root         (0) root         (0)    10055 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/fpn.py
--rwxrwxrwx   0 root         (0) root         (0)    16656 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/regnet.py
--rwxrwxrwx   0 root         (0) root         (0)    23658 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/resnet.py
--rwxrwxrwx   0 root         (0) root         (0)    15123 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/box_regression.py
--rwxrwxrwx   0 root         (0) root         (0)     6264 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/matcher.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.546506 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/
--rwxrwxrwx   0 root         (0) root         (0)      508 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      814 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/build.py
--rwxrwxrwx   0 root         (0) root         (0)    11550 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/dense_detector.py
--rwxrwxrwx   0 root         (0) root         (0)    13213 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/fcos.py
--rwxrwxrwx   0 root         (0) root         (0)    10335 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/panoptic_fpn.py
--rwxrwxrwx   0 root         (0) root         (0)    13710 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    18265 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/retinanet.py
--rwxrwxrwx   0 root         (0) root         (0)     9720 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/semantic_seg.py
--rwxrwxrwx   0 root         (0) root         (0)    10832 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/mmdet_wrapper.py
--rwxrwxrwx   0 root         (0) root         (0)    11316 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/poolers.py
--rwxrwxrwx   0 root         (0) root         (0)     4046 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/postprocessing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.609471 roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/
--rwxrwxrwx   0 root         (0) root         (0)      231 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      836 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/build.py
--rwxrwxrwx   0 root         (0) root         (0)     8128 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/proposal_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    23814 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/rpn.py
--rwxrwxrwx   0 root         (0) root         (0)     8807 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/rrpn.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.676432 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/
--rwxrwxrwx   0 root         (0) root         (0)      768 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4077 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/box_head.py
--rwxrwxrwx   0 root         (0) root         (0)    12990 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/cascade_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    25274 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/fast_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    11156 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/keypoint_head.py
--rwxrwxrwx   0 root         (0) root         (0)    12169 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/mask_head.py
--rwxrwxrwx   0 root         (0) root         (0)    37701 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/roi_heads.py
--rwxrwxrwx   0 root         (0) root         (0)    11158 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)     2334 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/sampling.py
--rwxrwxrwx   0 root         (0) root         (0)    12416 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/modeling/test_time_augmentation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.730401 roof_mask_Yv8-0.5.8/detectron2/solver/
--rwxrwxrwx   0 root         (0) root         (0)      298 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/solver/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11127 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/solver/build.py
--rwxrwxrwx   0 root         (0) root         (0)     8648 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.8/detectron2/solver/lr_scheduler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.812354 roof_mask_Yv8-0.5.8/detectron2/structures/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14429 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/boxes.py
--rwxrwxrwx   0 root         (0) root         (0)     4557 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/image_list.py
--rwxrwxrwx   0 root         (0) root         (0)     6542 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/instances.py
--rwxrwxrwx   0 root         (0) root         (0)     9030 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/keypoints.py
--rwxrwxrwx   0 root         (0) root         (0)    19802 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/masks.py
--rwxrwxrwx   0 root         (0) root         (0)    18853 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/structures/rotated_boxes.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.876318 roof_mask_Yv8-0.5.8/detectron2/tracking/
--rwxrwxrwx   0 root         (0) root         (0)      580 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2216 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/base_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)    11858 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/bbox_iou_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     7486 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/hungarian_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     4142 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     1106 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     5288 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.946280 roof_mask_Yv8-0.5.8/detectron2/utils/
--rwxrwxrwx   0 root         (0) root         (0)      175 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/README.md
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-04-18 18:45:50.000000 roof_mask_Yv8-0.5.8/detectron2/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6017 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.8/detectron2/utils/analysis.py
--rwxrwxrwx   0 root         (0) root         (0)     8391 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.8/detectron2/utils/collect_env.py
--rwxrwxrwx   0 root         (0) root         (0)     4096 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.8/detectron2/utils/colormap.py
--rwxrwxrwx   0 root         (0) root         (0)     5610 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.8/detectron2/utils/comm.py
--rwxrwxrwx   0 root         (0) root         (0)     1838 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.8/detectron2/utils/develop.py
--rwxrwxrwx   0 root         (0) root         (0)     5644 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.8/detectron2/utils/env.py
--rwxrwxrwx   0 root         (0) root         (0)    17024 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/events.py
--rwxrwxrwx   0 root         (0) root         (0)     1189 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/file_io.py
--rwxrwxrwx   0 root         (0) root         (0)     7807 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2583 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/memory.py
--rwxrwxrwx   0 root         (0) root         (0)     1874 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/registry.py
--rwxrwxrwx   0 root         (0) root         (0)     1064 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/serialize.py
--rwxrwxrwx   0 root         (0) root         (0)     4833 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/testing.py
--rwxrwxrwx   0 root         (0) root         (0)    11319 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/video_visualizer.py
--rwxrwxrwx   0 root         (0) root         (0)    51159 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/visualizer.py
--rwxrwxrwx   0 root         (0) root         (0)    52915 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.8/detectron2/utils/visualizer_new.py
--rwxrwxrwx   0 root         (0) root         (0)      107 2023-04-17 21:19:17.000000 roof_mask_Yv8-0.5.8/readme.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:41.991252 roof_mask_Yv8-0.5.8/roof_mask_Yv8.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      473 2023-04-28 21:01:37.000000 roof_mask_Yv8-0.5.8/roof_mask_Yv8.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     9347 2023-04-28 21:01:39.000000 roof_mask_Yv8-0.5.8/roof_mask_Yv8.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-28 21:01:37.000000 roof_mask_Yv8-0.5.8/roof_mask_Yv8.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-28 21:01:37.000000 roof_mask_Yv8-0.5.8/roof_mask_Yv8.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.062211 roof_mask_Yv8-0.5.8/scoring/
--rwxrwxrwx   0 root         (0) root         (0)     4374 2023-04-27 20:39:18.000000 roof_mask_Yv8-0.5.8/scoring/score_yolov8.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-28 21:02:22.035967 roof_mask_Yv8-0.5.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      632 2023-04-28 21:01:16.000000 roof_mask_Yv8-0.5.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.138168 roof_mask_Yv8-0.5.8/ultralytics/
--rwxrwxrwx   0 root         (0) root         (0)      295 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.214124 roof_mask_Yv8-0.5.8/ultralytics/hub/
--rwxrwxrwx   0 root         (0) root         (0)     3421 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/hub/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5206 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/hub/auth.py
--rwxrwxrwx   0 root         (0) root         (0)     8690 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/hub/session.py
--rwxrwxrwx   0 root         (0) root         (0)     9723 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/hub/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.274090 roof_mask_Yv8-0.5.8/ultralytics/nn/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/nn/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    24083 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/nn/autobackend.py
--rwxrwxrwx   0 root         (0) root         (0)    11839 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/nn/autoshape.py
--rwxrwxrwx   0 root         (0) root         (0)    20062 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/nn/modules.py
--rwxrwxrwx   0 root         (0) root         (0)    26619 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/nn/tasks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.332057 roof_mask_Yv8-0.5.8/ultralytics/yolo/
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.399019 roof_mask_Yv8-0.5.8/ultralytics/yolo/cfg/
--rwxrwxrwx   0 root         (0) root         (0)    17582 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/cfg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6237 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/cfg/default.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.461983 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/
--rwxrwxrwx   0 root         (0) root         (0)      483 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    31285 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/augment.py
--rwxrwxrwx   0 root         (0) root         (0)     8919 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/base.py
--rwxrwxrwx   0 root         (0) root         (0)     8614 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/build.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.526945 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15194 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rwxrwxrwx   0 root         (0) root         (0)    17226 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rwxrwxrwx   0 root         (0) root         (0)    49861 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/v5loader.py
--rwxrwxrwx   0 root         (0) root         (0)    12740 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataset_wrappers.py
--rwxrwxrwx   0 root         (0) root         (0)    22728 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/data/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.573919 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    41854 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/exporter.py
--rwxrwxrwx   0 root         (0) root         (0)    21469 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/model.py
--rwxrwxrwx   0 root         (0) root         (0)    14720 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/predictor.py
--rwxrwxrwx   0 root         (0) root         (0)    17378 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/results.py
--rwxrwxrwx   0 root         (0) root         (0)    29843 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/trainer.py
--rwxrwxrwx   0 root         (0) root         (0)    10358 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/validator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.630886 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/
--rwxrwxrwx   0 root         (0) root         (0)    25215 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3823 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/autobatch.py
--rwxrwxrwx   0 root         (0) root         (0)     5414 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/benchmarks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.696849 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/
--rwxrwxrwx   0 root         (0) root         (0)      171 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3783 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/base.py
--rwxrwxrwx   0 root         (0) root         (0)     5286 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/clearml.py
--rwxrwxrwx   0 root         (0) root         (0)    11929 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/comet.py
--rwxrwxrwx   0 root         (0) root         (0)     3189 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/hub.py
--rwxrwxrwx   0 root         (0) root         (0)     2512 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/mlflow.py
--rwxrwxrwx   0 root         (0) root         (0)      385 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/raytune.py
--rwxrwxrwx   0 root         (0) root         (0)     1297 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/tensorboard.py
--rwxrwxrwx   0 root         (0) root         (0)     1593 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/wb.py
--rwxrwxrwx   0 root         (0) root         (0)    14190 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/checks.py
--rwxrwxrwx   0 root         (0) root         (0)     2412 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/dist.py
--rwxrwxrwx   0 root         (0) root         (0)    10052 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/downloads.py
--rwxrwxrwx   0 root         (0) root         (0)      251 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/errors.py
--rwxrwxrwx   0 root         (0) root         (0)     3105 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/files.py
--rwxrwxrwx   0 root         (0) root         (0)    11394 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/instance.py
--rwxrwxrwx   0 root         (0) root         (0)     2889 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/loss.py
--rwxrwxrwx   0 root         (0) root         (0)    35693 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/metrics.py
--rwxrwxrwx   0 root         (0) root         (0)    28503 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/ops.py
--rwxrwxrwx   0 root         (0) root         (0)    20613 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/plotting.py
--rwxrwxrwx   0 root         (0) root         (0)    10233 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/tal.py
--rwxrwxrwx   0 root         (0) root         (0)    19694 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/torch_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     2302 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/tuner.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.748818 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/
--rwxrwxrwx   0 root         (0) root         (0)      157 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.804786 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/
--rwxrwxrwx   0 root         (0) root         (0)      390 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1459 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/predict.py
--rwxrwxrwx   0 root         (0) root         (0)     6388 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/train.py
--rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/val.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.873747 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/
--rwxrwxrwx   0 root         (0) root         (0)      276 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2005 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/predict.py
--rwxrwxrwx   0 root         (0) root         (0)     9886 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/train.py
--rwxrwxrwx   0 root         (0) root         (0)    12516 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/val.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.933713 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/
--rwxrwxrwx   0 root         (0) root         (0)      246 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2076 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/predict.py
--rwxrwxrwx   0 root         (0) root         (0)     7145 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/train.py
--rwxrwxrwx   0 root         (0) root         (0)    10050 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/val.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:42.999675 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/
--rwxrwxrwx   0 root         (0) root         (0)      294 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2657 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/predict.py
--rwxrwxrwx   0 root         (0) root         (0)     7664 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/train.py
--rwxrwxrwx   0 root         (0) root         (0)    11922 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/val.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 21:01:43.049647 roof_mask_Yv8-0.5.8/yolo_roof/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.8/yolo_roof/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    34971 2023-04-27 21:40:20.000000 roof_mask_Yv8-0.5.8/yolo_roof/detect_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    21398 2023-04-21 14:28:18.000000 roof_mask_Yv8-0.5.8/yolo_roof/geo_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    49443 2023-04-28 19:31:42.000000 roof_mask_Yv8-0.5.8/yolo_roof/report_functions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:46.947111 roof_mask_Yv8-0.5.9/
+-rwxrwxrwx   0 root         (0) root         (0)      184 2023-05-03 19:47:33.000000 roof_mask_Yv8-0.5.9/.gitignore
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-04-20 18:44:18.000000 roof_mask_Yv8-0.5.9/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      473 2023-05-05 19:35:23.095466 roof_mask_Yv8-0.5.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:46.994084 roof_mask_Yv8-0.5.9/detectron2/
+-rwxrwxrwx   0 root         (0) root         (0)      258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.054049 roof_mask_Yv8-0.5.9/detectron2/checkpoint/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/checkpoint/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17782 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/checkpoint/c2_model_loading.py
+-rwxrwxrwx   0 root         (0) root         (0)     5685 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/checkpoint/catalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     5258 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.118013 roof_mask_Yv8-0.5.9/detectron2/config/
+-rwxrwxrwx   0 root         (0) root         (0)      599 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/config/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7890 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/config/compat.py
+-rwxrwxrwx   0 root         (0) root         (0)     9211 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/config/config.py
+-rwxrwxrwx   0 root         (0) root         (0)    29512 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/config/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)     2719 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/config/instantiate.py
+-rwxrwxrwx   0 root         (0) root         (0)    14944 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/config/lazy.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.169983 roof_mask_Yv8-0.5.9/detectron2/data/
+-rwxrwxrwx   0 root         (0) root         (0)      644 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7378 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/data/benchmark.py
+-rwxrwxrwx   0 root         (0) root         (0)    20605 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/data/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     7224 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/data/catalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     9164 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/data/common.py
+-rwxrwxrwx   0 root         (0) root         (0)     8169 2023-04-17 21:04:23.000000 roof_mask_Yv8-0.5.9/detectron2/data/dataset_mapper.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.223953 roof_mask_Yv8-0.5.9/detectron2/data/datasets/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      523 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10174 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/builtin.py
+-rwxrwxrwx   0 root         (0) root         (0)    21841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/builtin_meta.py
+-rwxrwxrwx   0 root         (0) root         (0)    13167 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/cityscapes.py
+-rwxrwxrwx   0 root         (0) root         (0)     7821 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/cityscapes_panoptic.py
+-rwxrwxrwx   0 root         (0) root         (0)    23465 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/coco.py
+-rwxrwxrwx   0 root         (0) root         (0)     8977 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/coco_panoptic.py
+-rwxrwxrwx   0 root         (0) root         (0)     9623 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/lvis.py
+-rwxrwxrwx   0 root         (0) root         (0)   223757 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/lvis_v0_5_categories.py
+-rwxrwxrwx   0 root         (0) root         (0)   219177 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/lvis_v1_categories.py
+-rwxrwxrwx   0 root         (0) root         (0)    39414 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rwxrwxrwx   0 root         (0) root         (0)     3128 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/pascal_voc.py
+-rwxrwxrwx   0 root         (0) root         (0)      169 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/datasets/register_coco.py
+-rwxrwxrwx   0 root         (0) root         (0)    22841 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/detection_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.274924 roof_mask_Yv8-0.5.9/detectron2/data/samplers/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/samplers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11789 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/samplers/distributed_sampler.py
+-rwxrwxrwx   0 root         (0) root         (0)     1944 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.332891 roof_mask_Yv8-0.5.9/detectron2/data/transforms/
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/transforms/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14117 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/transforms/augmentation.py
+-rwxrwxrwx   0 root         (0) root         (0)    23069 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/transforms/augmentation_impl.py
+-rwxrwxrwx   0 root         (0) root         (0)    12629 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/data/transforms/transform.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.379864 roof_mask_Yv8-0.5.9/detectron2/engine/
+-rwxrwxrwx   0 root         (0) root         (0)      340 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/engine/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    26868 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/engine/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)    25497 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/engine/hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)     4089 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/engine/launch.py
+-rwxrwxrwx   0 root         (0) root         (0)    14104 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/engine/train_loop.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.434833 roof_mask_Yv8-0.5.9/detectron2/evaluation/
+-rwxrwxrwx   0 root         (0) root         (0)      671 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/evaluation/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8369 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/evaluation/cityscapes_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)    30423 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/evaluation/coco_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     8156 2023-04-17 21:04:24.000000 roof_mask_Yv8-0.5.9/detectron2/evaluation/evaluator.py
+-rwxrwxrwx   0 root         (0) root         (0)     5078 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/evaluation/fast_eval_api.py
+-rwxrwxrwx   0 root         (0) root         (0)    15018 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/evaluation/lvis_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     7500 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/evaluation/panoptic_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)    10862 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/evaluation/pascal_voc_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     7608 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/evaluation/rotated_coco_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     8191 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/evaluation/sem_seg_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     2614 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/evaluation/testing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.491801 roof_mask_Yv8-0.5.9/detectron2/export/
+-rwxrwxrwx   0 root         (0) root         (0)      513 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/export/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      336 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9280 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/export/api.py
+-rwxrwxrwx   0 root         (0) root         (0)    21035 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/export/c10.py
+-rwxrwxrwx   0 root         (0) root         (0)     7803 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/export/caffe2_export.py
+-rwxrwxrwx   0 root         (0) root         (0)     6674 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/export/caffe2_inference.py
+-rwxrwxrwx   0 root         (0) root         (0)    17034 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/export/caffe2_modeling.py
+-rwxrwxrwx   0 root         (0) root         (0)     5033 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/export/caffe2_patch.py
+-rwxrwxrwx   0 root         (0) root         (0)    11807 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/export/flatten.py
+-rwxrwxrwx   0 root         (0) root         (0)    38071 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/export/shared.py
+-rwxrwxrwx   0 root         (0) root         (0)     5008 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/export/torchscript.py
+-rwxrwxrwx   0 root         (0) root         (0)    11526 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/export/torchscript_patch.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.550767 roof_mask_Yv8-0.5.9/detectron2/layers/
+-rwxrwxrwx   0 root         (0) root         (0)      839 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/layers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5764 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/layers/aspp.py
+-rwxrwxrwx   0 root         (0) root         (0)    12131 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/layers/batch_norm.py
+-rwxrwxrwx   0 root         (0) root         (0)     3024 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/layers/blocks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.605736 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/
+-rwxrwxrwx   0 root         (0) root         (0)      122 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.682692 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/ROIAlignRotated/
+-rwxrwxrwx   0 root         (0) root         (0)     2870 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated.h
+-rwxrwxrwx   0 root         (0) root         (0)    16031 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cpu.cpp
+-rwxrwxrwx   0 root         (0) root         (0)    13876 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cuda.cu
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.727666 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/box_iou_rotated/
+-rwxrwxrwx   0 root         (0) root         (0)      988 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated.h
+-rwxrwxrwx   0 root         (0) root         (0)     1090 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cpu.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     4454 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cuda.cu
+-rwxrwxrwx   0 root         (0) root         (0)    10844 2023-04-17 21:04:25.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_utils.h
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.791630 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/cocoeval/
+-rwxrwxrwx   0 root         (0) root         (0)    20746 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/cocoeval/cocoeval.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     3515 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/cocoeval/cocoeval.h
+-rwxrwxrwx   0 root         (0) root         (0)      622 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/cuda_version.cu
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.842601 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/deformable/
+-rwxrwxrwx   0 root         (0) root         (0)     8384 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/deformable/deform_conv.h
+-rwxrwxrwx   0 root         (0) root         (0)    31785 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/deformable/deform_conv_cuda.cu
+-rwxrwxrwx   0 root         (0) root         (0)    44279 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/deformable/deform_conv_cuda_kernel.cu
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.901568 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/nms_rotated/
+-rwxrwxrwx   0 root         (0) root         (0)     1089 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/nms_rotated/nms_rotated.h
+-rwxrwxrwx   0 root         (0) root         (0)     2307 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/nms_rotated/nms_rotated_cpu.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     4859 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/nms_rotated/nms_rotated_cuda.cu
+-rwxrwxrwx   0 root         (0) root         (0)     3167 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/csrc/vision.cpp
+-rwxrwxrwx   0 root         (0) root         (0)    16978 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/deform_conv.py
+-rwxrwxrwx   0 root         (0) root         (0)     4204 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/losses.py
+-rwxrwxrwx   0 root         (0) root         (0)    10881 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/mask_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)     6490 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/nms.py
+-rwxrwxrwx   0 root         (0) root         (0)     3098 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/roi_align.py
+-rwxrwxrwx   0 root         (0) root         (0)     3302 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/roi_align_rotated.py
+-rwxrwxrwx   0 root         (0) root         (0)      652 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/rotated_boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)      661 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/shape_spec.py
+-rwxrwxrwx   0 root         (0) root         (0)     4893 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/layers/wrappers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:47.947541 roof_mask_Yv8-0.5.9/detectron2/modeling/
+-rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15443 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/anchor_generator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.015502 roof_mask_Yv8-0.5.9/detectron2/modeling/backbone/
+-rwxrwxrwx   0 root         (0) root         (0)      475 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/backbone/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1543 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/backbone/backbone.py
+-rwxrwxrwx   0 root         (0) root         (0)     1015 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/backbone/build.py
+-rwxrwxrwx   0 root         (0) root         (0)    10055 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/backbone/fpn.py
+-rwxrwxrwx   0 root         (0) root         (0)    16656 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/backbone/regnet.py
+-rwxrwxrwx   0 root         (0) root         (0)    23658 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/backbone/resnet.py
+-rwxrwxrwx   0 root         (0) root         (0)    15123 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/box_regression.py
+-rwxrwxrwx   0 root         (0) root         (0)     6264 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/matcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.077466 roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/
+-rwxrwxrwx   0 root         (0) root         (0)      508 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      814 2023-04-17 21:04:26.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/build.py
+-rwxrwxrwx   0 root         (0) root         (0)    11550 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/dense_detector.py
+-rwxrwxrwx   0 root         (0) root         (0)    13213 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/fcos.py
+-rwxrwxrwx   0 root         (0) root         (0)    10335 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rwxrwxrwx   0 root         (0) root         (0)    13710 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    18265 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/retinanet.py
+-rwxrwxrwx   0 root         (0) root         (0)     9720 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/semantic_seg.py
+-rwxrwxrwx   0 root         (0) root         (0)    10832 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/mmdet_wrapper.py
+-rwxrwxrwx   0 root         (0) root         (0)    11316 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/poolers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4046 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/postprocessing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.137432 roof_mask_Yv8-0.5.9/detectron2/modeling/proposal_generator/
+-rwxrwxrwx   0 root         (0) root         (0)      231 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/proposal_generator/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      836 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/proposal_generator/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     8128 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/proposal_generator/proposal_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    23814 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/proposal_generator/rpn.py
+-rwxrwxrwx   0 root         (0) root         (0)     8807 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.193401 roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/
+-rwxrwxrwx   0 root         (0) root         (0)      768 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4077 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/box_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    12990 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    25274 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/fast_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    11156 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/keypoint_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    12169 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/mask_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    37701 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/roi_heads.py
+-rwxrwxrwx   0 root         (0) root         (0)    11158 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)     2334 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/sampling.py
+-rwxrwxrwx   0 root         (0) root         (0)    12416 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/modeling/test_time_augmentation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.240374 roof_mask_Yv8-0.5.9/detectron2/solver/
+-rwxrwxrwx   0 root         (0) root         (0)      298 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/solver/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11127 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/solver/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     8648 2023-04-17 21:04:27.000000 roof_mask_Yv8-0.5.9/detectron2/solver/lr_scheduler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.296342 roof_mask_Yv8-0.5.9/detectron2/structures/
+-rwxrwxrwx   0 root         (0) root         (0)      645 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/structures/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14429 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/structures/boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)     4557 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/structures/image_list.py
+-rwxrwxrwx   0 root         (0) root         (0)     6542 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/structures/instances.py
+-rwxrwxrwx   0 root         (0) root         (0)     9030 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/structures/keypoints.py
+-rwxrwxrwx   0 root         (0) root         (0)    19802 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/structures/masks.py
+-rwxrwxrwx   0 root         (0) root         (0)    18853 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/structures/rotated_boxes.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.351311 roof_mask_Yv8-0.5.9/detectron2/tracking/
+-rwxrwxrwx   0 root         (0) root         (0)      580 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/tracking/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2216 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/tracking/base_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)    11858 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/tracking/bbox_iou_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     7486 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/tracking/hungarian_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     4142 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     1106 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/tracking/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     5288 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.402282 roof_mask_Yv8-0.5.9/detectron2/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      175 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.9/detectron2/utils/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-04-18 18:45:50.000000 roof_mask_Yv8-0.5.9/detectron2/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6017 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.9/detectron2/utils/analysis.py
+-rwxrwxrwx   0 root         (0) root         (0)     8391 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.9/detectron2/utils/collect_env.py
+-rwxrwxrwx   0 root         (0) root         (0)     4096 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.9/detectron2/utils/colormap.py
+-rwxrwxrwx   0 root         (0) root         (0)     5610 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.9/detectron2/utils/comm.py
+-rwxrwxrwx   0 root         (0) root         (0)     1838 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.9/detectron2/utils/develop.py
+-rwxrwxrwx   0 root         (0) root         (0)     5644 2023-04-18 18:45:48.000000 roof_mask_Yv8-0.5.9/detectron2/utils/env.py
+-rwxrwxrwx   0 root         (0) root         (0)    17024 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.9/detectron2/utils/events.py
+-rwxrwxrwx   0 root         (0) root         (0)     1189 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.9/detectron2/utils/file_io.py
+-rwxrwxrwx   0 root         (0) root         (0)     7807 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.9/detectron2/utils/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2583 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.9/detectron2/utils/memory.py
+-rwxrwxrwx   0 root         (0) root         (0)     1874 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.9/detectron2/utils/registry.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.9/detectron2/utils/serialize.py
+-rwxrwxrwx   0 root         (0) root         (0)     4833 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.9/detectron2/utils/testing.py
+-rwxrwxrwx   0 root         (0) root         (0)    11319 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.9/detectron2/utils/video_visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    51159 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.9/detectron2/utils/visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    52915 2023-04-18 18:45:49.000000 roof_mask_Yv8-0.5.9/detectron2/utils/visualizer_new.py
+-rwxrwxrwx   0 root         (0) root         (0)      107 2023-04-17 21:19:17.000000 roof_mask_Yv8-0.5.9/readme.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.444258 roof_mask_Yv8-0.5.9/roof_mask_Yv8.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      473 2023-05-05 19:34:45.000000 roof_mask_Yv8-0.5.9/roof_mask_Yv8.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     9347 2023-05-05 19:34:46.000000 roof_mask_Yv8-0.5.9/roof_mask_Yv8.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-05 19:34:45.000000 roof_mask_Yv8-0.5.9/roof_mask_Yv8.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-05-05 19:34:45.000000 roof_mask_Yv8-0.5.9/roof_mask_Yv8.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.496229 roof_mask_Yv8-0.5.9/scoring/
+-rwxrwxrwx   0 root         (0) root         (0)     4474 2023-05-05 18:46:12.000000 roof_mask_Yv8-0.5.9/scoring/score_yolov8.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-05 19:35:23.159467 roof_mask_Yv8-0.5.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      632 2023-05-05 19:33:55.000000 roof_mask_Yv8-0.5.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.552197 roof_mask_Yv8-0.5.9/ultralytics/
+-rwxrwxrwx   0 root         (0) root         (0)      295 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/ultralytics/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.607165 roof_mask_Yv8-0.5.9/ultralytics/hub/
+-rwxrwxrwx   0 root         (0) root         (0)     3421 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/ultralytics/hub/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5206 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/ultralytics/hub/auth.py
+-rwxrwxrwx   0 root         (0) root         (0)     8690 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/ultralytics/hub/session.py
+-rwxrwxrwx   0 root         (0) root         (0)     9723 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/ultralytics/hub/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.679124 roof_mask_Yv8-0.5.9/ultralytics/nn/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/ultralytics/nn/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    24083 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/ultralytics/nn/autobackend.py
+-rwxrwxrwx   0 root         (0) root         (0)    11839 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/ultralytics/nn/autoshape.py
+-rwxrwxrwx   0 root         (0) root         (0)    20062 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/ultralytics/nn/modules.py
+-rwxrwxrwx   0 root         (0) root         (0)    26619 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/ultralytics/nn/tasks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.733094 roof_mask_Yv8-0.5.9/ultralytics/yolo/
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-04-17 21:04:28.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.799056 roof_mask_Yv8-0.5.9/ultralytics/yolo/cfg/
+-rwxrwxrwx   0 root         (0) root         (0)    17582 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/cfg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6237 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/cfg/default.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.857024 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/
+-rwxrwxrwx   0 root         (0) root         (0)      483 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    31285 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/augment.py
+-rwxrwxrwx   0 root         (0) root         (0)     8919 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/base.py
+-rwxrwxrwx   0 root         (0) root         (0)     8614 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/build.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.913991 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/dataloaders/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/dataloaders/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15194 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rwxrwxrwx   0 root         (0) root         (0)    17226 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rwxrwxrwx   0 root         (0) root         (0)    49861 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/dataloaders/v5loader.py
+-rwxrwxrwx   0 root         (0) root         (0)    12740 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/dataset_wrappers.py
+-rwxrwxrwx   0 root         (0) root         (0)    22728 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/data/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:48.958965 roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    41854 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/exporter.py
+-rwxrwxrwx   0 root         (0) root         (0)    21469 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/model.py
+-rwxrwxrwx   0 root         (0) root         (0)    14720 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/predictor.py
+-rwxrwxrwx   0 root         (0) root         (0)    17378 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/results.py
+-rwxrwxrwx   0 root         (0) root         (0)    29843 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/trainer.py
+-rwxrwxrwx   0 root         (0) root         (0)    10358 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/validator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:49.013934 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/
+-rwxrwxrwx   0 root         (0) root         (0)    25215 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3823 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/autobatch.py
+-rwxrwxrwx   0 root         (0) root         (0)     5414 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/benchmarks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:49.079897 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/
+-rwxrwxrwx   0 root         (0) root         (0)      171 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3783 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/base.py
+-rwxrwxrwx   0 root         (0) root         (0)     5286 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/clearml.py
+-rwxrwxrwx   0 root         (0) root         (0)    11929 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/comet.py
+-rwxrwxrwx   0 root         (0) root         (0)     3189 2023-04-17 21:04:29.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/hub.py
+-rwxrwxrwx   0 root         (0) root         (0)     2512 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/mlflow.py
+-rwxrwxrwx   0 root         (0) root         (0)      385 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/raytune.py
+-rwxrwxrwx   0 root         (0) root         (0)     1297 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rwxrwxrwx   0 root         (0) root         (0)     1593 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/wb.py
+-rwxrwxrwx   0 root         (0) root         (0)    14190 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/checks.py
+-rwxrwxrwx   0 root         (0) root         (0)     2412 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/dist.py
+-rwxrwxrwx   0 root         (0) root         (0)    10052 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/downloads.py
+-rwxrwxrwx   0 root         (0) root         (0)      251 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/errors.py
+-rwxrwxrwx   0 root         (0) root         (0)     3105 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/files.py
+-rwxrwxrwx   0 root         (0) root         (0)    11394 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/instance.py
+-rwxrwxrwx   0 root         (0) root         (0)     2889 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/loss.py
+-rwxrwxrwx   0 root         (0) root         (0)    35693 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/metrics.py
+-rwxrwxrwx   0 root         (0) root         (0)    28503 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/ops.py
+-rwxrwxrwx   0 root         (0) root         (0)    20613 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/plotting.py
+-rwxrwxrwx   0 root         (0) root         (0)    10233 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/tal.py
+-rwxrwxrwx   0 root         (0) root         (0)    19694 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/torch_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     2302 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/tuner.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:49.133866 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/
+-rwxrwxrwx   0 root         (0) root         (0)      157 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:49.208823 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/classify/
+-rwxrwxrwx   0 root         (0) root         (0)      390 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/classify/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1459 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/classify/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     6388 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/classify/train.py
+-rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/classify/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:49.263792 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/detect/
+-rwxrwxrwx   0 root         (0) root         (0)      276 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/detect/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2005 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/detect/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     9886 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/detect/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    12516 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/detect/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:49.327755 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/pose/
+-rwxrwxrwx   0 root         (0) root         (0)      246 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/pose/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2076 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/pose/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     7145 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/pose/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    10050 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/pose/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:49.372730 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/segment/
+-rwxrwxrwx   0 root         (0) root         (0)      294 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/segment/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2657 2023-04-17 21:04:30.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/segment/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)     7664 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/segment/train.py
+-rwxrwxrwx   0 root         (0) root         (0)    11922 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/segment/val.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 19:34:49.420702 roof_mask_Yv8-0.5.9/yolo_roof/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 21:04:31.000000 roof_mask_Yv8-0.5.9/yolo_roof/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    34076 2023-05-05 16:10:28.000000 roof_mask_Yv8-0.5.9/yolo_roof/detect_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    21677 2023-05-05 16:50:57.000000 roof_mask_Yv8-0.5.9/yolo_roof/geo_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    57368 2023-05-05 16:33:24.000000 roof_mask_Yv8-0.5.9/yolo_roof/report_functions.py
```

### Comparing `roof_mask_Yv8-0.5.8/detectron2/checkpoint/c2_model_loading.py` & `roof_mask_Yv8-0.5.9/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/checkpoint/catalog.py` & `roof_mask_Yv8-0.5.9/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/checkpoint/detection_checkpoint.py` & `roof_mask_Yv8-0.5.9/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/config/__init__.py` & `roof_mask_Yv8-0.5.9/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/config/compat.py` & `roof_mask_Yv8-0.5.9/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/config/config.py` & `roof_mask_Yv8-0.5.9/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/config/defaults.py` & `roof_mask_Yv8-0.5.9/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/config/instantiate.py` & `roof_mask_Yv8-0.5.9/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/config/lazy.py` & `roof_mask_Yv8-0.5.9/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/__init__.py` & `roof_mask_Yv8-0.5.9/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/benchmark.py` & `roof_mask_Yv8-0.5.9/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/build.py` & `roof_mask_Yv8-0.5.9/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/catalog.py` & `roof_mask_Yv8-0.5.9/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/common.py` & `roof_mask_Yv8-0.5.9/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/dataset_mapper.py` & `roof_mask_Yv8-0.5.9/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/datasets/__init__.py` & `roof_mask_Yv8-0.5.9/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/datasets/builtin.py` & `roof_mask_Yv8-0.5.9/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/datasets/builtin_meta.py` & `roof_mask_Yv8-0.5.9/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/datasets/cityscapes.py` & `roof_mask_Yv8-0.5.9/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/datasets/cityscapes_panoptic.py` & `roof_mask_Yv8-0.5.9/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/datasets/coco.py` & `roof_mask_Yv8-0.5.9/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/datasets/coco_panoptic.py` & `roof_mask_Yv8-0.5.9/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis.py` & `roof_mask_Yv8-0.5.9/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis_v0_5_categories.py` & `roof_mask_Yv8-0.5.9/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis_v1_categories.py` & `roof_mask_Yv8-0.5.9/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/datasets/lvis_v1_category_image_count.py` & `roof_mask_Yv8-0.5.9/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/datasets/pascal_voc.py` & `roof_mask_Yv8-0.5.9/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/detection_utils.py` & `roof_mask_Yv8-0.5.9/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/samplers/distributed_sampler.py` & `roof_mask_Yv8-0.5.9/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/samplers/grouped_batch_sampler.py` & `roof_mask_Yv8-0.5.9/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/transforms/augmentation.py` & `roof_mask_Yv8-0.5.9/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/transforms/augmentation_impl.py` & `roof_mask_Yv8-0.5.9/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/data/transforms/transform.py` & `roof_mask_Yv8-0.5.9/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/engine/defaults.py` & `roof_mask_Yv8-0.5.9/detectron2/engine/defaults.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/engine/hooks.py` & `roof_mask_Yv8-0.5.9/detectron2/engine/hooks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/engine/launch.py` & `roof_mask_Yv8-0.5.9/detectron2/engine/launch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/engine/train_loop.py` & `roof_mask_Yv8-0.5.9/detectron2/engine/train_loop.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/evaluation/__init__.py` & `roof_mask_Yv8-0.5.9/detectron2/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/evaluation/cityscapes_evaluation.py` & `roof_mask_Yv8-0.5.9/detectron2/evaluation/cityscapes_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/evaluation/coco_evaluation.py` & `roof_mask_Yv8-0.5.9/detectron2/evaluation/coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/evaluation/evaluator.py` & `roof_mask_Yv8-0.5.9/detectron2/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/evaluation/fast_eval_api.py` & `roof_mask_Yv8-0.5.9/detectron2/evaluation/fast_eval_api.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/evaluation/lvis_evaluation.py` & `roof_mask_Yv8-0.5.9/detectron2/evaluation/lvis_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/evaluation/panoptic_evaluation.py` & `roof_mask_Yv8-0.5.9/detectron2/evaluation/panoptic_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/evaluation/pascal_voc_evaluation.py` & `roof_mask_Yv8-0.5.9/detectron2/evaluation/pascal_voc_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/evaluation/rotated_coco_evaluation.py` & `roof_mask_Yv8-0.5.9/detectron2/evaluation/rotated_coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/evaluation/sem_seg_evaluation.py` & `roof_mask_Yv8-0.5.9/detectron2/evaluation/sem_seg_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/evaluation/testing.py` & `roof_mask_Yv8-0.5.9/detectron2/evaluation/testing.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/export/README.md` & `roof_mask_Yv8-0.5.9/detectron2/export/README.md`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/export/api.py` & `roof_mask_Yv8-0.5.9/detectron2/export/api.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/export/c10.py` & `roof_mask_Yv8-0.5.9/detectron2/export/c10.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/export/caffe2_export.py` & `roof_mask_Yv8-0.5.9/detectron2/export/caffe2_export.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/export/caffe2_inference.py` & `roof_mask_Yv8-0.5.9/detectron2/export/caffe2_inference.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/export/caffe2_modeling.py` & `roof_mask_Yv8-0.5.9/detectron2/export/caffe2_modeling.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/export/caffe2_patch.py` & `roof_mask_Yv8-0.5.9/detectron2/export/caffe2_patch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/export/flatten.py` & `roof_mask_Yv8-0.5.9/detectron2/export/flatten.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/export/shared.py` & `roof_mask_Yv8-0.5.9/detectron2/export/shared.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/export/torchscript.py` & `roof_mask_Yv8-0.5.9/detectron2/export/torchscript.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/export/torchscript_patch.py` & `roof_mask_Yv8-0.5.9/detectron2/export/torchscript_patch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/__init__.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/aspp.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/batch_norm.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/blocks.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated.h` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated.h`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cpu.cpp` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cpu.cpp`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cuda.cu` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/ROIAlignRotated/ROIAlignRotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated.h` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated.h`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cpu.cpp` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cpu.cpp`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cuda.cu` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_utils.h` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/box_iou_rotated/box_iou_rotated_utils.h`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cocoeval/cocoeval.cpp` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/cocoeval/cocoeval.cpp`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cocoeval/cocoeval.h` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/cocoeval/cocoeval.h`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/cuda_version.cu` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/cuda_version.cu`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/deform_conv.h` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/deformable/deform_conv.h`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/deform_conv_cuda.cu` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/deformable/deform_conv_cuda.cu`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/deformable/deform_conv_cuda_kernel.cu` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/deformable/deform_conv_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/nms_rotated.h` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/nms_rotated/nms_rotated.h`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/nms_rotated_cpu.cpp` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/nms_rotated/nms_rotated_cpu.cpp`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/nms_rotated/nms_rotated_cuda.cu` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/nms_rotated/nms_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/csrc/vision.cpp` & `roof_mask_Yv8-0.5.9/detectron2/layers/csrc/vision.cpp`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/deform_conv.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/losses.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/mask_ops.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/nms.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/roi_align.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/roi_align_rotated.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/rotated_boxes.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/shape_spec.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/layers/wrappers.py` & `roof_mask_Yv8-0.5.9/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/__init__.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/anchor_generator.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/backbone.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/build.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/fpn.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/regnet.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/backbone/resnet.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/box_regression.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/matcher.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/build.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/dense_detector.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/fcos.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/panoptic_fpn.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/rcnn.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/retinanet.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/meta_arch/semantic_seg.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/mmdet_wrapper.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/poolers.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/postprocessing.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/build.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/proposal_utils.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/rpn.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/proposal_generator/rrpn.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/__init__.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/box_head.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/cascade_rcnn.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/fast_rcnn.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/keypoint_head.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/mask_head.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/roi_heads.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/sampling.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/modeling/test_time_augmentation.py` & `roof_mask_Yv8-0.5.9/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/solver/build.py` & `roof_mask_Yv8-0.5.9/detectron2/solver/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/solver/lr_scheduler.py` & `roof_mask_Yv8-0.5.9/detectron2/solver/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/structures/__init__.py` & `roof_mask_Yv8-0.5.9/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/structures/boxes.py` & `roof_mask_Yv8-0.5.9/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/structures/image_list.py` & `roof_mask_Yv8-0.5.9/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/structures/instances.py` & `roof_mask_Yv8-0.5.9/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/structures/keypoints.py` & `roof_mask_Yv8-0.5.9/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/structures/masks.py` & `roof_mask_Yv8-0.5.9/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/structures/rotated_boxes.py` & `roof_mask_Yv8-0.5.9/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/tracking/__init__.py` & `roof_mask_Yv8-0.5.9/detectron2/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/tracking/base_tracker.py` & `roof_mask_Yv8-0.5.9/detectron2/tracking/base_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/tracking/bbox_iou_tracker.py` & `roof_mask_Yv8-0.5.9/detectron2/tracking/bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/tracking/hungarian_tracker.py` & `roof_mask_Yv8-0.5.9/detectron2/tracking/hungarian_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py` & `roof_mask_Yv8-0.5.9/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/tracking/utils.py` & `roof_mask_Yv8-0.5.9/detectron2/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py` & `roof_mask_Yv8-0.5.9/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/analysis.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/collect_env.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/colormap.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/comm.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/develop.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/env.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/events.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/file_io.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/logger.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/memory.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/registry.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/serialize.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/testing.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/video_visualizer.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/visualizer.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/detectron2/utils/visualizer_new.py` & `roof_mask_Yv8-0.5.9/detectron2/utils/visualizer_new.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/roof_mask_Yv8.egg-info/SOURCES.txt` & `roof_mask_Yv8-0.5.9/roof_mask_Yv8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/scoring/score_yolov8.py` & `roof_mask_Yv8-0.5.9/scoring/score_yolov8.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import os
-#import sys
 import logging
 import base64
 import json
-#import torch
-#import cv2
-#import requests
-#import numpy as np
-#from io import BytesIO
-#from PIL import Image
 import zipfile
+import glob
 
 from yolo_roof.geo_functions import image_download
 from yolo_roof.detect_functions import load_yolov8_model, roof_condition_predict, roof_predict_5models
 from yolo_roof.report_functions import generate_condition_model, generate_merged_model_damage_equip_pdf#, zip_download_file
 
 score_logger = logging.getLogger("score_logger")
 score_logger.setLevel(logging.INFO)
@@ -76,30 +70,30 @@
     except Exception as inst:
         err_code, err_msg = inst.args    
         logging.error(err_msg)
         return dict(status=err_code)
 
     score_logger.info("RL: roof model is working")
     
-    input_files = 1
-    roof_condition_predict(yolo_roof_condition_model, file_root_path, input_files)
+    roof_condition_predict(yolo_roof_condition_model, file_root_path)
     roof_predict_5models(yolo_roof_model, yolo_roof_type_model, yolo_roof_material_model,
-                         yolo_data_all_model,yolo_phase3_model,file_root_path, input_files)
+                         yolo_data_all_model,yolo_phase3_model,file_root_path)
 
     score_logger.info("RL: roof model finished working")
     generate_condition_model(file_root_path) 
     generate_merged_model_damage_equip_pdf(file_root_path) 
     
     score_logger.info("RL: roof report done")
     
-    #zip_download_file(file_name='roof.zip')
-    #score_logger.info("RL: download file done")
-    
-    pdf_path = "./roof_score_new_20230101/"+address+".pdf" # bad idea hardcoding this, deal with this later
-    pdf_zip_path = "./roof_score_new_20230101/"+address+".pdf.zip"
+    # The PDF report filename use Ecopia's standardized name, which may be different to the user input 
+    # and thus we need to retrieve the PDF file using glob.
+    pdf_path = glob.glob(file_root_path+"/roof_score_new_20230101/*.pdf")[0] # bad idea hardcoding this, deal with this later
+    pdf_zip_path = pdf_path+".zip"
+    #pdf_path = file_root_path+"/roof_score_new_20230101/"+address+".pdf" # bad idea hardcoding this, deal with this later
+    #pdf_zip_path = file_root_path+"/roof_score_new_20230101/"+address+".pdf.zip"
 
     with zipfile.ZipFile(pdf_zip_path, 'w', compression=zipfile.ZIP_DEFLATED, compresslevel=9) as myzip:
         myzip.write(pdf_path, os.path.basename(pdf_path)) 
 
     with open(pdf_zip_path, mode="rb") as pdf_zip_file:
         contents=pdf_zip_file.read()
```

### Comparing `roof_mask_Yv8-0.5.8/setup.py` & `roof_mask_Yv8-0.5.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## test upload
 import setuptools
 
 setuptools.setup(
     name = "roof_mask_Yv8",
-    version = "0.5.8",
+    version = "0.5.9",
     author = "Ruixu",
     author_email = "lrxjason@gmail.com",
     description = "upload pip package test",
     long_description = 'package supporing Yolo_v8 roof model backend.',
     long_description_content_type="text/markdown",
     url="https://github.com/lrxjason/roof_model_test/",
     packages=setuptools.find_packages(),
```

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/hub/__init__.py` & `roof_mask_Yv8-0.5.9/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/hub/auth.py` & `roof_mask_Yv8-0.5.9/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/hub/session.py` & `roof_mask_Yv8-0.5.9/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/hub/utils.py` & `roof_mask_Yv8-0.5.9/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/nn/autobackend.py` & `roof_mask_Yv8-0.5.9/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/nn/autoshape.py` & `roof_mask_Yv8-0.5.9/ultralytics/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/nn/modules.py` & `roof_mask_Yv8-0.5.9/ultralytics/nn/modules.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/nn/tasks.py` & `roof_mask_Yv8-0.5.9/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/cfg/__init__.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/cfg/default.yaml` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/augment.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/base.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/data/base.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/build.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/data/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataloaders/v5loader.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataset.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/dataset_wrappers.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/data/utils.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/exporter.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/model.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/model.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/predictor.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/results.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/results.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/trainer.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/engine/validator.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/engine/validator.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/__init__.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/autobatch.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/benchmarks.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/base.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/clearml.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/comet.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/hub.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/mlflow.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/tensorboard.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/callbacks/wb.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/checks.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/dist.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/downloads.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/files.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/instance.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/loss.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/metrics.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/ops.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/plotting.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/tal.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/torch_utils.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/utils/tuner.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/predict.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/classify/predict.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/train.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/classify/train.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/classify/val.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/classify/val.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/predict.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/detect/predict.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/train.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/detect/train.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/detect/val.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/detect/val.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/predict.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/pose/predict.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/train.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/pose/train.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/pose/val.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/pose/val.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/predict.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/segment/predict.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/train.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/segment/train.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/ultralytics/yolo/v8/segment/val.py` & `roof_mask_Yv8-0.5.9/ultralytics/yolo/v8/segment/val.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.8/yolo_roof/detect_functions.py` & `roof_mask_Yv8-0.5.9/yolo_roof/detect_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from concurrent import futures
 
 #### shapely ###
 import shapely
 import shapely.wkt
 from shapely.ops import unary_union
 from shapely.geometry import Polygon, MultiPoint
-from shapely.geometry import Polygon
 
 ### torch ###
 import torch
 import torch.backends.cudnn as cudnn
 
 ### detectron2 ###
 from detectron2.data import DatasetCatalog
@@ -192,15 +191,15 @@
     new_images = []
     ann_id = 1
     new_image_id = 1
     
     if input_files:
         for image_path in tqdm(input_files):
             image_folder = os.path.splitext(image_path)[0]
-            if not(os.path.isdir(image_folder)) and save_image:
+            if not(os.path.isdir(image_folder)):
                 os.makedirs(image_folder)
 
             img = read_image(image_path, format="BGR")
             
             if os.path.isdir(output_folder):
                 out_filename = os.path.join(image_folder,trainingDataset +'.jpg')
                 out_filename2 = os.path.join(model_folder, os.path.basename(image_path))
@@ -498,15 +497,15 @@
                      "images": new_images,
                      "annotations": new_annotations
                      }
 
         with open(os.path.join(model_folder,new_json_file), "w") as jsonfile:
             json.dump(json_data, jsonfile, sort_keys=True, indent=4)
 
-################################ for json only
+################################ image is just for visulization result will save to the json file
         if save_image:
             vis_out = merge_polygones(output_folder,os.path.join(model_folder,new_json_file),trainingDataset)
             output_image = vis_out.get_image()[:, :, ::-1]
             return output_image
         else:
             return 1
 
@@ -548,15 +547,15 @@
     img_pil.save(img_byte, format='JPEG')
     binary_str2 = img_byte.getvalue()
     imageData = base64.b64encode(binary_str2)
     base64_string = imageData.decode(ENCODING)
     return base64_string
 
 def merge_polygones(image_folder,json_file,trainingDataset):
-    allColors = [(255,0,0), (0,255,0), (0,0,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8
+    allColors = [(0,0,255), (255,0,0), (125,75,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8
     filename = str(uuid.uuid4())
     register_coco_instances(filename, {'thing_colors':allColors}, json_file, image_folder)
     metadata = MetadataCatalog.get(filename)
     dicts = DatasetCatalog.get(filename)
     model_folder = os.path.join(image_folder,'prediction_' + trainingDataset)
     logging.info(f"Merging {trainingDataset} polygons")
     for dic in dicts:
@@ -575,17 +574,21 @@
 def inputimage_list(input_folder):
     files = os.listdir(input_folder)
     input_files = [os.path.join(input_folder, x) for x in files if os.path.splitext(x)[1] in ['.jpg','.png']]
     return input_files
 
 
 def roof_predict_5models(yolo_roof_model,yolo_roof_type_model, yolo_roof_material_model,
-                         yolo_data_all_model,yolo_phase3_model, file_root_path, input_files,
+                         yolo_data_all_model,yolo_phase3_model, file_root_path, 
                          demoFolder='roof_score_new_20230101'):
 
+    # demonFolder should be a absolute path so that its localtion does not depends on the caller
+    if not os.path.isabs(demoFolder): 
+        demoFolder=os.path.join(file_root_path, demoFolder)
+
     ############################################ input Image
     input_files = inputimage_list(input_folder = demoFolder)
     # logging.info(input_files)
     ########################################## dataset config
     imgsetUrl =  os.path.join(file_root_path,'test_360.jpg')
 
     cocoJsonPairs = {
@@ -604,34 +607,34 @@
             catMap = {str(cat['id']): cat['name'] for cat in cocoFile['categories']}  # coco file category ID starts from 1
             logging.info(catMap)
             catIDs = [int(key) for key in catMap.keys()] # when detectron2 load a coco dataset, the categories are sorted by IDs, and mapped to [1, lengthOfCatetories] as a subset of [1,80).
 
             # To make sure the labels are in the same order as the IDs when passed to register the dataset
             catIDs.sort() 
             labels = [catMap[str(catID)] for catID in catIDs]
-            allColors = [(255,0,0), (0,255,0), (0,0,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8 
+            allColors = [(0,0,255), (255,0,0), (125,75,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8 
             # 12 colors; repeat 8 times in case there are more labels than 12; need a better way to assign the colors
             colors = allColors[:len(labels)]
             logging.info('dataset: %s has %i labels and %i colors ' % (datasetName, len(labels), len(colors)))
             register_coco_instances(datasetName, {'thing_classes':labels, 'thing_colors':colors}, jsonURL, imgsetUrl) 
             # the 2nd parameter is metadata, in this case we pass over thing_classes for Visualizer to use    
         else: 
             logging.info('%s already registered!' % datasetName)
 
     ############################################# Models
-    last_roof_boundary_result = mask_prediction(yolo_roof_model, input_files, trainingDataset='Roof_boundary', output_folder=demoFolder, thresh_hold=0.426, cut_image = False, tile_len = 960, tile_overlap = 200, save_image=True)
-    # last_roof_type_result = mask_prediction(yolo_roof_type_model, input_files, trainingDataset='Roof_type', output_folder=demoFolder, thresh_hold=0.295, cut_image = False, tile_len = 1536, tile_overlap = 200, save_image=True)
-    # last_roof_material_result = mask_prediction(yolo_roof_material_model, input_files, trainingDataset='Roof_material', output_folder=demoFolder, thresh_hold=0.253, cut_image = False, tile_len = 1536, tile_overlap = 200, save_image=True)
-    last_data_all_result = mask_prediction(yolo_data_all_model, input_files, trainingDataset='Data_all_equipment_damage', output_folder=demoFolder, thresh_hold=0.22, cut_image = True, tile_len = 800, tile_overlap = 200, save_image=True)
-    last_phase3_result = mask_prediction(yolo_phase3_model, input_files, trainingDataset='Phase3_equipment_damage', output_folder=demoFolder, thresh_hold=0.203, cut_image = True, tile_len = 800, tile_overlap = 200, save_image=True)
-    
-    
+    last_roof_boundary_result = mask_prediction(yolo_roof_model, input_files, trainingDataset='Roof_boundary', output_folder=demoFolder, thresh_hold=0.426, cut_image = False, tile_len = 1280, tile_overlap = 200, save_image=False)
+    last_data_all_result = mask_prediction(yolo_data_all_model, input_files, trainingDataset='Data_all_equipment_damage', output_folder=demoFolder, thresh_hold=0.2, cut_image = True, tile_len = 800, tile_overlap = 200, save_image=False)
+    last_phase3_result = mask_prediction(yolo_phase3_model, input_files, trainingDataset='Phase3_equipment_damage', output_folder=demoFolder, thresh_hold=0.2, cut_image = True, tile_len = 800, tile_overlap = 200, save_image=False)
+
     
-def roof_condition_predict(yolo_roof_condition_model, file_root_path,
-                           input_files, demoFolder='roof_score_new_20230101'):
+
+def roof_condition_predict(yolo_roof_condition_model, file_root_path, demoFolder='roof_score_new_20230101'):
+    # demonFolder should be a absolute path so that its localtion does not depends on the caller
+    if not os.path.isabs(demoFolder): 
+        demoFolder=os.path.join(file_root_path, demoFolder)
 
     ############################################ input Image
     input_files = inputimage_list(input_folder = demoFolder)
     # logging.info(input_files)
     ########################################## dataset config
     imgsetUrl =  os.path.join(file_root_path,'test_360.jpg')
 
@@ -648,26 +651,19 @@
             catMap = {str(cat['id']): cat['name'] for cat in cocoFile['categories']}  # coco file category ID starts from 1
             logging.info(catMap)
             catIDs = [int(key) for key in catMap.keys()] # when detectron2 load a coco dataset, the categories are sorted by IDs, and mapped to [1, lengthOfCatetories] as a subset of [1,80).
 
             # To make sure the labels are in the same order as the IDs when passed to register the dataset
             catIDs.sort() 
             labels = [catMap[str(catID)] for catID in catIDs]
-            allColors = [(255,0,0), (0,255,0), (0,0,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8 
+            allColors = [(0,0,255), (255,0,0), (125,75,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8 
             # 12 colors; repeat 8 times in case there are more labels than 12; need a better way to assign the colors
             colors = allColors[:len(labels)]
             logging.info('dataset: %s has %i labels and %i colors ' % (datasetName, len(labels), len(colors)))
             register_coco_instances(datasetName, {'thing_classes':labels, 'thing_colors':colors}, jsonURL, imgsetUrl) 
             # the 2nd parameter is metadata, in this case we pass over thing_classes for Visualizer to use    
         else: 
             logging.info('%s already registered!' % datasetName)
 
     ############################################# Models
-    # last_roof_boundary_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition', output_folder=demoFolder, thresh_hold=0.244, cut_image = False, tile_len = 960, tile_overlap = 200,save_image=False)
-    
-    # last_roof_boundary_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition_three_classes', output_folder=demoFolder, thresh_hold=0.245, cut_image = False, tile_len = 960, tile_overlap = 200, save_image=False)
-    
-    # last_roof_condition_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition_three_classes', output_folder=demoFolder, thresh_hold=0.236, cut_image = False, tile_len = 1280, tile_overlap = 200, save_image=True)
+    last_roof_condition_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition_three_classes', output_folder=demoFolder, thresh_hold=0.15, cut_image = False, tile_len = 1280, tile_overlap = 200, save_image=False)
 
-    last_roof_condition_result = mask_prediction(yolo_roof_condition_model, input_files, trainingDataset='Roof_condition_three_classes', output_folder=demoFolder, thresh_hold=0.15, cut_image = False, tile_len = 1280, tile_overlap = 200, save_image=True)
-
-
```

### Comparing `roof_mask_Yv8-0.5.8/yolo_roof/geo_functions.py` & `roof_mask_Yv8-0.5.9/yolo_roof/geo_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,18 @@
         The first item in the list is from the geocoding app, where most likely the input address is, while the others are buildings (fully or partially) on the same parcel.
         The first item contains 'wkt', which is the 'orig_wkt' from the address API, and 'clipped_wkt', which is the wkt from the address API, so it's consistent with the rest of ftpts from the parcel API.
         @addr is a string of the full address.
         '''
         self.address = addr
         r1 = self.ecopia_addr_API(self.address)
         result1 = r1.json()
-
+        
+        # update address name with ecopia format address
+        self.address = result1['result']['format_name']
+        
         ftpt1 = dict()
         ftpt1['id'] = result1['result']['id']
         ftpt1['wkt'] = result1['result']['orig_wkt']
         ftpt1['clipped_wkt'] = result1['result']['wkt']
         ftpt1['location'] = result1['result']['location']
 
         ftpts = [ftpt1]
@@ -329,21 +332,21 @@
     equatorial_circumference = 2 * math.pi * 6378137
     meter_per_pixels = equatorial_circumference * math.cos(math.radians(latitude)) / math.pow(2,zoom_level+8)
     return meter_per_pixels
 
 def image_download(input_address, name, file_root_path):
     excel_file_path = os.path.join(file_root_path,'roof_score_new_20230101.csv')
     image_folder_name = os.path.splitext(os.path.basename(excel_file_path))[0]
-    demoFolder = image_folder_name
-    # make a image folder by excel name
-    if not(os.path.isdir(image_folder_name)):
-        os.makedirs(image_folder_name)
+    # demoFolder uses absolute path to remove the dependency on the location of the caller
+    demoFolder = os.path.join(file_root_path, image_folder_name)
+    if not(os.path.isdir(demoFolder)):
+        os.makedirs(demoFolder)
     else:
-        shutil.rmtree(image_folder_name)
-        os.makedirs(image_folder_name)
+        shutil.rmtree(demoFolder)
+        os.makedirs(demoFolder)
         
 
     # load the excel file
     excel_file = pd.read_csv(excel_file_path)
     # updating address value
     excel_file.loc[0, 'location_Address'] = input_address
     excel_file.loc[0, 'InsuredName'] = name
@@ -394,14 +397,17 @@
             csv_image_level.append('')
             csv_image_date.append('')
             csv_gsd.append('')
             continue
 
         # image acquire
         check_date = Today_date
+        
+        # using ecopia format address as output address
+        address = Ecopia_API.address
 
         # zoom level 21 is better than others because the training set almost all level21
         Nearmap_API = Nearmap_Image(address_boundary,zoom_level=21, date=check_date)
         try:
             # 0	1.0	111 km
             # 1	0.1	11.1 km
             # 2	0.01	1.11 km
@@ -427,15 +433,15 @@
 
             image, zoom_level, date = Nearmap_API.boundary2image()
             # image_name = address + '_' + str(zoom_level)+ '_'+ date
             image_name = address
             logging.info(f'index:{i}, address:{address}')
             image_text = image_text + f'[{Nearmap_API.x0}, {Nearmap_API.y1}, {Nearmap_API.x1}, {Nearmap_API.y0}]'
             logging.info(image_text)
-            cv2.imwrite(os.path.join(image_folder_name, image_name) + '.jpg', image)
+            cv2.imwrite(os.path.join(demoFolder, image_name) + '.jpg', image)
             image_name_list.append(image_name)
             csv_image_boundary.append(address_boundary)
             csv_image_info.append(image_text)
             csv_image_level.append(int(zoom_level))
             csv_image_date.append(date)
             gsd = pixels_to_meters(latitude = (address_boundary[2] + address_boundary[0])/2, zoom_level = zoom_level)
             csv_gsd.append(gsd)
@@ -466,16 +472,17 @@
                             'InsuredName':insured_name,
                             'PolicyExpirationDate':policy_expiration_date,
                             'Image date': csv_image_date,
                             'Image level': csv_image_level,
                             'Image boundary': csv_image_boundary,
                             'Image info': csv_image_info,
                             'Image gsd (meters/pixels)': csv_gsd})
-    out_csv.to_csv(os.path.join(image_folder_name,'image.csv'), index=False, header=True) 
-
+    out_csv.to_csv(os.path.join(demoFolder,'image.csv'), index=False, header=True)
+    
+    
     # re-throw exceptions (e.g., from geo-coding vender and image-vender) so that the errors can be relayed to the end user.  
     # Exception-throwing-catching is a more generic solution than passing the error message via and csv file, and I (qiang_wang)
     # plan to move away from the csv file(s)
     if 'Nearmap image is not available here.' in image_text:
         raise Exception(11, image_text) # 11 is the error code, image_text is the error message 
     elif 'image is too big' in image_text:
         raise Exception(21, image_text)
```

### Comparing `roof_mask_Yv8-0.5.8/yolo_roof/report_functions.py` & `roof_mask_Yv8-0.5.9/yolo_roof/report_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -487,67 +487,222 @@
 def generate_displayed_polygones(image_folder,json_file,trainingDataset):
     allColors = [(0,0,255), (255,0,0), (125,75,255), (255,255,0), (255,0,255), (0,255,255), (75,125,255), (125,75,255), (75,255,125), (125,255,75), (255,125,75), (255,75,125)]*8
     filename = str(uuid.uuid4())
     register_coco_instances(filename, {'thing_colors':allColors}, json_file, image_folder)
     metadata = MetadataCatalog.get(filename)
     dicts = DatasetCatalog.get(filename)
     model_folder = os.path.join(image_folder,'prediction_' + trainingDataset)
-    print(f"Generating {trainingDataset} polygons")
+    print(f"Plotting {trainingDataset} polygons")
     for dic in dicts:
         img = utils.read_image(dic["file_name"], "RGB")
         visualizer = Visualizer(img, metadata=metadata, instance_mode=ColorMode.SEGMENTATION)
         vis = visualizer.draw_dataset_dict(dic)
         out_filename = os.path.join(os.path.splitext(os.path.basename(dic["file_name"]))[0],trainingDataset +'_merged.jpg')
         
         out_filename2_extention = os.path.splitext(os.path.basename(dic["file_name"]))[1]
         out_filename2 = os.path.basename(dic["file_name"]).replace(out_filename2_extention,'_merged'+out_filename2_extention)
         vis.save(os.path.join(image_folder,out_filename))
         # vis.save(os.path.join(model_folder,out_filename2)) # model folder is not necessary
-    print("Gereating Finished.")
+    print("Plotting Finished.")
     return vis
 
 
 def generate_displayed_condition_polygones_and_colors(image_folder,json_file,trainingDataset):
     coco_json = COCO(json_file)
     imgIds = coco_json.getImgIds()
 
-    print(f"Merging {trainingDataset} polygons")
+    print(f"Plotting {trainingDataset} polygons")
     for img_id in range(len(imgIds)):
         # get image information
         coco_img_info = coco_json.loadImgs(imgIds[img_id])[0]
         # get the raw image annotations Id
         annIds = coco_json.getAnnIds(imgIds=coco_img_info['id'])
         # get annotations from annotation Id
         annotations = coco_json.loadAnns(annIds)
 
         img = cv2.imread(os.path.join(image_folder,coco_img_info['file_name']))
-
+        y_max = img.shape[0]
+        x_max = img.shape[1]
         for i, ann in enumerate(annotations):
             bbox = ann['bbox']
+            polygon_pts = np.array(ann['segmentation'][0], np.int32).reshape(len(ann['segmentation'][0]) // 2, 2)
+            left_top = min(polygon_pts, key=lambda x: (x[0], x[1]))
+            # left_bottom = min(polygon_pts, key=lambda x: (x[0], -x[1]))
+            text_x = left_top[0]+5
+            text_y = left_top[1]+30
+            if text_y > y_max:
+                text_y = left_top[1]-30
+            polygon_pts = polygon_pts.reshape((-1, 1, 2))
+            
+
             score = int(ann['scores'])
 
             if score < 40:
                 condition_color = (0,0,255) # red
             elif score >70:
                 condition_color = (0,255,0) # green
             else:
                 condition_color = (0,255,255) # yellow
 
-            img = cv2.putText(img, str(i+1), (int(bbox[0]+5),int(bbox[1]+30)), fontFace=cv2.FONT_HERSHEY_SIMPLEX, 
-                       fontScale=1, color=condition_color, thickness=2, lineType=cv2.LINE_AA)
-            img = cv2.rectangle(img, (int(bbox[0]),int(bbox[1])), (int(bbox[0] + bbox[2]),int(bbox[1] + bbox[3])), color=condition_color, thickness=3)
-        
+            ##################### BOX DISPLAY
+            # img = cv2.putText(img, str(i+1), (int(bbox[0]+5),int(bbox[1]+30)), fontFace=cv2.FONT_HERSHEY_SIMPLEX, 
+            #            fontScale=1, color=condition_color, thickness=2, lineType=cv2.LINE_AA)
+            # img = cv2.rectangle(img, (int(bbox[0]),int(bbox[1])), (int(bbox[0] + bbox[2]),int(bbox[1] + bbox[3])), color=condition_color, thickness=3)
+            ############################# POLYGON DISPLAY
+            img = cv2.polylines(img, [polygon_pts], isClosed=True, color=condition_color, thickness=3)
+            img = cv2.putText(img, str(i+1), (int(text_x),int(text_y)), fontFace=cv2.FONT_HERSHEY_SIMPLEX, 
+                           fontScale=1.2, color=condition_color, thickness=2, lineType=cv2.LINE_AA)
+            #################################################
         out_filename = os.path.join(os.path.splitext(coco_img_info["file_name"])[0], trainingDataset +'_merged.jpg')
         cv2.imwrite(os.path.join(image_folder,out_filename),img)
 
-    print("Merging Finished.")
+    print("Plottinging Finished.")
     return img
 
 
-def generate_referral_condition_json(demoFolder, coco_json, new_json_file_name):
+
+def generate_referral_condition_using_boundary_json(demoFolder, condition_json, boundary_json, phase2_json, phase3_json, new_json_file_name):
+    
+    imgIds = condition_json.getImgIds()
+    catIds = condition_json.getCatIds(catNms=[], supNms=[], catIds=[])
+    categories = condition_json.loadCats(catIds)    
+    new_json_file = os.path.join(demoFolder, new_json_file_name)
+    new_images = []
+    new_annotations = []
+    ann_id = 1
+    new_image_id = 1
+    
+    cats = phase3_json.loadCats(phase3_json.getCatIds())
+    for cat in cats:
+        if cat['name'] == 'Tarp':
+            tarp_id = cat['id']
+    
+    ###
+    weights = np.array([0, 50, 100])
+    ###
+    
+    for img_id in range(len(imgIds)):
+        # get image information
+        coco_img_info = boundary_json.loadImgs(imgIds[img_id])[0]
+
+        ann_start = ann_id
+        ####################### tarp ##############################
+        # get the raw image annotations Id
+        annIds = phase3_json.getAnnIds(imgIds=coco_img_info['id'])
+        # get annotations from annotation Id
+        anns = phase3_json.loadAnns(annIds)
+        tarp_polygon = []
+        for ann in anns:
+            if ann['category_id'] == tarp_id:
+                # tarp_polygon.append(ann['segmentation'][0])
+                tarp = ann['segmentation'][0]
+                tarp_polygon.append(Polygon(np.array(tarp).reshape(len(tarp) // 2, 2)))
+
+        ###################### condition ############################
+
+        annIds = condition_json.getAnnIds(imgIds=coco_img_info['id'])
+        anns = condition_json.loadAnns(annIds)
+        condition_polygons = []
+        condition_scores = []
+        for ann in anns:
+            if ann['area'] < 100*100:
+                continue
+            current_condition_polygon = Polygon(np.array(ann['segmentation'][0]).reshape(len(ann['segmentation'][0]) // 2, 2))
+            condition_polygons.append(current_condition_polygon)
+
+            #### weighted three probs
+            score = np.array(ann['scores'])
+            new_score = weights.dot(score/score.sum())
+
+            #### if tarp score divide by 2
+            for trap in tarp_polygon:
+                if current_condition_polygon.intersects(trap):
+                    new_score = new_score//2
+
+            condition_scores.append(new_score)
+
+
+        ########################### boundary ###############################
+        annIds = boundary_json.getAnnIds(imgIds=coco_img_info['id'])
+        anns = boundary_json.loadAnns(annIds)
+
+        for ann in anns:
+            current_boundary_polygon = Polygon(np.array(ann['segmentation'][0]).reshape(len(ann['segmentation'][0]) // 2, 2))
+            
+            boundary_condition_scores = []
+            boundary_condition_areas = []
+            for condition_polygon, condition_score in zip(condition_polygons, condition_scores):
+                if current_boundary_polygon.intersects(condition_polygon):
+                    boundary_condition_scores.append(condition_score)
+                    boundary_condition_areas.append(condition_polygon.area)
+
+            area_np = np.array(boundary_condition_areas)
+            score_np = np.array(boundary_condition_scores)
+            coco_score = score_np.dot(area_np/area_np.sum())
+            
+            if boundary_condition_scores == []:
+                continue
+            
+            #### category we don't care. We are using score to plot
+            if coco_score < 40:
+                category_id = 0
+            elif coco_score >70:
+                category_id = 2
+            else:
+                category_id = 1
+            #############################
+            
+            new_annotations.append({"id": ann_id,
+                                    "image_id": new_image_id,
+                                    "category_id": ann['category_id'],
+                                    "iscrowd": 0,
+                                    "area": ann['area'],
+                                    "scores": coco_score,
+                                    "bbox": ann['bbox'],
+                                    "segmentation": ann['segmentation']
+                                    })
+            # get new annotation id
+            ann_id += 1
+
+        # get new image id
+        new_image_id += 1
+        # append image information to coco jason file list
+        new_images.append(coco_img_info)
+
+    info = {"year": 2022,
+            "version": "1.0",
+            "description": "Phase 2 data and coco json file",
+            "contributor": "Ruixu Liu, Delin Shen, Aaron Lee and Qiang Wang",
+            }
+
+    json_data = {"info": info,
+                 "categories": categories,
+                 "images": new_images,
+                 "annotations": new_annotations
+                 }
+
+    with open(new_json_file, "w") as jsonfile:
+        json.dump(json_data, jsonfile, sort_keys=True, indent=4)
+        
+        
+def generate_referral_condition_json(demoFolder, coco_json, damage_json, new_json_file_name):
+
+    imgIds = damage_json.getImgIds()
+    cats = damage_json.loadCats(damage_json.getCatIds())
+    for cat in cats:
+        if cat['name'] == 'Tarp':
+            tarp_id = cat['id']
+    annIds = damage_json.getAnnIds()
+    anns = damage_json.loadAnns(annIds)
+    tarp_polygon = []
+    for ann in anns:
+        if ann['category_id'] == tarp_id:
+            # tarp_polygon.append(ann['segmentation'][0])
+            tarp = ann['segmentation'][0]
+            tarp_polygon.append(Polygon(np.array(tarp).reshape(len(tarp) // 2, 2)))
     catIds = coco_json.getCatIds(catNms=[], supNms=[], catIds=[])
     categories = coco_json.loadCats(catIds)    
     imgIds = coco_json.getImgIds()
     new_json_file = os.path.join(demoFolder, new_json_file_name)
     new_images = []
     new_annotations = []
     ann_id = 1
@@ -567,14 +722,20 @@
 
         ann_start = ann_id
         for ann in annotations:
             if ann['area'] < 100*100:
                 continue
             score = np.array(ann['scores'])
             new_score = weights.dot(score/score.sum())
+            
+            current_polygon = Polygon(np.array(ann['segmentation'][0]).reshape(len(ann['segmentation'][0]) // 2, 2))
+            for trap in tarp_polygon:
+                if current_polygon.intersects(trap):
+                    new_score = new_score//2
+            
             # append annotation to coco jason file list
             new_annotations.append({"id": ann_id,
                                     "image_id": new_image_id,
                                     "category_id": ann['category_id'],
                                     "iscrowd": 0,
                                     "area": ann['area'],
                                     "scores": new_score,
@@ -602,17 +763,30 @@
                  }
 
     with open(new_json_file, "w") as jsonfile:
         json.dump(json_data, jsonfile, sort_keys=True, indent=4)
   
     
 def generate_condition_model(file_root_path, demoFolder = 'roof_score_new_20230101'):
+    # demonFolder should be a absolute path so that its localtion does not depends on the caller
+    if not os.path.isabs(demoFolder): 
+        demoFolder=os.path.join(file_root_path, demoFolder)
+
     pred_condition_file = os.path.join(demoFolder,'prediction_Roof_condition_three_classes/Roof_condition_three_classes_all_in_one.json')
+    pred_phase3_file = os.path.join(demoFolder,'prediction_Phase3_equipment_damage/Phase3_equipment_damage_all_in_one.json')
+    pred_phase2_file = os.path.join(demoFolder,'prediction_Data_all_equipment_damage/Data_all_equipment_damage_all_in_one.json')
+    pred_boundary_file = os.path.join(demoFolder,'prediction_Roof_boundary/Roof_boundary_all_in_one.json')
+    
     pred_condition = COCO(pred_condition_file)
-    generate_referral_condition_json(demoFolder, pred_condition,'Referral_condition.json')
+    pred_phase3 = COCO(pred_phase3_file)
+    pred_phase2 = COCO(pred_phase2_file)
+    pred_boundary = COCO(pred_boundary_file)
+    
+    
+    generate_referral_condition_using_boundary_json(demoFolder, pred_condition, pred_boundary, pred_phase2, pred_phase3, 'Referral_condition.json')
     vis_out = generate_displayed_condition_polygones_and_colors(demoFolder,os.path.join(demoFolder, 'Referral_condition.json'),'Roof_condition_three_classes')
     
     referral_condition = COCO(os.path.join(demoFolder, 'Referral_condition.json'))
     all_condition_score = []
     for referral_condition_id in referral_condition.getImgIds():
         coco_img_info = referral_condition.loadImgs(referral_condition_id)[0]
         address = os.path.splitext(coco_img_info['file_name'])[0]
@@ -641,23 +815,27 @@
         all_condition_score.append(condition_dict)
         df = pd.DataFrame.from_dict([condition_dict])
         df.to_csv(os.path.join(demoFolder,address+'/condition_referral.csv'), index=False, header=True)
     df = pd.DataFrame.from_dict(all_condition_score)
     df.to_csv(os.path.join(demoFolder,'all_condition.csv'), index=False, header=True)
 
 def generate_merged_model_damage_equip_pdf(file_root_path, demoFolder = 'roof_score_new_20230101'):
+    # demonFolder should be a absolute path so that its localtion does not depends on the caller
+    if not os.path.isabs(demoFolder): 
+        demoFolder=os.path.join(file_root_path, demoFolder)
+
     pred_phase3_file = os.path.join(demoFolder,'prediction_Phase3_equipment_damage/Phase3_equipment_damage_all_in_one.json')
     pred_data_all_file = os.path.join(demoFolder, 'prediction_Data_all_equipment_damage/Data_all_equipment_damage_all_in_one.json')
     pred_boundary_file =os.path.join(demoFolder, 'prediction_Roof_boundary/Roof_boundary_all_in_one.json')
     # Load prediction file as COCO formate
     pred_phase3 = COCO(pred_phase3_file)
     pred_data_all = COCO(pred_data_all_file)
     pred_boundary = COCO(pred_boundary_file)
     # read in referral rules and create corresponding functions
-    referral_label_file = os.path.join(file_root_path,'referral_labels_20230315.json')
+    referral_label_file = os.path.join(file_root_path,'referral_labels_20230504.json')
     referral_damage_label_file = os.path.join(file_root_path,'referral_labels_20230421_for_merged_damage.json')
     referral_equip_label_file = os.path.join(file_root_path,'referral_labels_20230421_for_merged_equip.json')
     
     with open(referral_damage_label_file) as f1:
         ref_json = json.load(f1)
         cat_damage = [x for x in ref_json]
     generate_multi_model_referral_roof_boundary_based_json(demoFolder, [pred_data_all, pred_phase3], pred_boundary,cat_damage,'Referral_damage_all.json')
@@ -798,14 +976,15 @@
             if i%8==0:
                 text.textLine(line)
                 line = ''
             line+= f'#{i+1}/{roof_socres[i]}  '
         
         text.textLine(line)
         total_point = 0
+        text.setFillColor(colors.blue)
 
 ############################### SB referral 2.1
         total_score = overall_roof_condition_score[address_index]
         if key_name[i] == 'Tarp' and row[i]>0:
             if row[Tarp_index] == 1:
                 total_score/= 2
             else:
@@ -825,26 +1004,28 @@
         text.textLine(line)
         text.setFillColor(colors.blue)
         #################################
         for i in range(key_name_index+1, len(key_name)):
             if i == pixels_area_key:
                 gsd_area = row[gsd_key] * row[gsd_key] * row[pixels_area_key]
                 # text.textLine(f'Roof area: {int(gsd_area)} m\u00b2')
-                text.textLine(f'Roof area: {int(gsd_area * 10.764)} ft\u00b2')
+                text.textLine(f'Footprint area: {int(gsd_area * 10.764)} ft\u00b2')
                 continue
             if int(row[i]) == 0:
                 line = key_name[i] + ': ' + 'Not detected'
                 # text.textLine(line)     # Hide no detected case
             elif int(row[i]) == 1:
                 if key_name[i] == 'Pipeline' or key_name[i] =='Solar panel': 
                     line = key_name[i] + ': ' + 'Detected'
                     text.textLine(line)
                 if key_name[i] == 'Staining' or key_name[i] =='Water pooling' or key_name[i] =='Other damage':
                     line = key_name[i] + ': ' + 'Minor'
+                    text.setFillColor(colors.magenta)
                     text.textLine(line)
+                    text.setFillColor(colors.blue)
                 if key_name[i] == 'Skylight':
                     line = key_name[i] + ': ' + 'Minimal'
                     text.textLine(line)
                 if key_name[i] =='HVAC/Cooling tower':
                     # line = key_name[i] + ': ' + 'Minimal'
                     line = key_name[i] + ': ' + f'Minimal ({row[HVAC_index]})'
                     text.textLine(line)
@@ -863,15 +1044,17 @@
                     line = key_name[i] + ': ' + f'A few ({row[HVAC_index]})'
             else:
                 if key_name[i] == 'Pipeline' or key_name[i] =='Solar panel': 
                     line = key_name[i] + ': ' + 'Detected'
                     text.textLine(line)
                 if key_name[i] == 'Staining' or key_name[i] =='Water pooling' or key_name[i] =='Other damage':
                     line = key_name[i] + ': ' + 'Major'
+                    text.setFillColor(colors.magenta)
                     text.textLine(line)
+                    text.setFillColor(colors.blue)
                 if key_name[i] == 'Skylight':
                     line = key_name[i] + ': ' + 'Many'
                     text.textLine(line)
                 if key_name[i] =='HVAC/Cooling tower':
                     # line = key_name[i] + ': ' + 'Many'
                     line = key_name[i] + ': ' + f'Many ({row[HVAC_index]})'
                     text.textLine(line)
@@ -1091,8 +1274,8 @@
     msg["Subject"] = Header(mail_title, 'utf-8')
     msg["From"] = sender_qq_mail
     msg["To"] = receiver_email
 
     smtp.sendmail(sender_qq_mail, receiver_email, msg.as_string())
 
     smtp.quit()
-    print('Finish send email.')
+    print('Finish send email.')
```

