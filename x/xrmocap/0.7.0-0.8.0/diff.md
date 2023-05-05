# Comparing `tmp/xrmocap-0.7.0.tar.gz` & `tmp/xrmocap-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xrmocap-0.7.0.tar", last modified: Fri Dec 23 03:38:24 2022, max compression
+gzip compressed data, was "dist/xrmocap-0.8.0.tar", last modified: Fri May  5 08:32:01 2023, max compression
```

## Comparing `xrmocap-0.7.0.tar` & `xrmocap-0.8.0.tar`

### file list

```diff
@@ -1,146 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2022-12-23 03:38:24.000000 xrmocap-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2022-12-23 03:38:22.000000 xrmocap-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2022-12-23 03:38:24.000000 xrmocap-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2022-12-23 03:38:22.000000 xrmocap-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/core/estimation/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/estimation/base_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/estimation/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/estimation/mperson_smpl_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/estimation/mview_mperson_end2end_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17365 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/estimation/mview_mperson_topdown_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21318 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/estimation/mview_sperson_smpl_estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/evaluation/align_keypoints3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/evaluation/bottom_up_association_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/evaluation/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/evaluation/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    16515 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/evaluation/mvp_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20827 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/evaluation/top_down_association_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/core/hook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/hook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/core/hook/smplify_hook/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/hook/smplify_hook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/hook/smplify_hook/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/hook/smplify_hook/smplify_base_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/hook/smplify_hook/smplify_verbose_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/core/train/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/train/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23837 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/train/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/core/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/visualization/visualize_keypoints2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/core/visualization/visualize_keypoints3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/data_structure/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/data_structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/data_structure/body_model/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/data_structure/body_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15243 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/data_structure/body_model/smpl_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/data_structure/body_model/smplx_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/data_structure/body_model/smplxd_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/data_structure/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11366 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/data_structure/limbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32387 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/data_structure/smc_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/human_perception/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/human_perception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/human_perception/bbox_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/human_perception/bbox_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/human_perception/bbox_detection/mmdet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/human_perception/bbox_detection/mmtrack_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/human_perception/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/human_perception/keypoints_estimation/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/human_perception/keypoints_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/human_perception/keypoints_estimation/mediapipe_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/human_perception/keypoints_estimation/mmpose_top_down_estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/io/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/io/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/io/h5py_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/io/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/model/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/architecture/affinity_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/architecture/base_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/architecture/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19590 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/architecture/multi_view_pose_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/model/body_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/body_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/body_model/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/body_model/smpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/body_model/smplx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/model/registrant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/registrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/registrant/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/registrant/optimizable_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    43358 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/registrant/smplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/registrant/smplifyx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/model/registrant/smplifyxd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/transform/bbox/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/bbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/transform/convention/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/convention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/convention/bbox_convention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/transform/convention/keypoints_convention/
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/convention/keypoints_convention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/convention/keypoints_convention/campus.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/convention/keypoints_convention/fourdag_19.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/convention/keypoints_convention/human_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/convention/keypoints_convention/paf.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/convention/keypoints_convention/panoptic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/transform/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/image/base_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/image/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/image/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/image/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/image/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/image/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/aniposelib_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/fourdag_base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31777 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/fourdag_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/median_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/nan_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/rm_duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/smpl_shape_aware_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/trajectory_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/transform/limbs/
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/limbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/transform/point/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/point/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/transform/rotation/
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/transform/rotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/utils/camera_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/utils/distribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/utils/ffmpeg_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/utils/fourdag_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/utils/mvp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/utils/mvpose_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/utils/triangulation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2022-12-23 03:38:22.000000 xrmocap-0.7.0/xrmocap/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-23 03:38:24.000000 xrmocap-0.7.0/xrmocap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-05-05 08:32:01.000000 xrmocap-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-05-05 08:31:55.000000 xrmocap-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-05 08:32:01.000000 xrmocap-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-05 08:31:55.000000 xrmocap-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/core/estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/estimation/base_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/estimation/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/estimation/mperson_smpl_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/estimation/mview_mperson_end2end_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17365 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/estimation/mview_mperson_topdown_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19973 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/estimation/mview_sperson_smpl_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/base_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/bottom_up_association_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/end2end_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/metric_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/core/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/metrics/base_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/metrics/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/metrics/mpjpe_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/metrics/pa_mpjpe_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/metrics/pck_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/metrics/pcp_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/metrics/precision_recall_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/metrics/prediction_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/evaluation/top_down_association_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/core/hook/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/hook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/core/hook/smplify_hook/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/hook/smplify_hook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/hook/smplify_hook/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/hook/smplify_hook/smplify_base_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/hook/smplify_hook/smplify_verbose_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/core/train/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/train/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23757 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/train/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/core/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/core/visualization/render/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/visualization/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/visualization/render/mpr_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/visualization/visualize_keypoints2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/visualization/visualize_keypoints3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/core/visualization/visualize_smpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/data_structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/data_structure/body_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/data_structure/body_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/data_structure/body_model/smpl_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/data_structure/body_model/smplx_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/data_structure/body_model/smplxd_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/data_structure/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11366 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/data_structure/limbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32837 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/data_structure/smc_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/human_perception/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/human_perception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/human_perception/bbox_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/human_perception/bbox_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/human_perception/bbox_detection/mmdet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/human_perception/bbox_detection/mmdet_trt_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/human_perception/bbox_detection/mmtrack_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/human_perception/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/human_perception/keypoints_estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/human_perception/keypoints_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/human_perception/keypoints_estimation/mediapipe_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/human_perception/keypoints_estimation/mmpose_top_down_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/human_perception/keypoints_estimation/mmpose_trt_top_down_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/io/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/io/h5py_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/io/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/model/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/architecture/affinity_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/architecture/base_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/architecture/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19590 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/architecture/multi_view_pose_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/model/body_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/body_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/body_model/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/body_model/smpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/body_model/smplx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/model/registrant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/model/registrant/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/handler/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/handler/betas_prior_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/handler/body_pose_prior_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/handler/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/handler/keypoint3d_limb_length_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/handler/keypoint3d_mse_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/handler/multiview_keypoint2d_mse_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/optimizable_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43465 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/smplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/smplifyx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/model/registrant/smplifyxd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/transform/bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/bbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/transform/convention/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/convention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/convention/bbox_convention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/transform/convention/keypoints_convention/
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/convention/keypoints_convention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/convention/keypoints_convention/campus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/convention/keypoints_convention/fourdag_19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/convention/keypoints_convention/human_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/convention/keypoints_convention/paf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/convention/keypoints_convention/panoptic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/transform/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/image/base_image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/image/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/image/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/image/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/image/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/image/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/aniposelib_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/fourdag_base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31777 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/fourdag_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/median_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/nan_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/prior_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/rm_duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/smpl_shape_aware_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/trajectory_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/transform/limbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/limbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/transform/point/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/point/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/transform/rotation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/transform/rotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/utils/camera_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/utils/distribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/utils/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/utils/ffmpeg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/utils/fourdag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/utils/mvp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/utils/mvpose_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/utils/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/utils/triangulation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 08:31:55.000000 xrmocap-0.8.0/xrmocap/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 08:32:01.000000 xrmocap-0.8.0/xrmocap.egg-info/top_level.txt
```

### Comparing `xrmocap-0.7.0/PKG-INFO` & `xrmocap-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: xrmocap
-Version: 0.7.0
+Version: 0.8.0
 Summary: UNKNOWN
 Home-page: https://github.com/openxrlab/xrmocap
 Author: 
 Author-email: 
 License: Apache License 2.0
 Description: <br/>
         
         <div align="center">
             <img src="resources/xrmocap-logo.png" width="600"/>
         </div>
         
         <br/>
         
