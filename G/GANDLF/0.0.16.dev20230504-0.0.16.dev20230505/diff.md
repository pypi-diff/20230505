# Comparing `tmp/GANDLF-0.0.16.dev20230504.tar.gz` & `tmp/GANDLF-0.0.16.dev20230505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.16.dev20230504.tar", last modified: Thu May  4 03:13:22 2023, max compression
+gzip compressed data, was "GANDLF-0.0.16.dev20230505.tar", last modified: Fri May  5 03:13:28 2023, max compression
```

## Comparing `GANDLF-0.0.16.dev20230504.tar` & `GANDLF-0.0.16.dev20230505.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.605307 GANDLF-0.0.16.dev20230504/
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.529307 GANDLF-0.0.16.dev20230504/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.533306 GANDLF-0.0.16.dev20230504/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.541307 GANDLF-0.0.16.dev20230504/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.549306 GANDLF-0.0.16.dev20230504/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.549306 GANDLF-0.0.16.dev20230504/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.553307 GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.557307 GANDLF-0.0.16.dev20230504/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.557307 GANDLF-0.0.16.dev20230504/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.557307 GANDLF-0.0.16.dev20230504/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.561307 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.565307 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.569307 GANDLF-0.0.16.dev20230504/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.573307 GANDLF-0.0.16.dev20230504/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.573307 GANDLF-0.0.16.dev20230504/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/metrics/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.585307 GANDLF-0.0.16.dev20230504/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.597307 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.597307 GANDLF-0.0.16.dev20230504/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30843 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.597307 GANDLF-0.0.16.dev20230504/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.601307 GANDLF-0.0.16.dev20230504/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 03:13:13.000000 GANDLF-0.0.16.dev20230504/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:13:22.533306 GANDLF-0.0.16.dev20230504/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-04 03:13:22.000000 GANDLF-0.0.16.dev20230504/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-04 03:13:22.000000 GANDLF-0.0.16.dev20230504/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:13:22.000000 GANDLF-0.0.16.dev20230504/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:10:42.000000 GANDLF-0.0.16.dev20230504/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-04 03:13:22.000000 GANDLF-0.0.16.dev20230504/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 03:13:22.000000 GANDLF-0.0.16.dev20230504/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-04 03:13:22.605307 GANDLF-0.0.16.dev20230504/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 03:13:22.605307 GANDLF-0.0.16.dev20230504/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-04 03:10:20.000000 GANDLF-0.0.16.dev20230504/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.376448 GANDLF-0.0.16.dev20230505/
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.292448 GANDLF-0.0.16.dev20230505/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.296448 GANDLF-0.0.16.dev20230505/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.304448 GANDLF-0.0.16.dev20230505/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.308448 GANDLF-0.0.16.dev20230505/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.312448 GANDLF-0.0.16.dev20230505/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.316448 GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.316448 GANDLF-0.0.16.dev20230505/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.320448 GANDLF-0.0.16.dev20230505/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.320448 GANDLF-0.0.16.dev20230505/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.324448 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.328448 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.332448 GANDLF-0.0.16.dev20230505/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.332448 GANDLF-0.0.16.dev20230505/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.336448 GANDLF-0.0.16.dev20230505/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/metrics/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.352448 GANDLF-0.0.16.dev20230505/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.364448 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.368448 GANDLF-0.0.16.dev20230505/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30843 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.368448 GANDLF-0.0.16.dev20230505/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.372448 GANDLF-0.0.16.dev20230505/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-05 03:13:19.000000 GANDLF-0.0.16.dev20230505/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:13:28.296448 GANDLF-0.0.16.dev20230505/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-05 03:13:28.000000 GANDLF-0.0.16.dev20230505/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-05 03:13:28.000000 GANDLF-0.0.16.dev20230505/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:13:28.000000 GANDLF-0.0.16.dev20230505/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:10:46.000000 GANDLF-0.0.16.dev20230505/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-05 03:13:28.000000 GANDLF-0.0.16.dev20230505/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 03:13:28.000000 GANDLF-0.0.16.dev20230505/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-05 03:13:28.372448 GANDLF-0.0.16.dev20230505/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-05 03:10:19.000000 GANDLF-0.0.16.dev20230505/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 03:13:28.376448 GANDLF-0.0.16.dev20230505/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-05 03:10:20.000000 GANDLF-0.0.16.dev20230505/setup.py
```

### Comparing `GANDLF-0.0.16.dev20230504/CODE_OF_CONDUCT.md` & `GANDLF-0.0.16.dev20230505/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/CONTRIBUTING.md` & `GANDLF-0.0.16.dev20230505/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.16.dev20230505/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.16.dev20230505/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/cli/__init__.py` & `GANDLF-0.0.16.dev20230505/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/cli/config_generator.py` & `GANDLF-0.0.16.dev20230505/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/cli/deploy.py` & `GANDLF-0.0.16.dev20230505/GANDLF/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/cli/main_run.py` & `GANDLF-0.0.16.dev20230505/GANDLF/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.16.dev20230505/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.16.dev20230505/GANDLF/cli/post_training_model_optimization.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.16.dev20230505/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/cli/recover_config.py` & `GANDLF-0.0.16.dev20230505/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.16.dev20230505/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/compute/generic.py` & `GANDLF-0.0.16.dev20230505/GANDLF/compute/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.16.dev20230505/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.16.dev20230505/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/compute/step.py` & `GANDLF-0.0.16.dev20230505/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/compute/training_loop.py` & `GANDLF-0.0.16.dev20230505/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/__init__.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.16.dev20230505/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.16.dev20230505/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.16.dev20230505/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.16.dev20230505/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/inference_manager.py` & `GANDLF-0.0.16.dev20230505/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/logger.py` & `GANDLF-0.0.16.dev20230505/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/losses/__init__.py` & `GANDLF-0.0.16.dev20230505/GANDLF/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/losses/hybrid.py` & `GANDLF-0.0.16.dev20230505/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/losses/regression.py` & `GANDLF-0.0.16.dev20230505/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/losses/segmentation.py` & `GANDLF-0.0.16.dev20230505/GANDLF/losses/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/metrics/__init__.py` & `GANDLF-0.0.16.dev20230505/GANDLF/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/metrics/classification.py` & `GANDLF-0.0.16.dev20230505/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/metrics/generic.py` & `GANDLF-0.0.16.dev20230505/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/metrics/regression.py` & `GANDLF-0.0.16.dev20230505/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.16.dev20230505/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/MSDNet.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/__init__.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/brain_age.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/deep_unet.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/densenet.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/efficientnet.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/fcn.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/imagenet_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/light_unet.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/modelBase.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/resnet.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/sdnet.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/transunet.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/uinc.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/unet.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/unetr.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/models/vgg.py` & `GANDLF-0.0.16.dev20230505/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.16.dev20230505/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.16.dev20230505/GANDLF/optimizers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/parseConfig.py` & `GANDLF-0.0.16.dev20230505/GANDLF/parseConfig.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.16.dev20230505/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.16.dev20230505/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/training_manager.py` & `GANDLF-0.0.16.dev20230505/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/utils/__init__.py` & `GANDLF-0.0.16.dev20230505/GANDLF/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/utils/generic.py` & `GANDLF-0.0.16.dev20230505/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.16.dev20230505/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/utils/imaging.py` & `GANDLF-0.0.16.dev20230505/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/utils/modelbase.py` & `GANDLF-0.0.16.dev20230505/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/utils/modelio.py` & `GANDLF-0.0.16.dev20230505/GANDLF/utils/modelio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.16.dev20230505/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/utils/tensor.py` & `GANDLF-0.0.16.dev20230505/GANDLF/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF/utils/write_parse.py` & `GANDLF-0.0.16.dev20230505/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.16.dev20230505/GANDLF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.16.dev20230504
+Version: 0.0.16.dev20230505
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230504 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230505 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.16.dev20230504/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.16.dev20230505/GANDLF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/HISTORY.md` & `GANDLF-0.0.16.dev20230505/HISTORY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/LICENSE` & `GANDLF-0.0.16.dev20230505/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/PKG-INFO` & `GANDLF-0.0.16.dev20230505/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.16.dev20230504
+Version: 0.0.16.dev20230505
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230504 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230505 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.16.dev20230504/README.md` & `GANDLF-0.0.16.dev20230505/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/SECURITY.md` & `GANDLF-0.0.16.dev20230505/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/gandlf_anonymizer` & `GANDLF-0.0.16.dev20230505/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/gandlf_collectStats` & `GANDLF-0.0.16.dev20230505/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/gandlf_configGenerator` & `GANDLF-0.0.16.dev20230505/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/gandlf_constructCSV` & `GANDLF-0.0.16.dev20230505/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/gandlf_deploy` & `GANDLF-0.0.16.dev20230505/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/gandlf_optimizeModel` & `GANDLF-0.0.16.dev20230505/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/gandlf_patchMiner` & `GANDLF-0.0.16.dev20230505/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/gandlf_preprocess` & `GANDLF-0.0.16.dev20230505/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/gandlf_recoverConfig` & `GANDLF-0.0.16.dev20230505/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/gandlf_run` & `GANDLF-0.0.16.dev20230505/gandlf_run`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/gandlf_verifyInstall` & `GANDLF-0.0.16.dev20230505/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230504/setup.py` & `GANDLF-0.0.16.dev20230505/setup.py`

 * *Files identical despite different names*