-        <div align="left">
+        <div align="center">
         
         [![Documentation](https://readthedocs.org/projects/xrmocap/badge/?version=latest)](https://xrmocap.readthedocs.io/en/latest/?badge=latest)
         [![actions](https://github.com/openxrlab/xrmocap/workflows/build/badge.svg)](https://github.com/openxrlab/xrmocap/actions)
         [![codecov](https://codecov.io/gh/openxrlab/xrmocap/branch/main/graph/badge.svg)](https://codecov.io/gh/openxrlab/xrmocap)
         [![PyPI](https://img.shields.io/pypi/v/xrmocap)](https://pypi.org/project/xrmocap/)
         [![Percentage of issues still open](https://isitmaintained.com/badge/open/openxrlab/xrmocap.svg)](https://github.com/openxrlab/xrmocap/issues)
         
@@ -92,14 +92,15 @@
         
         <details open>
         <summary>(click to collapse)</summary>
         
         - [x] [Campus](https://campar.in.tum.de/Chair/MultiHumanPose) (CVPR'2014)
         - [x] [Shelf](https://campar.in.tum.de/Chair/MultiHumanPose) (CVPR'2014)
         - [x] [CMU Panoptic](http://domedb.perception.cs.cmu.edu/) (ICCV'2015)
+        - [x] [4D Association](https://github.com/zhangyux15/multiview_human_dataset) (CVPR'2020)
         
         </details>
         
         
         ## Getting Started
         
         Please see [getting_started.md](docs/en/getting_started.md) for the basic usage of XRMoCap.
```

### Comparing `xrmocap-0.7.0/README.md` & `xrmocap-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div align="center">
     <img src="resources/xrmocap-logo.png" width="600"/>
 </div>
 
 <br/>
 
-<div align="left">
+<div align="center">
 
 [![Documentation](https://readthedocs.org/projects/xrmocap/badge/?version=latest)](https://xrmocap.readthedocs.io/en/latest/?badge=latest)
 [![actions](https://github.com/openxrlab/xrmocap/workflows/build/badge.svg)](https://github.com/openxrlab/xrmocap/actions)
 [![codecov](https://codecov.io/gh/openxrlab/xrmocap/branch/main/graph/badge.svg)](https://codecov.io/gh/openxrlab/xrmocap)
 [![PyPI](https://img.shields.io/pypi/v/xrmocap)](https://pypi.org/project/xrmocap/)
 [![Percentage of issues still open](https://isitmaintained.com/badge/open/openxrlab/xrmocap.svg)](https://github.com/openxrlab/xrmocap/issues)
 
@@ -84,14 +84,15 @@
 
 <details open>
 <summary>(click to collapse)</summary>
 
 - [x] [Campus](https://campar.in.tum.de/Chair/MultiHumanPose) (CVPR'2014)
 - [x] [Shelf](https://campar.in.tum.de/Chair/MultiHumanPose) (CVPR'2014)
 - [x] [CMU Panoptic](http://domedb.perception.cs.cmu.edu/) (ICCV'2015)
+- [x] [4D Association](https://github.com/zhangyux15/multiview_human_dataset) (CVPR'2020)
 
 </details>
 
 
 ## Getting Started
 
 Please see [getting_started.md](docs/en/getting_started.md) for the basic usage of XRMoCap.
```

### Comparing `xrmocap-0.7.0/setup.cfg` & `xrmocap-0.8.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 [isort]
 line_length = 79
 multi_line_output = 5
 include_trailing_comma = true
 known_standard_library = pkg_resources,setuptools
 known_first_party = xrmocap
-known_third_party = PIL,cv2,filterpy,h5py,matplotlib,mediapipe,mmcv,mmhuman3d,numpy,prettytable,pytest,pytorch3d,scipy,smplx,sphinx_rtd_theme,torch,torchvision,tqdm,xrprimer
+known_third_party = PIL,cv2,filterpy,h5py,matplotlib,mmcv,mmhuman3d,numpy,prettytable,pytest,pytorch3d,scipy,smplx,sphinx_rtd_theme,torch,torchvision,tqdm,xrprimer
 no_lines_before = STDLIB,LOCALFOLDER
 default_section = THIRDPARTY
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `xrmocap-0.7.0/setup.py` & `xrmocap-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/core/estimation/__init__.py` & `xrmocap-0.8.0/xrmocap/core/estimation/__init__.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/core/estimation/builder.py` & `xrmocap-0.8.0/xrmocap/core/estimation/builder.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/core/estimation/mperson_smpl_estimator.py` & `xrmocap-0.8.0/xrmocap/core/estimation/mperson_smpl_estimator.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/core/estimation/mview_mperson_end2end_estimator.py` & `xrmocap-0.8.0/xrmocap/core/estimation/mview_mperson_end2end_estimator.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/core/estimation/mview_mperson_topdown_estimator.py` & `xrmocap-0.8.0/xrmocap/core/estimation/mview_mperson_topdown_estimator.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/core/estimation/mview_sperson_smpl_estimator.py` & `xrmocap-0.8.0/xrmocap/core/estimation/mview_sperson_smpl_estimator.py`

 * *Files 4% similar despite different names*

```diff
@@ -231,68 +231,39 @@
         keypoints2d_list = self.estimate_keypoints2d(img_arr=mview_img_arr)
         keypoints3d = self.estimate_keypoints3d(
             cam_param=cam_param, keypoints2d_list=keypoints2d_list)
         smpl_data = self.estimate_smpl(
             keypoints3d=keypoints3d, init_smpl_data=init_smpl_data)
         return keypoints2d_list, keypoints3d, smpl_data
 
-    def estimate_keypoints2d(
-        self,
-        img_arr: Union[None, np.ndarray] = None,
-        img_paths: Union[None, List[List[str]]] = None,
-    ) -> List[Keypoints]:
+    def estimate_keypoints2d(self, img_arr: np.ndarray) -> List[Keypoints]:
         """Estimate keypoints2d in a top-down way.
 
         Args:
-            img_arr (Union[None, np.ndarray], optional):
+            img_arr (np.ndarray):
                 A multi-view image array, in shape
-                [n_view, n_frame, h, w, c]. Defaults to None.
-            img_paths (Union[None, List[List[str]]], optional):
-                A nested list of image paths, in shape
-                [n_view, n_frame]. Defaults to None.
+                [n_view, n_frame, h, w, c].
 
         Returns:
             List[Keypoints]:
                 A list of keypoints2d instances.
         """
         self.logger.info('Estimating keypoints2d.')
-        input_list = [img_arr, img_paths]
-        input_count = 0
-        for input_instance in input_list:
-            if input_instance is not None:
-                input_count += 1
-        if input_count > 1:
-            self.logger.error('Redundant input!\n' +
-                              'Please offer only one between' +
-                              ' img_arr, img_paths.')
-            raise ValueError
         ret_list = []
         for view_index in range(img_arr.shape[0]):
-            if img_arr is not None:
-                view_img_arr = img_arr[view_index]
-                bbox_list = self.bbox_detector.infer_array(
-                    image_array=view_img_arr,
-                    disable_tqdm=(not self.verbose),
-                    multi_person=False)
-                kps2d_list, _, _ = self.kps2d_estimator.infer_array(
-                    image_array=view_img_arr,
-                    bbox_list=bbox_list,
-                    disable_tqdm=(not self.verbose),
-                )
-            else:
-                bbox_list = self.bbox_detector.infer_frames(
-                    frame_path_list=img_paths,
-                    disable_tqdm=(not self.verbose),
-                    multi_person=True,
-                    load_batch_size=self.load_batch_size)
-                kps2d_list, _, _ = self.kps2d_estimator.infer_frames(
-                    frame_path_list=img_paths,
-                    bbox_list=bbox_list,
-                    disable_tqdm=(not self.verbose),
-                    load_batch_size=self.load_batch_size)
+            view_img_arr = img_arr[view_index]
+            bbox_list = self.bbox_detector.infer_array(
+                image_array=view_img_arr,
+                disable_tqdm=(not self.verbose),
+                multi_person=False)
+            kps2d_list, _, _ = self.kps2d_estimator.infer_array(
+                image_array=view_img_arr,
+                bbox_list=bbox_list,
+                disable_tqdm=(not self.verbose),
+            )
             if len(kps2d_list) == 1 and \
                     len(kps2d_list[0]) == 1 and \
                     kps2d_list[0][0] is None:
                 kps2d_list = [[]]
             keypoints2d = self.kps2d_estimator.get_keypoints_from_result(
                 kps2d_list)
             ret_list.append(keypoints2d)
```

### Comparing `xrmocap-0.7.0/xrmocap/core/evaluation/builder.py` & `xrmocap-0.8.0/xrmocap/core/evaluation/builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from mmcv.utils import Registry
 
 from .bottom_up_association_evaluation import BottomUpAssociationEvaluation
-from .mvp_evaluation import MVPEvaluation
+from .end2end_evaluation import End2EndEvaluation
 from .top_down_association_evaluation import TopDownAssociationEvaluation
 
 EVALUATION = Registry('evaluation')
 
 EVALUATION.register_module(
     name='TopDownAssociationEvaluation', module=TopDownAssociationEvaluation)
-EVALUATION.register_module(name='MVPEvaluation', module=MVPEvaluation)
+EVALUATION.register_module(name='End2EndEvaluation', module=End2EndEvaluation)
 EVALUATION.register_module(
     name='BottomUpAssociationEvaluation', module=BottomUpAssociationEvaluation)
 
 
 def build_evaluation(cfg):
     """Build a matching instance."""
     return EVALUATION.build(cfg)
```

### Comparing `xrmocap-0.7.0/xrmocap/core/evaluation/mvp_evaluation.py` & `xrmocap-0.8.0/xrmocap/human_perception/keypoints_estimation/mmpose_top_down_estimator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,417 +1,340 @@
-# yapf: disable
+import cv2
 import logging
 import numpy as np
-import os
-import time
-import torch
-from prettytable import PrettyTable
-from torch.utils.data import DataLoader
+from tqdm import tqdm
 from typing import List, Tuple, Union
+from xrprimer.utils.ffmpeg_utils import video_to_array
 from xrprimer.utils.log_utils import get_logger
 
-from xrmocap.core.evaluation.align_keypoints3d import align_keypoints3d
 from xrmocap.data_structure.keypoints import Keypoints
-from xrmocap.model.architecture.base_architecture import BaseArchitecture
-from xrmocap.utils.distribute_utils import collect_results, is_main_process
-from xrmocap.utils.mvp_utils import (
-    AverageMeter, convert_result_to_kps, norm2absolute,
-)
-from .metrics import calc_limbs_accuracy, evaluate
-
-# yapf: enable
-
-
-class MVPEvaluation:
-    """Evaluation for MvP method."""
-
-    def __init__(
-        self,
-        test_loader: DataLoader,
-        selected_limbs_name: List[List[str]] = [],
-        additional_limbs_names: List[List[str]] = [],
-        n_max_person: int = 10,
-        dataset_name: Union[None, str] = None,
-        pred_kps3d_convention: str = 'coco',
-        gt_kps3d_convention: str = 'coco',
-        print_freq: int = 100,
-        final_output_dir: Union[None, str] = None,
-        logger: Union[None, str, logging.Logger] = None,
-    ):
-        """Initialization for the class.
+from xrmocap.transform.convention.keypoints_convention import get_keypoint_num
+
+try:
+    from mmcv import digit_version
+    from mmpose import __version__ as mmpose_version
+    from mmpose.apis import inference_top_down_pose_model, init_pose_model
+    has_mmpose = True
+    import_exception = ''
+except (ImportError, ModuleNotFoundError):
+    has_mmpose = False
+    import traceback
+    stack_str = ''
+    for line in traceback.format_stack():
+        if 'frozen' not in line:
+            stack_str += line + '\n'
+    import_exception = traceback.format_exc() + '\n'
+    import_exception = stack_str + import_exception
+
+
+class MMposeTopDownEstimator:
+
+    def __init__(self,
+                 mmpose_kwargs: dict,
+                 bbox_thr: float = 0.0,
+                 logger: Union[None, str, logging.Logger] = None) -> None:
+        """Init a detector from mmpose.
 
         Args:
-            test_loader (DataLoader):
-                Test dataloader.
-            selected_limbs_name (List[List[str]], optional):
-                The name of selected
-                limbs in evaluation. Defaults to [].
-            additional_limbs_names (List[List[str]], optional):
-                Names at both ends of the limb. Defaults to [].
-            n_max_person (int, optional):
-                Number of maximum person the model can predict. Defaults to 10.
-            dataset_name (Union[None, str], optional):
-                Name of the dataset. Defaults to None.
-            pred_kps3d_convention (str, optional):
-                Keypoints3d convention of the predicted keypoints.
-                Defaults to 'coco'.
-            gt_kps3d_convention (str, optional):
-                Keypoints3d convention of the ground-truth keypoints.
-                Defaults to 'coco'.
-            print_freq (int, optional):
-                Printing frequency. Defaults to 100.
-            final_output_dir (Union[None, str], optional):
-                Directory to output folder. Defaults to None.
+            mmpose_kwargs (dict):
+                A dict contains args of mmpose.apis.init_detector.
+                Necessary keys: config, checkpoint
+                Optional keys: device
+            bbox_thr (float, optional):
+                Threshold of a bbox. Those have lower scores will be ignored.
+                Defaults to 0.0.
             logger (Union[None, str, logging.Logger], optional):
                 Logger for logging. If None, root logger will be selected.
                 Defaults to None.
         """
-
+        # build the pose model from a config file and a checkpoint file
+        self.pose_model = init_pose_model(**mmpose_kwargs)
+        # mmpose inference api takes one image per call
+        self.batch_size = 1
+        self.bbox_thr = bbox_thr
         self.logger = get_logger(logger)
+        if not has_mmpose:
+            self.logger.error(import_exception)
+            raise ModuleNotFoundError(
+                'Please install mmpose to run detection.')
+        self.use_old_api = False
+        if digit_version(mmpose_version) <= digit_version('0.13.0'):
+            self.use_old_api = True
 
-        self.test_loader = test_loader
-        self.dataset_name = dataset_name
-        self.print_freq = print_freq
-        self.output_dir = final_output_dir
-        self.dataset = test_loader.dataset
-        self.gt_n_frame = test_loader.dataset.len
-        self.pred_kps3d_convention = pred_kps3d_convention
-        self.n_max_person = n_max_person
-        self.selected_limbs_name = selected_limbs_name
-        self.additional_limbs_names = additional_limbs_names
-        self.gt_kps3d_convention = gt_kps3d_convention
-
-    def run(
-        self,
-        model: BaseArchitecture,
-        threshold: float = 0.1,
-        is_train: bool = False,
-    ):
-
-        # validate model and get predictions
-        preds_single = self.model_validate(
-            model,
-            threshold=threshold,
-            is_train=is_train,
-        )
-        kps3d_pred_list = collect_results(preds_single, len(self.dataset))
-
-        # save predicted keypoints3d
-        precision = None
-        if is_main_process():
-            n_frame = len(kps3d_pred_list)
-            n_kps = kps3d_pred_list[0].shape[1]
-            kps3d_pred = np.full((n_frame, self.n_max_person, n_kps, 4),
-                                 np.nan)
-
-            for frame_idx, per_frame_kps3d in enumerate(kps3d_pred_list):
-                if len(per_frame_kps3d) > 0:
-                    n_valid_person, keypoints3d_pred_valid = \
-                        convert_result_to_kps([per_frame_kps3d])
-                    kps3d_pred[
-                        frame_idx, :n_valid_person] = keypoints3d_pred_valid
-
-            keypoints3d_pred = Keypoints(
-                dtype='numpy',
-                kps=kps3d_pred,
-                mask=kps3d_pred[..., -1] > 0,
-                convention=self.pred_kps3d_convention,
-                logger=self.logger)
+    def get_keypoints_convention_name(self) -> str:
+        """Get data_source from dataset type in config file of the pose model.
 
-            # convert gt to keypoints3d
-            gt_n_person = np.max(
-                np.array([
-                    scene_keypoints.get_person_number()
-                    for scene_keypoints in self.dataset.gt3d
-                ]))
-            gt_n_kps = self.dataset.gt3d[0].get_keypoints_number()
-            kps3d_gt = np.full((self.gt_n_frame, gt_n_person, gt_n_kps, 4),
-                               np.nan)
-            mask_gt = np.full((self.gt_n_frame, gt_n_person, gt_n_kps), np.nan)
-
-            start_frame = 0
-            for keypoints3d_gt_scene in self.dataset.gt3d:
-
-                kps3d_gt_scene = keypoints3d_gt_scene.get_keypoints().numpy(
-                )  # [n_frame, n_person, n_kps, 4]
-                mask_gt_scene = keypoints3d_gt_scene.get_mask().numpy(
-                )  # [n_frame, n_person, n_kps]
-
-                n_frame, n_person, _, _ = kps3d_gt_scene.shape
-                end_frame = min(start_frame + n_frame, self.gt_n_frame)
-
-                kps3d_gt[start_frame:end_frame, :n_person, ...] = \
-                    kps3d_gt_scene[:end_frame-start_frame, ...]
-                mask_gt[start_frame:end_frame, :n_person, ...] = \
-                    mask_gt_scene[:end_frame-start_frame, ...]
-                start_frame = end_frame
-
-            keypoints3d_gt = Keypoints(
-                dtype='numpy',
-                kps=kps3d_gt,
-                mask=mask_gt,
-                convention=self.gt_kps3d_convention,
-                logger=self.logger)
+        Returns:
+            str:
+                Name of the keypoints convention. Must be
+                a key of KEYPOINTS_FACTORY.
+        """
+        return __translate_data_source__(
+            self.pose_model.cfg.data['test']['type'])
 
-            if not is_train:
-                pred_file = os.path.join(self.output_dir, 'pred_kps3d.npz')
-                gt_file = os.path.join(self.output_dir, 'gt_kps3d.npz')
-
-                self.logger.info(f'Saving 3D keypoints to: {pred_file}')
-                keypoints3d_pred.dump(pred_file)
-                self.logger.info(f'Saving 3D keypoints to: {gt_file}')
-                keypoints3d_gt.dump(gt_file)
-
-            # quantitative evaluation and print result
-            if 'panoptic' in self.dataset_name:
-                tb = PrettyTable()
-                mpjpe_threshold = np.arange(25, 155, 25)
-
-                aps, recs, mpjpe, recall500 = \
-                    self.evaluate_map(keypoints3d_pred, keypoints3d_gt)
-
-                tb.field_names = ['Threshold/mm'] + \
-                    [f'{i}' for i in mpjpe_threshold]
-                tb.add_row(['AP'] + [f'{ap * 100:.2f}' for ap in aps])
-                tb.add_row(['Recall'] + [f'{re * 100:.2f}' for re in recs])
-                tb.add_row(['recall@500mm'] +
-                           [f'{recall500 * 100:.2f}' for re in recs])
-                self.logger.info('\n' + tb.get_string())
-                self.logger.info(f'MPJPE: {mpjpe:.2f}mm')
-
-                precision = np.mean(aps[0])
-
-            elif 'campus' in self.dataset_name \
-                    or 'shelf' in self.dataset_name:
-
-                pred_keypoints3d_, gt_keypoints3d_, limbs = align_keypoints3d(
-                    keypoints3d_pred, keypoints3d_gt,
-                    self.pred_kps3d_convention, self.selected_limbs_name,
-                    self.additional_limbs_names)
-                check_result, eval_table = calc_limbs_accuracy(
-                    pred_keypoints3d_,
-                    gt_keypoints3d_,
-                    limbs,
-                    logger=self.logger)
-
-                person_wise_avg = np.sum(
-                    check_result > 0, axis=(0, 2)) / np.sum(
-                        np.abs(check_result), axis=(0, 2))
-                precision = np.sum(person_wise_avg) / len(person_wise_avg)
-
-                self.logger.info('\n' + eval_table.get_string())
-                evel_dict = evaluate(
-                    pred_keypoints3d_,
-                    gt_keypoints3d_,
-                    scale=1.,
-                    logger=self.logger)
-                self.logger.info('MPJPE: {:.2f} ± {:.2f} mm'.format(
-                    evel_dict['mpjpe_mean'], evel_dict['mpjpe_std']))
-                self.logger.info(
-                    f'PA-MPJPE: {evel_dict["pa_mpjpe_mean"]:.2f} ± '
-                    f'{evel_dict["pa_mpjpe_std"]:.2f} mm')
-                self.logger.info(f'PCK@50mm: {evel_dict["pck"][50]:.2f} %')
-                self.logger.info(f'PCK@100mm: {evel_dict["pck"][100]:.2f} %')
+    def infer_array(self,
+                    image_array: Union[np.ndarray, list],
+                    bbox_list: Union[tuple, list],
+                    disable_tqdm: bool = False,
+                    return_heatmap: bool = False) -> Tuple[list, list]:
+        """Infer frames already in memory(ndarray type).
+
+        Args:
+            image_array (Union[np.ndarray, list]):
+                BGR image ndarray in shape [n_frame, height, width, 3],
+                or a list of image ndarrays in shape [height, width, 3] while
+                len(list) == n_frame.
+            bbox_list (Union[tuple, list]):
+                A list of human bboxes.
+                Shape of the nested lists is (n_frame, n_human, 5).
+                Each bbox is a bbox_xyxy with a bbox_score at last.
+            disable_tqdm (bool, optional):
+                Whether to disable the entire progressbar wrapper.
+                Defaults to False.
+            return_heatmap (bool, optional):
+                Whether to return heatmap.
+                Defaults to False.
 
+        Returns:
+            Tuple[list, list]:
+                keypoints_list (list):
+                    A list of human keypoints.
+                    Shape of the nested lists is
+                    (n_frame, n_human, n_keypoints, 3).
+                    Each keypoint is an array of (x, y, confidence).
+                heatmap_list (list):
+                    A list of keypoint heatmaps. len(heatmap_list) == n_frame
+                    and the shape of heatmap_list[f] is
+                    (n_human, n_keypoints, width, height).
+                bbox_list (list):
+                    A list of human bboxes.
+                    Shape of the nested lists is (n_frame, n_human, 5).
+                    Each bbox is a bbox_xyxy with a bbox_score at last.
+                    It could be smaller than the input bbox_list,
+                    if there's no keypoints detected in some bbox.
+        """
+        ret_kps_list = []
+        ret_heatmap_list = []
+        ret_bbox_list = []
+        n_frame = len(image_array)
+        n_kps = get_keypoint_num(self.get_keypoints_convention_name())
+        for start_index in tqdm(
+                range(0, n_frame, self.batch_size), disable=disable_tqdm):
+            end_index = min(n_frame, start_index + self.batch_size)
+            # mmpose takes only one frame
+            img_arr = image_array[start_index]
+            person_results = []
+            for frame_index in range(start_index, end_index, 1):
+                bboxes_in_frame = []
+                for idx, bbox in enumerate(bbox_list[frame_index]):
+                    if bbox[4] > 0.0:
+                        bboxes_in_frame.append({'bbox': bbox, 'id': idx})
+                person_results = bboxes_in_frame
+            if not self.use_old_api:
+                img_input = dict(imgs_or_paths=img_arr)
+            else:
+                img_input = dict(img_or_path=img_arr)
+            if len(bboxes_in_frame) > 0:
+                pose_results, returned_outputs = inference_top_down_pose_model(
+                    model=self.pose_model,
+                    person_results=person_results,
+                    bbox_thr=self.bbox_thr,
+                    format='xyxy',
+                    dataset=self.pose_model.cfg.data['test']['type'],
+                    return_heatmap=return_heatmap,
+                    outputs=None,
+                    **img_input)
+                frame_kps_results = np.zeros(
+                    shape=(
+                        len(bbox_list[frame_index]),
+                        n_kps,
+                        3,
+                    ))
+                frame_heatmap_results = [
+                    None,
+                ] * len(bbox_list[frame_index])
+                frame_bbox_results = np.zeros(
+                    shape=(len(bbox_list[frame_index]), 5))
+                for idx, person_dict in enumerate(pose_results):
+                    id = person_dict['id']
+                    bbox = person_dict['bbox']
+                    keypoints = person_dict['keypoints']
+                    frame_bbox_results[id] = bbox
+                    frame_kps_results[id] = keypoints
+                    if return_heatmap:
+                        # returned_outputs[0]['heatmap'].shape:
+                        # 1, 133, 96, 72
+                        frame_heatmap_results[id] = returned_outputs[0][
+                            'heatmap'][idx]
+                        ret_heatmap_list += [frame_heatmap_results]
+                frame_kps_results = frame_kps_results.tolist()
+                frame_bbox_results = frame_bbox_results.tolist()
             else:
-                self.logger.warning(f'Dataset {self.dataset_name} '
-                                    'is not yet implemented.')
-                raise NotImplementedError
-
-        return precision
-
-    def model_validate(self,
-                       model: BaseArchitecture,
-                       threshold: float,
-                       is_train: bool = False):
-        """Validate model during training or testing.
+                frame_kps_results = []
+                frame_bbox_results = []
+            ret_kps_list += [frame_kps_results]
+            ret_bbox_list += [frame_bbox_results]
+        return ret_kps_list, ret_heatmap_list, ret_bbox_list
+
+    def infer_frames(
+            self,
+            frame_path_list: list,
+            bbox_list: Union[tuple, list],
+            disable_tqdm: bool = False,
+            return_heatmap: bool = False,
+            load_batch_size: Union[None, int] = None) -> Tuple[list, list]:
+        """Infer frames from file.
 
         Args:
-            model (BaseArchitecture):
-                Model to be evaluated.
-            threshold (float):
-                Confidence threshold to filter non-human keypoints.
-            is_train (bool, optional):
-                True if it is called during trainig. Defaults to False.
+            frame_path_list (list):
+                A list of frames' absolute paths.
+            bbox_list (Union[tuple, list]):
+                A list of human bboxes.
+                Shape of the nested lists is (n_frame, n_human, 5).
+                Each bbox is a bbox_xyxy with a bbox_score at last.
+            disable_tqdm (bool, optional):
+                Whether to disable the entire progressbar wrapper.
+                Defaults to False.
+            return_heatmap (bool, optional):
+                Whether to return heatmap.
+                Defaults to False.
+            load_batch_size (Union[None, int], optional):
+                How many frames are loaded at the same time.
+                Defaults to None, load all frames in frame_path_list.
 
         Returns:
-            float: model evaluation result, precision
+            Tuple[list, list]:
+                keypoints_list (list):
+                    A list of human keypoints.
+                    Shape of the nested lists is
+                    (n_frame, n_human, n_keypoints, 3).
+                    Each keypoint is an array of (x, y, confidence).
+                heatmap_list (list):
+                    A list of keypoint heatmaps. len(heatmap_list) == n_frame
+                    and the shape of heatmap_list[f] is
+                    (n_human, n_keypoints, width, height).
         """
-        batch_time = AverageMeter()
-        data_time = AverageMeter()
+        ret_kps_list = []
+        ret_heatmap_list = []
+        ret_boox_list = []
+        if load_batch_size is None:
+            load_batch_size = len(frame_path_list)
+        for start_idx in range(0, len(frame_path_list), load_batch_size):
+            end_idx = min(len(frame_path_list), start_idx + load_batch_size)
+            if load_batch_size < len(frame_path_list):
+                self.logger.info(
+                    'Processing mmpose on frames' +
+                    f'({start_idx}-{end_idx})/{len(frame_path_list)}')
+            image_array_list = []
+            for frame_abs_path in frame_path_list[start_idx:end_idx]:
+                img_np = cv2.imread(frame_abs_path)
+                image_array_list.append(img_np)
+            batch_pose_list, batch_heatmap_list, batch_boox_list = \
+                self.infer_array(
+                    image_array=image_array_list,
+                    bbox_list=bbox_list[start_idx:end_idx],
+                    disable_tqdm=disable_tqdm,
+                    return_heatmap=return_heatmap)
+            ret_kps_list += batch_pose_list
+            ret_heatmap_list += batch_heatmap_list
+            ret_boox_list += batch_boox_list
+        return ret_kps_list, ret_heatmap_list, ret_boox_list
+
+    def infer_video(self,
+                    video_path: str,
+                    bbox_list: Union[tuple, list],
+                    disable_tqdm: bool = False,
+                    return_heatmap: bool = False) -> Tuple[list, list]:
+        """Infer frames from a video file.
 
-        model.eval()
+        Args:
+            video_path (str):
+                Path to the video to be detected.
+            bbox_list (Union[tuple, list]):
+                A list of human bboxes.
+                Shape of the nested lists is (n_frame, n_human, 5).
+                Each bbox is a bbox_xyxy with a bbox_score at last.
+            disable_tqdm (bool, optional):
+                Whether to disable the entire progressbar wrapper.
+                Defaults to False.
+            return_heatmap (bool, optional):
+                Whether to return heatmap.
+                Defaults to False.
 
-        preds = []
-        with torch.no_grad():
-            end = time.time()
-            for i, (inputs, meta) in enumerate(self.test_loader):
-                data_time.update(time.time() - end)
-                assert len(inputs) == self.dataset.n_views
-                output = model(views=inputs, meta=meta)
-
-                gt_kps3d = meta[0]['kps3d'].float()
-                n_kps = gt_kps3d.shape[2]
-                bs, n_queries = output['pred_logits'].shape[:2]
-
-                src_poses = output['pred_poses']['outputs_coord']. \
-                    view(bs, n_queries, n_kps, 3)
-                src_poses = norm2absolute(src_poses, model.module.grid_size,
-                                          model.module.grid_center)
-                score = output['pred_logits'][:, :, 1:2].sigmoid()
-                score = score.unsqueeze(2).expand(-1, -1, n_kps, -1)
-                temp = (score > threshold).float() - 1
-
-                pred = torch.cat([src_poses, temp, score], dim=-1)
-                pred = pred.detach().cpu().numpy()
-                for b in range(pred.shape[0]):
-                    preds.append(pred[b])
-
-                batch_time.update(time.time() - end)
-                end = time.time()
-                if (i % self.print_freq == 0 or i
-                        == len(self.test_loader) - 1) and is_main_process():
-                    gpu_memory_usage = torch.cuda.memory_allocated(0)
-                    speed = len(inputs) * inputs[0].size(0) / batch_time.val
-                    msg = f'Test: [{i}/{len(self.test_loader)}]\t' \
-                        f'Time: {batch_time.val:.3f}s ' \
-                        f'({batch_time.avg:.3f}s)\t' \
-                        f'Speed: {speed:.1f} samples/s\t' \
-                        f'Data: {data_time.val:.3f}s ' \
-                        f'({data_time.avg:.3f}s)\t' \
-                        f'Memory {gpu_memory_usage:.1f}'
-                    self.logger.info(msg)
-
-        return preds
-
-    def evaluate_map(
-        self,
-        pred_keypoints3d: Keypoints,
-        gt_keypoints3d: Keypoints,
-        threshold: float = 0.1) \
-            -> Tuple[List[float], List[float], float, float]:
-        """Evaluate MPJPE, mAP and recall based on MPJPE. Mainly for panoptic
-        predictions.
+        Returns:
+            Tuple[list, list]:
+                keypoints_list (list):
+                    A list of human keypoints.
+                    Shape of the nested lists is
+                    (n_frame, n_human, n_keypoints, 3).
+                    Each keypoint is an array of (x, y, confidence).
+                heatmap_list (list):
+                    A list of keypoint heatmaps. len(heatmap_list) == n_frame
+                    and the shape of heatmap_list[f] is
+                    (n_human, n_keypoints, width, height).
+        """
+        image_array = video_to_array(input_path=video_path, logger=self.logger)
+        ret_kps_list, ret_heatmap_list, ret_boox_list = self.infer_array(
+            image_array=image_array,
+            bbox_list=bbox_list,
+            disable_tqdm=disable_tqdm,
+            return_heatmap=return_heatmap)
+        return ret_kps_list, ret_heatmap_list, ret_boox_list
+
+    def get_keypoints_from_result(
+            self, kps2d_list: List[list]) -> Union[Keypoints, None]:
+        """Convert returned keypoints2d into an instance of class Keypoints.
 
         Args:
-            pred_keypoints3d (Keypoints):
-                Predicted 3D keypoints.
-            threshold (float):
-                Threshold for valid keypoints. Defaults to 0.1.
+            kps2d_list (List[list]):
+                A list of human keypoints, returned by
+                infer methods.
+                Shape of the nested lists is
+                (n_frame, n_human, n_keypoints, 3).
 
         Returns:
-            Tuple[List[float], List[float], float, float]:
-                List of AP, list of recall, MPJPE value and recall@500mm.
+            Union[Keypoints, None]:
+                An instance of Keypoints with mask and
+                convention, data type is numpy.
+                If no one has been detected in any frame,
+                a None will be returned.
         """
+        # shape: (n_frame, n_human, n_keypoints, 3)
+        n_frame = len(kps2d_list)
+        human_count_list = [len(human_list) for human_list in kps2d_list]
+        if len(human_count_list) > 0:
+            n_human = max(human_count_list)
+        else:
+            n_human = 0
+        n_keypoints = get_keypoint_num(self.get_keypoints_convention_name())
+        if n_human > 0:
+            kps2d_arr = np.zeros(shape=(n_frame, n_human, n_keypoints, 3))
+            mask_arr = np.ones_like(kps2d_arr[..., 0], dtype=np.uint8)
+            for f_idx in range(n_frame):
+                if len(kps2d_list[f_idx]) <= 0:
+                    mask_arr[f_idx, ...] = 0
+                    continue
+                for h_idx in range(n_human):
+                    if h_idx < len(kps2d_list[f_idx]):
+                        mask_arr[f_idx, h_idx, ...] = np.sign(
+                            np.array(kps2d_list[f_idx][h_idx])[:, -1])
+                        kps2d_arr[f_idx,
+                                  h_idx, :, :] = kps2d_list[f_idx][h_idx]
+                    else:
+                        mask_arr[f_idx, h_idx, ...] = 0
+            keypoints2d = Keypoints(
+                kps=kps2d_arr,
+                mask=mask_arr,
+                convention=self.get_keypoints_convention_name(),
+                logger=self.logger)
+        else:
+            keypoints2d = None
+        return keypoints2d
 
-        pred_kps3d = pred_keypoints3d.get_keypoints()
-        gt_kps3d = gt_keypoints3d.get_keypoints()
-        gt_n_frame, _, _, _ = gt_kps3d.shape
-        pred_n_frame, _, n_kps, _ = pred_kps3d.shape
-        total_gt = 0
-        eval_list = []
-        if not pred_n_frame == gt_n_frame:
-            self.logger.error(f'Frame number mismatch: {pred_n_frame} '
-                              f'pred and {self.gt_n_frame} gt')
-            raise ValueError
-
-        trans_ground = np.array([[1.0, 0.0, 0.0], [0.0, 0.0, -1.0],
-                                 [0.0, 1.0, 0.0]])
-
-        for frame_idx_all_scenes in range(gt_n_frame):
-
-            gt_frame_kps3d = gt_kps3d[frame_idx_all_scenes, :, :n_kps, :]
-            check_valid = np.sum(gt_frame_kps3d, axis=1)  # [n_person, 4]
-            gt_frame_kps3d = gt_frame_kps3d[check_valid[:, -1] > 0]
-
-            gt_frame_kps3d = [
-                gt_person_kps3d[:, 0:3].dot(trans_ground)
-                for gt_person_kps3d in gt_frame_kps3d
-            ]
-            if len(gt_frame_kps3d) == 0:
-                continue
-
-            pred_frame_kps3d_valid = pred_kps3d[frame_idx_all_scenes].copy()
-
-            for pred_person_kps3d in pred_frame_kps3d_valid:
-                mpjpes = []
-                for gt_person_kps3d in gt_frame_kps3d:
-                    vis = gt_person_kps3d[:, -1] > threshold
-
-                    mpjpe = np.mean(
-                        np.sqrt(
-                            np.sum(
-                                (np.array(pred_person_kps3d[vis, 0:3]) -
-                                 np.array(gt_person_kps3d[vis, 0:3]))**2,
-                                axis=-1)))
-                    mpjpes.append(mpjpe)
-                min_gt = np.argmin(mpjpes)
-                min_mpjpe = np.min(mpjpes)
-                score = pred_person_kps3d[0, -1]
-                eval_list.append({
-                    'mpjpe': float(min_mpjpe),
-                    'score': float(score),
-                    'gt_id': int(total_gt + min_gt)
-                })
-
-            total_gt += len(gt_frame_kps3d)
-
-        mpjpe_threshold = np.arange(25, 155, 25)
-        aps = []
-        recs = []
-        for t in mpjpe_threshold:
-            ap, rec = self._eval_list_to_ap(eval_list, total_gt, t)
-            aps.append(ap)
-            recs.append(rec)
-
-        return \
-            aps, \
-            recs, \
-            self._eval_list_to_mpjpe(eval_list), \
-            self._eval_list_to_recall(eval_list, total_gt)
-
-    def _eval_list_to_ap(self, eval_list, total_gt, threshold):
-        """convert evaluation result to ap."""
-        eval_list.sort(key=lambda k: k['score'], reverse=True)
-        total_num = len(eval_list)
-
-        tp = np.zeros(total_num)
-        fp = np.zeros(total_num)
-        gt_det = []
-        for i, item in enumerate(eval_list):
-            if item['mpjpe'] < threshold and item['gt_id'] not in gt_det:
-                tp[i] = 1
-                gt_det.append(item['gt_id'])
-            else:
-                fp[i] = 1
-        tp = np.cumsum(tp)
-        fp = np.cumsum(fp)
-        recall = tp / (total_gt + 1e-5)
-        precise = tp / (tp + fp + 1e-5)
-        for n in range(total_num - 2, -1, -1):
-            precise[n] = max(precise[n], precise[n + 1])
-
-        precise = np.concatenate(([0], precise, [0]))
-        recall = np.concatenate(([0], recall, [1]))
-        index = np.where(recall[1:] != recall[:-1])[0]
-        ap = np.sum((recall[index + 1] - recall[index]) * precise[index + 1])
-
-        return ap, recall[-2]
-
-    def _eval_list_to_mpjpe(self, eval_list, threshold=500):
-        """convert evaluation result to mpjpe."""
-        eval_list.sort(key=lambda k: k['score'], reverse=True)
-        gt_det = []
-
-        mpjpes = []
-        for i, item in enumerate(eval_list):
-            if item['mpjpe'] < threshold and item['gt_id'] not in gt_det:
-                mpjpes.append(item['mpjpe'])
-                gt_det.append(item['gt_id'])
-
-        return np.mean(mpjpes) if len(mpjpes) > 0 else np.inf
-
-    def _eval_list_to_recall(self, eval_list, total_gt, threshold=500):
-        """convert evaluation result to recall."""
-        gt_ids = [e['gt_id'] for e in eval_list if e['mpjpe'] < threshold]
 
-        return len(np.unique(gt_ids)) / total_gt
+def __translate_data_source__(mmpose_dataset_name):
+    if mmpose_dataset_name == 'TopDownSenseWholeBodyDataset':
+        return 'sense_whole_body'
+    elif mmpose_dataset_name == 'TopDownCocoWholeBodyDataset':
+        return 'coco_wholebody'
+    else:
+        raise NotImplementedError
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xrmocap-0.7.0/xrmocap/core/evaluation/top_down_association_evaluation.py` & `xrmocap-0.8.0/xrmocap/core/evaluation/bottom_up_association_evaluation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,294 +1,214 @@
 # yapf: disable
-import csv
 import logging
 import numpy as np
 import os.path as osp
-import time
-from prettytable import PrettyTable
+import prettytable
+import string
 from tqdm import tqdm
-from typing import List, Tuple, Union
-from xrprimer.utils.log_utils import get_logger
+from typing import List, Union
 from xrprimer.utils.path_utils import prepare_output_path
 
-from xrmocap.data.data_visualization.builder import (
-    BaseDataVisualization, build_data_visualization,
-)
-from xrmocap.data.dataset.builder import MviewMpersonDataset, build_dataset
+from xrmocap.data.data_visualization.builder import BaseDataVisualization
+from xrmocap.data.dataset.builder import MviewMpersonDataset
 from xrmocap.data_structure.keypoints import Keypoints
-from xrmocap.ops.top_down_association.builder import (
-    MvposeAssociator, build_top_down_associator,
+from xrmocap.ops.bottom_up_association.builder import (
+    FourDAGAssociator, build_bottom_up_associator,
 )
 from xrmocap.transform.convention.keypoints_convention import (
     convert_keypoints, get_keypoint_idx, get_keypoint_num,
 )
-from xrmocap.transform.limbs import get_limbs_from_keypoints
-from xrmocap.utils.geometry import compute_similarity_transform
 from xrmocap.utils.mvpose_utils import (
-    add_campus_jaw_headtop, add_campus_jaw_headtop_mask, check_limb_is_correct,
-    compute_mpjpe, vectorize_distance,
+    add_campus_jaw_headtop, add_campus_jaw_headtop_mask,
 )
+from .base_evaluation import BaseEvaluation
+from .metrics.base_metric import BaseMetric
 
 # yapf: enable
 
 
-class TopDownAssociationEvaluation:
-    """Top-down association evaluation."""
+class BottomUpAssociationEvaluation(BaseEvaluation):
+    """Bottom-up association evaluation."""
 
     def __init__(self,
                  output_dir: str,
-                 selected_limbs_name: List[List[str]],
-                 additional_limbs_names: List[List[str]],
                  dataset: Union[dict, MviewMpersonDataset],
-                 associator: Union[dict, MvposeAssociator],
+                 associator: Union[dict, FourDAGAssociator],
+                 metric_list: List[Union[dict, BaseMetric]],
                  dataset_visualization: Union[None, dict,
                                               BaseDataVisualization] = None,
                  pred_kps3d_convention: str = 'coco',
                  eval_kps3d_convention: str = 'campus',
+                 pick_dict: Union[dict, None] = None,
                  logger: Union[None, str, logging.Logger] = None) -> None:
         """Initialization for the class.
 
         Args:
             output_dir (str): The path to save results.
-            selected_limbs_name (List[List[str]]): The name of selected
-                limbs in evaluation.
-            additional_limbs_names (List[List[str]]):
-                Names at both ends of the limb.
             dataset (Union[dict, MviewMpersonDataset])
             associator (Union[dict, MvposeAssociator])
+            metric_list (List[Union[dict, BaseMetric]]):
+                A list of metrics to be evaluated.
             dataset_visualization
                 (Union[None, dict, BaseDataVisualization], optional):
                 Defaults to None.
             pred_kps3d_convention (str, optional): Target convention of
                 keypoints3d, Defaults to 'coco'.
             eval_kps3d_convention (str, optional): the convention of
                 keypoints3d for evaluation, Defaults to 'campus'.
+            pick_dict (Union[dict, None], optional):
+                Selected metrics to be printed in the final table.
+                Defaults to None.
             logger (Union[None, str, logging.Logger], optional):
                 Logger for logging. If None, root logger will be selected.
                 Defaults to None.
         """
 
-        self.output_dir = output_dir
+        BaseEvaluation.__init__(
+            self,
+            dataset=dataset,
+            output_dir=output_dir,
+            metric_list=metric_list,
+            pick_dict=pick_dict,
+            dataset_visualization=dataset_visualization,
+            eval_kps3d_convention=eval_kps3d_convention,
+            logger=logger)
+
         self.pred_kps3d_convention = pred_kps3d_convention
-        self.eval_kps3d_convention = eval_kps3d_convention
-        self.additional_limbs_names = additional_limbs_names
-        self.selected_limbs_name = selected_limbs_name
-        self.logger = get_logger(logger)
-
-        if isinstance(dataset, dict):
-            dataset['logger'] = self.logger
-            self.dataset = build_dataset(dataset)
-        else:
-            self.dataset = dataset
+        self.n_views = self.dataset.n_views
 
         if isinstance(associator, dict):
             associator['logger'] = self.logger
-            self.associator = build_top_down_associator(associator)
+            associator['n_views'] = self.n_views
+            self.associator = build_bottom_up_associator(associator)
         else:
             self.associator = associator
 
-        if isinstance(dataset_visualization, dict):
-            dataset_visualization['logger'] = self.logger
-            self.dataset_visualization = build_data_visualization(
-                dataset_visualization)
-        else:
-            self.dataset_visualization = dataset_visualization
-
     def run(self, overwrite: bool = False):
         prepare_output_path(
             output_path=self.output_dir,
             allowed_suffix='',
             path_type='dir',
             overwrite=overwrite,
             logger=self.logger)
         n_frame = len(self.dataset)
         n_kps = get_keypoint_num(convention=self.pred_kps3d_convention)
         pred_kps3d = np.zeros(shape=(n_frame, 1, n_kps, 4))
-        matched_kps2d_idx = [[] for _ in range(n_frame)]
+        pred_kps2d = np.zeros(shape=(n_frame, 1, self.n_views, n_kps, 3))
         gt_kps3d = None
         max_identity = 0
         end_of_clip_idxs = []
         identities = []
         for frame_idx, frame_item in enumerate(tqdm(self.dataset)):
-            mview_img_tensor, _, _, _, kps3d, end_of_clip, kw_data = frame_item
+            _, _, _, _, kps3d, end_of_clip, kps2d, pafs = frame_item
             if end_of_clip:
                 end_of_clip_idxs.append(frame_idx)
             fisheye_list = self.dataset.fisheye_params[0]
-            mview_img_arr = np.asarray(mview_img_tensor * 255).astype(np.uint8)
-            mview_kps2d_list = kw_data['kps2d']
-            mview_bbox2d_list = kw_data['bbox2d']
             # prepare input for associate single frame
-            mview_keypoints2d_list = []
-            for view_idx, kps2d in enumerate(mview_kps2d_list):
-                keypoints2d = Keypoints(
-                    dtype='numpy',
-                    kps=kps2d.unsqueeze(0),
-                    mask=kps2d[..., -1].unsqueeze(0) > 0,
-                    convention=self.dataset.kps2d_convention,
-                    logger=self.logger)
-                mview_keypoints2d_list.append(keypoints2d)
-            self.associator.set_cameras(fisheye_list)
-
-            keypoints2d_idx, predict_keypoints3d, identities = \
-                self.associator.associate_frame(
-                    mview_img_arr=mview_img_arr,
-                    mview_bbox2d=mview_bbox2d_list,
-                    mview_keypoints2d=mview_keypoints2d_list,
-                    affinity_type='geometry_mean'
-                )
 
+            self.associator.set_cameras(fisheye_list)
+            predict_keypoints3d, identities, multi_kps2d, _ = \
+                self.associator.associate_frame(kps2d, pafs, end_of_clip)
             # save predict kps3d
             for idx, identity in enumerate(identities):
                 if identity > max_identity:
                     n_identity = identity - max_identity
                     pred_kps3d = np.concatenate(
                         (pred_kps3d,
                          np.zeros(shape=(n_frame, n_identity, n_kps, 4))),
                         axis=1)
+                    pred_kps2d = np.concatenate(
+                        (pred_kps2d,
+                         np.zeros(
+                             shape=(n_frame, n_identity, self.n_views, n_kps,
+                                    3))),
+                        axis=1)
                     max_identity = identity
                 pred_kps3d[frame_idx,
                            identity] = predict_keypoints3d.get_keypoints()[0,
                                                                            idx]
-            for i in range(max_identity + 1):
-                if i in identities:
-                    index = identities.index(i)
-                    matched_kps2d_idx[frame_idx].append(keypoints2d_idx[index])
+                # prepare 2d associate result
+                if identity in multi_kps2d:
+                    pred_kps2d[frame_idx, identity] = multi_kps2d[identity]
             # save ground truth kps3d
             if gt_kps3d is None:
                 gt_kps3d = kps3d.numpy()[np.newaxis]
             else:
                 gt_kps3d = np.concatenate(
                     (gt_kps3d, kps3d.numpy()[np.newaxis]), axis=0)
 
-        pred_keypoints3d = Keypoints(
+        pred_keypoints3d_raw = Keypoints(
             dtype='numpy',
             kps=pred_kps3d,
             mask=pred_kps3d[..., -1] > 0,
             convention=self.pred_kps3d_convention,
             logger=self.logger)
-        gt_keypoints3d = Keypoints(
+        gt_keypoints3d_raw = Keypoints(
             dtype='numpy',
             kps=gt_kps3d,
             mask=gt_kps3d[..., -1] > 0,
             convention=self.dataset.gt_kps3d_convention,
             logger=self.logger)
-
         mscene_keypoints_paths = []
+
+        # prepare result
         scene_start_idx = 0
         for scene_idx, scene_end_idx in enumerate(end_of_clip_idxs):
-            scene_keypoints = pred_keypoints3d.clone()
+            scene_keypoints = pred_keypoints3d_raw.clone()
             kps3d = scene_keypoints.get_keypoints()[
                 scene_start_idx:scene_end_idx + 1, ...]
             mask = scene_keypoints.get_mask()[scene_start_idx:scene_end_idx +
                                               1, ...]
             scene_keypoints.set_keypoints(kps3d)
             scene_keypoints.set_mask(mask)
             npz_path = osp.join(self.output_dir,
                                 f'scene{scene_idx}_pred_keypoints3d.npz')
             scene_keypoints.dump(npz_path)
-            scence_matched_kps2d_idx = matched_kps2d_idx[
-                scene_start_idx:scene_end_idx + 1]
-            np.save(
-                osp.join(self.output_dir,
-                         f'scene{scene_idx}_matched_kps2d_idx.npy'),
-                scence_matched_kps2d_idx)
             mscene_keypoints_paths.append(npz_path)
+
+            npz_path = osp.join(self.output_dir,
+                                f'scene{scene_idx}_associate_keypoints2d')
+            associate_kps2d = pred_kps2d[scene_start_idx:scene_end_idx + 1,
+                                         ...]
+            np.save(npz_path, associate_kps2d)
+
             scene_start_idx = scene_end_idx + 1
 
-        pred_keypoints3d_, gt_keypoints3d_, limbs = self.align_keypoints3d(
-            pred_keypoints3d, gt_keypoints3d)
-        self.calc_limbs_accuracy(pred_keypoints3d_, gt_keypoints3d_, limbs)
-        pck_50, pck_100, mpjpe, pa_mpjpe = self.evaluate(
-            pred_keypoints3d_, gt_keypoints3d_)
+        pred_keypoints3d, gt_keypoints3d = self.align_keypoints3d(
+            pred_keypoints3d_raw, gt_keypoints3d_raw,
+            self.eval_kps3d_convention)
+
+        # evaluate and print results
+        eval_results, full_results = self.metric_manager(
+            pred_keypoints3d=pred_keypoints3d, gt_keypoints3d=gt_keypoints3d)
+
+        table = prettytable.PrettyTable()
+        table.field_names = ['Metric name', 'Value']
+        for metric_name, metric_dict in eval_results.items():
+            for key, value in metric_dict.items():
+                table.add_row([f'{metric_name}: {key}', f'{value:.2f}'])
+        table_str = '\n' + table.get_string()
+        self.logger.info(table_str)
 
+        # visualization
         if self.dataset_visualization is not None:
             self.dataset_visualization.pred_kps3d_paths = \
                 mscene_keypoints_paths
             self.dataset_visualization.run(overwrite=overwrite)
 
-    def evaluate(self,
-                 pred_keypoints3d: Keypoints,
-                 gt_keypoints3d: Keypoints,
-                 pck_50_thres=50,
-                 pck_100_thres=100,
-                 scale=1000.) -> dict:
-        # There must be no np.nan in the pred_keypoints3d
-        mpjpe, pa_mpjpe, pck_50, pck_100 = [], [], [], []
-        n_frame = gt_keypoints3d.get_frame_number()
-        gt_kps3d = gt_keypoints3d.get_keypoints()[..., :3]
-        gt_kps3d_mask = gt_keypoints3d.get_mask()
-        pred_kps3d = pred_keypoints3d.get_keypoints()[..., :3]
-        pred_kps3d_mask = pred_keypoints3d.get_mask()
-        pred_kps3d_convention = pred_keypoints3d.get_convention()
-        gt_kps3d_convention = gt_keypoints3d.get_convention()
-        for frame_idx in range(n_frame):
-            if not gt_kps3d_mask[frame_idx].any():
-                continue
-            gt_kps3d_idxs = np.where(
-                np.sum(gt_kps3d_mask[frame_idx], axis=1) > 0)[0]
-            for gt_kps3d_idx in gt_kps3d_idxs:
-                f_gt_kps3d = gt_kps3d[frame_idx][gt_kps3d_idx]
-                f_pred_kps3d = pred_kps3d[frame_idx][
-                    np.sum(pred_kps3d_mask[frame_idx], axis=1) > 0]
-                if len(f_pred_kps3d) == 0:
-                    continue
-
-                dist = vectorize_distance(f_gt_kps3d[np.newaxis], f_pred_kps3d)
-                f_pred_kps3d = f_pred_kps3d[np.argmin(dist[0])]
-
-                if np.all((f_pred_kps3d == 0)):
-                    continue
-
-                # MPJPE
-                f_pred_keypoints = Keypoints(
-                    kps=np.concatenate(
-                        (f_pred_kps3d, np.ones_like(f_pred_kps3d[..., 0:1])),
-                        axis=-1),
-                    convention=pred_kps3d_convention)
-                f_gt_keypoints = Keypoints(
-                    kps=np.concatenate(
-                        (f_gt_kps3d, np.ones_like(f_gt_kps3d[..., 0:1])),
-                        axis=-1),
-                    convention=gt_kps3d_convention)
-                mpjpe.append(
-                    compute_mpjpe(
-                        f_pred_keypoints, f_gt_keypoints, align=True))
-
-                # PA-MPJPE
-                _, _, rotation, scaling, transl = compute_similarity_transform(
-                    f_gt_kps3d, f_pred_kps3d, compute_optimal_scale=True)
-                pred_kps3d_pa = (scaling * f_pred_kps3d.dot(rotation)) + transl
-
-                pred_keypoints_pa = Keypoints(
-                    kps=np.concatenate(
-                        (pred_kps3d_pa, np.ones_like(pred_kps3d_pa[..., 0:1])),
-                        axis=-1),
-                    convention=pred_kps3d_convention)
-                pa_mpjpe_i = compute_mpjpe(
-                    pred_keypoints_pa, f_gt_keypoints, align=True)
-                pa_mpjpe.append(pa_mpjpe_i)
-
-                pck_50.append(np.mean(pa_mpjpe_i <= (pck_50_thres / scale)))
-                pck_100.append(np.mean(pa_mpjpe_i <= (pck_100_thres / scale)))
-        mpjpe = np.asarray(mpjpe) * scale  # m to mm
-        pa_mpjpe = np.asarray(pa_mpjpe) * scale  # m to mm
-        mpjpe_mean, mpjpe_std = np.mean(mpjpe), np.std(mpjpe)
-        pa_mpjpe_mean, pa_mpjpe_std = np.mean(pa_mpjpe), np.std(pa_mpjpe)
-        pck_50 = np.mean(pck_50) * 100.  # percentage
-        pck_100 = np.mean(pck_100) * 100.  # percentage
-        self.logger.info(f'MPJPE: {mpjpe_mean:.2f} ± {mpjpe_std:.2f} mm')
-        self.logger.info(f'PA-MPJPE: {pa_mpjpe_mean:.2f} ±'
-                         f'{pa_mpjpe_std:.2f} mm')
-        self.logger.info(f'PCK@{pck_50_thres}mm: {pck_50:.2f} %')
-        self.logger.info(f'PCK@{pck_100_thres}mm: {pck_100:.2f} %')
-        return pck_50, pck_100, mpjpe, pa_mpjpe
-
     def align_keypoints3d(self, pred_keypoints3d: Keypoints,
-                          gt_keypoints3d: Keypoints):
-        ret_limbs = []
+                          gt_keypoints3d: Keypoints,
+                          eval_kps3d_convention: string):
+        """align keypoints convention.
+
+        Args:
+            pred_keypoints3d (Keypoints): prediction of keypoints
+            gt_keypoints3d (Keypoints): ground true of keypoints
+            eval_kps3d_convention (string): keypoints convention to align
+        """
         gt_nose = None
         pred_nose = None
         pred_kps3d_convention = pred_keypoints3d.get_convention()
         gt_kps3d_convention = gt_keypoints3d.get_convention()
         if gt_kps3d_convention == 'panoptic':
             gt_nose_index = get_keypoint_idx(
                 name='nose_openpose', convention=gt_kps3d_convention)
@@ -296,43 +216,37 @@
 
         if pred_kps3d_convention == 'coco':
             pred_nose_index = get_keypoint_idx(
                 name='nose', convention=pred_kps3d_convention)
             pred_nose = pred_keypoints3d.get_keypoints()[:, :,
                                                          pred_nose_index, :3]
 
-        if pred_kps3d_convention != self.eval_kps3d_convention:
+        if pred_kps3d_convention == 'fourdag_19' or\
+                pred_kps3d_convention == 'openpose_25':
+            pred_leftear_index = get_keypoint_idx(
+                name='left_ear_openpose', convention=pred_kps3d_convention)
+            pre_rightear_index = get_keypoint_idx(
+                name='right_ear_openpose', convention=pred_kps3d_convention)
+            head_center = (
+                pred_keypoints3d.get_keypoints()[:, :, pred_leftear_index, :3]
+                + pred_keypoints3d.get_keypoints()[:, :,
+                                                   pre_rightear_index, :3]) / 2
+            pred_nose = head_center
+
+        if pred_kps3d_convention != eval_kps3d_convention:
             pred_keypoints3d = convert_keypoints(
                 keypoints=pred_keypoints3d,
-                dst=self.eval_kps3d_convention,
+                dst=eval_kps3d_convention,
                 approximate=True)
-        if gt_kps3d_convention != self.eval_kps3d_convention:
+        if gt_kps3d_convention != eval_kps3d_convention:
             gt_keypoints3d = convert_keypoints(
                 keypoints=gt_keypoints3d,
-                dst=self.eval_kps3d_convention,
+                dst=eval_kps3d_convention,
                 approximate=True)
 
-        limbs = get_limbs_from_keypoints(
-            keypoints=pred_keypoints3d, fill_limb_names=True)
-        limb_name_list = []
-        conn_list = []
-        for limb_name, conn in limbs.get_connections_by_names().items():
-            limb_name_list.append(limb_name)
-            conn_list.append(conn)
-
-        for idx, limb_name in enumerate(limb_name_list):
-            if limb_name in self.selected_limbs_name:
-                ret_limbs.append(conn_list[idx])
-
-        for conn_names in self.additional_limbs_names:
-            kps_idx_0 = get_keypoint_idx(
-                name=conn_names[0], convention=self.eval_kps3d_convention)
-            kps_idx_1 = get_keypoint_idx(
-                name=conn_names[1], convention=self.eval_kps3d_convention)
-            ret_limbs.append(np.array([kps_idx_0, kps_idx_1], dtype=np.int32))
         pred_kps3d_mask = pred_keypoints3d.get_mask()
         pred_kps3d = pred_keypoints3d.get_keypoints()[..., :3]
         if pred_nose is not None:
             pred_kps3d = add_campus_jaw_headtop(pred_nose, pred_kps3d)
             pred_kps3d_mask = add_campus_jaw_headtop_mask(pred_kps3d_mask)
 
         gt_kps3d_mask = gt_keypoints3d.get_mask()
@@ -342,127 +256,14 @@
             gt_kps3d_mask = add_campus_jaw_headtop_mask(gt_kps3d_mask)
 
         pred_kps3d = np.concatenate(
             (pred_kps3d, pred_kps3d_mask[..., np.newaxis]), axis=-1)
         pred_keypoints3d = Keypoints(
             kps=pred_kps3d,
             mask=pred_kps3d_mask,
-            convention=self.eval_kps3d_convention)
+            convention=eval_kps3d_convention)
         gt_kps3d = np.concatenate((gt_kps3d, gt_kps3d_mask[..., np.newaxis]),
                                   axis=-1)
         gt_keypoints3d = Keypoints(
-            kps=gt_kps3d,
-            mask=gt_kps3d_mask,
-            convention=self.eval_kps3d_convention)
-
-        return pred_keypoints3d, gt_keypoints3d, ret_limbs
+            kps=gt_kps3d, mask=gt_kps3d_mask, convention=eval_kps3d_convention)
 
-    def calc_limbs_accuracy(self,
-                            pred_keypoints3d,
-                            gt_keypoints3d,
-                            limbs,
-                            dump_dir=None) -> Tuple[np.ndarray, list]:
-        n_frame = gt_keypoints3d.get_frame_number()
-        n_gt_person = gt_keypoints3d.get_person_number()
-        gt_kps3d = gt_keypoints3d.get_keypoints()[..., :3]
-        gt_kps3d_mask = gt_keypoints3d.get_mask()
-        pred_kps3d = pred_keypoints3d.get_keypoints()[..., :3]
-        pred_kps3d_mask = pred_keypoints3d.get_mask()
-        check_result = np.zeros((n_frame, n_gt_person, len(limbs) + 1),
-                                dtype=np.int32)
-        accuracy_cnt = 0
-        error_cnt = 0
-
-        for idx in range(n_frame):
-            if not gt_kps3d_mask[idx].any():
-                continue
-            gt_kps3d_idxs = np.where(np.sum(gt_kps3d_mask[idx], axis=1) > 0)[0]
-            for gt_kps3d_idx in gt_kps3d_idxs:
-                f_gt_kps3d = gt_kps3d[idx][gt_kps3d_idx]
-                f_pred_kps3d = pred_kps3d[idx][
-                    np.sum(pred_kps3d_mask[idx], axis=1) > 0]
-                if len(f_pred_kps3d) == 0:
-                    continue
-
-                dist = vectorize_distance(f_gt_kps3d[np.newaxis], f_pred_kps3d)
-                f_pred_kps3d = f_pred_kps3d[np.argmin(dist[0])]
-
-                for i, limb in enumerate(limbs):
-                    start_point, end_point = limb
-                    if check_limb_is_correct(f_pred_kps3d[start_point],
-                                             f_pred_kps3d[end_point],
-                                             f_gt_kps3d[start_point],
-                                             f_gt_kps3d[end_point]):
-                        check_result[idx, gt_kps3d_idx, i] = 1
-                        accuracy_cnt += 1
-                    else:
-                        check_result[idx, gt_kps3d_idx, i] = -1
-                        error_cnt += 1
-                gt_hip = (f_gt_kps3d[2] + f_gt_kps3d[3]) / 2
-                pred_hip = (f_pred_kps3d[2] + f_pred_kps3d[3]) / 2
-                if check_limb_is_correct(pred_hip, f_pred_kps3d[12], gt_hip,
-                                         f_gt_kps3d[12]):
-                    check_result[idx, gt_kps3d_idx, -1] = 1
-                    accuracy_cnt += 1
-                else:
-                    check_result[idx, gt_kps3d_idx, -1] = -1
-                    error_cnt += 1
-        bone_group = dict([('Head', np.array([8])), ('Torso', np.array([9])),
-                           ('Upper arms', np.array([5, 6])),
-                           ('Lower arms', np.array([4, 7])),
-                           ('Upper legs', np.array([1, 2])),
-                           ('Lower legs', np.array([0, 3]))])
-
-        person_wise_avg = np.sum(
-            check_result > 0, axis=(0, 2)) / np.sum(
-                np.abs(check_result), axis=(0, 2))
-
-        bone_wise_result = dict()
-        bone_person_wise_result = dict()
-        for k, v in bone_group.items():
-            bone_wise_result[k] = np.sum(check_result[:, :, v] > 0) / np.sum(
-                np.abs(check_result[:, :, v]))
-            bone_person_wise_result[k] = np.sum(
-                check_result[:, :, v] > 0, axis=(0, 2)) / np.sum(
-                    np.abs(check_result[:, :, v]), axis=(0, 2))
-
-        tb = PrettyTable()
-        tb.field_names = ['Bone Group'] + [
-            f'Actor {i}'
-            for i in range(bone_person_wise_result['Head'].shape[0])
-        ] + ['Average']
-        list_tb = [tb.field_names]
-        for k, v in bone_person_wise_result.items():
-            this_row = [k] + [np.char.mod('%.4f', i) for i in v
-                              ] + [np.char.mod('%.4f',
-                                               np.sum(v) / len(v))]
-            list_tb.append([
-                float(i) if isinstance(i, type(np.array([]))) else i
-                for i in this_row
-            ])
-            tb.add_row(this_row)
-        this_row = ['Total'] + [
-            np.char.mod('%.4f', i) for i in person_wise_avg
-        ] + [
-            np.char.mod('%.4f',
-                        np.sum(person_wise_avg) / len(person_wise_avg))
-        ]
-        tb.add_row(this_row)
-        list_tb.append([
-            float(i) if isinstance(i, type(np.array([]))) else i
-            for i in this_row
-        ])
-        if dump_dir:
-            np.save(
-                osp.join(
-                    dump_dir,
-                    time.strftime('%Y_%m_%d_%H_%M',
-                                  time.localtime(time.time()))), check_result)
-            with open(
-                    osp.join(
-                        dump_dir,
-                        time.strftime('%Y_%m_%d_%H_%M.csv',
-                                      time.localtime(time.time()))), 'w') as f:
-                writer = csv.writer(f)
-                writer.writerows(list_tb)
-        self.logger.info('\n' + tb.get_string())
-        return check_result, list_tb
+        return pred_keypoints3d, gt_keypoints3d
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xrmocap-0.7.0/xrmocap/core/hook/smplify_hook/smplify_base_hook.py` & `xrmocap-0.8.0/xrmocap/core/hook/smplify_hook/smplify_base_hook.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/core/hook/smplify_hook/smplify_verbose_hook.py` & `xrmocap-0.8.0/xrmocap/core/hook/smplify_hook/smplify_verbose_hook.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/core/train/trainer.py` & `xrmocap-0.8.0/xrmocap/core/train/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,18 +261,17 @@
 
         mvp_cfg = dict(
             type='MviewPoseTransformer', is_train=True, logger=self.logger)
         mvp_cfg.update(self.mvp_setup)
         model = build_architecture(mvp_cfg)
 
         eval_cfg = dict(
-            type='MVPEvaluation',
             test_loader=test_loader,
             print_freq=self.print_freq,
-            final_output_dir=self.final_output_dir,
+            output_dir=self.final_output_dir,
             logger=self.logger)
         eval_cfg.update(self.evaluation_setup)
         evaluation = build_evaluation(eval_cfg)
 
         model.to(self.device)
         model.criterion.to(self.device)
 
@@ -437,18 +436,17 @@
 
         mvp_cfg = dict(
             type='MviewPoseTransformer', is_train=False, logger=self.logger)
         mvp_cfg.update(self.mvp_setup)
         model = build_architecture(mvp_cfg)
 
         eval_cfg = dict(
-            type='MVPEvaluation',
             test_loader=test_loader,
             print_freq=self.print_freq,
-            final_output_dir=self.final_output_dir,
+            output_dir=self.final_output_dir,
             logger=self.logger)
         eval_cfg.update(self.evaluation_setup)
         evaluation = build_evaluation(eval_cfg)
 
         model.to(self.device)
         model.criterion.to(self.device)
```

### Comparing `xrmocap-0.7.0/xrmocap/core/visualization/visualize_keypoints2d.py` & `xrmocap-0.8.0/xrmocap/core/visualization/visualize_keypoints2d.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/core/visualization/visualize_keypoints3d.py` & `xrmocap-0.8.0/xrmocap/core/visualization/visualize_keypoints3d.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/data_structure/body_model/smpl_data.py` & `xrmocap-0.8.0/xrmocap/data_structure/body_model/smpl_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,29 +25,24 @@
     }
     FULL_POSE_KEYS = {
         'global_orient',
         'body_pose',
     }
 
     def __init__(self,
-                 src_dict: dict = None,
                  gender: Union[Literal['female', 'male', 'neutral'],
                                None] = None,
                  fullpose: Union[np.ndarray, torch.Tensor, None] = None,
                  transl: Union[np.ndarray, torch.Tensor, None] = None,
                  betas: Union[np.ndarray, torch.Tensor, None] = None,
+                 mask: Union[np.ndarray, torch.Tensor, None] = None,
                  logger: Union[None, str, logging.Logger] = None) -> None:
-        """Construct a SMPLData instance with pre-set values. If any of gender,
-        fullpose, transl, betas is provided, it will override the item in
-        source_dict.
+        """Construct a SMPLData instance with pre-set values.
 
         Args:
-            src_dict (dict, optional):
-                A dict with items in HumanData fashion.
-                Defaults to None.
             gender (Union[
                     Literal['female', 'male', 'neutral'], None], optional):
                 Gender of the body model.
                 Should be one among ["female", "male", "neutral"].
                 Defaults to None.
             fullpose (Union[np.ndarray, torch.Tensor, None], optional):
                 A tensor or ndarray for fullpose, in shape [n_frame, 24, 3].
@@ -56,22 +51,24 @@
                 A tensor or ndarray for translation, in shape [n_frame, 3].
                 Defaults to None, zero-tensor will be created.
             betas (Union[np.ndarray, torch.Tensor, None], optional):
                 A tensor or ndarray for translation,
                 in shape [n_frame, betas_dim].
                 Defaults to None,
                 zero-tensor in shape [n_frame, 10] will be created.
+            mask (Union[np.ndarray, torch.Tensor, None], optional):
+                A tensor or ndarray for framewise visibility mask,
+                in shape [n_frame, ].
+                Defaults to None,
+                one-tensor in shape [n_frame, ] will be created.
             logger (Union[None, str, logging.Logger], optional):
                 Logger for logging. If None, root logger will be selected.
                 Defaults to None.
         """
-        if src_dict is not None:
-            super().__init__(src_dict)
-        else:
-            super().__init__()
+        super().__init__()
         self.n_body_joints = self.__class__.DEFAULT_BODY_JOINTS_NUM
         self.logger = get_logger(logger)
         if gender is None and 'gender' not in self:
             gender = 'neutral'
         if gender is not None:
             self.set_gender(gender)
         if fullpose is None and 'fullpose' not in self:
@@ -83,14 +80,18 @@
             transl = np.zeros(shape=(self.get_batch_size(), 3))
         if transl is not None:
             self.set_transl(transl)
         if betas is None and 'betas' not in self:
             betas = np.zeros(shape=(self.get_batch_size(), 10))
         if betas is not None:
             self.set_betas(betas)
+        if mask is None and 'mask' not in self:
+            mask = np.ones(shape=(self.get_batch_size()))
+        if mask is not None:
+            self.set_mask(mask)
 
     @classmethod
     def fromfile(cls, npz_path: str) -> 'SMPLData':
         """Construct a body model data structure from an npz file.
 
         Args:
             npz_path (str):
@@ -101,14 +102,38 @@
                 A SMPLData instance load from file.
         """
         ret_instance = cls()
         ret_instance.load(npz_path)
         return ret_instance
 
     @classmethod
+    def from_dict(cls, smpl_data_dict: Union['SMPLData', dict]) -> 'SMPLData':
+        """Construct a body model data structure from a SMPLData, or a degraded
+        smpl_data in dict type.
+
+        Args:
+            smpl_data_dict (dict):
+                A degraded smpl_data in dict type.
+
+        Returns:
+            SMPLData:
+                A SMPLData instance load from dict.
+        """
+        min_keys = {'gender', 'fullpose', 'transl', 'betas'}
+        assert min_keys <= smpl_data_dict.keys()
+        ret_instance = cls(
+            gender=smpl_data_dict['gender'],
+            fullpose=smpl_data_dict['fullpose'],
+            transl=smpl_data_dict['transl'],
+            betas=smpl_data_dict['betas'],
+        )
+
+        return ret_instance
+
+    @classmethod
     def get_fullpose_dim(cls) -> int:
         """Get dimension of full pose.
 
         Returns:
             int:
                 Dim value. Full pose shall be
                 in shape (frame_n, dim, 3)
@@ -203,14 +228,35 @@
             raise TypeError
         if len(betas.shape) == 1:
             betas = betas[np.newaxis, ...]
         betas_dim = betas.shape[-1]
         betas_np = betas.reshape(-1, betas_dim)
         super().__setitem__('betas', betas_np)
 
+    def set_mask(self, mask: Union[np.ndarray, torch.Tensor]) -> None:
+        """Set framewise mask data.
+
+        Args:
+            mask (Union[np.ndarray, torch.Tensor]):
+                Visibility mask in ndarray or tensor,
+                in shape [batch_size, ].
+
+        Raises:
+            TypeError: Type of mask is not correct.
+        """
+        if isinstance(mask, np.ndarray):
+            mask_np = mask.reshape(-1).astype(np.uint8)
+        elif isinstance(mask, torch.Tensor):
+            mask_np = mask.detach().cpu().numpy().reshape(-1).astype(np.uint8)
+        else:
+            self.logger.error('Type of mask is not correct.\n' +
+                              f'Type: {type(mask)}.')
+            raise TypeError
+        super().__setitem__('mask', mask_np)
+
     def __setitem__(self, __k: Any, __v: Any) -> None:
         """Set item according to its key.
 
         Args:
             __k (Any): Key in dict.
             __v (Any): Value in dict.
         """
@@ -218,14 +264,16 @@
             self.set_gender(__v)
         elif __k == 'transl':
             self.set_transl(__v)
         elif __k == 'fullpose':
             self.set_fullpose(__v)
         elif __k == 'betas':
             self.set_betas(__v)
+        elif __k == 'mask':
+            self.set_mask(__v)
         else:
             super().__setitem__(__k, __v)
 
     def get_batch_size(self) -> int:
         """Get batch size.
 
         Returns:
@@ -291,14 +339,30 @@
         betas = self.__getitem__('betas')
         if repeat_betas and\
                 betas.shape[0] == 1 and\
                 betas.shape[0] != batch_size:
             betas = betas.repeat(repeats=batch_size, axis=0)
         return betas
 
+    def get_mask(self) -> np.ndarray:
+        """Get mask.
+
+        Returns:
+            ndarray: mask in shape [batch_size, ].
+        """
+        return self.__getitem__('mask').reshape(-1)
+
+    def get_gender(self) -> str:
+        """Get gender.
+
+        Returns:
+            str: gender in ['neutral', 'female', 'male'].
+        """
+        return self.__getitem__('gender')
+
     def to_param_dict(self, repeat_betas: bool = True) -> dict:
         """Split fullpose into global_orient and body_pose, return all the
         necessary parameters in one dict.
 
         Args:
             repeat_betas (bool, optional):
                 Whether to repeat betas when its first dim doesn't match
@@ -371,15 +435,16 @@
                 self.logger.error(
                     'File exists while overwrite option not checked.\n' +
                     f'npz_path: {npz_path}')
                 raise FileExistsError
         np.savez_compressed(npz_path, **self)
 
     def from_param_dict(self, smpl_dict: dict) -> None:
-        """Load SMPL parameters from smpl_dict.
+        """Load SMPL parameters from smpl_dict, which is the output of a body
+        model in most cases.
 
         Args:
             smpl_dict (dict):
                 A dict of ndarray|Tensor parameters.
                 global_orient and body_pose are necessary,
                 transl and betas are optional.
                 Other keys are ignored.
@@ -408,19 +473,25 @@
 
         fullpose = concat_func([global_orient, body_pose], dim=1)
         self.set_fullpose(fullpose)
         if 'transl' in smpl_dict:
             self.set_transl(smpl_dict['transl'])
         if 'betas' in smpl_dict:
             self.set_betas(smpl_dict['betas'])
+        # reset mask to make sure correspondence
+        self.set_mask(np.ones(shape=(self.get_batch_size())))
 
     def load(self, npz_path: str):
         """Load data from npz_path and update them to self.
 
         Args:
             npz_path (str):
                 Path to a dumped npz file.
         """
         with np.load(npz_path, allow_pickle=True) as npz_file:
             tmp_data_dict = dict(npz_file)
             for key, value in tmp_data_dict.items():
+                if isinstance(value, np.ndarray) and\
+                        len(value.shape) == 0:
+                    # value is not an ndarray before dump
+                    value = value.item()
                 self.__setitem__(key, value)
```

### Comparing `xrmocap-0.7.0/xrmocap/data_structure/body_model/smplx_data.py` & `xrmocap-0.8.0/xrmocap/data_structure/body_model/smplx_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,30 +27,25 @@
     }
     FULL_POSE_KEYS = {
         'global_orient', 'body_pose', 'left_hand_pose', 'right_hand_pose',
         'jaw_pose', 'leye_pose', 'reye_pose'
     }
 
     def __init__(self,
-                 src_dict: dict = None,
                  gender: Union[Literal['female', 'male', 'neutral'],
                                None] = None,
                  fullpose: Union[np.ndarray, torch.Tensor, None] = None,
                  transl: Union[np.ndarray, torch.Tensor, None] = None,
                  betas: Union[np.ndarray, torch.Tensor, None] = None,
                  expression: Union[np.ndarray, torch.Tensor, None] = None,
+                 mask: Union[np.ndarray, torch.Tensor, None] = None,
                  logger: Union[None, str, logging.Logger] = None) -> None:
-        """Construct a SMPLXData instance with pre-set values. If any of
-        gender, fullpose, transl, betas is provided, it will override the item
-        in source_dict.
+        """Construct a SMPLXData instance with pre-set values.
 
         Args:
-            src_dict (dict, optional):
-                A dict with items in HumanData fashion.
-                Defaults to None.
             gender (Union[
                     Literal['female', 'male', 'neutral'], None], optional):
                 Gender of the body model.
                 Should be one among ["female", "male", "neutral"].
                 Defaults to None.
             fullpose (Union[np.ndarray, torch.Tensor, None], optional):
                 A tensor or ndarray for fullpose, in shape [frame_num, 24, 3].
@@ -64,33 +59,63 @@
                 Defaults to None,
                 zero-tensor in shape [frame_num, 10] will be created.
             expression (Union[np.ndarray, torch.Tensor, None], optional):
                 A tensor or ndarray for expression,
                 in shape [frame_num, expression_dim].
                 Defaults to None,
                 zero-tensor in shape [frame_num, 10] will be created.
+            mask (Union[np.ndarray, torch.Tensor, None], optional):
+                A tensor or ndarray for framewise visibility mask,
+                in shape [n_frame, ].
+                Defaults to None,
+                one-tensor in shape [n_frame, ] will be created.
             logger (Union[None, str, logging.Logger], optional):
                 Logger for logging. If None, root logger will be selected.
                 Defaults to None.
         """
         SMPLData.__init__(
             self,
-            src_dict=src_dict,
             gender=gender,
             transl=transl,
             fullpose=fullpose,
             betas=betas,
+            mask=mask,
             logger=logger)
         if expression is None and 'expression' not in self:
             expression = np.zeros(shape=(self.get_batch_size(), 10))
         if expression is not None:
             self.set_expression(expression)
         self.body_joints_num = self.__class__.DEFAULT_BODY_JOINTS_NUM
 
     @classmethod
+    def from_dict(cls, smpl_data_dict: Union['SMPLXData',
+                                             dict]) -> 'SMPLXData':
+        """Construct a body model data structure from a SMPLXData, or a
+        degraded smplx_data in dict type.
+
+        Args:
+            smplx_data_dict (dict):
+                A degraded smplx_data in dict type.
+
+        Returns:
+            SMPLXData:
+                A SMPLXData instance load from dict.
+        """
+        smplx_data_dict = smpl_data_dict
+        min_keys = {'gender', 'fullpose', 'transl', 'betas', 'expression'}
+        assert min_keys <= smplx_data_dict.keys()
+        ret_instance = cls(
+            gender=smplx_data_dict['gender'],
+            fullpose=smplx_data_dict['fullpose'],
+            transl=smplx_data_dict['transl'],
+            betas=smplx_data_dict['betas'],
+            expression=smplx_data_dict['expression'])
+        return ret_instance
+
+    @classmethod
     def get_fullpose_dim(cls) -> int:
         """Get dimension of full pose.
 
         Returns:
             int:
                 Dim value. Full pose shall be
                 in shape (frame_n, dim, 3)
@@ -156,21 +181,22 @@
         """
         if __k == 'expression':
             self.set_expression(__v)
         else:
             SMPLData.__setitem__(self, __k, __v)
 
     def from_param_dict(self, smplx_dict: dict) -> None:
-        """Load SMPLX parameters from smplx_dict.
+        """Load SMPLX parameters from smplx_dict, which is the output of a body
+        model in most cases.
 
         Args:
             smplx_dict (dict):
                 A dict of ndarray|Tensor parameters.
                 global_orient and body_pose are necessary,
-                jaw_pose, leye_pose, reye_pose,
+                expression, jaw_pose, leye_pose, reye_pose,
                 left_hand_pose, right_hand_pose, transl and
                 betas are optional.
                 Other keys are ignored.
 
         Raises:
             KeyError: missing necessary keys.
         """
@@ -257,14 +283,16 @@
         ],
                                dim=1)
         self.set_fullpose(fullpose)
         if 'transl' in smplx_dict:
             self.set_transl(smplx_dict['transl'])
         if 'betas' in smplx_dict:
             self.set_betas(smplx_dict['betas'])
+        if 'expression' in smplx_dict:
+            self.set_expression(smplx_dict['expression'])
 
     def to_param_dict(self,
                       repeat_betas: bool = True,
                       repeat_expression: bool = True) -> dict:
         """Split fullpose into global_orient, body_pose, jaw_pose, leye_pose,
         reye_pose, left_hand_pose, right_hand_pose, return all the necessary
         parameters in one dict.
@@ -284,34 +312,36 @@
                 jaw_pose, leye_pose, reye_pose, left_hand_pose,
                 right_hand_pose, expression.
         """
         dict_to_return = SMPLData.to_param_dict(
             self, repeat_betas=repeat_betas)
         dict_to_return.pop('body_pose')
         fullpose = self.get_fullpose()
+        batch_size = self.get_batch_size()
         start_idx = 1
         body_pose = fullpose[:, start_idx:start_idx +
                              self.__class__.BODY_POSE_LEN].reshape(
-                                 self.get_batch_size(), -1)
+                                 batch_size, -1)
         start_idx += self.__class__.BODY_POSE_LEN
         jaw_pose = fullpose[:, start_idx:start_idx +
                             self.__class__.JAW_POSE_LEN].reshape(-1, 3)
         start_idx += self.__class__.JAW_POSE_LEN
         leye_pose = fullpose[:, start_idx:start_idx +
                              self.__class__.EYE_POSE_LEN].reshape(-1, 3)
         start_idx += self.__class__.EYE_POSE_LEN
         reye_pose = fullpose[:, start_idx:start_idx +
                              self.__class__.EYE_POSE_LEN].reshape(-1, 3)
         start_idx += self.__class__.EYE_POSE_LEN
         left_hand_pose = fullpose[:, start_idx:start_idx +
-                                  self.__class__.HAND_POSE_LEN].reshape(-1, 3)
+                                  self.__class__.HAND_POSE_LEN].reshape(
+                                      batch_size, -1)
         start_idx += self.__class__.HAND_POSE_LEN
         right_hand_pose = fullpose[:, start_idx:start_idx +
                                    self.__class__.HAND_POSE_LEN].reshape(
-                                       -1, 3)
+                                       batch_size, -1)
         expression = self.get_expression(repeat_expression=repeat_expression)
         dict_to_return.update({
             'body_pose': body_pose,
             'jaw_pose': jaw_pose,
             'leye_pose': leye_pose,
             'reye_pose': reye_pose,
             'left_hand_pose': left_hand_pose,
```

### Comparing `xrmocap-0.7.0/xrmocap/data_structure/body_model/smplxd_data.py` & `xrmocap-0.8.0/xrmocap/data_structure/body_model/smplxd_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,31 +15,26 @@
 # yapf: enable
 
 
 class SMPLXDData(SMPLXData):
     NUM_VERTS = 10475
 
     def __init__(self,
-                 src_dict: dict = None,
                  gender: Union[Literal['female', 'male', 'neutral'],
                                None] = None,
                  fullpose: Union[np.ndarray, torch.Tensor, None] = None,
                  transl: Union[np.ndarray, torch.Tensor, None] = None,
                  betas: Union[np.ndarray, torch.Tensor, None] = None,
                  expression: Union[np.ndarray, torch.Tensor, None] = None,
                  displacement: Union[np.ndarray, torch.Tensor, None] = None,
+                 mask: Union[np.ndarray, torch.Tensor, None] = None,
                  logger: Union[None, str, logging.Logger] = None) -> None:
-        """Construct a SMPLXData instance with pre-set values. If any of
-        gender, fullpose, transl, betas is provided, it will override the item
-        in source_dict.
+        """Construct a SMPLXData instance with pre-set values.
 
         Args:
-            src_dict (dict, optional):
-                A dict with items in HumanData fashion.
-                Defaults to None.
             gender (Union[
                     Literal['female', 'male', 'neutral'], None], optional):
                 Gender of the body model.
                 Should be one among ["female", "male", "neutral"].
                 Defaults to None.
             fullpose (Union[np.ndarray, torch.Tensor, None], optional):
                 A tensor or ndarray for fullpose, in shape [frame_num, 24, 3].
@@ -55,66 +50,100 @@
             expression (Union[np.ndarray, torch.Tensor, None], optional):
                 A tensor or ndarray for expression,
                 in shape [frame_num, expression_dim].
                 Defaults to None,
                 zero-tensor in shape [frame_num, 10] will be created.
             displacement (Union[np.ndarray, torch.Tensor, None], optional):
                 A tensor or ndarray for displacement,
-                in shape [frame_num, NUM_VERTS].
+                in shape [frame_num, NUM_VERTS, 3].
                 Defaults to None,
                 zero-tensor in shape [frame_num, NUM_VERTS] will be created.
+            mask (Union[np.ndarray, torch.Tensor, None], optional):
+                A tensor or ndarray for framewise visibility mask,
+                in shape [n_frame, ].
+                Defaults to None,
+                one-tensor in shape [n_frame, ] will be created.
             logger (Union[None, str, logging.Logger], optional):
                 Logger for logging. If None, root logger will be selected.
                 Defaults to None.
         """
         SMPLXData.__init__(
             self,
-            src_dict=src_dict,
             gender=gender,
             transl=transl,
             fullpose=fullpose,
             betas=betas,
             expression=expression,
+            mask=mask,
             logger=logger)
         if displacement is None and 'displacement' not in self:
             displacement = np.zeros(
-                shape=(self.get_batch_size(), self.__class__.NUM_VERTS))
+                shape=(self.get_batch_size(), self.__class__.NUM_VERTS, 3))
         if displacement is not None:
             self.set_displacement(displacement)
 
+    @classmethod
+    def from_dict(cls, smpl_data_dict: Union['SMPLXDData',
+                                             dict]) -> 'SMPLXDData':
+        """Construct a body model data structure from a SMPLXDData, or a
+        degraded smplxd_data in dict type.
+
+        Args:
+            smplxd_data_dict (dict):
+                A degraded smplxd_data in dict type.
+
+        Returns:
+            SMPLXData:
+                A SMPLXDData instance load from dict.
+        """
+        smplxd_data_dict = smpl_data_dict
+        min_keys = {
+            'gender', 'fullpose', 'transl', 'betas', 'expression',
+            'displacement'
+        }
+        assert min_keys <= smplxd_data_dict.keys()
+        ret_instance = cls(
+            gender=smplxd_data_dict['gender'],
+            fullpose=smplxd_data_dict['fullpose'],
+            transl=smplxd_data_dict['transl'],
+            betas=smplxd_data_dict['betas'],
+            expression=smplxd_data_dict['expression'],
+            displacement=smplxd_data_dict['displacement'])
+        return ret_instance
+
     def set_displacement(
             self, displacement: Union[np.ndarray, torch.Tensor]) -> None:
         """Set displacement data.
 
         Args:
             displacement (Union[np.ndarray, torch.Tensor]):
                 Displacement parameters in ndarray or tensor,
-                in shape [batch_size, NUM_VERTS].
+                in shape [batch_size, NUM_VERTS, 3].
 
         Raises:
             TypeError: Type of displacement is not correct.
         """
         if isinstance(displacement, torch.Tensor):
             displacement = displacement.detach().cpu().numpy()
         elif not isinstance(displacement, np.ndarray):
             self.logger.error('Type of displacement is not correct.\n' +
                               f'Type: {type(displacement)}.')
             raise TypeError
-        if len(displacement.shape) == 1:
-            displacement = displacement[np.newaxis, ...]
-        displacement_dim = displacement.shape[-1]
-        displacement_np = displacement.reshape(-1, displacement_dim)
-        dict.__setitem__(self, 'displacement', displacement_np)
+        if len(displacement.shape) < 3:
+            self.logger.error('Shape of displacement is not correct.\n' +
+                              f'Shape: {type(displacement.shape)}.')
+            raise ValueError
+        dict.__setitem__(self, 'displacement', displacement)
 
     def get_displacement(self) -> np.ndarray:
         """Get displacement.
 
         Returns:
             ndarray:
-                Displacement in shape [batch_size, NUM_VERTS].
+                Displacement in shape [batch_size, NUM_VERTS, 3].
         """
         displacement = self.__getitem__('displacement')
         return displacement
 
     def __setitem__(self, __k: Any, __v: Any) -> None:
         """Set item according to its key.
 
@@ -124,15 +153,16 @@
         """
         if __k == 'displacement':
             self.set_displacement(__v)
         else:
             SMPLXData.__setitem__(self, __k, __v)
 
     def from_param_dict(self, smplxd_dict: dict) -> None:
-        """Load SMPLX+D parameters from smplxd_dict.
+        """Load SMPLX+D parameters from smplxd_dict, which is the output of a
+        body model in most cases.
 
         Args:
             smplx_dict (dict):
                 A dict of ndarray|Tensor parameters.
                 global_orient and body_pose are necessary,
                 jaw_pose, leye_pose, reye_pose,
                 left_hand_pose, right_hand_pose, transl and
```

### Comparing `xrmocap-0.7.0/xrmocap/data_structure/keypoints.py` & `xrmocap-0.8.0/xrmocap/data_structure/keypoints.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/data_structure/limbs.py` & `xrmocap-0.8.0/xrmocap/data_structure/limbs.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/data_structure/smc_reader.py` & `xrmocap-0.8.0/xrmocap/data_structure/smc_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 import cv2
-import h5py
 import json
 import numpy as np
 import tqdm
 
+try:
+    import h5py
+    has_h5py = True
+    import_exception = ''
+except (ImportError, ModuleNotFoundError):
+    has_h5py = False
+    import traceback
+    stack_str = ''
+    for line in traceback.format_stack():
+        if 'frozen' not in line:
+            stack_str += line + '\n'
+    import_exception = traceback.format_exc() + '\n'
+    import_exception = stack_str + import_exception
+
 
 class SMCReader:
 
     def __init__(self, file_path, body_model=None):
         """Read SenseMocapFile endswith ".smc".
 
         Args:
             file_path (str):
                 Path to an SMC file.
             body_model (nn.Module or dict):
                 Only needed for SMPL transformation to device frame
                 if nn.Module: a body_model instance
                 if dict: a body_model config
         """
+        if not has_h5py:
+            raise ImportError(import_exception)
         self.smc = h5py.File(file_path, 'r')
         self.__calibration_dict__ = None
         self.action_id = self.smc.attrs['action_id']
         self.actor_id = self.smc.attrs['actor_id']
         self.datetime_str = self.smc.attrs['datetime_str']  # .decode()
         self.kinect_num_frames = self.smc['Kinect'].attrs['num_frame']
         self.num_kinects = self.smc['Kinect'].attrs['num_device']
```

### Comparing `xrmocap-0.7.0/xrmocap/human_perception/bbox_detection/mmdet_detector.py` & `xrmocap-0.8.0/xrmocap/human_perception/bbox_detection/mmdet_detector.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/human_perception/bbox_detection/mmtrack_detector.py` & `xrmocap-0.8.0/xrmocap/human_perception/bbox_detection/mmtrack_detector.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/human_perception/keypoints_estimation/mediapipe_estimator.py` & `xrmocap-0.8.0/xrmocap/human_perception/keypoints_estimation/mediapipe_estimator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 import cv2
 import logging
-import mediapipe as mp
 import numpy as np
 from tqdm import tqdm
 from typing import List, Tuple, Union
 from xrprimer.utils.ffmpeg_utils import video_to_array
 from xrprimer.utils.log_utils import get_logger
 
 from xrmocap.data_structure.keypoints import Keypoints
 from xrmocap.transform.convention.keypoints_convention import get_keypoint_num
 
+try:
+    import mediapipe as mp
+    has_mediapipe = True
+    import_exception = ''
+except (ImportError, ModuleNotFoundError):
+    has_mediapipe = False
+    import traceback
+    stack_str = ''
+    for line in traceback.format_stack():
+        if 'frozen' not in line:
+            stack_str += line + '\n'
+    import_exception = traceback.format_exc() + '\n'
+    import_exception = stack_str + import_exception
+
 
 class MediapipeEstimator():
 
     def __init__(self,
                  mediapipe_kwargs: dict,
                  bbox_thr: float = 0.0,
                  logger: Union[None, str, logging.Logger] = None) -> None:
@@ -28,14 +41,18 @@
                 Threshold of a bbox. Those have lower scores will be ignored.
                 Defaults to 0.0.
             logger (Union[None, str, logging.Logger], optional):
                 Logger for logging. If None, root logger will be selected.
                 Defaults to None.
         """
         # build the pose model
+        if not has_mediapipe:
+            self.logger.error(import_exception)
+            raise ModuleNotFoundError(
+                'Please install mediapipe by `pip install mediapipe`.')
         mp_pose = mp.solutions.pose
         self.pose_model = mp_pose.Pose(**mediapipe_kwargs)
         self.bbox_thr = bbox_thr
         self.logger = get_logger(logger)
         self.convention = 'mediapipe_body'
 
     def get_keypoints_convention_name(self) -> str:
```

### Comparing `xrmocap-0.7.0/xrmocap/human_perception/keypoints_estimation/mmpose_top_down_estimator.py` & `xrmocap-0.8.0/xrmocap/core/evaluation/end2end_evaluation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,340 +1,313 @@
-import cv2
+# yapf: disable
 import logging
 import numpy as np
-from tqdm import tqdm
-from typing import List, Tuple, Union
-from xrprimer.utils.ffmpeg_utils import video_to_array
-from xrprimer.utils.log_utils import get_logger
+import os
+import prettytable
+import time
+import torch
+from torch.utils.data import DataLoader
+from typing import List, Union
 
+from xrmocap.data.data_visualization.builder import BaseDataVisualization
 from xrmocap.data_structure.keypoints import Keypoints
-from xrmocap.transform.convention.keypoints_convention import get_keypoint_num
-
-try:
-    from mmcv import digit_version
-    from mmpose import __version__ as mmpose_version
-    from mmpose.apis import inference_top_down_pose_model, init_pose_model
-    has_mmpose = True
-    import_exception = ''
-except (ImportError, ModuleNotFoundError):
-    has_mmpose = False
-    import traceback
-    stack_str = ''
-    for line in traceback.format_stack():
-        if 'frozen' not in line:
-            stack_str += line + '\n'
-    import_exception = traceback.format_exc() + '\n'
-    import_exception = stack_str + import_exception
-
-
-class MMposeTopDownEstimator:
-
-    def __init__(self,
-                 mmpose_kwargs: dict,
-                 bbox_thr: float = 0.0,
-                 logger: Union[None, str, logging.Logger] = None) -> None:
-        """Init a detector from mmpose.
+from xrmocap.model.architecture.base_architecture import BaseArchitecture
+from xrmocap.utils.distribute_utils import collect_results, is_main_process
+from xrmocap.utils.eval_utils import align_convention_mask
+from xrmocap.utils.mvp_utils import (
+    AverageMeter, convert_result_to_kps, norm2absolute,
+)
+from .base_evaluation import BaseEvaluation
+from .metrics.base_metric import BaseMetric
+
+# yapf: enable
+
+
+class End2EndEvaluation(BaseEvaluation):
+
+    def __init__(
+        self,
+        test_loader: DataLoader,
+        output_dir: str,
+        metric_list: List[Union[dict, BaseMetric]],
+        trans_matrix: Union[List[List[float]], None] = None,
+        checkpoint_select: str = 'pcp_total_mean',
+        n_max_person: int = 10,
+        dataset_name: Union[None, str] = None,
+        pred_kps3d_convention: str = 'coco',
+        gt_kps3d_convention: str = 'coco',
+        eval_kps3d_convention: str = 'human_data',
+        pick_dict: Union[dict, None] = None,
+        print_freq: int = 100,
+        dataset_visualization: Union[None, dict, BaseDataVisualization] = None,
+        logger: Union[None, str, logging.Logger] = None,
+    ) -> None:
+        """Evaluation for end-to-end methods. For model validation during
+        training and model evaluation.
 
         Args:
-            mmpose_kwargs (dict):
-                A dict contains args of mmpose.apis.init_detector.
-                Necessary keys: config, checkpoint
-                Optional keys: device
-            bbox_thr (float, optional):
-                Threshold of a bbox. Those have lower scores will be ignored.
-                Defaults to 0.0.
-            logger (Union[None, str, logging.Logger], optional):
-                Logger for logging. If None, root logger will be selected.
+            test_loader (DataLoader):
+                Test dataloader.
+            output_dir (str):
+                Output directory.
+            metric_list (List[Union[dict, BaseMetric]]):
+                A list of metrics to be evaluated.
+            trans_matrix (Union[List[List[float]], None], optional):
+                A rotation matrix to transform the ground truth world
+                coordinate to align with prediction world coordinate.
+            checkpoint_select (str, optional):
+                Name of metric in the metric list to be used for
+                checkpoint selection. Defaults to 'pcp_total_mean'.
+            n_max_person (int, optional):
+                Number of maximum person the model can predict.
+                Defaults to 10.
+            dataset_name (Union[None, str], optional):
+                Name of the dataset. Defaults to None.
+            pred_kps3d_convention (str, optional):
+                Keypoint convention of predicted keypoints3d.
+                Defaults to 'coco'.
+            gt_kps3d_convention (str, optional):
+                Keypoint convention of ground-truth keypoints3d.
+                Defaults to 'coco'.
+            eval_kps3d_convention (str, optional):
+                A keypoint convention used for evaluation.
+                It is recommended to use human_data if pred_kps3d_convention
+                and gt_kps3d_convention are different.
+                Defaults to 'human_data'.
+            pick_dict (Union[dict, None], optional):
+                Selected metrics to be printed in the final table.
                 Defaults to None.
+            print_freq (int, optional):
+                Printing frequencty during model validation. Defaults to 100.
+            dataset_visualization (Union[None, dict,
+                BaseDataVisualization], optional):
+                Dataset visualization. Defaults to None.
+            logger (Union[None, str, logging.Logger], optional):
+                Logger for logging. If None, root logger will be
+                selected. Defaults to None.
         """
-        # build the pose model from a config file and a checkpoint file
-        self.pose_model = init_pose_model(**mmpose_kwargs)
-        # mmpose inference api takes one image per call
-        self.batch_size = 1
-        self.bbox_thr = bbox_thr
-        self.logger = get_logger(logger)
-        if not has_mmpose:
-            self.logger.error(import_exception)
-            raise ModuleNotFoundError(
-                'Please install mmpose to run detection.')
-        self.use_old_api = False
-        if digit_version(mmpose_version) <= digit_version('0.13.0'):
-            self.use_old_api = True
-
-    def get_keypoints_convention_name(self) -> str:
-        """Get data_source from dataset type in config file of the pose model.
-
-        Returns:
-            str:
-                Name of the keypoints convention. Must be
-                a key of KEYPOINTS_FACTORY.
-        """
-        return __translate_data_source__(
-            self.pose_model.cfg.data['test']['type'])
 
-    def infer_array(self,
-                    image_array: Union[np.ndarray, list],
-                    bbox_list: Union[tuple, list],
-                    disable_tqdm: bool = False,
-                    return_heatmap: bool = False) -> Tuple[list, list]:
-        """Infer frames already in memory(ndarray type).
+        BaseEvaluation.__init__(
+            self,
+            dataset=test_loader.dataset,
+            output_dir=output_dir,
+            metric_list=metric_list,
+            pick_dict=pick_dict,
+            dataset_visualization=dataset_visualization,
+            eval_kps3d_convention=eval_kps3d_convention,
+            logger=logger)
+
+        self.test_loader = test_loader
+        self.dataset_name = dataset_name
+        self.print_freq = print_freq
+        self.n_frame = test_loader.dataset.len
+        self.pred_kps3d_convention = pred_kps3d_convention
+        self.n_max_person = n_max_person
+        self.gt_kps3d_convention = gt_kps3d_convention
+        self.checkpoint_select = checkpoint_select
+        self.trans_matrix = np.array(trans_matrix)
+
+    def run(self,
+            model: BaseArchitecture,
+            threshold: float = 0.1,
+            is_train: bool = False,
+            overwrite: bool = False) -> float:
+        """Run the evaluation.
 
         Args:
-            image_array (Union[np.ndarray, list]):
-                BGR image ndarray in shape [n_frame, height, width, 3],
-                or a list of image ndarrays in shape [height, width, 3] while
-                len(list) == n_frame.
-            bbox_list (Union[tuple, list]):
-                A list of human bboxes.
-                Shape of the nested lists is (n_frame, n_human, 5).
-                Each bbox is a bbox_xyxy with a bbox_score at last.
-            disable_tqdm (bool, optional):
-                Whether to disable the entire progressbar wrapper.
-                Defaults to False.
-            return_heatmap (bool, optional):
-                Whether to return heatmap.
-                Defaults to False.
+            model (BaseArchitecture):
+                Model to be evaluated.
+            threshold (float, optional):
+                Threshold for the predicted confidence.
+                Defaults to 0.1.
+            is_train (bool, optional):
+                If is model validation in training, no keypoints or
+                inference results will be saved. Defaults to False.
+            overwrite (bool, optional):
+                Overwrite the output folder. Defaults to False.
 
         Returns:
-            Tuple[list, list]:
-                keypoints_list (list):
-                    A list of human keypoints.
-                    Shape of the nested lists is
-                    (n_frame, n_human, n_keypoints, 3).
-                    Each keypoint is an array of (x, y, confidence).
-                heatmap_list (list):
-                    A list of keypoint heatmaps. len(heatmap_list) == n_frame
-                    and the shape of heatmap_list[f] is
-                    (n_human, n_keypoints, width, height).
-                bbox_list (list):
-                    A list of human bboxes.
-                    Shape of the nested lists is (n_frame, n_human, 5).
-                    Each bbox is a bbox_xyxy with a bbox_score at last.
-                    It could be smaller than the input bbox_list,
-                    if there's no keypoints detected in some bbox.
+            accuracy: selected metric evaluation result.
         """
-        ret_kps_list = []
-        ret_heatmap_list = []
-        ret_bbox_list = []
-        n_frame = len(image_array)
-        n_kps = get_keypoint_num(self.get_keypoints_convention_name())
-        for start_index in tqdm(
-                range(0, n_frame, self.batch_size), disable=disable_tqdm):
-            end_index = min(n_frame, start_index + self.batch_size)
-            # mmpose takes only one frame
-            img_arr = image_array[start_index]
-            person_results = []
-            for frame_index in range(start_index, end_index, 1):
-                bboxes_in_frame = []
-                for idx, bbox in enumerate(bbox_list[frame_index]):
-                    if bbox[4] > 0.0:
-                        bboxes_in_frame.append({'bbox': bbox, 'id': idx})
-                person_results = bboxes_in_frame
-            if not self.use_old_api:
-                img_input = dict(imgs_or_paths=img_arr)
-            else:
-                img_input = dict(img_or_path=img_arr)
-            if len(bboxes_in_frame) > 0:
-                pose_results, returned_outputs = inference_top_down_pose_model(
-                    model=self.pose_model,
-                    person_results=person_results,
-                    bbox_thr=self.bbox_thr,
-                    format='xyxy',
-                    dataset=self.pose_model.cfg.data['test']['type'],
-                    return_heatmap=return_heatmap,
-                    outputs=None,
-                    **img_input)
-                frame_kps_results = np.zeros(
-                    shape=(
-                        len(bbox_list[frame_index]),
-                        n_kps,
-                        3,
-                    ))
-                frame_heatmap_results = [
-                    None,
-                ] * len(bbox_list[frame_index])
-                frame_bbox_results = np.zeros(
-                    shape=(len(bbox_list[frame_index]), 5))
-                for idx, person_dict in enumerate(pose_results):
-                    id = person_dict['id']
-                    bbox = person_dict['bbox']
-                    keypoints = person_dict['keypoints']
-                    frame_bbox_results[id] = bbox
-                    frame_kps_results[id] = keypoints
-                    if return_heatmap:
-                        # returned_outputs[0]['heatmap'].shape:
-                        # 1, 133, 96, 72
-                        frame_heatmap_results[id] = returned_outputs[0][
-                            'heatmap'][idx]
-                        ret_heatmap_list += [frame_heatmap_results]
-                frame_kps_results = frame_kps_results.tolist()
-                frame_bbox_results = frame_bbox_results.tolist()
-            else:
-                frame_kps_results = []
-                frame_bbox_results = []
-            ret_kps_list += [frame_kps_results]
-            ret_bbox_list += [frame_bbox_results]
-        return ret_kps_list, ret_heatmap_list, ret_bbox_list
 
-    def infer_frames(
-            self,
-            frame_path_list: list,
-            bbox_list: Union[tuple, list],
-            disable_tqdm: bool = False,
-            return_heatmap: bool = False,
-            load_batch_size: Union[None, int] = None) -> Tuple[list, list]:
-        """Infer frames from file.
+        # prepare output folder
+        BaseEvaluation.run(self, overwrite=overwrite)
 
-        Args:
-            frame_path_list (list):
-                A list of frames' absolute paths.
-            bbox_list (Union[tuple, list]):
-                A list of human bboxes.
-                Shape of the nested lists is (n_frame, n_human, 5).
-                Each bbox is a bbox_xyxy with a bbox_score at last.
-            disable_tqdm (bool, optional):
-                Whether to disable the entire progressbar wrapper.
-                Defaults to False.
-            return_heatmap (bool, optional):
-                Whether to return heatmap.
-                Defaults to False.
-            load_batch_size (Union[None, int], optional):
-                How many frames are loaded at the same time.
-                Defaults to None, load all frames in frame_path_list.
+        # get predicted Keypoints3d from model
+        preds_single = self.model_validate(model, threshold=threshold)
+        pred_kps3d_list = collect_results(preds_single, len(self.dataset))
+
+        accuracy = None
+        if is_main_process():
+            # prepare predicted Keypoints3d
+            # Add approximated points and update masks here if needed
+            # e.g. nose, jaw, headtop
+            n_frame = len(pred_kps3d_list)
+            pred_n_kps = pred_kps3d_list[0].shape[1]
+            pred_kps3d = np.full((n_frame, self.n_max_person, pred_n_kps, 4),
+                                 np.nan)
+
+            for frame_idx, per_frame_kps3d in enumerate(pred_kps3d_list):
+                if len(per_frame_kps3d) > 0:
+                    n_valid_person, keypoints3d_pred_valid = \
+                        convert_result_to_kps([per_frame_kps3d])
+                    pred_kps3d[
+                        frame_idx, :n_valid_person] = keypoints3d_pred_valid
+
+            pred_keypoints3d_raw = Keypoints(
+                dtype='numpy',
+                kps=pred_kps3d,
+                mask=pred_kps3d[..., -1] > 0,
+                convention=self.pred_kps3d_convention,
+                logger=self.logger)
 
-        Returns:
-            Tuple[list, list]:
-                keypoints_list (list):
-                    A list of human keypoints.
-                    Shape of the nested lists is
-                    (n_frame, n_human, n_keypoints, 3).
-                    Each keypoint is an array of (x, y, confidence).
-                heatmap_list (list):
-                    A list of keypoint heatmaps. len(heatmap_list) == n_frame
-                    and the shape of heatmap_list[f] is
-                    (n_human, n_keypoints, width, height).
-        """
-        ret_kps_list = []
-        ret_heatmap_list = []
-        ret_boox_list = []
-        if load_batch_size is None:
-            load_batch_size = len(frame_path_list)
-        for start_idx in range(0, len(frame_path_list), load_batch_size):
-            end_idx = min(len(frame_path_list), start_idx + load_batch_size)
-            if load_batch_size < len(frame_path_list):
-                self.logger.info(
-                    'Processing mmpose on frames' +
-                    f'({start_idx}-{end_idx})/{len(frame_path_list)}')
-            image_array_list = []
-            for frame_abs_path in frame_path_list[start_idx:end_idx]:
-                img_np = cv2.imread(frame_abs_path)
-                image_array_list.append(img_np)
-            batch_pose_list, batch_heatmap_list, batch_boox_list = \
-                self.infer_array(
-                    image_array=image_array_list,
-                    bbox_list=bbox_list[start_idx:end_idx],
-                    disable_tqdm=disable_tqdm,
-                    return_heatmap=return_heatmap)
-            ret_kps_list += batch_pose_list
-            ret_heatmap_list += batch_heatmap_list
-            ret_boox_list += batch_boox_list
-        return ret_kps_list, ret_heatmap_list, ret_boox_list
-
-    def infer_video(self,
-                    video_path: str,
-                    bbox_list: Union[tuple, list],
-                    disable_tqdm: bool = False,
-                    return_heatmap: bool = False) -> Tuple[list, list]:
-        """Infer frames from a video file.
+            # prepare gt Keypoints3d
+            gt_n_person = np.max(
+                np.array([
+                    scene_keypoints.get_person_number()
+                    for scene_keypoints in self.dataset.gt3d
+                ]))
+            gt_n_kps = self.dataset.gt3d[0].get_keypoints_number()
+            gt_kps3d = np.full((self.n_frame, gt_n_person, gt_n_kps, 4),
+                               np.nan)
+            gt_mask = np.full((self.n_frame, gt_n_person, gt_n_kps), np.nan)
+
+            start_frame = 0
+            for gt_keypoints3d_scene in self.dataset.gt3d:
+
+                gt_kps3d_scene = gt_keypoints3d_scene.get_keypoints().numpy(
+                )  # [n_frame, n_person, n_kps, 4]
+                gt_mask_scene = gt_keypoints3d_scene.get_mask().numpy(
+                )  # [n_frame, n_person, n_kps]
+
+                n_frame, n_person, _, _ = gt_kps3d_scene.shape
+                end_frame = min(start_frame + n_frame, self.n_frame)
+
+                gt_kps3d[start_frame:end_frame, :n_person, ...] = \
+                    gt_kps3d_scene[:end_frame-start_frame, ...]
+                gt_mask[start_frame:end_frame, :n_person, ...] = \
+                    gt_mask_scene[:end_frame-start_frame, ...]
+                start_frame = end_frame
+
+            if self.dataset_name == 'panoptic' and \
+                    self.trans_matrix is not None:
+                for frame_idx in range(self.n_frame):
+                    for person_idx in range(gt_n_person):
+                        gt_kps3d[frame_idx, person_idx, :, :3] = \
+                            gt_kps3d[frame_idx, person_idx, :, :3].dot(
+                                self.trans_matrix)
+
+            gt_keypoints3d_raw = Keypoints(
+                dtype='numpy',
+                kps=gt_kps3d,
+                mask=gt_mask,
+                convention=self.gt_kps3d_convention,
+                logger=self.logger)
 
-        Args:
-            video_path (str):
-                Path to the video to be detected.
-            bbox_list (Union[tuple, list]):
-                A list of human bboxes.
-                Shape of the nested lists is (n_frame, n_human, 5).
-                Each bbox is a bbox_xyxy with a bbox_score at last.
-            disable_tqdm (bool, optional):
-                Whether to disable the entire progressbar wrapper.
-                Defaults to False.
-            return_heatmap (bool, optional):
-                Whether to return heatmap.
-                Defaults to False.
+            # convert pred and gt to the same convention before passing
+            # to metric manager, human_data recommended
+            gt_keypoints3d, pred_keypoints3d = \
+                align_convention_mask(pred_keypoints3d_raw,
+                                      gt_keypoints3d_raw,
+                                      self.pred_kps3d_convention,
+                                      self.gt_kps3d_convention,
+                                      self.eval_kps3d_convention,
+                                      self.logger)
+
+            # evaluate and print results
+            eval_results, full_results = self.metric_manager(
+                pred_keypoints3d=pred_keypoints3d,
+                gt_keypoints3d=gt_keypoints3d)
+
+            table = prettytable.PrettyTable()
+            table.field_names = ['Metric name', 'Value']
+            for metric_name, metric_dict in eval_results.items():
+                for key, value in metric_dict.items():
+                    table.add_row([f'{metric_name}: {key}', f'{value:.2f}'])
+            table_str = '\n' + table.get_string()
+            self.logger.info(table_str)
 
-        Returns:
-            Tuple[list, list]:
-                keypoints_list (list):
-                    A list of human keypoints.
-                    Shape of the nested lists is
-                    (n_frame, n_human, n_keypoints, 3).
-                    Each keypoint is an array of (x, y, confidence).
-                heatmap_list (list):
-                    A list of keypoint heatmaps. len(heatmap_list) == n_frame
-                    and the shape of heatmap_list[f] is
-                    (n_human, n_keypoints, width, height).
-        """
-        image_array = video_to_array(input_path=video_path, logger=self.logger)
-        ret_kps_list, ret_heatmap_list, ret_boox_list = self.infer_array(
-            image_array=image_array,
-            bbox_list=bbox_list,
-            disable_tqdm=disable_tqdm,
-            return_heatmap=return_heatmap)
-        return ret_kps_list, ret_heatmap_list, ret_boox_list
-
-    def get_keypoints_from_result(
-            self, kps2d_list: List[list]) -> Union[Keypoints, None]:
-        """Convert returned keypoints2d into an instance of class Keypoints.
+            if self.checkpoint_select in full_results:
+                accuracy = full_results[self.checkpoint_select]
+            else:
+                self.logger.warning(
+                    'Metric for checkpoint selection '
+                    f'{self.checkpoint_select} is not available, '
+                    'This may cause troubles in training,'
+                    'please check the config.')
+                if is_train:
+                    raise KeyError
+
+            # save and visualize when it is not train
+            if not is_train:
+                pred_file_path = os.path.join(self.output_dir,
+                                              'pred_keypoints3d.npz')
+                gt_file_path = os.path.join(self.output_dir,
+                                            'gt_keypoints3d.npz')
+
+                self.logger.info(f'Saving 3D keypoints to: {pred_file_path}')
+                pred_keypoints3d.dump(pred_file_path)
+                self.logger.info(f'Saving 3D keypoints to: {gt_file_path}')
+                gt_keypoints3d.dump(gt_file_path)
+
+                if self.dataset_visualization is not None:
+                    self.dataset_visualization.pred_kps3d_paths = \
+                        pred_file_path
+                    self.dataset_visualization.run(overwrite=overwrite)
 
-        Args:
-            kps2d_list (List[list]):
-                A list of human keypoints, returned by
-                infer methods.
-                Shape of the nested lists is
-                (n_frame, n_human, n_keypoints, 3).
+        return accuracy
 
-        Returns:
-            Union[Keypoints, None]:
-                An instance of Keypoints with mask and
-                convention, data type is numpy.
-                If no one has been detected in any frame,
-                a None will be returned.
+    def model_validate(self, model: BaseArchitecture, threshold: float):
+        """Validate model during training or testing.
+
+        Args:
+            model (BaseArchitecture):
+                Model to be evaluated.
+            threshold (float):
+                Confidence threshold to filter non-human keypoints.
         """
-        # shape: (n_frame, n_human, n_keypoints, 3)
-        n_frame = len(kps2d_list)
-        human_count_list = [len(human_list) for human_list in kps2d_list]
-        if len(human_count_list) > 0:
-            n_human = max(human_count_list)
-        else:
-            n_human = 0
-        n_keypoints = get_keypoint_num(self.get_keypoints_convention_name())
-        if n_human > 0:
-            kps2d_arr = np.zeros(shape=(n_frame, n_human, n_keypoints, 3))
-            mask_arr = np.ones_like(kps2d_arr[..., 0], dtype=np.uint8)
-            for f_idx in range(n_frame):
-                if len(kps2d_list[f_idx]) <= 0:
-                    mask_arr[f_idx, ...] = 0
-                    continue
-                for h_idx in range(n_human):
-                    if h_idx < len(kps2d_list[f_idx]):
-                        mask_arr[f_idx, h_idx, ...] = np.sign(
-                            np.array(kps2d_list[f_idx][h_idx])[:, -1])
-                        kps2d_arr[f_idx,
-                                  h_idx, :, :] = kps2d_list[f_idx][h_idx]
-                    else:
-                        mask_arr[f_idx, h_idx, ...] = 0
-            keypoints2d = Keypoints(
-                kps=kps2d_arr,
-                mask=mask_arr,
-                convention=self.get_keypoints_convention_name(),
-                logger=self.logger)
-        else:
-            keypoints2d = None
-        return keypoints2d
+        batch_time = AverageMeter()
+        data_time = AverageMeter()
+
+        model.eval()
 
+        preds = []
+        with torch.no_grad():
+            end = time.time()
+            for i, (inputs, meta) in enumerate(self.test_loader):
+                data_time.update(time.time() - end)
+                assert len(inputs) == self.dataset.n_views
+                output = model(views=inputs, meta=meta)
+
+                gt_kps3d = meta[0]['kps3d'].float()
+                n_kps = gt_kps3d.shape[2]
+                bs, n_queries = output['pred_logits'].shape[:2]
+
+                src_poses = output['pred_poses']['outputs_coord']. \
+                    view(bs, n_queries, n_kps, 3)
+                src_poses = norm2absolute(src_poses, model.module.grid_size,
+                                          model.module.grid_center)
+                score = output['pred_logits'][:, :, 1:2].sigmoid()
+                score = score.unsqueeze(2).expand(-1, -1, n_kps, -1)
+                temp = (score > threshold).float() - 1
+
+                pred = torch.cat([src_poses, temp, score], dim=-1)
+                pred = pred.detach().cpu().numpy()
+                for b in range(pred.shape[0]):
+                    preds.append(pred[b])
+
+                batch_time.update(time.time() - end)
+                end = time.time()
+                if (i % self.print_freq == 0 or i
+                        == len(self.test_loader) - 1) and is_main_process():
+                    gpu_memory_usage = torch.cuda.memory_allocated(0)
+                    speed = len(inputs) * inputs[0].size(0) / batch_time.val
+                    msg = f'Test: [{i}/{len(self.test_loader)}]\t' \
+                        f'Time: {batch_time.val:.3f}s ' \
+                        f'({batch_time.avg:.3f}s)\t' \
+                        f'Speed: {speed:.1f} samples/s\t' \
+                        f'Data: {data_time.val:.3f}s ' \
+                        f'({data_time.avg:.3f}s)\t' \
+                        f'Memory {gpu_memory_usage:.1f}'
+                    self.logger.info(msg)
 
-def __translate_data_source__(mmpose_dataset_name):
-    if mmpose_dataset_name == 'TopDownSenseWholeBodyDataset':
-        return 'sense_whole_body'
-    elif mmpose_dataset_name == 'TopDownCocoWholeBodyDataset':
-        return 'coco_wholebody'
-    else:
-        raise NotImplementedError
+        return preds
```

### Comparing `xrmocap-0.7.0/xrmocap/io/__init__.py` & `xrmocap-0.8.0/xrmocap/io/__init__.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/io/camera.py` & `xrmocap-0.8.0/xrmocap/io/camera.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/io/h5py_helper.py` & `xrmocap-0.8.0/xrmocap/io/h5py_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io
 import numpy as np
 
 
 class H5Helper:
     """Some helper function related to h5py."""
     h5_element_type = \
-        (np.int64, np.float64, str, np.float, float, np.float32, int)
+        (np.int64, np.float64, str, float, np.float32, int)
     h5_list_type = \
         (list, np.ndarray)
 
     @staticmethod
     def save_attrs_to_h5file(h5file: h5py.File,
                              root_key: str = '/',
                              dic: dict = {}):
```

### Comparing `xrmocap-0.7.0/xrmocap/io/image.py` & `xrmocap-0.8.0/xrmocap/io/image.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/model/architecture/affinity_estimator.py` & `xrmocap-0.8.0/xrmocap/model/architecture/affinity_estimator.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/model/architecture/base_architecture.py` & `xrmocap-0.8.0/xrmocap/model/architecture/base_architecture.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/model/architecture/multi_view_pose_transformer.py` & `xrmocap-0.8.0/xrmocap/model/architecture/multi_view_pose_transformer.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/model/body_model/smpl.py` & `xrmocap-0.8.0/xrmocap/model/body_model/smpl.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/model/body_model/smplx.py` & `xrmocap-0.8.0/xrmocap/model/body_model/smplx.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     NUM_VERTS = 10475
     NUM_FACES = 20908
 
     def __init__(self,
                  *args,
                  use_face_contour: bool = True,
                  use_pca: bool = False,
-                 flat_hand_mean: bool = True,
+                 flat_hand_mean: bool = False,
                  keypoint_convention: str = 'smplx',
                  joints_regressor: str = None,
                  extra_joints_regressor: str = None,
                  logger: Union[None, str, logging.Logger] = None,
                  **kwargs) -> None:
         """Extension of the official SMPLX implementation.
 
@@ -98,15 +98,19 @@
             **kwargs: extra arguments for SMPLX
 
         Returns:
             output: contains output parameters and attributes
         """
 
         kwargs['get_skin'] = True
-        smplx_output = super(SMPLX, self).forward(*args, **kwargs)
+        smplx_output = super(SMPLX, self).forward(
+            *args,
+            return_verts=return_verts,
+            return_full_pose=return_full_pose,
+            **kwargs)
 
         if not hasattr(self, 'joints_regressor'):
             joints = smplx_output.joints
         else:
             joints = vertices2joints(self.joints_regressor,
                                      smplx_output.vertices)
```

### Comparing `xrmocap-0.7.0/xrmocap/model/registrant/optimizable_parameters.py` & `xrmocap-0.8.0/xrmocap/model/registrant/optimizable_parameters.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/model/registrant/smplify.py` & `xrmocap-0.8.0/xrmocap/model/registrant/smplify.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,17 +177,20 @@
             else:
                 init_param = None
             ret_param = self.__match_init_batch_size__(
                 init_param=init_param,
                 default_param=getattr(self.body_model, key),
                 batch_size=batch_size)
             ret_dict[key] = ret_param
-        if self.use_one_betas_per_video and 'betas' not in init_dict:
-            betas = torch.zeros(1, self.body_model.betas.shape[-1]).to(
-                self.device)
+        if self.use_one_betas_per_video:
+            if 'betas' not in init_dict:
+                betas = torch.zeros(1, self.body_model.betas.shape[-1]).to(
+                    self.device)
+            else:
+                betas = init_dict['betas'].mean(dim=0, keepdim=True)
             ret_dict['betas'] = betas
         return ret_dict
 
     def __call__(self,
                  input_list: List[BaseInput],
                  init_param_dict: dict = {},
                  return_verts: bool = False,
@@ -896,15 +899,15 @@
             weight[self.hand_keypoint_idxs] * hand_weight
 
         # 2nd priority: use_shoulder_hip_only
         if use_shoulder_hip_only:
             weight = torch.zeros([n_keypoints]).to(self.device)
             weight[self.shoulder_hip_keypoint_idxs] = 1.0
             if shoulder_weight is not None and hip_weight is not None and \
-                    body_weight * face_weight * hand_weight == 0.0:
+                    body_weight + face_weight + hand_weight == 0.0:
                 weight[self.shoulder_keypoint_idxs] = \
                     weight[self.shoulder_keypoint_idxs] * shoulder_weight
                 weight[self.hip_keypoint_idxs] = \
                     weight[self.hip_keypoint_idxs] * hip_weight
             else:
                 self.logger.error(
                     'use_shoulder_hip_only is deprecated, '
```

### Comparing `xrmocap-0.7.0/xrmocap/model/registrant/smplifyx.py` & `xrmocap-0.8.0/xrmocap/model/registrant/smplifyx.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             weight[self.face_keypoint_idxs] * face_weight
 
         # 2nd priority: use_shoulder_hip_only
         if use_shoulder_hip_only:
             weight = torch.zeros([n_keypoints]).to(self.device)
             weight[self.shoulder_hip_keypoint_idxs] = 1.0
             if shoulder_weight is not None and hip_weight is not None and \
-                    body_weight * face_weight * hand_weight == 0.0:
+                    body_weight + face_weight + hand_weight == 0.0:
                 weight[self.shoulder_keypoint_idxs] = \
                     weight[self.shoulder_keypoint_idxs] * shoulder_weight
                 weight[self.hip_keypoint_idxs] = \
                     weight[self.hip_keypoint_idxs] * hip_weight
             else:
                 self.logger.error(
                     'use_shoulder_hip_only is deprecated, '
```

### Comparing `xrmocap-0.7.0/xrmocap/model/registrant/smplifyxd.py` & `xrmocap-0.8.0/xrmocap/model/registrant/smplifyxd.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/bbox/__init__.py` & `xrmocap-0.8.0/xrmocap/transform/bbox/__init__.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/convention/bbox_convention.py` & `xrmocap-0.8.0/xrmocap/transform/convention/bbox_convention.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/convention/keypoints_convention/__init__.py` & `xrmocap-0.8.0/xrmocap/transform/convention/keypoints_convention/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from . import campus, fourdag_19, human_data, panoptic  # noqa:F401
 from .paf import ALL_PAF_MAPPING
 
 # yapf: enable
 if isinstance(KEYPOINTS_FACTORY, dict):
     KEYPOINTS_FACTORY['campus'] = campus.CAMPUS_KEYPOINTS
     KEYPOINTS_FACTORY['panoptic'] = panoptic.PANOPTIC_KEYPOINTS
+    KEYPOINTS_FACTORY['panoptic_15'] = panoptic.PANOPTIC15_KEYPOINTS
     KEYPOINTS_FACTORY['fourdag_19'] = fourdag_19.FOURDAG19_KEYPOINTS
 
 
 def convert_keypoints(
     keypoints: Keypoints,
     dst: str,
     approximate: bool = False,
@@ -258,7 +259,48 @@
         keypoints_factory (dict, optional): A class to store the attributes.
             Defaults to KEYPOINTS_FACTORY.
     Returns:
         List[str]: keypoint names
     """
     keypoints = keypoints_factory[convention]
     return keypoints
+
+
+def get_intersection_mask(convention_a: str,
+                          convention_b: str,
+                          dst_convention: str = 'human_data') -> np.ndarray:
+    """Get a intersection mask of two different conventions.
+
+    Args:
+        convention_a (str):
+            First convention name.
+        convention_b (str):
+            Second convention name.
+        dst_convention (str):
+            Destination convention name.
+            Defaults to human_data.
+
+    Returns:
+        np.ndarray:
+            Intersection mask in the format of
+            destination convention. [1, 1, n_kps]
+    """
+
+    def get_converted_mask(src_convention, dst_convention):
+        n_kps = get_keypoint_num(src_convention)
+        dummy_kps3d = np.ones((1, 1, n_kps, 4))
+        dummy_keypoints3d = Keypoints(
+            dtype='numpy',
+            kps=dummy_kps3d,
+            mask=dummy_kps3d[..., -1] > 0,
+            convention=src_convention)
+
+        dummy_keypoints3d_converted = convert_keypoints(
+            dummy_keypoints3d, dst=dst_convention, approximate=True)
+        converted_mask = dummy_keypoints3d_converted.get_mask()
+        return converted_mask
+
+    converted_mask_a = get_converted_mask(convention_a, dst_convention)
+    converted_mask_b = get_converted_mask(convention_b, dst_convention)
+    intersection_mask = np.multiply(converted_mask_a, converted_mask_b)
+
+    return intersection_mask
```

### Comparing `xrmocap-0.7.0/xrmocap/transform/convention/keypoints_convention/fourdag_19.py` & `xrmocap-0.8.0/xrmocap/transform/convention/keypoints_convention/fourdag_19.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/convention/keypoints_convention/human_data.py` & `xrmocap-0.8.0/xrmocap/transform/convention/keypoints_convention/human_data.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/convention/keypoints_convention/panoptic.py` & `xrmocap-0.8.0/xrmocap/transform/convention/keypoints_convention/panoptic.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,8 +26,35 @@
 00000190: 5f61 6e6b 6c65 5f6f 7065 6e70 6f73 6527  _ankle_openpose'
 000001a0: 2c0a 2020 2020 276c 6566 745f 6579 655f  ,.    'left_eye_
 000001b0: 6f70 656e 706f 7365 272c 0a20 2020 2027  openpose',.    '
 000001c0: 6c65 6674 5f65 6172 5f6f 7065 6e70 6f73  left_ear_openpos
 000001d0: 6527 2c0a 2020 2020 2772 6967 6874 5f65  e',.    'right_e
 000001e0: 7965 5f6f 7065 6e70 6f73 6527 2c0a 2020  ye_openpose',.  
 000001f0: 2020 2772 6967 6874 5f65 6172 5f6f 7065    'right_ear_ope
-00000200: 6e70 6f73 6527 2c0a 5d0a                 npose',.].
+00000200: 6e70 6f73 6527 2c0a 5d0a 0a50 414e 4f50  npose',.]..PANOP
+00000210: 5449 4331 355f 4b45 5950 4f49 4e54 5320  TIC15_KEYPOINTS 
+00000220: 3d20 5b0a 2020 2020 276e 6563 6b5f 6f70  = [.    'neck_op
+00000230: 656e 706f 7365 272c 0a20 2020 2027 6e6f  enpose',.    'no
+00000240: 7365 5f6f 7065 6e70 6f73 6527 2c0a 2020  se_openpose',.  
+00000250: 2020 2770 656c 7669 735f 6f70 656e 706f    'pelvis_openpo
+00000260: 7365 272c 0a20 2020 2027 6c65 6674 5f73  se',.    'left_s
+00000270: 686f 756c 6465 725f 6f70 656e 706f 7365  houlder_openpose
+00000280: 272c 0a20 2020 2027 6c65 6674 5f65 6c62  ',.    'left_elb
+00000290: 6f77 5f6f 7065 6e70 6f73 6527 2c0a 2020  ow_openpose',.  
+000002a0: 2020 276c 6566 745f 7772 6973 745f 6f70    'left_wrist_op
+000002b0: 656e 706f 7365 272c 0a20 2020 2027 6c65  enpose',.    'le
+000002c0: 6674 5f68 6970 5f6f 7065 6e70 6f73 6527  ft_hip_openpose'
+000002d0: 2c0a 2020 2020 276c 6566 745f 6b6e 6565  ,.    'left_knee
+000002e0: 5f6f 7065 6e70 6f73 6527 2c0a 2020 2020  _openpose',.    
+000002f0: 276c 6566 745f 616e 6b6c 655f 6f70 656e  'left_ankle_open
+00000300: 706f 7365 272c 0a20 2020 2027 7269 6768  pose',.    'righ
+00000310: 745f 7368 6f75 6c64 6572 5f6f 7065 6e70  t_shoulder_openp
+00000320: 6f73 6527 2c0a 2020 2020 2772 6967 6874  ose',.    'right
+00000330: 5f65 6c62 6f77 5f6f 7065 6e70 6f73 6527  _elbow_openpose'
+00000340: 2c0a 2020 2020 2772 6967 6874 5f77 7269  ,.    'right_wri
+00000350: 7374 5f6f 7065 6e70 6f73 6527 2c0a 2020  st_openpose',.  
+00000360: 2020 2772 6967 6874 5f68 6970 5f6f 7065    'right_hip_ope
+00000370: 6e70 6f73 6527 2c0a 2020 2020 2772 6967  npose',.    'rig
+00000380: 6874 5f6b 6e65 655f 6f70 656e 706f 7365  ht_knee_openpose
+00000390: 272c 0a20 2020 2027 7269 6768 745f 616e  ',.    'right_an
+000003a0: 6b6c 655f 6f70 656e 706f 7365 272c 0a5d  kle_openpose',.]
+000003b0: 0a                                       .
```

### Comparing `xrmocap-0.7.0/xrmocap/transform/image/base_image_transform.py` & `xrmocap-0.8.0/xrmocap/transform/image/base_image_transform.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/image/builder.py` & `xrmocap-0.8.0/xrmocap/transform/image/builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # yapf: disable
 from mmcv.utils import Registry
 from torchvision.transforms import Normalize, Resize, ToTensor
 
-from .color import BGR2RGB
+from .color import BGR2RGB, RGB2BGR
 from .convert import CV2ToPIL
 from .load import LoadImageCV2, LoadImagePIL
 from .shape import WarpAffine
 
 # yapf: enable
 
 IMAGE_TRANSFORM = Registry('image_transform')
 IMAGE_TRANSFORM.register_module(name='BGR2RGB', module=BGR2RGB)
+IMAGE_TRANSFORM.register_module(name='RGB2BGR', module=RGB2BGR)
 IMAGE_TRANSFORM.register_module(name='LoadImageCV2', module=LoadImageCV2)
 IMAGE_TRANSFORM.register_module(name='LoadImagePIL', module=LoadImagePIL)
 IMAGE_TRANSFORM.register_module(name='CV2ToPIL', module=CV2ToPIL)
 IMAGE_TRANSFORM.register_module(name='Resize', module=Resize)
 IMAGE_TRANSFORM.register_module(name='ToTensor', module=ToTensor)
 IMAGE_TRANSFORM.register_module(name='Normalize', module=Normalize)
 IMAGE_TRANSFORM.register_module(name='WarpAffine', module=WarpAffine)
```

### Comparing `xrmocap-0.7.0/xrmocap/transform/image/convert.py` & `xrmocap-0.8.0/xrmocap/transform/image/convert.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/image/load.py` & `xrmocap-0.8.0/xrmocap/transform/image/load.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/image/shape.py` & `xrmocap-0.8.0/xrmocap/transform/image/shape.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/__init__.py` & `xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/aniposelib_optimizer.py` & `xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/aniposelib_optimizer.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/base_optimizer.py` & `xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/builder.py` & `xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from .aniposelib_optimizer import AniposelibOptimizer
 from .base_optimizer import BaseOptimizer
 from .fourdag_base_optimizer import FourDAGBaseOptimizer
 from .fourdag_optimization import FourDAGOptimizer
 from .median_smooth import MedianSmooth
 from .nan_interpolation import NanInterpolation
+from .prior_optimizer import PriorConstraint
 from .rm_duplicate import RemoveDuplicate
 from .smpl_shape_aware_optimizer import SMPLShapeAwareOptimizer
 from .trajectory_optimizer import TrajectoryOptimizer
 
 KEYPOINTS3D_OPTIMIZERS = Registry('keypoints3d_optimizer')
 
 KEYPOINTS3D_OPTIMIZERS.register_module(
@@ -24,12 +25,14 @@
     name='SMPLShapeAwareOptimizer', module=SMPLShapeAwareOptimizer)
 KEYPOINTS3D_OPTIMIZERS.register_module(
     name='RemoveDuplicate', module=RemoveDuplicate)
 KEYPOINTS3D_OPTIMIZERS.register_module(
     name='FourDAGBaseOptimizer', module=FourDAGBaseOptimizer)
 KEYPOINTS3D_OPTIMIZERS.register_module(
     name='FourDAGOptimizer', module=FourDAGOptimizer)
+KEYPOINTS3D_OPTIMIZERS.register_module(
+    name='PriorConstraint', module=PriorConstraint)
 
 
 def build_keypoints3d_optimizer(cfg) -> BaseOptimizer:
     """Build keypoints3d optimizer."""
     return KEYPOINTS3D_OPTIMIZERS.build(cfg)
```

### Comparing `xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/fourdag_base_optimizer.py` & `xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/fourdag_base_optimizer.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/fourdag_optimization.py` & `xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/fourdag_optimization.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/median_smooth.py` & `xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/median_smooth.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/nan_interpolation.py` & `xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/nan_interpolation.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/rm_duplicate.py` & `xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/rm_duplicate.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,18 @@
 
         kps3d_optim = np.full((n_frame, n_max_person, n_kps, 4), np.nan)
 
         for frame_idx in range(n_frame):
             kps3d_frame = kps3d[frame_idx, ...]
             kps3d_frame = kps3d_frame[~np.isnan(kps3d_frame[:, 0, 0])]
 
+            # skip empty frame
+            if kps3d_frame.shape[0] == 0:
+                continue
+
             # calculate distance and remove duplicate
             dist = self.get_kps3d_dist(kps3d_frame)
 
             remove_idxs = []
             keep_idxs = []
             for person_idx, per_person_dist in enumerate(dist):
                 if person_idx not in remove_idxs \
```

### Comparing `xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/smpl_shape_aware_optimizer.py` & `xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/smpl_shape_aware_optimizer.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/keypoints3d/optim/trajectory_optimizer.py` & `xrmocap-0.8.0/xrmocap/transform/keypoints3d/optim/trajectory_optimizer.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/limbs/__init__.py` & `xrmocap-0.8.0/xrmocap/transform/limbs/__init__.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/point/__init__.py` & `xrmocap-0.8.0/xrmocap/transform/point/__init__.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/transform/rotation/__init__.py` & `xrmocap-0.8.0/xrmocap/transform/rotation/__init__.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/utils/camera_utils.py` & `xrmocap-0.8.0/xrmocap/utils/camera_utils.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/utils/distribute_utils.py` & `xrmocap-0.8.0/xrmocap/utils/distribute_utils.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/utils/ffmpeg_utils.py` & `xrmocap-0.8.0/xrmocap/utils/ffmpeg_utils.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/utils/fourdag_utils.py` & `xrmocap-0.8.0/xrmocap/utils/fourdag_utils.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/utils/geometry.py` & `xrmocap-0.8.0/xrmocap/utils/geometry.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,78 +4,14 @@
 import torch
 from typing import Union
 from xrprimer.utils.log_utils import get_logger
 
 from xrmocap.transform.convention.bbox_convention import convert_bbox
 
 
-def compute_similarity_transform(X: np.ndarray,
-                                 Y: np.ndarray,
-                                 compute_optimal_scale=False):
-    """A port of MATLAB's `procrustes` function to Numpy. Adapted from
-    http://stackoverflow.com/a/18927641/1884420.
-
-    Args:
-        X (np.ndarray): Array NxM of targets, with N number of points and
-           M point dimensionality.
-        Y (np.ndarray): Array NxM of inputs
-        compute_optimal_scale (bool, optional): whether we compute optimal
-            scale or force it to be 1. Defaults to False.
-
-    Returns:
-        d: squared error after transformation
-        Z (np.ndarray): transformed Y
-        T (np.ndarray): computed rotation
-        b: scaling
-        c: translation
-    """
-    muX = X.mean(0)
-    muY = Y.mean(0)
-
-    X0 = X - muX
-    Y0 = Y - muY
-
-    ssX = (X0**2.).sum()
-    ssY = (Y0**2.).sum()
-
-    # centred Frobenius norm
-    normX = np.sqrt(ssX)
-    normY = np.sqrt(ssY)
-
-    # scale to equal (unit) norm
-    X0 = X0 / normX
-    Y0 = Y0 / normY
-
-    # optimum rotation matrix of Y
-    A = np.dot(X0.T, Y0)
-    U, s, Vt = np.linalg.svd(A, full_matrices=False)
-    V = Vt.T
-    T = np.dot(V, U.T)
-
-    # Make sure we have a rotation
-    detT = np.linalg.det(T)
-    V[:, -1] *= np.sign(detT)
-    s[-1] *= np.sign(detT)
-    T = np.dot(V, U.T)
-
-    traceTA = s.sum()
-
-    if compute_optimal_scale:  # Compute optimum scaling of Y.
-        b = traceTA * normX / normY
-        d = 1 - traceTA**2
-        Z = normX * traceTA * np.dot(Y0, T) + muX
-    else:  # If no scaling allowed
-        b = 1
-        d = 1 + ssY / ssX - 2 * traceTA * normY / normX
-        Z = normY * np.dot(Y0, T) + muX
-
-    c = muX - b * np.dot(muY, T)
-    return d, Z, T, b, c
-
-
 def get_affine_transform(center,
                          scale,
                          rot,
                          output_size,
                          shift=np.array([0, 0], dtype=np.float32),
                          inv=0):
     """This function calculates affine transformation from given center, scale,
```

### Comparing `xrmocap-0.7.0/xrmocap/utils/mvp_utils.py` & `xrmocap-0.8.0/xrmocap/utils/mvp_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 import numpy
 import os
 import time
 import torch
 import torch.backends.cudnn as cudnn
 import torch.nn as nn
+from datetime import datetime
 from pathlib import Path
 from typing import Union
 
 from xrmocap.utils.distribute_utils import is_main_process
 
 
 class AverageMeter(object):
@@ -67,20 +68,22 @@
     root_output_dir = (this_dir / '..' / '..' / output_dir).resolve()
 
     if not root_output_dir.exists() and is_main_process():
         root_output_dir.mkdir()
 
     model = get_model_name(model, resnet_layer)
     cfg_name = os.path.basename(cfg_name).split('.')[0]
+    now = datetime.now()
+    time_stamp = now.strftime('%Y%m%d%H%M%S')
 
     # get final output dir
-    final_output_dir = os.path.join(root_output_dir, dataset, model, cfg_name)
+    final_output_dir = os.path.join(root_output_dir, dataset, model,
+                                    cfg_name + '_' + time_stamp)
 
-    if (not os.path.exists(final_output_dir)):
-        os.makedirs(final_output_dir)
+    os.makedirs(final_output_dir, exist_ok=True)
 
     # get logger file under final output dir
     time_str = time.strftime('%Y-%m-%d-%H-%M')
     log_file = f'{cfg_name}_{time_str}_{state}.log'
     log_file = os.path.join(final_output_dir, log_file)
 
     return log_file, final_output_dir
```

### Comparing `xrmocap-0.7.0/xrmocap/utils/mvpose_utils.py` & `xrmocap-0.8.0/xrmocap/utils/mvpose_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -299,37 +299,30 @@
     a = a.reshape(N, -1)
     M = b.shape[0]
     b = b.reshape(M, -1)
     a2 = np.tile(np.sum(a**2, axis=1).reshape(-1, 1), (1, M))
     b2 = np.tile(np.sum(b**2, axis=1), (N, 1))
     dist = a2 + b2 - 2 * (a @ b.T)
     dist = np.sqrt(dist)
-    dist[np.where(np.isnan(dist))] = 1000
+    dist[np.where(np.isnan(dist))] = 1e8
     return dist
 
 
 def add_campus_jaw_headtop(nose, kps3d_campus):
     for frame_idx in range(nose.shape[0]):
         for i, kps3d in enumerate(kps3d_campus[frame_idx]):
             add_kps3d = np.zeros((2, 3))
 
-            hip_center = (kps3d[2] + kps3d[3]) / 2
-            shouler_cneter = (kps3d[8] + kps3d[9]) / 2
-            head_center = nose[frame_idx][i]
-            add_kps3d[0] = shouler_cneter + (head_center -
-                                             shouler_cneter) * 0.5
-            face_dir = np.cross(shouler_cneter - hip_center,
-                                kps3d[8] - kps3d[9])
-            if np.isnan(face_dir).any():
-                add_kps3d[1] = shouler_cneter + (
-                    head_center - shouler_cneter) * np.array([0.75, 0.75, 1.5])
-            else:
-                face_dir = face_dir / np.linalg.norm(face_dir)
-                z_dir = np.array([0., 0., 1.], dtype=np.float)
-                add_kps3d[1] = add_kps3d[0] + face_dir * 0.125 + z_dir * 0.145
+            add_kps3d[0] = (kps3d[8] + kps3d[9]) / 2  # Use middle of shoulder
+            add_kps3d[1] = nose[frame_idx][i]  # use nose
+            add_kps3d[1] = add_kps3d[0] + (
+                add_kps3d[1] - add_kps3d[0]) * np.array([0.75, 0.75, 1.5])
+            add_kps3d[0] = add_kps3d[0] + (nose[frame_idx][i] -
+                                           add_kps3d[0]) * np.array(
+                                               [1. / 2., 1. / 2., 1. / 2.])
 
             kps3d[-2:] = add_kps3d
     return kps3d_campus
 
 
 def add_campus_jaw_headtop_mask(kps3d_mask):
     mask = np.zeros_like(kps3d_mask[:, :, -2:])
```

### Comparing `xrmocap-0.7.0/xrmocap/utils/triangulation_utils.py` & `xrmocap-0.8.0/xrmocap/utils/triangulation_utils.py`

 * *Files identical despite different names*

### Comparing `xrmocap-0.7.0/xrmocap/version.py` & `xrmocap-0.8.0/xrmocap/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenXRLab. All rights reserved.
 
-__version__ = '0.7.0'
+__version__ = '0.8.0'
 
 
 def parse_version_info(version_str):
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `xrmocap-0.7.0/xrmocap.egg-info/PKG-INFO` & `xrmocap-0.8.0/xrmocap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: xrmocap
-Version: 0.7.0
+Version: 0.8.0
 Summary: UNKNOWN
 Home-page: https://github.com/openxrlab/xrmocap
 Author: 
 Author-email: 
 License: Apache License 2.0
 Description: <br/>
         
         <div align="center">
             <img src="resources/xrmocap-logo.png" width="600"/>
         </div>
         
         <br/>
         
-        <div align="left">
+        <div align="center">
         
         [![Documentation](https://readthedocs.org/projects/xrmocap/badge/?version=latest)](https://xrmocap.readthedocs.io/en/latest/?badge=latest)
         [![actions](https://github.com/openxrlab/xrmocap/workflows/build/badge.svg)](https://github.com/openxrlab/xrmocap/actions)
         [![codecov](https://codecov.io/gh/openxrlab/xrmocap/branch/main/graph/badge.svg)](https://codecov.io/gh/openxrlab/xrmocap)
         [![PyPI](https://img.shields.io/pypi/v/xrmocap)](https://pypi.org/project/xrmocap/)
         [![Percentage of issues still open](https://isitmaintained.com/badge/open/openxrlab/xrmocap.svg)](https://github.com/openxrlab/xrmocap/issues)
         
@@ -92,14 +92,15 @@
         
         <details open>
         <summary>(click to collapse)</summary>
         
         - [x] [Campus](https://campar.in.tum.de/Chair/MultiHumanPose) (CVPR'2014)
         - [x] [Shelf](https://campar.in.tum.de/Chair/MultiHumanPose) (CVPR'2014)
         - [x] [CMU Panoptic](http://domedb.perception.cs.cmu.edu/) (ICCV'2015)
+        - [x] [4D Association](https://github.com/zhangyux15/multiview_human_dataset) (CVPR'2020)
         
         </details>
         
         
         ## Getting Started
         
         Please see [getting_started.md](docs/en/getting_started.md) for the basic usage of XRMoCap.
```

### Comparing `xrmocap-0.7.0/xrmocap.egg-info/SOURCES.txt` & `xrmocap-0.8.0/xrmocap.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -14,47 +14,61 @@
 xrmocap/core/estimation/base_estimator.py
 xrmocap/core/estimation/builder.py
 xrmocap/core/estimation/mperson_smpl_estimator.py
 xrmocap/core/estimation/mview_mperson_end2end_estimator.py
 xrmocap/core/estimation/mview_mperson_topdown_estimator.py
 xrmocap/core/estimation/mview_sperson_smpl_estimator.py
 xrmocap/core/evaluation/__init__.py
-xrmocap/core/evaluation/align_keypoints3d.py
+xrmocap/core/evaluation/base_evaluation.py
 xrmocap/core/evaluation/bottom_up_association_evaluation.py
 xrmocap/core/evaluation/builder.py
-xrmocap/core/evaluation/metrics.py
-xrmocap/core/evaluation/mvp_evaluation.py
+xrmocap/core/evaluation/end2end_evaluation.py
+xrmocap/core/evaluation/metric_manager.py
 xrmocap/core/evaluation/top_down_association_evaluation.py
+xrmocap/core/evaluation/metrics/__init__.py
+xrmocap/core/evaluation/metrics/base_metric.py
+xrmocap/core/evaluation/metrics/builder.py
+xrmocap/core/evaluation/metrics/mpjpe_metric.py
+xrmocap/core/evaluation/metrics/pa_mpjpe_metric.py
+xrmocap/core/evaluation/metrics/pck_metric.py
+xrmocap/core/evaluation/metrics/pcp_metric.py
+xrmocap/core/evaluation/metrics/precision_recall_metric.py
+xrmocap/core/evaluation/metrics/prediction_matcher.py
 xrmocap/core/hook/__init__.py
 xrmocap/core/hook/smplify_hook/__init__.py
 xrmocap/core/hook/smplify_hook/builder.py
 xrmocap/core/hook/smplify_hook/smplify_base_hook.py
 xrmocap/core/hook/smplify_hook/smplify_verbose_hook.py
 xrmocap/core/train/__init__.py
 xrmocap/core/train/builder.py
 xrmocap/core/train/trainer.py
 xrmocap/core/visualization/__init__.py
 xrmocap/core/visualization/visualize_keypoints2d.py
 xrmocap/core/visualization/visualize_keypoints3d.py
+xrmocap/core/visualization/visualize_smpl.py
+xrmocap/core/visualization/render/__init__.py
+xrmocap/core/visualization/render/mpr_renderer.py
 xrmocap/data_structure/__init__.py
 xrmocap/data_structure/keypoints.py
 xrmocap/data_structure/limbs.py
 xrmocap/data_structure/smc_reader.py
 xrmocap/data_structure/body_model/__init__.py
 xrmocap/data_structure/body_model/smpl_data.py
 xrmocap/data_structure/body_model/smplx_data.py
 xrmocap/data_structure/body_model/smplxd_data.py
 xrmocap/human_perception/__init__.py
 xrmocap/human_perception/builder.py
 xrmocap/human_perception/bbox_detection/__init__.py
 xrmocap/human_perception/bbox_detection/mmdet_detector.py
+xrmocap/human_perception/bbox_detection/mmdet_trt_detector.py
 xrmocap/human_perception/bbox_detection/mmtrack_detector.py
 xrmocap/human_perception/keypoints_estimation/__init__.py
 xrmocap/human_perception/keypoints_estimation/mediapipe_estimator.py
 xrmocap/human_perception/keypoints_estimation/mmpose_top_down_estimator.py
+xrmocap/human_perception/keypoints_estimation/mmpose_trt_top_down_estimator.py
 xrmocap/io/__init__.py
 xrmocap/io/camera.py
 xrmocap/io/h5py_helper.py
 xrmocap/io/image.py
 xrmocap/model/__init__.py
 xrmocap/model/architecture/__init__.py
 xrmocap/model/architecture/affinity_estimator.py
@@ -67,14 +81,22 @@
 xrmocap/model/body_model/smplx.py
 xrmocap/model/registrant/__init__.py
 xrmocap/model/registrant/builder.py
 xrmocap/model/registrant/optimizable_parameters.py
 xrmocap/model/registrant/smplify.py
 xrmocap/model/registrant/smplifyx.py
 xrmocap/model/registrant/smplifyxd.py
+xrmocap/model/registrant/handler/__init__.py
+xrmocap/model/registrant/handler/base_handler.py
+xrmocap/model/registrant/handler/betas_prior_handler.py
+xrmocap/model/registrant/handler/body_pose_prior_handler.py
+xrmocap/model/registrant/handler/builder.py
+xrmocap/model/registrant/handler/keypoint3d_limb_length_handler.py
+xrmocap/model/registrant/handler/keypoint3d_mse_handler.py
+xrmocap/model/registrant/handler/multiview_keypoint2d_mse_handler.py
 xrmocap/transform/__init__.py
 xrmocap/transform/bbox/__init__.py
 xrmocap/transform/convention/__init__.py
 xrmocap/transform/convention/bbox_convention.py
 xrmocap/transform/convention/keypoints_convention/__init__.py
 xrmocap/transform/convention/keypoints_convention/campus.py
 xrmocap/transform/convention/keypoints_convention/fourdag_19.py
@@ -93,22 +115,25 @@
 xrmocap/transform/keypoints3d/optim/aniposelib_optimizer.py
 xrmocap/transform/keypoints3d/optim/base_optimizer.py
 xrmocap/transform/keypoints3d/optim/builder.py
 xrmocap/transform/keypoints3d/optim/fourdag_base_optimizer.py
 xrmocap/transform/keypoints3d/optim/fourdag_optimization.py
 xrmocap/transform/keypoints3d/optim/median_smooth.py
 xrmocap/transform/keypoints3d/optim/nan_interpolation.py
+xrmocap/transform/keypoints3d/optim/prior_optimizer.py
 xrmocap/transform/keypoints3d/optim/rm_duplicate.py
 xrmocap/transform/keypoints3d/optim/smpl_shape_aware_optimizer.py
 xrmocap/transform/keypoints3d/optim/trajectory_optimizer.py
 xrmocap/transform/limbs/__init__.py
 xrmocap/transform/point/__init__.py
 xrmocap/transform/rotation/__init__.py
 xrmocap/utils/__init__.py
 xrmocap/utils/camera_utils.py
 xrmocap/utils/distribute_utils.py
+xrmocap/utils/eval_utils.py
 xrmocap/utils/ffmpeg_utils.py
 xrmocap/utils/fourdag_utils.py
 xrmocap/utils/geometry.py
 xrmocap/utils/mvp_utils.py
 xrmocap/utils/mvpose_utils.py
+xrmocap/utils/time_utils.py
 xrmocap/utils/triangulation_utils.py
```

