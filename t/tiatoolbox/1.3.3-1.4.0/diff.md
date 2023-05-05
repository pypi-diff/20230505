# Comparing `tmp/tiatoolbox-1.3.3.tar.gz` & `tmp/tiatoolbox-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiatoolbox-1.3.3.tar", last modified: Thu Mar  2 14:23:02 2023, max compression
+gzip compressed data, was "tiatoolbox-1.4.0.tar", last modified: Fri May  5 13:47:15 2023, max compression
```

## Comparing `tiatoolbox-1.3.3.tar` & `tiatoolbox-1.4.0.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.067525 tiatoolbox-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-02 14:19:51.000000 tiatoolbox-1.3.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-03-02 14:19:51.000000 tiatoolbox-1.3.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-03-02 14:19:51.000000 tiatoolbox-1.3.3/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-03-02 14:19:51.000000 tiatoolbox-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-02 14:19:51.000000 tiatoolbox-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-03-02 14:19:51.000000 tiatoolbox-1.3.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-03-02 14:23:02.067525 tiatoolbox-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-03-02 14:19:51.000000 tiatoolbox-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-02 14:23:02.067525 tiatoolbox-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:01.983524 tiatoolbox-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:01.991524 tiatoolbox-1.3.3/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_arch_idars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_arch_mapde.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_arch_micronet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_arch_nuclick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_arch_sccnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_arch_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_arch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_arch_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_hovernetplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_multi_task_segmentor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_nucleus_instance_segmentor.py
--rw-r--r--   0 runner    (1001) docker     (123)    39391 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_patch_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29697 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/models/test_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    58982 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_annotation_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_annotation_tilerendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_meta_ngff_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_save_tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_slide_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_slide_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_stainaugment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_stainnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_tiatoolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_tiffreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_tileserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_tissuemask.py
--rw-r--r--   0 runner    (1001) docker     (123)    49064 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    16161 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_wsi_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_wsimeta.py
--rw-r--r--   0 runner    (1001) docker     (123)    83206 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tests/test_wsireader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:01.991524 tiatoolbox-1.3.3/tiatoolbox/
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:01.995524 tiatoolbox-1.3.3/tiatoolbox/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/annotation/dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)   108988 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/annotation/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:01.999524 tiatoolbox-1.3.3/tiatoolbox/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/cli/nucleus_instance_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/cli/patch_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/cli/read_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/cli/save_tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/cli/semantic_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/cli/show_wsi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/cli/slide_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/cli/slide_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/cli/stain_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/cli/tissue_mask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:01.999524 tiatoolbox-1.3.3/tiatoolbox/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28821 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/pretrained_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/remote_samples.yaml
--rw-r--r--   0 runner    (1001) docker     (123)  2018995 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/target_image.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:01.963523 tiatoolbox-1.3.3/tiatoolbox/data/visualization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:01.963523 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.011524 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    59306 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/css/fontawesome-all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   125385 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/css/ol-ext.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/css/ol.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.019524 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   670414 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/js/ol-ext.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1262003 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/js/ol.js
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/js/polyfill.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.043525 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   134294 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   747470 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   133988 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34034 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   144562 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33736 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   203030 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   917989 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   202744 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.043525 tiatoolbox-1.3.3/tiatoolbox/data/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/data/visualization/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.043525 tiatoolbox-1.3.3/tiatoolbox/models/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.047525 tiatoolbox-1.3.3/tiatoolbox/models/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28016 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/architecture/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/architecture/hovernetplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/architecture/idars.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/architecture/mapde.py
--rw-r--r--   0 runner    (1001) docker     (123)    17461 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/architecture/micronet.py
--rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/architecture/nuclick.py
--rw-r--r--   0 runner    (1001) docker     (123)    13041 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/architecture/sccnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/architecture/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/architecture/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/architecture/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.047525 tiatoolbox-1.3.3/tiatoolbox/models/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/dataset/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/dataset/dataset_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/dataset/info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.051525 tiatoolbox-1.3.3/tiatoolbox/models/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29666 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/engine/nucleus_instance_segmentor.py
--rw-r--r--   0 runner    (1001) docker     (123)    33466 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/engine/patch_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    64367 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/engine/semantic_segmentor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/models/models_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/tiatoolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.055525 tiatoolbox-1.3.3/tiatoolbox/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19823 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    31152 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/tools/patchextraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    22228 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/tools/pyramid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.055525 tiatoolbox-1.3.3/tiatoolbox/tools/registration/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/tools/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56475 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/tools/registration/wsi_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/tools/stainaugment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/tools/stainextract.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/tools/stainnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/tools/tissuemask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.063525 tiatoolbox-1.3.3/tiatoolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/utils/env_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23888 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31554 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    30618 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/utils/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.063525 tiatoolbox-1.3.3/tiatoolbox/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/visualization/tileserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.063525 tiatoolbox-1.3.3/tiatoolbox/wsicore/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/wsicore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:02.067525 tiatoolbox-1.3.3/tiatoolbox/wsicore/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/wsicore/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/wsicore/metadata/ngff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/wsicore/save_tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/wsicore/slide_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/wsicore/wsimeta.py
--rw-r--r--   0 runner    (1001) docker     (123)   195042 2023-03-02 14:19:52.000000 tiatoolbox-1.3.3/tiatoolbox/wsicore/wsireader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 14:23:01.995524 tiatoolbox-1.3.3/tiatoolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-03-02 14:23:01.000000 tiatoolbox-1.3.3/tiatoolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-03-02 14:23:01.000000 tiatoolbox-1.3.3/tiatoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-02 14:23:01.000000 tiatoolbox-1.3.3/tiatoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-02 14:23:01.000000 tiatoolbox-1.3.3/tiatoolbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 14:23:01.000000 tiatoolbox-1.3.3/tiatoolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-02 14:23:01.000000 tiatoolbox-1.3.3/tiatoolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-02 14:23:01.000000 tiatoolbox-1.3.3/tiatoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.845422 tiatoolbox-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    34851 2023-05-05 13:47:15.845422 tiatoolbox-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-05 13:42:54.000000 tiatoolbox-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.749420 tiatoolbox-1.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-05 13:47:15.845422 tiatoolbox-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.761420 tiatoolbox-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.773420 tiatoolbox-1.4.0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_idars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_mapde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_micronet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_nuclick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_sccnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_arch_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_hovernetplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_multi_task_segmentor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_nucleus_instance_segmentor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39420 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_patch_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29697 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/models/test_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74022 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_annotation_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_annotation_tilerendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_meta_ngff_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_save_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_slide_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_slide_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_stainaugment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_stainnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_tiatoolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_tiffreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_tileserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_tissuemask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49055 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16424 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_wsi_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_wsimeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90197 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tests/test_wsireader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.773420 tiatoolbox-1.4.0/tiatoolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.773420 tiatoolbox-1.4.0/tiatoolbox/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/annotation/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124137 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/annotation/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.781421 tiatoolbox-1.4.0/tiatoolbox/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/nucleus_instance_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/patch_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/read_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/save_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/semantic_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/show_wsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/slide_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/slide_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/stain_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/cli/tissue_mask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.785421 tiatoolbox-1.4.0/tiatoolbox/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29735 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/pretrained_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/remote_samples.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)  2018995 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/target_image.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.745420 tiatoolbox-1.4.0/tiatoolbox/data/visualization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.745420 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.793421 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    59306 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/fontawesome-all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   125385 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/ol-ext.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/ol.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.801421 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   670414 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/js/ol-ext.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1262003 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/js/ol.js
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/js/polyfill.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.821421 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   134294 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   747470 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   133988 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34034 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   144562 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33736 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   203030 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   917989 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   202744 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.821421 tiatoolbox-1.4.0/tiatoolbox/data/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/data/visualization/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.821421 tiatoolbox-1.4.0/tiatoolbox/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.829422 tiatoolbox-1.4.0/tiatoolbox/models/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28016 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/hovernetplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/idars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/mapde.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/micronet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/nuclick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/sccnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14209 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/architecture/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.829422 tiatoolbox-1.4.0/tiatoolbox/models/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/dataset/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/dataset/dataset_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/dataset/info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.829422 tiatoolbox-1.4.0/tiatoolbox/models/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/engine/multi_task_segmentor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31587 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/engine/nucleus_instance_segmentor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33563 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/engine/patch_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64566 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/engine/semantic_segmentor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/models/models_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tiatoolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.833422 tiatoolbox-1.4.0/tiatoolbox/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19823 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27806 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/patchextraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/pyramid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.837422 tiatoolbox-1.4.0/tiatoolbox/tools/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57079 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/registration/wsi_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/stainaugment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/stainextract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/stainnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/tools/tissuemask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.841422 tiatoolbox-1.4.0/tiatoolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/env_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23901 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31597 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11241 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30713 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/utils/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.841422 tiatoolbox-1.4.0/tiatoolbox/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/visualization/tileserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.841422 tiatoolbox-1.4.0/tiatoolbox/wsicore/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/wsicore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.845422 tiatoolbox-1.4.0/tiatoolbox/wsicore/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/wsicore/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/wsicore/metadata/ngff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12205 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/wsicore/wsimeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)   213228 2023-05-05 13:42:55.000000 tiatoolbox-1.4.0/tiatoolbox/wsicore/wsireader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:47:15.773420 tiatoolbox-1.4.0/tiatoolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    34851 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 13:47:15.000000 tiatoolbox-1.4.0/tiatoolbox.egg-info/top_level.txt
```

### Comparing `tiatoolbox-1.3.3/AUTHORS.md` & `tiatoolbox-1.4.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/CONTRIBUTING.rst` & `tiatoolbox-1.4.0/CONTRIBUTING.rst`

 * *Files 8% similar despite different names*

```diff
@@ -73,21 +73,20 @@
 4. Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
 5. When you're done making changes, check that your changes pass flake8 and the
-   tests, including testing other Python versions with tox::
+   tests::
 
     $ flake8 tiatoolbox tests
     $ python setup.py test or pytest
-    $ tox
 
-   To get flake8 and tox, just pip install them into your virtualenv.
+   To get flake8, just pip install them into your virtualenv.
 
 6. Commit your changes and push your branch to GitHub::
 
     $ git add .
     $ git commit -m "Your detailed description of your changes."
     $ git push origin name-of-your-bugfix-or-feature
 
@@ -98,15 +97,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 3.7, 3.8, 3.9 and 3.10, and for PyPy. Check
+3. The pull request should work for Python 3.8, 3.9 and 3.10, and for PyPy. Check
    https://travis-ci.com/tialab/tiatoolbox/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `tiatoolbox-1.3.3/HISTORY.md` & `tiatoolbox-1.4.0/HISTORY.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,58 @@
 # History
 
+## 1.4.0 (2023-04-24)
+
+### Major Updates and Feature Improvements
+
+- Adds Python 3.11 support \[experimental\] #500
+  - Python 3.11 is not fully supported by `pytorch` https://github.com/pytorch/pytorch/issues/86566 and `openslide` https://github.com/openslide/openslide-python/pull/188
+- Removes Python 3.7 support
+  - This allows upgrading all the dependencies which were dependent on an older version of Python.
+- Adds Neighbourhood Querying Support To AnnotationStore #540
+  - This enables easy and efficient querying of annotations within a neighbourhood of other annotations.
+- Adds `MultiTaskSegmentor` engine #424
+- Fixes an issue with stain augmentation to apply augmentation to only tissue regions.
+  - #546 contributed by @navidstuv
+- Filters logger output to stdout instead of stderr.
+  - Fixes #255
+- Allows import of some modules at higher level for improved usability
+  - `WSIReader` can now be imported as `from tiatoolbox.wsicore import WSIReader`
+  - `WSIMeta` can now be imported as `from tiatoolbox.wsicore import WSIMeta`
+  - `HoVerNet`, `HoVerNetPlus`, `IDaRS`, `MapDe`, `MicroNet`, `NuClick`, `SCCNN` can now be imported as \`from tiatoolbox.models import HoVerNet, HoVerNetPlus, IDaRS, MapDe, MicroNet, NuClick, SCCNN
+- Improves `PatchExtractor` performance. Updates `WSIPatchDataset` to be consistent. #571
+- Updates documentation for `License` for clarity on source code and model weights license.
+
+### Changes to API
+
+- Updates SCCNN architecture to make it consistent with other models. #544
+
+### Bug Fixes and Other Changes
+
+- Fixes Parsing Missing Omero Version NGFF Metadata #568
+  - Fixes #535 raised by @benkamphaus
+- Fixes reading of DICOM WSIs at the correct level #564
+  - Fixes #529
+- Fixes `scipy`, `matplotlib`, `scikit-image` deprecated code
+- Fixes breaking changes in `DICOMWSIReader` to make it compatible with latest `wsidicom` version. #539, #580
+- Updates `shapely` dependency to version >=2.0.0 and fixes any breaking changes.
+- Fixes bug with `DictionaryStore.bquery` and `geometry=None`, i.e. only a where predicate given.
+  - Partly Fixes #532 raised by @blaginin
+- Fixes local tests for Windows/Linux
+- Fixes `flake8`, `deepsource` errors.
+- Uses `logger` instead of `warnings` and `print` statements to properly log runs.
+
+### Development related changes
+
+- Upgrades dependencies which are dependent on Python 3.7
+- Moves `requirements*.txt` files to `requirements` folder
+- Removes `tox`
+- Uses `pyproject.toml` for `bdist_wheel`, `pytest` and `isort`
+- Adds `joblib` and `numba` as dependencies.
+
 ## 1.3.3 (2023-03-02)
 
 ### Major Updates and Feature Improvements
 
 - Restricts dependency versions for long term stability of the current version
 
 ### Changes to API
@@ -14,15 +63,14 @@
 
 - Fix bug related to reading scikit-image
 
 ### Development related changes
 
 - Restricts dependency versions for compatibility
 
-
 ## 1.3.2 (2023-02-17)
 
 ### Major Updates and Feature Improvements
 
 None
 
 ### Changes to API
@@ -33,15 +81,14 @@
 
 - Fix bug related to reading DICOM files
 
 ### Development related changes
 
 - Restricts wsidicom version to \<0.7.0 for compatibility
 
-
 ## 1.3.1 (2022-12-20)
 
 ### Major Updates and Feature Improvements
 
 - Adds [NuClick](https://arxiv.org/abs/2005.14511) architecture #449
 - Adds Annotation Store Reader #476
 - Adds [DFBR](https://arxiv.org/abs/2202.09971) method for registering pair of images #510
```

### Comparing `tiatoolbox-1.3.3/LICENSE` & `tiatoolbox-1.4.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Tissue Image Analytics (TIA) Centre
+Model weights are provided under a different license. For details, please see
+https://tia-toolbox.readthedocs.io/en/latest/pretrained.html
+
+Copyright (c) 2023, Tissue Image Analytics (TIA) Centre
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `tiatoolbox-1.3.3/Makefile` & `tiatoolbox-1.4.0/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 clean-pyc: ## remove Python file artifacts
 	find . -name '*.pyc' -exec rm -f {} +
 	find . -name '*.pyo' -exec rm -f {} +
 	find . -name '*~' -exec rm -f {} +
 	find . -name '__pycache__' -exec rm -fr {} +
 
 clean-test: ## remove test and coverage artifacts
-	rm -fr .tox/
 	rm -f .coverage
 	rm -fr htmlcov/
 	rm -fr .pytest_cache
 
 clean-docs: ## remove documentation artifacts
 	rm -fr docs/_build/
 	rm -rf docs/_autosummary/
@@ -58,17 +57,14 @@
 
 lint: ## check style with flake8
 	flake8 tiatoolbox tests
 
 test: ## run tests quickly with the default Python
 	pytest
 
-test-all: ## run tests on every Python version with tox
-	tox
-
 coverage: ## check code coverage quickly with the default Python
 	pytest  --cov=tiatoolbox --cov-report=term --cov-report=html --cov-report=xml
 	$(BROWSER) htmlcov/index.html
 
 docs: clean-docs ## generate Sphinx HTML documentation, including API docs
 	sphinx-apidoc -o docs/ tiatoolbox
 	$(MAKE) -C docs clean
@@ -84,7 +80,10 @@
 dist: clean ## builds source and wheel package
 	python setup.py sdist
 	python setup.py bdist_wheel
 	ls -l dist
 
 install: clean ## install the package to the active Python's site-packages
 	python setup.py install
+
+update-notebook-urls: # Recursively update the notebook URLs in ./examples
+	find ./examples -name "*.ipynb" | sort | xargs python pre-commit/notebook_urls.py
```

### Comparing `tiatoolbox-1.3.3/PKG-INFO` & `tiatoolbox-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tiatoolbox
-Version: 1.3.3
+Version: 1.4.0
 Summary: Computational pathology toolbox developed by TIA Centre.
 Home-page: https://github.com/TissueImageAnalytics/tiatoolbox
 Author: TIA Centre
 Author-email: tia@dcs.warwick.ac.uk
 Keywords: tiatoolbox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/develop/docs/tiatoolbox-logo.png">
 </p>
@@ -39,16 +39,16 @@
             <img src="https://shields.io/conda/dn/conda-forge/tiatoolbox"  alt="conda-forge downloads"/>
     </a>
   <br>
   <a href="https://tia-toolbox.readthedocs.io/en/latest/?badge=latest">
     <img src="https://readthedocs.org/projects/tia-toolbox/badge/?version=latest" alt="Documentation Status" />
   </a>
   <br>
-  <a href="https://github.com/TissueImageAnalytics/tiatoolbox/blob/develop/LICENSE">
-    <img alt="GitHub license" src="https://img.shields.io/github/license/TissueImageAnalytics/tiatoolbox"></a>
+  <a href="#license">
+    <img alt="GitHub license" src="https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=green"></a>
   <br>
   <br>
   <a href="https://github.com/TissueImageAnalytics/tiatoolbox/actions/workflows/pip-install.yml">
     <img src="https://img.shields.io/pypi/pyversions/tiatoolbox.svg"  alt="Supported Python versions"/>
   </a>
  <a href="https://github.com/psf/black">
       <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code Style black"/>
@@ -102,15 +102,15 @@
 
 tiatoolbox supports various features through command line. For more information, please try `tiatoolbox --help`
 
 ### Prepare for development
 
 Prepare a computer as a convenient platform for further development of the Python package `tiatoolbox` and related programs as follows.
 
-1. Install [pre-requisite software](https://tia-toolbox.readthedocs.io/en/latest/installation.html)
+1. Install [pre-requisite software](https://tia-toolbox.readthedocs.io/en/latest/installation.html#prerequisites)
 1. Open a terminal window<br/>
 
 ```sh
     $ cd <future-home-of-tiatoolbox-directory>
 ```
 
 3. Download a complete copy of the `tiatoolbox`.
@@ -124,37 +124,37 @@
 ```sh
     $ cd tiatoolbox
 ```
 
 5. Create virtual environment for TIAToolbox using
 
 ```sh
-    $ conda env create -f requirements.dev.conda.yml # for linux/mac only.
+    $ conda create -n tiatoolbox-dev python=3.8 # select version of your choice
     $ conda activate tiatoolbox-dev
+    $ pip install -r requirements/requirements_dev.txt
 ```
 
 or
 
 ```sh
-    $ conda create -n tiatoolbox-dev python=3.8 # select version of your choice
+    $ conda env create -f requirements/requirements.dev.conda.yml # for linux/mac only.
     $ conda activate tiatoolbox-dev
-    $ pip install -r requirements_dev.txt
 ```
 
 6. To use the packages installed in the environment, run the command:
 
 ```sh
     $ conda activate tiatoolbox-dev
 ```
 
 ### License
 
-The source code TIA Toolbox (tiatoolbox) as hosted on GitHub is released under the [The 3-Clause BSD License].
+The source code TIA Toolbox (tiatoolbox) as hosted on GitHub is released under the [BSD-3-Clause license](https://github.com/TissueImageAnalytics/tiatoolbox/blob/develop/LICENSE). The full text of the licence is included in [LICENSE](https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/develop/LICENSE).
 
-The full text of the licence is included in [LICENSE](https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/develop/LICENSE).
+Models weights are dependent on the datasets that they were trained on. Please refer to the [documentation](https://tia-toolbox.readthedocs.io/en/latest/pretrained.html) for more details.
 
 ### Cite this repository
 
 If you find TIAToolbox useful or use it in your research, please consider citing our paper:
 
 ```
 @article{
@@ -170,26 +170,65 @@
     title = {{TIAToolbox as an end-to-end library for advanced tissue image analytics}},
     url = {https://www.nature.com/articles/s43856-022-00186-5},
     volume = {2},
     year = {2022}
 }
 ```
 
-### Auxiliary Files
 
-Auxiliary files, such as pre-trained model weights downloaded from the TIA Centre webpage (https://warwick.ac.uk/tia/), are provided under the [Creative Commons Attribution-NonCommercial-ShareAlike Version 4 (CC BY-NC-SA 4.0) license](https://creativecommons.org/licenses/by-nc-sa/4.0/).
+# History
 
-### Dual License
+## 1.4.0 (2023-04-24)
 
-If you would like to use any of the source code or auxiliary files (e.g. pre-trained model weights) under a different license agreement please contact the Tissue Image Analytics (TIA) Centre at the University of Warwick (tia@dcs.warwick.ac.uk).
+### Major Updates and Feature Improvements
 
-[the 3-clause bsd license]: https://opensource.org/licenses/BSD-3-Clause
+- Adds Python 3.11 support \[experimental\] #500
+  - Python 3.11 is not fully supported by `pytorch` https://github.com/pytorch/pytorch/issues/86566 and `openslide` https://github.com/openslide/openslide-python/pull/188
+- Removes Python 3.7 support
+  - This allows upgrading all the dependencies which were dependent on an older version of Python.
+- Adds Neighbourhood Querying Support To AnnotationStore #540
+  - This enables easy and efficient querying of annotations within a neighbourhood of other annotations.
+- Adds `MultiTaskSegmentor` engine #424
+- Fixes an issue with stain augmentation to apply augmentation to only tissue regions.
+  - #546 contributed by @navidstuv
+- Filters logger output to stdout instead of stderr.
+  - Fixes #255
+- Allows import of some modules at higher level for improved usability
+  - `WSIReader` can now be imported as `from tiatoolbox.wsicore import WSIReader`
+  - `WSIMeta` can now be imported as `from tiatoolbox.wsicore import WSIMeta`
+  - `HoVerNet`, `HoVerNetPlus`, `IDaRS`, `MapDe`, `MicroNet`, `NuClick`, `SCCNN` can now be imported as \`from tiatoolbox.models import HoVerNet, HoVerNetPlus, IDaRS, MapDe, MicroNet, NuClick, SCCNN
+- Improves `PatchExtractor` performance. Updates `WSIPatchDataset` to be consistent. #571
+- Updates documentation for `License` for clarity on source code and model weights license.
 
+### Changes to API
 
-# History
+- Updates SCCNN architecture to make it consistent with other models. #544
+
+### Bug Fixes and Other Changes
+
+- Fixes Parsing Missing Omero Version NGFF Metadata #568
+  - Fixes #535 raised by @benkamphaus
+- Fixes reading of DICOM WSIs at the correct level #564
+  - Fixes #529
+- Fixes `scipy`, `matplotlib`, `scikit-image` deprecated code
+- Fixes breaking changes in `DICOMWSIReader` to make it compatible with latest `wsidicom` version. #539, #580
+- Updates `shapely` dependency to version >=2.0.0 and fixes any breaking changes.
+- Fixes bug with `DictionaryStore.bquery` and `geometry=None`, i.e. only a where predicate given.
+  - Partly Fixes #532 raised by @blaginin
+- Fixes local tests for Windows/Linux
+- Fixes `flake8`, `deepsource` errors.
+- Uses `logger` instead of `warnings` and `print` statements to properly log runs.
+
+### Development related changes
+
+- Upgrades dependencies which are dependent on Python 3.7
+- Moves `requirements*.txt` files to `requirements` folder
+- Removes `tox`
+- Uses `pyproject.toml` for `bdist_wheel`, `pytest` and `isort`
+- Adds `joblib` and `numba` as dependencies.
 
 ## 1.3.3 (2023-03-02)
 
 ### Major Updates and Feature Improvements
 
 - Restricts dependency versions for long term stability of the current version
 
@@ -201,15 +240,14 @@
 
 - Fix bug related to reading scikit-image
 
 ### Development related changes
 
 - Restricts dependency versions for compatibility
 
-
 ## 1.3.2 (2023-02-17)
 
 ### Major Updates and Feature Improvements
 
 None
 
 ### Changes to API
@@ -220,15 +258,14 @@
 
 - Fix bug related to reading DICOM files
 
 ### Development related changes
 
 - Restricts wsidicom version to \<0.7.0 for compatibility
 
-
 ## 1.3.1 (2022-12-20)
 
 ### Major Updates and Feature Improvements
 
 - Adds [NuClick](https://arxiv.org/abs/2005.14511) architecture #449
 - Adds Annotation Store Reader #476
 - Adds [DFBR](https://arxiv.org/abs/2202.09971) method for registering pair of images #510
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: tiatoolbox Version: 1.3.3 Summary: Computational
+Metadata-Version: 2.1 Name: tiatoolbox Version: 1.4.0 Summary: Computational
 pathology toolbox developed by TIA Centre. Home-page: https://github.com/
 TissueImageAnalytics/tiatoolbox Author: TIA Centre Author-email:
 tia@dcs.warwick.ac.uk Keywords: tiatoolbox Classifier: Development Status :: 2
 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE License-File: AUTHORS.md
   [https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/develop/
                            docs/tiatoolbox-logo.png]
                            ****** TIA Toolbox ******
      **** Computational Pathology Toolbox developed at the TIA Centre ****
 [PyPI_Status] [pypi_Downloads]
 [conda-forge_badge] [conda-forge_downloads]
@@ -67,53 +67,81 @@
 installation.html). To understand better how the programs work, study the
 jupyter notebooks referred to under the heading **Examples Taster**. ###
 Command Line tiatoolbox supports various features through command line. For
 more information, please try `tiatoolbox --help` ### Prepare for development
 Prepare a computer as a convenient platform for further development of the
 Python package `tiatoolbox` and related programs as follows. 1. Install [pre-
 requisite software](https://tia-toolbox.readthedocs.io/en/latest/
-installation.html) 1. Open a terminal window
+installation.html#prerequisites) 1. Open a terminal window
 ```sh $ cd  ``` 3. Download a complete copy of the `tiatoolbox`. ```sh $ git
 clone https://github.com/TissueImageAnalytics/tiatoolbox.git ``` 4. Change
 directory to `tiatoolbox` ```sh $ cd tiatoolbox ``` 5. Create virtual
-environment for TIAToolbox using ```sh $ conda env create -
-f requirements.dev.conda.yml # for linux/mac only. $ conda activate tiatoolbox-
-dev ``` or ```sh $ conda create -n tiatoolbox-dev python=3.8 # select version
-of your choice $ conda activate tiatoolbox-dev $ pip install -
-r requirements_dev.txt ``` 6. To use the packages installed in the environment,
-run the command: ```sh $ conda activate tiatoolbox-dev ``` ### License The
-source code TIA Toolbox (tiatoolbox) as hosted on GitHub is released under the
-[The 3-Clause BSD License]. The full text of the licence is included in
-[LICENSE](https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/
-develop/LICENSE). ### Cite this repository If you find TIAToolbox useful or use
-it in your research, please consider citing our paper: ``` @article
-{ Pocock2022, author = {Pocock, Johnathan and Graham, Simon and Vu, Quoc Dang
-and Jahanifar, Mostafa and Deshpande, Srijay and Hadjigeorghiou, Giorgos and
-Shephard, Adam and Bashir, Raja Muhammad Saad and Bilal, Mohsin and Lu, Wenqi
-and Epstein, David and Minhas, Fayyaz and Rajpoot, Nasir M and Raza, Shan E
-Ahmed}, doi = {10.1038/s43856-022-00186-5}, issn = {2730-664X}, journal =
-{Communications Medicine}, month = {sep}, number = {1}, pages = {120},
-publisher = {Springer US}, title = {{TIAToolbox as an end-to-end library for
-advanced tissue image analytics}}, url = {https://www.nature.com/articles/
-s43856-022-00186-5}, volume = {2}, year = {2022} } ``` ### Auxiliary Files
-Auxiliary files, such as pre-trained model weights downloaded from the TIA
-Centre webpage (https://warwick.ac.uk/tia/), are provided under the [Creative
-Commons Attribution-NonCommercial-ShareAlike Version 4 (CC BY-NC-SA 4.0)
-license](https://creativecommons.org/licenses/by-nc-sa/4.0/). ### Dual License
-If you would like to use any of the source code or auxiliary files (e.g. pre-
-trained model weights) under a different license agreement please contact the
-Tissue Image Analytics (TIA) Centre at the University of Warwick
-(tia@dcs.warwick.ac.uk). [the 3-clause bsd license]: https://opensource.org/
-licenses/BSD-3-Clause # History ## 1.3.3 (2023-03-02) ### Major Updates and
-Feature Improvements - Restricts dependency versions for long term stability of
-the current version ### Changes to API None ### Bug Fixes and Other Changes -
-Fix bug related to reading scikit-image ### Development related changes -
-Restricts dependency versions for compatibility ## 1.3.2 (2023-02-17) ### Major
-Updates and Feature Improvements None ### Changes to API None ### Bug Fixes and
-Other Changes - Fix bug related to reading DICOM files ### Development related
+environment for TIAToolbox using ```sh $ conda create -n tiatoolbox-dev
+python=3.8 # select version of your choice $ conda activate tiatoolbox-dev $
+pip install -r requirements/requirements_dev.txt ``` or ```sh $ conda env
+create -f requirements/requirements.dev.conda.yml # for linux/mac only. $ conda
+activate tiatoolbox-dev ``` 6. To use the packages installed in the
+environment, run the command: ```sh $ conda activate tiatoolbox-dev ``` ###
+License The source code TIA Toolbox (tiatoolbox) as hosted on GitHub is
+released under the [BSD-3-Clause license](https://github.com/
+TissueImageAnalytics/tiatoolbox/blob/develop/LICENSE). The full text of the
+licence is included in [LICENSE](https://raw.githubusercontent.com/
+TissueImageAnalytics/tiatoolbox/develop/LICENSE). Models weights are dependent
+on the datasets that they were trained on. Please refer to the [documentation]
+(https://tia-toolbox.readthedocs.io/en/latest/pretrained.html) for more
+details. ### Cite this repository If you find TIAToolbox useful or use it in
+your research, please consider citing our paper: ``` @article{ Pocock2022,
+author = {Pocock, Johnathan and Graham, Simon and Vu, Quoc Dang and Jahanifar,
+Mostafa and Deshpande, Srijay and Hadjigeorghiou, Giorgos and Shephard, Adam
+and Bashir, Raja Muhammad Saad and Bilal, Mohsin and Lu, Wenqi and Epstein,
+David and Minhas, Fayyaz and Rajpoot, Nasir M and Raza, Shan E Ahmed}, doi =
+{10.1038/s43856-022-00186-5}, issn = {2730-664X}, journal = {Communications
+Medicine}, month = {sep}, number = {1}, pages = {120}, publisher = {Springer
+US}, title = {{TIAToolbox as an end-to-end library for advanced tissue image
+analytics}}, url = {https://www.nature.com/articles/s43856-022-00186-5}, volume
+= {2}, year = {2022} } ``` # History ## 1.4.0 (2023-04-24) ### Major Updates
+and Feature Improvements - Adds Python 3.11 support \[experimental\] #500 -
+Python 3.11 is not fully supported by `pytorch` https://github.com/pytorch/
+pytorch/issues/86566 and `openslide` https://github.com/openslide/openslide-
+python/pull/188 - Removes Python 3.7 support - This allows upgrading all the
+dependencies which were dependent on an older version of Python. - Adds
+Neighbourhood Querying Support To AnnotationStore #540 - This enables easy and
+efficient querying of annotations within a neighbourhood of other annotations.
+- Adds `MultiTaskSegmentor` engine #424 - Fixes an issue with stain
+augmentation to apply augmentation to only tissue regions. - #546 contributed
+by @navidstuv - Filters logger output to stdout instead of stderr. - Fixes #255
+- Allows import of some modules at higher level for improved usability -
+`WSIReader` can now be imported as `from tiatoolbox.wsicore import WSIReader` -
+`WSIMeta` can now be imported as `from tiatoolbox.wsicore import WSIMeta` -
+`HoVerNet`, `HoVerNetPlus`, `IDaRS`, `MapDe`, `MicroNet`, `NuClick`, `SCCNN`
+can now be imported as \`from tiatoolbox.models import HoVerNet, HoVerNetPlus,
+IDaRS, MapDe, MicroNet, NuClick, SCCNN - Improves `PatchExtractor` performance.
+Updates `WSIPatchDataset` to be consistent. #571 - Updates documentation for
+`License` for clarity on source code and model weights license. ### Changes to
+API - Updates SCCNN architecture to make it consistent with other models. #544
+### Bug Fixes and Other Changes - Fixes Parsing Missing Omero Version NGFF
+Metadata #568 - Fixes #535 raised by @benkamphaus - Fixes reading of DICOM WSIs
+at the correct level #564 - Fixes #529 - Fixes `scipy`, `matplotlib`, `scikit-
+image` deprecated code - Fixes breaking changes in `DICOMWSIReader` to make it
+compatible with latest `wsidicom` version. #539, #580 - Updates `shapely`
+dependency to version >=2.0.0 and fixes any breaking changes. - Fixes bug with
+`DictionaryStore.bquery` and `geometry=None`, i.e. only a where predicate
+given. - Partly Fixes #532 raised by @blaginin - Fixes local tests for Windows/
+Linux - Fixes `flake8`, `deepsource` errors. - Uses `logger` instead of
+`warnings` and `print` statements to properly log runs. ### Development related
+changes - Upgrades dependencies which are dependent on Python 3.7 - Moves
+`requirements*.txt` files to `requirements` folder - Removes `tox` - Uses
+`pyproject.toml` for `bdist_wheel`, `pytest` and `isort` - Adds `joblib` and
+`numba` as dependencies. ## 1.3.3 (2023-03-02) ### Major Updates and Feature
+Improvements - Restricts dependency versions for long term stability of the
+current version ### Changes to API None ### Bug Fixes and Other Changes - Fix
+bug related to reading scikit-image ### Development related changes - Restricts
+dependency versions for compatibility ## 1.3.2 (2023-02-17) ### Major Updates
+and Feature Improvements None ### Changes to API None ### Bug Fixes and Other
+Changes - Fix bug related to reading DICOM files ### Development related
 changes - Restricts wsidicom version to \<0.7.0 for compatibility ## 1.3.1
 (2022-12-20) ### Major Updates and Feature Improvements - Adds [NuClick](https:
 //arxiv.org/abs/2005.14511) architecture #449 - Adds Annotation Store Reader
 #476 - Adds [DFBR](https://arxiv.org/abs/2202.09971) method for registering
 pair of images #510 ### Changes to API - Adds a sample SVS loading function
 `tiatoolbox.data.small_svs()` to the data module #517 ### Bug Fixes and Other
 Changes - Simplifies example notebook for image reading for better readability
```

### Comparing `tiatoolbox-1.3.3/README.md` & `tiatoolbox-1.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,16 @@
             <img src="https://shields.io/conda/dn/conda-forge/tiatoolbox"  alt="conda-forge downloads"/>
     </a>
   <br>
   <a href="https://tia-toolbox.readthedocs.io/en/latest/?badge=latest">
     <img src="https://readthedocs.org/projects/tia-toolbox/badge/?version=latest" alt="Documentation Status" />
   </a>
   <br>
-  <a href="https://github.com/TissueImageAnalytics/tiatoolbox/blob/develop/LICENSE">
-    <img alt="GitHub license" src="https://img.shields.io/github/license/TissueImageAnalytics/tiatoolbox"></a>
+  <a href="#license">
+    <img alt="GitHub license" src="https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=green"></a>
   <br>
   <br>
   <a href="https://github.com/TissueImageAnalytics/tiatoolbox/actions/workflows/pip-install.yml">
     <img src="https://img.shields.io/pypi/pyversions/tiatoolbox.svg"  alt="Supported Python versions"/>
   </a>
  <a href="https://github.com/psf/black">
       <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code Style black"/>
@@ -81,15 +81,15 @@
 
 tiatoolbox supports various features through command line. For more information, please try `tiatoolbox --help`
 
 ### Prepare for development
 
 Prepare a computer as a convenient platform for further development of the Python package `tiatoolbox` and related programs as follows.
 
-1. Install [pre-requisite software](https://tia-toolbox.readthedocs.io/en/latest/installation.html)
+1. Install [pre-requisite software](https://tia-toolbox.readthedocs.io/en/latest/installation.html#prerequisites)
 1. Open a terminal window<br/>
 
 ```sh
     $ cd <future-home-of-tiatoolbox-directory>
 ```
 
 3. Download a complete copy of the `tiatoolbox`.
@@ -103,37 +103,37 @@
 ```sh
     $ cd tiatoolbox
 ```
 
 5. Create virtual environment for TIAToolbox using
 
 ```sh
-    $ conda env create -f requirements.dev.conda.yml # for linux/mac only.
+    $ conda create -n tiatoolbox-dev python=3.8 # select version of your choice
     $ conda activate tiatoolbox-dev
+    $ pip install -r requirements/requirements_dev.txt
 ```
 
 or
 
 ```sh
-    $ conda create -n tiatoolbox-dev python=3.8 # select version of your choice
+    $ conda env create -f requirements/requirements.dev.conda.yml # for linux/mac only.
     $ conda activate tiatoolbox-dev
-    $ pip install -r requirements_dev.txt
 ```
 
 6. To use the packages installed in the environment, run the command:
 
 ```sh
     $ conda activate tiatoolbox-dev
 ```
 
 ### License
 
-The source code TIA Toolbox (tiatoolbox) as hosted on GitHub is released under the [The 3-Clause BSD License].
+The source code TIA Toolbox (tiatoolbox) as hosted on GitHub is released under the [BSD-3-Clause license](https://github.com/TissueImageAnalytics/tiatoolbox/blob/develop/LICENSE). The full text of the licence is included in [LICENSE](https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/develop/LICENSE).
 
-The full text of the licence is included in [LICENSE](https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/develop/LICENSE).
+Models weights are dependent on the datasets that they were trained on. Please refer to the [documentation](https://tia-toolbox.readthedocs.io/en/latest/pretrained.html) for more details.
 
 ### Cite this repository
 
 If you find TIAToolbox useful or use it in your research, please consider citing our paper:
 
 ```
 @article{
@@ -148,17 +148,7 @@
     publisher = {Springer US},
     title = {{TIAToolbox as an end-to-end library for advanced tissue image analytics}},
     url = {https://www.nature.com/articles/s43856-022-00186-5},
     volume = {2},
     year = {2022}
 }
 ```
-
-### Auxiliary Files
-
-Auxiliary files, such as pre-trained model weights downloaded from the TIA Centre webpage (https://warwick.ac.uk/tia/), are provided under the [Creative Commons Attribution-NonCommercial-ShareAlike Version 4 (CC BY-NC-SA 4.0) license](https://creativecommons.org/licenses/by-nc-sa/4.0/).
-
-### Dual License
-
-If you would like to use any of the source code or auxiliary files (e.g. pre-trained model weights) under a different license agreement please contact the Tissue Image Analytics (TIA) Centre at the University of Warwick (tia@dcs.warwick.ac.uk).
-
-[the 3-clause bsd license]: https://opensource.org/licenses/BSD-3-Clause
```

#### html2text {}

```diff
@@ -57,40 +57,35 @@
 installation.html). To understand better how the programs work, study the
 jupyter notebooks referred to under the heading **Examples Taster**. ###
 Command Line tiatoolbox supports various features through command line. For
 more information, please try `tiatoolbox --help` ### Prepare for development
 Prepare a computer as a convenient platform for further development of the
 Python package `tiatoolbox` and related programs as follows. 1. Install [pre-
 requisite software](https://tia-toolbox.readthedocs.io/en/latest/
-installation.html) 1. Open a terminal window
+installation.html#prerequisites) 1. Open a terminal window
 ```sh $ cd  ``` 3. Download a complete copy of the `tiatoolbox`. ```sh $ git
 clone https://github.com/TissueImageAnalytics/tiatoolbox.git ``` 4. Change
 directory to `tiatoolbox` ```sh $ cd tiatoolbox ``` 5. Create virtual
-environment for TIAToolbox using ```sh $ conda env create -
-f requirements.dev.conda.yml # for linux/mac only. $ conda activate tiatoolbox-
-dev ``` or ```sh $ conda create -n tiatoolbox-dev python=3.8 # select version
-of your choice $ conda activate tiatoolbox-dev $ pip install -
-r requirements_dev.txt ``` 6. To use the packages installed in the environment,
-run the command: ```sh $ conda activate tiatoolbox-dev ``` ### License The
-source code TIA Toolbox (tiatoolbox) as hosted on GitHub is released under the
-[The 3-Clause BSD License]. The full text of the licence is included in
-[LICENSE](https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/
-develop/LICENSE). ### Cite this repository If you find TIAToolbox useful or use
-it in your research, please consider citing our paper: ``` @article
-{ Pocock2022, author = {Pocock, Johnathan and Graham, Simon and Vu, Quoc Dang
-and Jahanifar, Mostafa and Deshpande, Srijay and Hadjigeorghiou, Giorgos and
-Shephard, Adam and Bashir, Raja Muhammad Saad and Bilal, Mohsin and Lu, Wenqi
-and Epstein, David and Minhas, Fayyaz and Rajpoot, Nasir M and Raza, Shan E
-Ahmed}, doi = {10.1038/s43856-022-00186-5}, issn = {2730-664X}, journal =
-{Communications Medicine}, month = {sep}, number = {1}, pages = {120},
-publisher = {Springer US}, title = {{TIAToolbox as an end-to-end library for
-advanced tissue image analytics}}, url = {https://www.nature.com/articles/
-s43856-022-00186-5}, volume = {2}, year = {2022} } ``` ### Auxiliary Files
-Auxiliary files, such as pre-trained model weights downloaded from the TIA
-Centre webpage (https://warwick.ac.uk/tia/), are provided under the [Creative
-Commons Attribution-NonCommercial-ShareAlike Version 4 (CC BY-NC-SA 4.0)
-license](https://creativecommons.org/licenses/by-nc-sa/4.0/). ### Dual License
-If you would like to use any of the source code or auxiliary files (e.g. pre-
-trained model weights) under a different license agreement please contact the
-Tissue Image Analytics (TIA) Centre at the University of Warwick
-(tia@dcs.warwick.ac.uk). [the 3-clause bsd license]: https://opensource.org/
-licenses/BSD-3-Clause
+environment for TIAToolbox using ```sh $ conda create -n tiatoolbox-dev
+python=3.8 # select version of your choice $ conda activate tiatoolbox-dev $
+pip install -r requirements/requirements_dev.txt ``` or ```sh $ conda env
+create -f requirements/requirements.dev.conda.yml # for linux/mac only. $ conda
+activate tiatoolbox-dev ``` 6. To use the packages installed in the
+environment, run the command: ```sh $ conda activate tiatoolbox-dev ``` ###
+License The source code TIA Toolbox (tiatoolbox) as hosted on GitHub is
+released under the [BSD-3-Clause license](https://github.com/
+TissueImageAnalytics/tiatoolbox/blob/develop/LICENSE). The full text of the
+licence is included in [LICENSE](https://raw.githubusercontent.com/
+TissueImageAnalytics/tiatoolbox/develop/LICENSE). Models weights are dependent
+on the datasets that they were trained on. Please refer to the [documentation]
+(https://tia-toolbox.readthedocs.io/en/latest/pretrained.html) for more
+details. ### Cite this repository If you find TIAToolbox useful or use it in
+your research, please consider citing our paper: ``` @article{ Pocock2022,
+author = {Pocock, Johnathan and Graham, Simon and Vu, Quoc Dang and Jahanifar,
+Mostafa and Deshpande, Srijay and Hadjigeorghiou, Giorgos and Shephard, Adam
+and Bashir, Raja Muhammad Saad and Bilal, Mohsin and Lu, Wenqi and Epstein,
+David and Minhas, Fayyaz and Rajpoot, Nasir M and Raza, Shan E Ahmed}, doi =
+{10.1038/s43856-022-00186-5}, issn = {2730-664X}, journal = {Communications
+Medicine}, month = {sep}, number = {1}, pages = {120}, publisher = {Springer
+US}, title = {{TIAToolbox as an end-to-end library for advanced tissue image
+analytics}}, url = {https://www.nature.com/articles/s43856-022-00186-5}, volume
+= {2}, year = {2022} } ```
```

### Comparing `tiatoolbox-1.3.3/pyproject.toml` & `tiatoolbox-1.4.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+[tool.pytest.ini_options]
+  collect_ignore = ["setup.py", "benchmark/"]
+
 [tool.black]
   exclude = '''
   /(
       \.eggs
     | \.git
     | \.hg
     | \.mypy_cache
-    | \.tox
     | \.venv
     | _build
     | buck-out
     | build
     | dist
     | docs
     | data
@@ -31,7 +33,21 @@
     'if self.debug:',
     'pragma: no cover',
     'raise NotImplementedError',
     'if __name__ == .__main__.:',
   ]
   ignore_errors = true
   omit = ['tests/*', 'tiatoolbox/__main__.py', '*/utils/env_detection.py']
+
+[tool.isort]
+  profile = "black"
+  multi_line_output = 3
+  line_length = 88
+  filter_files = "True"
+  skip = [".gitignore", "benchmarks/*"]
+
+[build-system]
+  requires = ["setuptools"]
+  build-backend = "setuptools.build_meta"
+
+[tool.distutils.bdist_wheel]
+  universal = true
```

### Comparing `tiatoolbox-1.3.3/requirements.txt` & `tiatoolbox-1.4.0/requirements/requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # torch installation
---extra-index-url https://download.pytorch.org/whl/cu116; sys_platform != "darwin"
-albumentations>=1.2.0, <=1.3.0
-Click>=8.1.0, <=8.1.3
-defusedxml>=0.6.0, <=0.7.1
-flask>=2.2.2, <=2.2.3
-glymur>=0.11.7, <=0.12.2
-imagecodecs>=2021.11.20, <=2023.1.23
-jupyterlab>=3.4.8, <=3.6.1
-matplotlib>=3.5.3, <=3.7.0
-numpy>=1.21.6, <=1.23.5
+--extra-index-url https://download.pytorch.org/whl/cu117; sys_platform != "darwin"
+albumentations>=1.3.0, <=1.3.0
+Click>=8.1.3, <=8.1.3
+defusedxml>=0.7.1, <=0.7.1
+flask>=2.2.2, <=2.3.2
+glymur>=0.12.1, <=0.12.5
+imagecodecs>=2022.9.26, <=2023.3.16
+joblib>=1.1.1, <=1.2.0
+jupyterlab>=3.5.2, <=3.6.3
+matplotlib>=3.6.2, <=3.7.1
+numba>=0.57.0, <=0.57.0
+numpy>=1.23.5, <=1.24.3
 opencv-python>=4.6.0, <=4.7.0
-openslide-python>=1.1.2, <=1.2.0
-pandas>=1.3.5, <=1.5.3
-pillow>=9.2.0, <=9.4.0
-pydicom>=2.3.0, <=2.3.1 # Used by wsidicom
-pyyaml>=5.4, <=6.0
-requests>=2.28.1, <=2.28.2
-scikit-image>=0.19.0, <=0.19.3
-scikit-learn>=1.0.2, <=1.2.1
-scipy>=1.7.3, <=1.10.1
-shapely>=1.8.5, <2.0.0 # Remove 2.0.0 once AnnotationStore is compatible
-SimpleITK>=2.1.1, <=2.2.1
-sphinx>=4.3.2, <=6.1.3
-tifffile>=2021.11.2, <=2023.2.28
-torch>=1.13.0, <=1.13.1
-torchvision>=0.13.0, <=0.14.1
-tqdm>=4.63.0, <=4.64.1
-umap-learn>=0.5.0, <0.5.3
-wsidicom>=0.3.2, <0.7.0
-zarr>=2.12.0, <=2.14.2
+openslide-python>=1.2.0, <=1.2.0
+pandas>=2.0.0, <=2.0.1
+pillow>=9.3.0, <=9.5.0
+pydicom>=2.3.1, <=2.3.1 # Used by wsidicom
+pyyaml>=6.0, <=6.0
+requests>=2.28.1, <=2.30.0
+scikit-image>=0.20, <=0.20.0
+scikit-learn>=1.2.0, <=1.2.2
+scipy>=1.8, <=1.10.1
+shapely>=2.0.0, <=2.0.1
+SimpleITK>=2.2.1, <=2.2.1
+sphinx>=5.3.0, <=7.0.0
+tifffile>=2022.10.10, <=2023.4.12
+torch>=1.13.1, <=2.0.0
+torchvision>=0.14.1, <=0.15.1
+tqdm>=4.64.1, <=4.65.0
+umap-learn>=0.5.3, <=0.5.3
+wsidicom>=0.7.0, <=0.9.0
+zarr>=2.13.3, <=2.14.2
```

### Comparing `tiatoolbox-1.3.3/setup.py` & `tiatoolbox-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     readme = readme_file.read()
 
 with open("HISTORY.md") as history_file:
     history = history_file.read()
 
 install_requires = [
     line
-    for line in Path("requirements.txt").read_text().splitlines()
+    for line in Path("requirements/requirements.txt").read_text().splitlines()
     if line and line[0] not in ("-", "#")
 ]
 
 dependency_links = []
 
 if sys.platform != "darwin":
     dependency_links = ["https://download.pytorch.org/whl/cu113"]
@@ -30,24 +30,24 @@
 test_requirements = [
     "pytest>=3",
 ]
 
 setup(
     author="TIA Centre",
     author_email="tia@dcs.warwick.ac.uk",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     description="Computational pathology toolbox developed by TIA Centre.",
     dependency_links=dependency_links,
     entry_points={
         "console_scripts": [
             "tiatoolbox=tiatoolbox.cli:main",
         ],
@@ -59,10 +59,10 @@
     keywords="tiatoolbox",
     name="tiatoolbox",
     packages=find_packages(include=["tiatoolbox", "tiatoolbox.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/TissueImageAnalytics/tiatoolbox",
-    version="1.3.3",
+    version="1.4.0",
     zip_safe=False,
 )
```

### Comparing `tiatoolbox-1.3.3/tests/conftest.py` & `tiatoolbox-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/models/test_abc.py` & `tiatoolbox-1.4.0/tests/models/test_abc.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/models/test_arch_idars.py` & `tiatoolbox-1.4.0/tests/models/test_arch_idars.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Functional unit test package for IDARS."""
 
 import torch
 
-from tiatoolbox.models.architecture.idars import IDaRS
+from tiatoolbox.models import IDaRS
 
 
 def test_functional():
     """Functional test for architectures."""
     # test forward
     samples = torch.rand(4, 3, 224, 224, dtype=torch.float32)
     model = IDaRS("resnet18")
```

### Comparing `tiatoolbox-1.3.3/tests/models/test_arch_mapde.py` & `tiatoolbox-1.4.0/tests/models/test_arch_mapde.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Unit test package for SCCNN."""
 import numpy as np
 import torch
 
 from tiatoolbox import utils
+from tiatoolbox.models import MapDe
 from tiatoolbox.models.architecture import fetch_pretrained_weights
-from tiatoolbox.models.architecture.mapde import MapDe
 from tiatoolbox.wsicore.wsireader import WSIReader
 
 
 def _load_mapde(tmp_path, name):
     """Loads MapDe model with specified weights."""
     model = MapDe()
     fetch_pretrained_weights(name, f"{tmp_path}/weights.pth")
```

### Comparing `tiatoolbox-1.3.3/tests/models/test_arch_micronet.py` & `tiatoolbox-1.4.0/tests/models/test_arch_micronet.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import pathlib
 
 import numpy as np
 import pytest
 import torch
 
 from tiatoolbox import utils
+from tiatoolbox.models import MicroNet
 from tiatoolbox.models.architecture import fetch_pretrained_weights
-from tiatoolbox.models.architecture.micronet import MicroNet
 from tiatoolbox.models.engine.semantic_segmentor import SemanticSegmentor
 from tiatoolbox.utils import env_detection as toolbox_env
 from tiatoolbox.wsicore.wsireader import WSIReader
 
 
 def test_functionality(remote_sample, tmp_path):
     """Functionality test."""
@@ -70,10 +70,9 @@
         save_dir=tmp_path / "output",
     )
 
     output = np.load(output[0][1] + ".raw.0.npy")
     output_on_server = np.load(str(micronet_output))
     output_on_server = np.round(output_on_server, decimals=3)
     new_output = np.round(output[500:1000, 1000:1500, :], decimals=3)
-    true_values = output_on_server == new_output
-    percent_true = np.count_nonzero(true_values) / np.size(output_on_server)
-    assert percent_true > 0.999
+    diff = new_output - output_on_server
+    assert diff.mean() < 1e-5
```

### Comparing `tiatoolbox-1.3.3/tests/models/test_arch_nuclick.py` & `tiatoolbox-1.4.0/tests/models/test_arch_nuclick.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-"""Unit test package for Nuclick."""
+"""Unit test package for NuClick."""
 
 import pathlib
 
 import numpy as np
-import pytest
 import torch
 
+from tiatoolbox.models import NuClick
 from tiatoolbox.models.architecture import fetch_pretrained_weights
-from tiatoolbox.models.architecture.nuclick import NuClick
 from tiatoolbox.utils.misc import imread
 
 ON_GPU = False
 
 # Test pretrained Model =============================
 
 
-def test_functional_nuclcik(remote_sample, tmp_path):
-    """Tests for nuclick."""
+def test_functional_nuclick(remote_sample, tmp_path, caplog):
+    """Tests for NuClick."""
     # convert to pathlib Path to prevent wsireader complaint
     tile_path = pathlib.Path(remote_sample("patch-extraction-vf"))
     img = imread(tile_path)
 
     _pretrained_path = f"{tmp_path}/weights.pth"
     fetch_pretrained_weights("nuclick_original-pannuke", _pretrained_path)
 
     # test creation
-    model = NuClick(num_input_channels=5, num_output_channels=1)
+    _ = NuClick(num_input_channels=5, num_output_channels=1)
 
     # test inference
     # create image patch, inclusion and exclusion maps
     patch = img[63:191, 750:878, :]
     inclusion_map = np.zeros((128, 128))
     inclusion_map[64, 64] = 1
 
@@ -63,11 +62,11 @@
 
     # test post-processing without reconstruction
     _ = model.postproc(output)
 
     # test failed reconstruction in post-processing
     inclusion_map = np.zeros((128, 128))
     inclusion_map[0, 0] = 1
-    with pytest.warns(UserWarning, match=r"Nuclei reconstruction was not done"):
-        _ = model.postproc(
-            output, do_reconstruction=True, nuc_points=inclusion_map[np.newaxis, ...]
-        )
+    _ = model.postproc(
+        output, do_reconstruction=True, nuc_points=inclusion_map[np.newaxis, ...]
+    )
+    assert "Nuclei reconstruction was not done" in caplog.text
```

### Comparing `tiatoolbox-1.3.3/tests/models/test_arch_sccnn.py` & `tiatoolbox-1.4.0/tests/models/test_arch_sccnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Unit test package for SCCNN."""
 import numpy as np
 import torch
 
 from tiatoolbox import utils
+from tiatoolbox.models import SCCNN
 from tiatoolbox.models.architecture import fetch_pretrained_weights
-from tiatoolbox.models.architecture.sccnn import SCCNN
 from tiatoolbox.wsicore.wsireader import WSIReader
 
 
 def _load_sccnn(tmp_path, name):
     """Loads SCCNN model with specified weights."""
     model = SCCNN()
     fetch_pretrained_weights(name, f"{tmp_path}/weights.pth")
```

### Comparing `tiatoolbox-1.3.3/tests/models/test_arch_unet.py` & `tiatoolbox-1.4.0/tests/models/test_arch_unet.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/models/test_arch_utils.py` & `tiatoolbox-1.4.0/tests/models/test_arch_utils.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/models/test_arch_vanilla.py` & `tiatoolbox-1.4.0/tests/models/test_arch_vanilla.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/models/test_dataset.py` & `tiatoolbox-1.4.0/tests/models/test_dataset.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/models/test_feature_extractor.py` & `tiatoolbox-1.4.0/tests/models/test_feature_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,10 +103,10 @@
     # Inference mode
     model.eval()
     with torch.inference_mode():
         _features = model(patches).numpy()
     # ! must maintain same batch size and likely same ordering
     # ! else the output values will not exactly be the same (still < 1.0e-4
     # ! of epsilon though)
-    assert np.mean(np.abs(features[:4] - _features)) < 1.0e-4
+    assert np.mean(np.abs(features[:4] - _features)) < 1.0e-1
 
     _rm_dir(save_dir)
```

### Comparing `tiatoolbox-1.3.3/tests/models/test_hovernet.py` & `tiatoolbox-1.4.0/tests/models/test_hovernet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Unit test package for HoVerNet."""
 
 import numpy as np
 import pytest
 import torch
 import torch.nn as nn
 
+from tiatoolbox.models import HoVerNet
 from tiatoolbox.models.architecture import fetch_pretrained_weights
 from tiatoolbox.models.architecture.hovernet import (
     DenseBlock,
-    HoVerNet,
     ResidualBlock,
     TFSamepaddingLayer,
 )
 from tiatoolbox.wsicore.wsireader import WSIReader
 
 
 def test_functionality(remote_sample, tmp_path):
```

### Comparing `tiatoolbox-1.3.3/tests/models/test_hovernetplus.py` & `tiatoolbox-1.4.0/tests/models/test_hovernetplus.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Unit test package for HoVerNet+."""
 
 import torch
 
+from tiatoolbox.models import HoVerNetPlus
 from tiatoolbox.models.architecture import fetch_pretrained_weights
-from tiatoolbox.models.architecture.hovernetplus import HoVerNetPlus
 from tiatoolbox.utils.misc import imread
 from tiatoolbox.utils.transforms import imresize
 
 
 def test_functionality(remote_sample, tmp_path):
     """Functionality test."""
     tmp_path = str(tmp_path)
```

### Comparing `tiatoolbox-1.3.3/tests/models/test_nucleus_instance_segmentor.py` & `tiatoolbox-1.4.0/tests/models/test_nucleus_instance_segmentor.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/models/test_patch_predictor.py` & `tiatoolbox-1.4.0/tests/models/test_patch_predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,17 @@
     imgs = {"a": np.random.randint(0, 255, (4, 4, 4))}
     with pytest.raises(
         ValueError, match=r".*Input must be either a list/array of images.*"
     ):
         _ = PatchDataset(imgs)
 
     # ndarray of mixed dtype
-    imgs = np.array([np.random.randint(0, 255, (4, 5, 3)), "Should crash"])
+    imgs = np.array(
+        [np.random.randint(0, 255, (4, 5, 3)), "Should crash"], dtype=object
+    )
     with pytest.raises(ValueError, match="Provided input array is non-numerical."):
         _ = PatchDataset(imgs)
 
     # ndarray(s) of NHW images
     imgs = np.random.randint(0, 255, (4, 4, 4))
     with pytest.raises(ValueError, match=r".*array of the form HWC*"):
         _ = PatchDataset(imgs)
@@ -393,17 +395,20 @@
     )
     assert roi1.shape[0] == roi2.shape[0]
     assert roi1.shape[1] == roi2.shape[1]
     assert np.min(correlation) > 0.9, correlation
 
 
 def test_patch_dataset_abc():
-    """Test for ABC methods."""
-    # test missing definition for abstract
-    # intentionally created to check error
+    """Test for ABC methods.
+
+    Test missing definition for abstract intentionally created to check error.
+
+    """
+
     # skipcq
     class Proto(PatchDatasetABC):
         # skipcq
         def __init__(self):
             super().__init__()
 
     # crash due to undefined __getitem__
@@ -909,15 +914,15 @@
         return_labels=False,
         on_gpu=on_gpu,
     )
     predictions = output["predictions"]
     probabilities = output["probabilities"]
     for idx, probabilities_ in enumerate(probabilities):
         probabilities_max = max(probabilities_)
-        assert np.abs(probabilities_max - probabilities_check[idx]) <= 5e-6, (
+        assert np.abs(probabilities_max - probabilities_check[idx]) <= 1e-3, (
             pretrained_model,
             probabilities_max,
             probabilities_check[idx],
             predictions[idx],
             predictions_check[idx],
         )
         assert predictions[idx] == predictions_check[idx], (
```

### Comparing `tiatoolbox-1.3.3/tests/models/test_semantic_segmentation.py` & `tiatoolbox-1.4.0/tests/models/test_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/test_annotation_stores.py` & `tiatoolbox-1.4.0/tests/test_annotation_stores.py`

 * *Files 20% similar despite different names*

```diff
@@ -126,14 +126,23 @@
 
 def annotations_center_of_mass(annotations):
     """Compute the mean of the annotation centroids."""
     centroids = [annotation.geometry.centroid for annotation in annotations]
     return MultiPoint(centroids).centroid
 
 
+def test_annotation_repr():
+    """Test the repr of an annotation."""
+    annotation = Annotation(Polygon([(0, 0), (1, 1), (2, 0)]))
+    assert isinstance(repr(annotation), str)
+    assert repr(annotation).startswith("Annotation(")
+    assert "POLYGON" in repr(annotation)
+    assert repr(annotation).endswith(")")
+
+
 # Fixtures
 
 
 @pytest.fixture(scope="session")
 def cell_grid() -> List[Polygon]:
     """Generate a grid of fake cell boundary polygon annotations."""
     np.random.seed(0)
@@ -186,24 +195,24 @@
         SQLiteStore,
         "compile_options",
         lambda x: ["ENABLE_RTREE", "ENABLE_JSON1"],
         raising=True,
     )
     SQLiteStore()
     monkeypatch.setattr(SQLiteStore, "compile_options", lambda x: [], raising=True)
-    with pytest.raises(Exception, match="RTREE and JSON1"):
+    with pytest.raises(EnvironmentError, match="RTREE and JSON1"):
         SQLiteStore()
 
 
 def test_sqlite_store_compile_options_exception_v3_38(monkeypatch):
     monkeypatch.setattr(sqlite3, "sqlite_version_info", (3, 38, 0))
     monkeypatch.setattr(
         SQLiteStore, "compile_options", lambda x: ["OMIT_JSON"], raising=True
     )
-    with pytest.raises(Exception, match="JSON must not"):
+    with pytest.raises(EnvironmentError, match="JSON must not"):
         SQLiteStore()
 
 
 def test_sqlite_store_compile_options_missing_math(monkeypatch, caplog):
     """Test that a warning is shown if the sqlite math module is missing."""
     monkeypatch.setattr(
         SQLiteStore,
@@ -228,15 +237,15 @@
         store.create_index("foo", lambda g, p: "foo" in p)
 
 
 def test_sqlite_store_index_version_error(monkeypatch):
     """Test adding an index with SQlite <3.9."""
     store = SQLiteStore()
     monkeypatch.setattr(sqlite3, "sqlite_version_info", (3, 8, 0))
-    with pytest.raises(Exception, match="Requires sqlite version 3.9.0"):
+    with pytest.raises(EnvironmentError, match="Requires sqlite version 3.9.0"):
         store.create_index("foo", lambda _, p: "foo" in p)
 
 
 def test_sqlite_store_index_str(fill_store, tmp_path):
     """Test that adding an index improves performance."""
     _, store = fill_store(SQLiteStore, tmp_path / "polygon.db")
 
@@ -267,19 +276,19 @@
     """Test that creating an index without ANALYZE."""
     _, store = fill_store(SQLiteStore, tmp_path / "polygon.db")
     properties_predicate = "props['class']"
     store.create_index("test_index", properties_predicate, analyze=False)
     assert "test_index" in store.indexes()
 
 
-def test_sqlite_pquery_warn_no_index(fill_store):
+def test_sqlite_pquery_warn_no_index(fill_store, caplog):
     """Test that querying without an index warns."""
     _, store = fill_store(SQLiteStore, ":memory:")
-    with pytest.warns(UserWarning, match="index"):
-        store.pquery("*", unique=False)
+    store.pquery("*", unique=False)
+    assert "Query is not using an index." in caplog.text
     # Check that there is no warning after creating the index
     store.create_index("test_index", "props['class']")
     with pytest.warns(None) as record:
         store.pquery("props['class']")
         assert len(record) == 0
 
 
@@ -296,15 +305,15 @@
     with pytest.raises(sqlite3.OperationalError, match="no such index"):
         store.drop_index("test_index")
 
 
 def test_sqlite_store_unsupported_compression(sample_triangle):
     """Test that using an unsupported compression str raises error."""
     store = SQLiteStore(compression="foo")
-    with pytest.raises(Exception, match="Unsupported"):
+    with pytest.raises(ValueError, match="Unsupported"):
         _ = store.serialise_geometry(sample_triangle)
 
 
 def test_sqlite_optimize(fill_store, tmp_path):
     """Test optimizing the database."""
     _, store = fill_store(SQLiteStore, tmp_path / "polygon.db")
     store.optimize()
@@ -317,15 +326,15 @@
     deserialised = store.deserialize_geometry(serialised)
     assert deserialised.wkb == sample_triangle.wkb
 
 
 def test_sqlite_store_unsupported_decompression():
     """Test that using an unsupported decompression str raises error."""
     store = SQLiteStore(compression="foo")
-    with pytest.raises(Exception, match="Unsupported"):
+    with pytest.raises(ValueError, match="Unsupported"):
         _ = store.deserialize_geometry(bytes())
 
 
 def test_sqlite_store_wkt_deserialisation(sample_triangle):
     """Test WKT deserialisation."""
     store = SQLiteStore(compression=None)
     wkt = sample_triangle.wkt
@@ -509,14 +518,20 @@
     store.append_many([Annotation(Point(10, 10), {}), Annotation(Point(20, 20), {})])
     store.commit()
     store.close()
     store = SQLiteStore(tmp_path / "polygon2.db")
     assert len(store) == 2  # check explicitly committing works
 
 
+def test_init_base_class_exception():
+    """Test that the base class cannot be initialized."""
+    with pytest.raises(TypeError, match="abstract class"):
+        AnnotationStore()  # skipcq: PYL-E0110
+
+
 # Annotation Store Interface Tests (AnnotationStoreABC)
 
 
 class TestStore:
     scenarios = [
         ("Dictionary", {"store_cls": DictionaryStore}),
         ("SQLite", {"store_cls": SQLiteStore}),
@@ -1200,26 +1215,26 @@
     def test_load_cases_error(fill_store, store_cls):
         """Test that loading a store with an invalid file handle raises an exception."""
         store = store_cls()
         with pytest.raises(IOError, match="Invalid file handle or path"):
             store._load_cases(["foo"], lambda: None, lambda: None)
 
     @staticmethod
-    def test_py37_init(fill_store, store_cls, monkeypatch):
-        """Test that __init__ is compatible with Python 3.7."""
-        py37_version = (3, 7, 0)
+    def test_py38_init(fill_store, store_cls, monkeypatch):
+        """Test that __init__ is compatible with Python 3.8."""
+        py38_version = (3, 8, 0)
 
         class Connection(sqlite3.Connection):
             """Mock SQLite connection."""
 
             def create_function(self, name: str, num_params: int, func: Any) -> None:
                 """Mock create_function without `deterministic` kwarg."""
                 return self.create_function(self, name, num_params)
 
-        monkeypatch.setattr(sys, "version_info", py37_version)
+        monkeypatch.setattr(sys, "version_info", py38_version)
         monkeypatch.setattr(sqlite3, "Connection", Connection)
         _ = store_cls()
 
     @staticmethod
     def test_bquery(fill_store, store_cls):
         """Test querying a store with a bounding box."""
         _, store = fill_store(store_cls, ":memory:")
@@ -1631,7 +1646,491 @@
     @staticmethod
     def test_connection_to_path_io(store_cls, tmp_path):
         """Test converting a named file connection to a path."""
         path = tmp_path / "foo"
         with open(path, "w") as fh:
             store_cls._connection_to_path(fh)
             assert path == Path(fh.name)
+
+    @staticmethod
+    def test_nquery_boxpoint_boxpoint(store_cls):
+        """Test simple querying within a neighbourhood.
+
+        Test that a neighbourhood query returns the correct results
+        for a simple data store with two points.
+
+        .. code-block:: text
+
+             ^
+            3|--****-----C
+             |*      *   |
+            2|         * |
+             |     B    *|
+            1|   A       *
+             |          *|
+            0+---------*-->
+             0   1   2   3
+
+        Query for all points within a distance of 2 from A. Should
+        return a dictionary with a single key, "A", and a value of
+        {"B": B}.
+
+        """
+        store: AnnotationStore = store_cls()
+        ann_a = Annotation(
+            Point(1, 1),
+            {"class": "A"},
+        )
+        store["A"] = ann_a
+        ann_b = Annotation(
+            Point(1.4, 1.4),
+            {"class": "B"},
+        )
+        store["B"] = ann_b
+        # C is inside the bounding box of the radius around A but is not
+        # returned because it is not inside of the radius.
+        ann_c = Annotation(
+            Point(2.9, 2.9),
+            {"class": "C"},
+        )
+        store["C"] = ann_c
+        result = store.nquery(
+            where="props['class'] == 'A'",
+            n_where="props['class'] != 'A'",
+            distance=2,
+            mode="boxpoint-boxpoint",
+        )
+        assert isinstance(result, dict)
+        assert len(result) == 1
+        assert "A" in result
+        assert result["A"] == {"B": ann_b}
+
+    @staticmethod
+    def test_nquery_boxpoint_boxpoint_no_results(store_cls):
+        """Test querying within a neighbourhood with no results.
+
+        Test that a neighbourhood query returns an empty dictionary
+        when there are no results.
+
+        .. code-block:: text
+
+            3^
+            2|
+            1|
+            0+----->
+             0 1 2 3
+
+        Query for all points within a distance of 2 from A. Should
+        return an empty dictionary.
+
+        """
+        store: AnnotationStore = store_cls()
+        ann_a = Annotation(
+            Point(1, 1),
+            {"class": "A"},
+        )
+        store["A"] = ann_a
+        result = store.nquery(
+            where="props['class'] == 'A'",
+            n_where="props['class'] == 'B'",
+            distance=2,
+            mode="boxpoint-boxpoint",
+        )
+        assert isinstance(result, dict)
+        assert len(result) == 0
+
+    @staticmethod
+    def test_nquery_boxpoint_boxpoint_multiple(store_cls):
+        """Test querying within a neighbourhood with multiple results.
+
+        Test that a neighbourhood query returns the correct results
+        for a simple data store with four points.
+
+        .. code-block:: text
+
+            3^
+            2|   B
+            1| A C D <-- D is outside the neighbourhood
+            0+------>
+             0 1 2 3
+
+        Query for all points within a distance of 2 from A. Should
+        return a dictionary with a single key, "A", and a value of
+        {"B": B, "C": C}.
+
+        """
+        store: AnnotationStore = store_cls()
+        ann_a = Annotation(
+            Point(1, 1),
+            {"class": "A"},
+        )
+        store["A"] = ann_a
+
+        ann_b = Annotation(
+            Point(2, 2),
+            {"class": "B"},
+        )
+        store["B"] = ann_b
+
+        ann_c = Annotation(
+            Point(2, 1),
+            {"class": "C"},
+        )
+        store["C"] = ann_c
+
+        ann_d = Annotation(
+            Point(3, 1),
+            {"class": "D"},
+        )
+        store["D"] = ann_d
+
+        result = store.nquery(
+            where="props['class'] == 'A'",
+            n_where="(props['class'] == 'B') | (props['class'] == 'C')",
+            distance=2,
+            mode="boxpoint-boxpoint",
+        )
+        assert isinstance(result, dict)
+        assert len(result) == 1
+        assert "A" in result
+        assert result["A"] == {"B": ann_b, "C": ann_c}
+
+    @staticmethod
+    def test_nquery_poly_poly(store_cls):
+        """Test querying within a neighbourhood with multiple results.
+
+        Test that a neighbourhood query returns the correct results
+        for a simple data store with two polygons.
+
+        .. code-block:: text
+
+            3^
+            2|   B
+            1| A
+            0+------>
+             0 1 2 3
+
+        """
+        store: AnnotationStore = store_cls()
+
+        ann_a = Annotation(  # Triangle
+            Polygon([(0, 0), (0, 1), (1, 0)]),
+            {"class": "A"},
+        )
+        store["A"] = ann_a
+
+        ann_b = Annotation(  # Square
+            Polygon.from_bounds(1, 1, 2, 2),
+            {"class": "B"},
+        )
+        store["B"] = ann_b
+
+        result = store.nquery(
+            where="props['class'] == 'A'",
+            n_where="props['class'] == 'B'",
+            distance=2,
+            mode="poly-poly",
+        )
+        assert isinstance(result, dict)
+        assert len(result) == 1
+
+    @staticmethod
+    def test_nquery_poly_poly_vs_boxpoint_boxpoint(store_cls):
+        """Test querying within a neighbourhood with two polygons.
+
+        Test that a full polygon neighbourhood query returns results
+        where a centroid query would return no results.
+
+        .. code-block:: text
+
+             ^
+            3|
+             |         <----2---->
+            2|     +-----+     +-----+
+             |     |  +  |<-1->|  +  |
+            1|     +-----+     +-----+
+             |
+            0+------------------------>
+             0     1     2     3     4
+
+        """
+        store: AnnotationStore = store_cls()
+
+        ann_a = Annotation(
+            Polygon.from_bounds(1, 1, 2, 2),
+            {"class": "A"},
+        )
+        store["A"] = ann_a
+
+        ann_b = Annotation(
+            Polygon.from_bounds(3, 1, 4, 2),
+            {"class": "B"},
+        )
+        store["B"] = ann_b
+
+        distance = 1.25
+
+        result = store.nquery(
+            where="props['class'] == 'A'",
+            n_where="props['class'] == 'B'",
+            distance=distance,
+            mode="boxpoint-boxpoint",
+        )
+        assert isinstance(result, dict)
+        assert len(result) == 0
+
+        result = store.nquery(
+            where="props['class'] == 'A'",
+            n_where="props['class'] == 'B'",
+            distance=distance,
+            mode=("poly", "poly"),
+        )
+        assert isinstance(result, dict)
+        assert len(result) == 1
+
+    @staticmethod
+    def test_nquery_polygon_boundary_alt(store_cls):
+        """Test querying within a neighbourhood with two polygons.
+
+        This test is similar to test_nquery_polygon_boundary, but
+        the centroids are closer than the boundaries.
+
+        .. code-block:: text
+
+             ^
+            5|     +-----------------+
+             |     +---------------+ |
+            4|        <-----2----->| |  centroid-boundary = 2
+             |        <--1-->      | |  centroid-centroid = 1
+            3|     +-----+         | |
+             |     |  +  |  +  ^   | |  centroid-boundary = 2
+            2|     +-----+     |   | |
+             |        ^        |2  | |
+            1|        v1.5     v   | |  boundary-boundary = 1.5
+             |     +---------------+ |
+            0+-----+-----------------+-->
+             0     1     2     3     4
+        """
+        store: AnnotationStore = store_cls()
+
+        # Annotation A: A 1x1 box
+        ann_a = Annotation(
+            Polygon.from_bounds(1, 2, 2, 3),
+            {"class": "A"},
+        )
+        store["A"] = ann_a
+
+        # C shaped polygon around annotation A
+        ann_b = Annotation(
+            Polygon(
+                [
+                    (1, 0),
+                    (4, 0),
+                    (4, 5),
+                    (1, 5),
+                    (1, 4.5),
+                    (3.5, 4.5),
+                    (3.5, 0.5),
+                    (1, 0.5),
+                ]
+            ),
+            {"class": "B"},
+        )
+        store["B"] = ann_b
+
+        distance = 1.75
+
+        centroid = Polygon.from_bounds(*ann_b.geometry.bounds).centroid
+
+        print(centroid)
+        print(ann_a.geometry.centroid)
+        print(
+            centroid.buffer(distance)
+            .intersection(ann_a.geometry.centroid.buffer(distance))
+            .area
+        )
+
+        result = store.nquery(
+            where="props['class'] == 'A'",
+            n_where="props['class'] == 'B'",
+            distance=distance,
+            mode="boxpoint-boxpoint",
+        )
+        assert isinstance(result, dict)
+        assert len(result) == 1
+
+    @staticmethod
+    def test_nquery_overlapping_grid_box_box(store_cls):
+        """Find duplicate (overlapping) cell boundaries via bounding boxes.
+
+        This generates an :math:`n \\times n` (where :math:`n=10`) grid
+        of overlapping fake cell boundary polygons, where each polygon
+        has radius of 5 and the grid has a spacing of 30.
+
+        The grid is then queried with a "box-box" neighbourhood query
+        (intersection of bounding boxes) and a `distance` paramete of 0
+        (no expansion of bounding boxes).
+
+        """
+        store: AnnotationStore = store_cls()
+
+        grid_size = 10
+        spacing = 30
+        radius = 5
+        grid = np.ndindex((grid_size, grid_size))
+
+        for x, y in grid:
+            cell_a = cell_polygon(
+                (x * spacing + radius, y * spacing + radius), radius=radius
+            )
+            ann_a = Annotation(cell_a, {"class": "A"})
+            cell_b = cell_polygon(
+                (x * spacing + radius, y * spacing + radius), radius=radius
+            )
+            ann_b = Annotation(cell_b, {"class": "B"})
+
+            store[f"A_{x}_{y}"] = ann_a
+            store[f"B_{x}_{y}"] = ann_b
+
+        result = store.nquery(
+            where="props['class'] == 'A'",
+            n_where="props['class'] == 'B'",
+            distance=0,
+            mode="box-box",
+        )
+        assert isinstance(result, dict)
+        assert len(result) == grid_size**2
+        for v in result.values():
+            assert len(v) == 1
+
+    @staticmethod
+    def test_nquery_overlapping_grid_boxpoint_boxpoint(store_cls):
+        """Find duplicate (overlapping) cell boundaries via bbox centroid distance.
+
+        This generates an :math:`n \\times n` (where :math:`n=10`) grid
+        of overlapping fake cell boundary polygons, where each polygon
+        has radius of 5 and the grid has a spacing of 30.
+
+        The grid is then queried with a "boxpoint-boxpoint"
+        neighbourhood query and a `distance` of 2 (use a buffer of 2
+        around the point).
+
+        """
+        store: AnnotationStore = store_cls()
+
+        grid_size = 10
+        spacing = 10
+        radius = 5
+        grid = np.ndindex((grid_size, grid_size))
+
+        for x, y in grid:
+            cell_a = cell_polygon(
+                (x * spacing + radius, y * spacing + radius), radius=radius
+            )
+            ann_a = Annotation(cell_a, {"class": "A"})
+            cell_b = cell_polygon(
+                (x * spacing + radius, y * spacing + radius), radius=radius
+            )
+            ann_b = Annotation(cell_b, {"class": "B"})
+
+            store[f"A_{x}_{y}"] = ann_a
+            store[f"B_{x}_{y}"] = ann_b
+
+        result = store.nquery(
+            where="props['class'] == 'A'",
+            n_where="props['class'] == 'B'",
+            distance=2,
+            mode="boxpoint-boxpoint",
+        )
+        assert isinstance(result, dict)
+        assert len(result) == grid_size**2
+        for v in result.values():
+            assert len(v) == 1
+
+    @staticmethod
+    def test_nquery_overlapping_grid_poly_poly(store_cls):
+        """Find duplicate (overlapping) cell boundaries via polygon intersection.
+
+        This generates an :math:`n \\times n` (where :math:`n=10`) grid
+        of overlapping fake cell boundary polygons, where each polygon
+        has radius of 5 and the grid has a spacing of 30.
+
+        The grid is then queried with a "poly-poly" neighbourhood query
+        (intersection of polygons) and a `distance` parameter of 2.
+
+        """
+        store: AnnotationStore = store_cls()
+
+        grid_size = 10
+        spacing = 30
+        radius = 5
+        grid = np.ndindex((grid_size, grid_size))
+
+        for x, y in grid:
+            cell_a = cell_polygon(
+                (x * spacing + radius, y * spacing + radius), radius=radius
+            )
+            ann_a = Annotation(cell_a, {"class": "A"})
+            cell_b = cell_polygon(
+                (x * spacing + radius, y * spacing + radius), radius=radius
+            )
+            ann_b = Annotation(cell_b, {"class": "B"})
+
+            store[f"A_{x}_{y}"] = ann_a
+            store[f"B_{x}_{y}"] = ann_b
+
+        result = store.nquery(
+            where="props['class'] == 'A'",
+            n_where="props['class'] == 'B'",
+            distance=2,
+            mode="poly-poly",
+        )
+        assert isinstance(result, dict)
+        assert len(result) == grid_size**2
+        for v in result.values():
+            assert len(v) == 1
+
+    @staticmethod
+    def test_invalid_mode_type(store_cls):
+        store: AnnotationStore = store_cls()
+
+        with pytest.raises(TypeError, match="string or tuple of strings"):
+            store.nquery(
+                where="props['class'] == 'A'",
+                n_where="props['class'] == 'B'",
+                distance=2,
+                mode=123,
+            )
+
+    @staticmethod
+    def test_invalid_mode_format(store_cls):
+        store: AnnotationStore = store_cls()
+
+        with pytest.raises(ValueError, match="must be one of"):
+            store.nquery(
+                where="props['class'] == 'A'",
+                n_where="props['class'] == 'B'",
+                distance=2,
+                mode="invalid-invalid-invalid",
+            )
+
+    @staticmethod
+    def test_invalid_mode(store_cls):
+        store: AnnotationStore = store_cls()
+
+        with pytest.raises(ValueError, match="must be one of"):
+            store.nquery(
+                where="props['class'] == 'A'",
+                n_where="props['class'] == 'B'",
+                distance=2,
+                mode="invalid",
+            )
+
+    @staticmethod
+    def test_bquery_only_where(store_cls):
+        """Test that bquery when only a where predicate is given.
+
+        This simply checks for no exceptions raised about None values.
+
+        """
+        store = store_cls()
+        assert store.bquery(where="props['foo'] == 'bar'") == {}
```

### Comparing `tiatoolbox-1.3.3/tests/test_annotation_tilerendering.py` & `tiatoolbox-1.4.0/tests/test_annotation_tilerendering.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """tests for annotation rendering using
 AnnotationRenderer and AnnotationTileGenerator
 """
 from pathlib import Path
 from typing import List, Union
 
-import matplotlib.cm as cm
 import matplotlib.pyplot as plt
 import numpy as np
 import pytest
+from matplotlib import colormaps
 from PIL import Image, ImageFilter
 from scipy.ndimage import label
 from shapely.geometry import LineString, MultiPoint, MultiPolygon, Polygon
 from shapely.geometry.point import Point
 from skimage import data
 
 from tests.test_annotation_stores import cell_polygon
@@ -105,15 +105,15 @@
     tg = AnnotationTileGenerator(wsi.info, store, renderer, tile_size=256)
     for i, tile in enumerate(tg):
         if i > 5:
             break
         assert isinstance(tile, Image.Image)
         assert tile.size == (256, 256)
         plt.imshow(tile)
-        plt.show()
+        plt.show(block=False)
 
 
 def test_correct_number_rendered(fill_store, tmp_path):
     """Test that the expected number of annotations are rendered."""
     array = np.ones((1024, 1024))
     wsi = wsireader.VirtualWSIReader(array, mpp=(1, 1))
     _, store = fill_store(SQLiteStore, tmp_path / "test.db")
@@ -184,15 +184,15 @@
     wsi = wsireader.VirtualWSIReader(array, mpp=(1, 1))
     _, store = fill_store(SQLiteStore, tmp_path / "test.db")
     renderer = AnnotationRenderer(max_scale=1, zoomed_out_strat="decimate")
     tg = AnnotationTileGenerator(wsi.info, store, renderer, tile_size=256)
 
     thumb = tg.get_tile(1, 1, 1)
     plt.imshow(thumb)
-    plt.show()
+    plt.show(block=False)
     _, num = label(np.array(thumb)[:, :, 1])  # default colour is green
     assert num == 17  # expect 17 pts in bottom right quadrant
 
 
 def test_get_tile_negative_level(fill_store, tmp_path):
     """Test for IndexError on negative levels."""
     array = np.ones((1024, 1024))
@@ -245,39 +245,41 @@
     _, store = fill_store(SQLiteStore, tmp_path / "test.db")
     tg = MockTileGenerator(wsi.info, store, tile_size=224)
 
     tile = tg.get_tile(0, 0, 0)
     assert tile.size == (112, 112)
 
 
-def test_unknown_geometry(fill_store, tmp_path):
-    """Test warning when unknown geometries are present that cannot
+def test_unknown_geometry(fill_store, tmp_path, caplog):
+    """
+    Test warning when unknown geometries are present that cannot
     be rendered.
+
     """
     array = np.ones((1024, 1024))
     wsi = wsireader.VirtualWSIReader(array)
     _, store = fill_store(SQLiteStore, tmp_path / "test.db")
     store.append(
         Annotation(geometry=MultiPoint([(5.0, 5.0), (10.0, 10.0)]), properties={})
     )
     store.commit()
     renderer = AnnotationRenderer(max_scale=8, edge_thickness=0)
     tg = AnnotationTileGenerator(wsi.info, store, renderer, tile_size=256)
-    with pytest.warns(UserWarning, match="Unknown geometry"):
-        tg.get_tile(0, 0, 0)
+    tg.get_tile(0, 0, 0)
+    assert "Unknown geometry" in caplog.text
 
 
-def test_interp_pad_warning(fill_store, tmp_path):
+def test_interp_pad_warning(fill_store, tmp_path, caplog):
     """Test warning when providing unused options."""
     array = np.ones((1024, 1024))
     wsi = wsireader.VirtualWSIReader(array)
     _, store = fill_store(SQLiteStore, tmp_path / "test.db")
     tg = AnnotationTileGenerator(wsi.info, store, tile_size=256)
-    with pytest.warns(UserWarning, match="interpolation, pad_mode are unused"):
-        tg.get_tile(0, 0, 0, pad_mode="constant")
+    tg.get_tile(0, 0, 0, pad_mode="constant")
+    assert "interpolation, pad_mode are unused" in caplog.text
 
 
 def test_user_provided_cm(fill_store, tmp_path):
     """Test correct color mapping for user-provided cm name."""
     array = np.ones((1024, 1024))
     wsi = wsireader.VirtualWSIReader(array, mpp=(1, 1))
     _, store = fill_store(SQLiteStore, tmp_path / "test.db")
@@ -287,15 +289,15 @@
         edge_thickness=0,
     )
     tg = AnnotationTileGenerator(wsi.info, store, renderer, tile_size=256)
 
     tile = np.array(tg.get_tile(1, 0, 1))  # line here with prob=0.75
     color = tile[np.any(tile, axis=2), :3]
     color = color[0, :]
-    viridis_mapper = cm.get_cmap("viridis")
+    viridis_mapper = colormaps["viridis"]
     assert np.all(
         np.equal(color, (np.array(viridis_mapper(0.75)) * 255)[:3].astype(np.uint8))
     )  # expect rendered color to be viridis(0.75)
 
 
 def test_random_mapper():
     """Test random colour map dict for list."""
@@ -322,25 +324,27 @@
         rgba = renderer.mapper(ann_type)
         assert isinstance(rgba, tuple)
         assert len(rgba) == 4
         for val in rgba:
             assert 0 <= val <= 1
 
 
-def test_colour_prop_warning(fill_store, tmp_path):
-    """Test warning when rendering annotations in which the provided
+def test_colour_prop_warning(fill_store, tmp_path, caplog):
+    """
+    Test warning when rendering annotations in which the provided
     score_prop does not exist.
+
     """
     array = np.ones((1024, 1024))
     wsi = wsireader.VirtualWSIReader(array, mpp=(1, 1))
     _, store = fill_store(SQLiteStore, tmp_path / "test.db")
     renderer = AnnotationRenderer(score_prop="nonexistant_prop")
     tg = AnnotationTileGenerator(wsi.info, store, renderer, tile_size=256)
-    with pytest.warns(UserWarning, match="not found in properties"):
-        tg.get_tile(1, 0, 0)
+    tg.get_tile(1, 0, 0)
+    assert "not found in properties" in caplog.text
 
 
 def test_blur(fill_store, tmp_path):
     """Test blur."""
     array = np.ones((1024, 1024))
     wsi = wsireader.VirtualWSIReader(array, mpp=(1, 1))
     _, store = fill_store(SQLiteStore, tmp_path / "test.db")
@@ -372,23 +376,23 @@
 
 
 def test_secondary_cmap(fill_store, tmp_path):
     """Test secondary cmap."""
     array = np.ones((1024, 1024))
     wsi = wsireader.VirtualWSIReader(array, mpp=(1, 1))
     _, store = fill_store(SQLiteStore, tmp_path / "test.db")
-    cmap_dict = {"type": "line", "score_prop": "prob", "mapper": cm.get_cmap("viridis")}
+    cmap_dict = {"type": "line", "score_prop": "prob", "mapper": colormaps["viridis"]}
     renderer = AnnotationRenderer(
         score_prop="type", secondary_cmap=cmap_dict, edge_thickness=0
     )
     tg = AnnotationTileGenerator(wsi.info, store, renderer, tile_size=256)
     tile = np.array(tg.get_tile(1, 0, 1))  # line here with prob=0.75
     color = tile[np.any(tile, axis=2), :3]
     color = color[0, :]
-    viridis_mapper = cm.get_cmap("viridis")
+    viridis_mapper = colormaps["viridis"]
     assert np.all(
         np.equal(color, (np.array(viridis_mapper(0.75)) * 255)[:3].astype(np.uint8))
     )  # expect rendered color to be viridis(0.75)
 
 
 def test_unfilled_polys(fill_store, tmp_path):
     """Test unfilled polygons."""
```

### Comparing `tiatoolbox-1.3.3/tests/test_data.py` & `tiatoolbox-1.4.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/test_docs.py` & `tiatoolbox-1.4.0/tests/test_docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
     Validity checks are:
     1. The docstring examples are syntactically valid (can parse an AST).
     2. That the imports can be resolved.
 
     """
     for file in source_files:
-
         source = Path(file).read_text()
         tree = ast.parse(source)
         parser = doctest.DocTestParser()
         for node in ast.walk(tree):
             if not isinstance(node, (ast.FunctionDef, ast.ClassDef)):
                 continue
             docstring = ast.get_docstring(node)
```

### Comparing `tiatoolbox-1.3.3/tests/test_dsl.py` & `tiatoolbox-1.4.0/tests/test_dsl.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     properties = json.dumps(SAMPLE_PROPERTIES)
     assert json_contains(properties, "int")
     assert json_contains(json.dumps([1]), 1)
     assert not json_contains(properties, "foo")
 
 
 def sqlite_eval(query: Union[str, Number]):
-    """Evaluate an SQL predicate on dummpy data and return the result.
+    """Evaluate an SQL predicate on dummy data and return the result.
 
     Args:
         query (Union[str, Number]): SQL predicate to evaluate.
 
     Returns:
         bool: Result of the evaluation.
 
@@ -87,14 +87,29 @@
             assert query.count("(") == query.count(")")
             assert query.count("[") == query.count("]")
         cur.execute(f"SELECT {query} FROM test")
         (result,) = cur.fetchone()
     return result
 
 
+class TestSQLite:  # noqa: PIE798
+    """Test converting from our DSL to an SQLite backend."""
+
+    @staticmethod
+    def test_prop_or_prop():
+        """Test OR operator between two prop accesses."""
+        query = eval(  # skipcq: PYL-W0123
+            "(props['int'] == 2) | (props['int'] == 3)", SQL_GLOBALS, {}
+        )
+        assert str(query) == (
+            '((json_extract(properties, "$.int") == 2) OR '
+            '(json_extract(properties, "$.int") == 3))'
+        )
+
+
 class TestPredicate:
     """Test predicate statments with various backends."""
 
     scenarios = [
         (
             "Python",
             {
```

### Comparing `tiatoolbox-1.3.3/tests/test_graph.py` & `tiatoolbox-1.4.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/test_meta_ngff_dataclasses.py` & `tiatoolbox-1.4.0/tests/test_meta_ngff_dataclasses.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/test_metrics.py` & `tiatoolbox-1.4.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/test_patch_extraction.py` & `tiatoolbox-1.4.0/tests/test_patch_extraction.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         input_img=input_img,
         locations_list=locations_list,
         method_name="point",
         patch_size=(200, 200),
     )
 
     assert isinstance(points, patchextraction.PointsPatchExtractor)
+    assert len(points) == 1860
 
     sliding_window = patchextraction.get_patch_extractor(
         input_img=input_img,
         method_name="slidingwindow",
         patch_size=(200, 200),
     )
 
@@ -262,15 +263,15 @@
         img_patches_test.append(patch)
 
     img_patches_test = np.array(img_patches_test)
     assert np.all(img_patches == img_patches_test)
 
 
 def test_get_coordinates():
-    """Test get tile cooordinates functionality."""
+    """Test get tile coordinates functionality."""
     expected_output = np.array(
         [
             [0, 0, 4, 4],
             [4, 0, 8, 4],
         ]
     )
     output = PatchExtractor.get_coordinates(
@@ -420,120 +421,85 @@
             [8, 0, 12, 4],
             [8, 4, 12, 8],
         ]
     )
     mask = np.zeros([9, 6])
     mask[0:4, 3:8] = 1  # will flag first 2
     mask_reader = VirtualWSIReader(mask)
-
-    # Tests for (original) filter_coordinates method
-    # functionality test
-    flag_list = PatchExtractor.filter_coordinates(
-        mask_reader, bbox_list, resolution=1.0, units="baseline"
-    )
-    assert np.sum(flag_list - np.array([1, 1, 0, 0, 0, 0])) == 0
-
-    # Test for bad mask input
-    with pytest.raises(
-        ValueError, match="`mask_reader` should be wsireader.VirtualWSIReader."
-    ):
-        PatchExtractor.filter_coordinates(
-            mask, bbox_list, resolution=1.0, units="baseline"
-        )
-
-    # Test for bad bbox coordinate list in the input
-    with pytest.raises(ValueError, match=r".*should be ndarray of integer type.*"):
-        PatchExtractor.filter_coordinates(
-            mask_reader, bbox_list.tolist(), resolution=1.0, units="baseline"
-        )
-
-    # Test for incomplete coordinate list
-    with pytest.raises(ValueError, match=r".*`coordinates_list` of shape.*"):
-        PatchExtractor.filter_coordinates(
-            mask_reader, bbox_list[:, :2], resolution=1.0, units="baseline"
-        )
+    slide_shape = (6, 9)  # slide shape (w, h) at requested resolution
 
     ###############################################
-    # Tests for filter_coordinates_fast (new) method
+    # Tests for filter_coordinates (new) method
     _info = mask_reader.info
     _info.mpp = 1.0
     mask_reader._m_info = _info
 
     # functionality test
-    flag_list = PatchExtractor.filter_coordinates_fast(
+    flag_list = PatchExtractor.filter_coordinates(
         mask_reader,
         bbox_list,
-        coordinate_resolution=1.0,
-        coordinate_units="mpp",
-        mask_resolution=1,
+        slide_shape,
     )
     assert np.sum(flag_list - np.array([1, 1, 0, 0, 0, 0])) == 0
-    flag_list = PatchExtractor.filter_coordinates_fast(
-        mask_reader, bbox_list, coordinate_resolution=(1.0, 1.0), coordinate_units="mpp"
-    )
+    flag_list = PatchExtractor.filter_coordinates(mask_reader, bbox_list, slide_shape)
 
     # Test for bad mask input
     with pytest.raises(
         ValueError, match="`mask_reader` should be wsireader.VirtualWSIReader."
     ):
-        PatchExtractor.filter_coordinates_fast(
+        PatchExtractor.filter_coordinates(
             mask,
             bbox_list,
-            coordinate_resolution=1.0,
-            coordinate_units="mpp",
+            slide_shape,
         )
 
     # Test for bad bbox coordinate list in the input
     with pytest.raises(ValueError, match=r".*should be ndarray of integer type.*"):
-        PatchExtractor.filter_coordinates_fast(
+        PatchExtractor.filter_coordinates(
             mask_reader,
             bbox_list.tolist(),
-            coordinate_resolution=1,
-            coordinate_units="mpp",
+            slide_shape,
         )
 
     # Test for incomplete coordinate list
     with pytest.raises(ValueError, match=r".*`coordinates_list` must be of shape.*"):
-        PatchExtractor.filter_coordinates_fast(
+        PatchExtractor.filter_coordinates(
             mask_reader,
             bbox_list[:, :2],
-            coordinate_resolution=1,
-            coordinate_units="mpp",
+            slide_shape,
         )
 
     # Test for put of range min_mask_ratio
     with pytest.raises(ValueError, match="`min_mask_ratio` must be between 0 and 1."):
-        PatchExtractor.filter_coordinates_fast(
+        PatchExtractor.filter_coordinates(
             mask_reader,
             bbox_list,
-            coordinate_resolution=1.0,
-            coordinate_units="mpp",
+            slide_shape,
             min_mask_ratio=-0.5,
         )
     with pytest.raises(ValueError, match="`min_mask_ratio` must be between 0 and 1."):
-        PatchExtractor.filter_coordinates_fast(
+        PatchExtractor.filter_coordinates(
             mask_reader,
             bbox_list,
-            coordinate_resolution=1.0,
-            coordinate_units="mpp",
+            slide_shape,
             min_mask_ratio=1.1,
         )
 
 
-def test_mask_based_patch_extractor_ndpi(sample_ndpi):
+def test_mask_based_patch_extractor_ndpi(sample_ndpi, caplog):
     """Test SlidingWindowPatchExtractor with mask for ndpi image."""
     res = 0
     patch_size = stride = (400, 400)
     input_img = pathlib.Path(sample_ndpi)
     wsi = OpenSlideWSIReader(input_img=input_img)
     slide_dimensions = wsi.info.slide_dimensions
 
     # Generating a test mask to read patches from
     mask_dim = (int(slide_dimensions[0] / 10), int(slide_dimensions[1] / 10))
-    wsi_mask = np.zeros(mask_dim, dtype=np.uint8)
+    wsi_mask = np.zeros(mask_dim[::-1], dtype=np.uint8)  # reverse as dims are (w, h)
     # masking two column to extract patch from
     wsi_mask[:, :2] = 255
 
     # patch extraction based on the column mask
     patches = patchextraction.get_patch_extractor(
         input_img=input_img,
         input_mask=wsi_mask,
@@ -554,62 +520,63 @@
 
     # because we are using column mask to extract patches, we can expect
     # that the patches[1] is the from the second row (y) in the first column.
     assert np.all(patches[1] == patch)
     assert patches[0].shape == (patch_size[0], patch_size[1], 3)
 
     # Test None option for mask
-    patches = patchextraction.get_patch_extractor(
+    _ = patchextraction.get_patch_extractor(
         input_img=input_img,
         input_mask=None,
         method_name="slidingwindow",
         patch_size=patch_size,
         resolution=res,
         units="level",
         stride=stride[0],
     )
 
     # Test passing a VirtualWSI for mask
     mask_wsi = VirtualWSIReader(wsi_mask, info=wsi._m_info, mode="bool")
-    patches = patchextraction.get_patch_extractor(
+    _ = patchextraction.get_patch_extractor(
         input_img=wsi,
         input_mask=mask_wsi,
         method_name="slidingwindow",
         patch_size=patch_size,
         resolution=res,
         units="level",
         stride=None,
     )
 
     # Test `otsu` option for mask
-    patches = patchextraction.get_patch_extractor(
+    _ = patchextraction.get_patch_extractor(
         input_img=input_img,
         input_mask="otsu",
         method_name="slidingwindow",
         patch_size=patch_size[0],
         resolution=res,
         units="level",
         stride=stride,
     )
 
-    patches = patchextraction.get_patch_extractor(
+    _ = patchextraction.get_patch_extractor(
         input_img=wsi_mask,  # a numpy array to build VirtualSlideReader
         input_mask="morphological",
         method_name="slidingwindow",
         patch_size=patch_size,
         resolution=res,
         units="level",
         stride=stride,
     )
 
     # Test passing an empty mask
     wsi_mask = np.zeros(mask_dim, dtype=np.uint8)
-    with pytest.warns(UserWarning, match=".*No candidate coordinates left.*"):
-        _ = patchextraction.get_patch_extractor(
-            input_img=input_img,
-            input_mask=wsi_mask,
-            method_name="slidingwindow",
-            patch_size=patch_size,
-            resolution=res,
-            units="level",
-            stride=stride,
-        )
+
+    _ = patchextraction.get_patch_extractor(
+        input_img=input_img,
+        input_mask=wsi_mask,
+        method_name="slidingwindow",
+        patch_size=patch_size,
+        resolution=res,
+        units="level",
+        stride=stride,
+    )
+    assert "No candidate coordinates left" in caplog.text
```

### Comparing `tiatoolbox-1.3.3/tests/test_pyramid.py` & `tiatoolbox-1.4.0/tests/test_pyramid.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/test_save_tiles.py` & `tiatoolbox-1.4.0/tests/test_save_tiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             "--file-types",
             "*.ndpi, *.svs",
             "--tile-objective-value",
             "5",
             "--output-path",
             tmp_path,
             "--verbose",
-            "False",
+            "True",
         ],
     )
 
     assert save_svs_tiles_result.exit_code == 0
     assert (
         pathlib.Path(tmp_path)
         .joinpath("CMU-1-Small-Region.svs")
```

### Comparing `tiatoolbox-1.3.3/tests/test_scale.py` & `tiatoolbox-1.4.0/tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/test_slide_info.py` & `tiatoolbox-1.4.0/tests/test_slide_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,14 @@
 """Tests for code related to obtaining slide information."""
 
 import pathlib
 
 from click.testing import CliRunner
 
-from tiatoolbox import cli, utils
-from tiatoolbox.wsicore.slide_info import slide_info
-
-
-def test_slide_info(sample_all_wsis, tmp_path):
-    """Test for slide_info as a python function."""
-    file_types = ("*.ndpi", "*.svs", "*.mrxs", "*.jp2")
-    files_all = utils.misc.grab_files_from_dir(
-        input_path=sample_all_wsis,
-        file_types=file_types,
-    )
-
-    for curr_file in files_all:
-        slide_param = slide_info(input_path=curr_file, verbose=True)
-        out_path = tmp_path / slide_param.file_path.with_suffix(".yaml").name
-        utils.misc.save_yaml(slide_param.as_dict(), out_path)
-
+from tiatoolbox import cli
 
 # -------------------------------------------------------------------------------------
 # Command Line Interface
 # -------------------------------------------------------------------------------------
 
 
 def test_command_line_slide_info(sample_all_wsis, tmp_path):
@@ -38,14 +22,16 @@
             str(pathlib.Path(sample_all_wsis)),
             "--mode",
             "save",
             "--file-types",
             "*.ndpi, *.svs",
             "--output-path",
             str(tmp_path),
+            "--verbose",
+            "True",
         ],
     )
 
     assert slide_info_result.exit_code == 0
     assert pathlib.Path(tmp_path, "CMU-1-Small-Region.yaml").exists()
     assert pathlib.Path(tmp_path, "CMU-1.yaml").exists()
     assert not pathlib.Path(tmp_path, "test1.yaml").exists()
@@ -82,15 +68,15 @@
             "--img-input",
             sample_svs,
             "--file-types",
             "*.ndpi, *.svs",
             "--mode",
             "show",
             "--verbose",
-            "False",
+            "True",
         ],
     )
 
     assert slide_info_result.exit_code == 0
 
 
 def test_command_line_slide_info_file_not_found(sample_svs):
```

### Comparing `tiatoolbox-1.3.3/tests/test_slide_thumbnail.py` & `tiatoolbox-1.4.0/tests/test_slide_thumbnail.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/test_stainaugment.py` & `tiatoolbox-1.4.0/tests/test_stainaugment.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/test_stainnorm.py` & `tiatoolbox-1.4.0/tests/test_stainnorm.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/test_tiatoolbox.py` & `tiatoolbox-1.4.0/tests/test_tiatoolbox.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/test_tiffreader.py` & `tiatoolbox-1.4.0/tests/test_tiffreader.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         del pixels.attrib["PhysicalSizeY"]
     new_description = ElementTree.tostring(tree, encoding="unicode")
     monkeypatch.setattr(page, "description", new_description)
     monkeypatch.setattr(wsi, "_m_info", None)
     assert wsi.info.mpp is None
 
 
-def test_ome_missing_physicalsizey(monkeypatch):
+def test_ome_missing_physicalsizey(monkeypatch, caplog):
     """Test that an OME-TIFF can be read without physical size."""
     sample = _fetch_remote_sample("ome-brightfield-pyramid-1-small")
     wsi = wsireader.TIFFWSIReader(sample)
     page = wsi.tiff.pages[0]
     description = page.description
     tree = ElementTree.fromstring(description)
     namespaces = {
@@ -60,16 +60,16 @@
     images = tree.findall("ome:Image", namespaces)
     for image in images:
         pixels = image.find("ome:Pixels", namespaces)
         del pixels.attrib["PhysicalSizeY"]
     new_description = ElementTree.tostring(tree, encoding="unicode")
     monkeypatch.setattr(page, "description", new_description)
     monkeypatch.setattr(wsi, "_m_info", None)
-    with pytest.warns(UserWarning):
-        assert pytest.approx(wsi.info.mpp, abs=0.1) == 0.5
+    assert pytest.approx(wsi.info.mpp, abs=0.1) == 0.5
+    assert "Only one MPP value found. Using it for both X  and Y" in caplog.text
 
 
 def test_tiffreader_non_tiled_metadata(monkeypatch):
     """Test that fetching metadata for non-tiled TIFF works."""
     sample = _fetch_remote_sample("ome-brightfield-pyramid-1-small")
     wsi = wsireader.TIFFWSIReader(sample)
     monkeypatch.setattr(wsi.tiff, "is_ome", False)
```

### Comparing `tiatoolbox-1.3.3/tests/test_tileserver.py` & `tiatoolbox-1.4.0/tests/test_tileserver.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tests/test_tissuemask.py` & `tiatoolbox-1.4.0/tests/test_tissuemask.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,23 +145,23 @@
     assert mask_a.shape == thumb.shape[:2]
 
 
 def test_transform_before_fit_otsu():
     """Test otsu masker error on transform before fit."""
     image = np.ones((1, 10, 10))
     masker = tissuemask.OtsuTissueMasker()
-    with pytest.raises(Exception, match="Fit must be called before transform."):
+    with pytest.raises(SyntaxError, match="Fit must be called before transform."):
         masker.transform([image])[0]
 
 
 def test_transform_before_fit_morphological():
     """Test morphological masker error on transform before fit."""
     image = np.ones((1, 10, 10))
     masker = tissuemask.MorphologicalMasker()
-    with pytest.raises(Exception, match="Fit must be called before transform."):
+    with pytest.raises(SyntaxError, match="Fit must be called before transform."):
         masker.transform([image])[0]
 
 
 def test_transform_fit_otsu_wrong_shape():
     """Test giving the incorrect input shape to otsu masker."""
     image = np.ones((10, 10))
     masker = tissuemask.OtsuTissueMasker()
```

### Comparing `tiatoolbox-1.3.3/tests/test_utils.py` & `tiatoolbox-1.4.0/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         interpolation=cv2.INTER_CUBIC,
     )
     assert resized_img.shape == (1000, 500, 3)
 
     # test for dtype conversion, pairs of
     # (original type, converted type)
     test_dtypes = [
-        (np.bool, np.uint8),
+        (np.bool_, np.uint8),
         (np.int8, np.int16),
         (np.int16, np.int16),
         (np.int32, np.float32),
         (np.uint8, np.uint8),
         (np.uint16, np.uint16),
         (np.uint32, np.float32),
         (np.int64, np.float64),
@@ -1049,16 +1049,16 @@
     slide_dimensions = (1024, 1024)
 
     def edge_mask(bounds: Tuple[int, int, int, int]) -> np.ndarray:
         """Produce a mask of regions outside of the slide dimensions."""
         l, t, r, b = bounds
         slide_width, slide_height = slide_dimensions
         x, y = np.meshgrid(np.arange(l, r), np.arange(t, b), indexing="ij")
-        under = np.logical_or(x < 0, y < 0).astype(np.int)
-        over = np.logical_or(x >= slide_width, y >= slide_height).astype(np.int)
+        under = np.logical_or(x < 0, y < 0).astype(np.int_)
+        over = np.logical_or(x >= slide_width, y >= slide_height).astype(np.int_)
         return under, over
 
     loc = (-5, -5)
     size = (10, 10)
     bounds = utils.transforms.locsize2bounds(loc, size)
     under, over = edge_mask(bounds)
     region = -under + over
@@ -1431,28 +1431,29 @@
     store = utils.misc.store_from_dat(tmp_path / "test.dat")
     assert len(store) == 4
 
     result = store.query(where="props['type'] == 'A: 1'")
     assert len(result) == 1
 
 
-def test_invalid_poly(tmp_path):
+def test_invalid_poly(tmp_path, caplog):
     """Test that invalid polygons are dealt with correctly."""
     coords = [(0, 0), (0, 2), (1, 1), (2, 2), (2, 0), (1, 1), (0, 0)]
     poly = Polygon(coords)
     data = make_simple_dat()
     data["invalid"] = {
         "box": poly.bounds,
         "centroid": [poly.centroid.x, poly.centroid.y],
         "contour": np.array(poly.exterior.coords).tolist(),
         "type": 2,
     }
     joblib.dump(data, tmp_path / "test.dat")
-    with pytest.warns(UserWarning, match="Invalid geometry found, fix"):
-        store = utils.misc.store_from_dat(tmp_path / "test.dat")
+    store = utils.misc.store_from_dat(tmp_path / "test.dat")
+
+    assert "Invalid geometry found, fix" in caplog.text
 
     result = store.query(where="props['type'] == 2")
     assert next(iter(result.values())).geometry.is_valid
 
 
 def test_from_multi_head_dat_type_dict(tmp_path):
     """Test generating a store from a .dat file with multiple heads, with typedict."""
```

### Comparing `tiatoolbox-1.3.3/tests/test_visualization.py` & `tiatoolbox-1.4.0/tests/test_visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,19 @@
     label_info_fail = copy.deepcopy(label_info_full)
     label_info_fail[1] = ("ABC", (255, 255))
     with pytest.raises(ValueError, match=r".*Wrong `label_info` format.*"):
         _ = overlay_prediction_mask(thumb, merged, label_info=label_info_fail)
 
     # Test normal run, should not crash.
     thumb_float = thumb / 255.0
-    _ = overlay_prediction_mask(thumb_float, merged, label_info=label_info_full)
-    _ = overlay_prediction_mask(thumb, merged, label_info=label_info_full)
+    ax = overlay_prediction_mask(thumb_float, merged, label_info=label_info_full)
+    ax.remove()
+    ax = overlay_prediction_mask(thumb, merged, label_info=label_info_full)
+    ax.remove()
+
     ax = plt.subplot(1, 2, 1)
     _ = overlay_prediction_mask(thumb, merged, ax=ax)
     _ = overlay_prediction_mask(thumb_float, merged, min_val=0.5, return_ax=False)
 
 
 def test_overlay_probability_map(sample_wsi_dict):
     """Test functional run for overlaying merged patch prediction of wsi."""
```

### Comparing `tiatoolbox-1.3.3/tests/test_wsi_registration.py` & `tiatoolbox-1.4.0/tests/test_wsi_registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import cv2
 import numpy as np
 import pytest
 
 from tiatoolbox.tools.registration.wsi_registration import (
     AffineWSITransformer,
     DFBRegister,
+    apply_affine_transformation,
     apply_bspline_transform,
     estimate_bspline_transform,
     match_histograms,
     prealignment,
 )
 from tiatoolbox.utils.metrics import dice
 from tiatoolbox.utils.misc import imread
@@ -183,25 +184,26 @@
 
 
 def test_warning(
     fixed_image,
     moving_image,
     fixed_mask,
     moving_mask,
+    caplog,
 ):
     """Test for displaying warning in prealignment function."""
     fixed_img = imread(pathlib.Path(fixed_image))
     moving_img = imread(pathlib.Path(moving_image))
     fixed_mask = imread(pathlib.Path(fixed_mask))
     moving_mask = imread(pathlib.Path(moving_mask))
     fixed_img, moving_img = fixed_img[:, :, 0], moving_img[:, :, 0]
-    with pytest.warns(UserWarning):
-        _ = prealignment(
-            fixed_img, moving_img, fixed_mask, moving_mask, dice_overlap=0.9
-        )
+
+    _ = prealignment(fixed_img, moving_img, fixed_mask, moving_mask, dice_overlap=0.9)
+
+    assert "Not able to find the best transformation" in caplog.text
 
 
 def test_match_histogram_inputs():
     """Test for inputs to match_histogram function."""
     image_a = np.random.randint(256, size=(256, 256, 3))
     image_b = np.random.randint(256, size=(256, 256, 3))
     with pytest.raises(
@@ -209,16 +211,22 @@
     ):
         _, _ = match_histograms(image_a, image_b)
 
 
 def test_match_histograms():
     """Test for preprocessing/normalization of an image pair."""
     image_a = np.random.randint(256, size=(256, 256))
-    image_b = np.random.randint(256, size=(256, 256))
-    _, _ = match_histograms(image_a, image_b, 3)
+    image_b = np.zeros(shape=(256, 256), dtype=int)
+    out_a, out_b = match_histograms(image_a, image_b, 3)
+    assert np.all(out_a == image_a)
+    assert np.all(out_b == 255)
+
+    out_a, out_b = match_histograms(image_b, image_a, 3)
+    assert np.all(out_a == 255)
+    assert np.all(out_b == image_a)
 
     image_a = np.random.randint(256, size=(256, 256, 1))
     image_b = np.random.randint(256, size=(256, 256, 1))
     _, _ = match_histograms(image_a, image_b)
 
     image_a = np.array(
         [
@@ -434,39 +442,40 @@
         )
 
 
 def test_bspline_transform(fixed_image, moving_image, fixed_mask, moving_mask):
     """Test for estimate_bspline_transform function."""
     fixed_img = imread(fixed_image)
     moving_img = imread(moving_image)
-    fixed_msk = imread(fixed_mask)
-    moving_msk = imread(moving_mask)
+    fixed_mask_ = imread(fixed_mask)
+    moving_mask_ = imread(moving_mask)
 
     rigid_transform = np.array(
         [[-0.99683, -0.00333, 338.69983], [-0.03201, -0.98420, 770.22941], [0, 0, 1]]
     )
-    moving_img = cv2.warpAffine(
-        moving_img, rigid_transform[0:-1][:], fixed_img.shape[:2][::-1]
-    )
-    moving_msk = cv2.warpAffine(
-        moving_msk, rigid_transform[0:-1][:], fixed_img.shape[:2][::-1]
-    )
+    moving_img = apply_affine_transformation(fixed_img, moving_img, rigid_transform)
+    moving_mask_ = apply_affine_transformation(fixed_img, moving_mask_, rigid_transform)
 
     # Grayscale images as input
     transform = estimate_bspline_transform(
-        fixed_img[:, :, 0], moving_img[:, :, 0], fixed_msk[:, :, 0], moving_msk[:, :, 0]
+        fixed_img[:, :, 0],
+        moving_img[:, :, 0],
+        fixed_mask_[:, :, 0],
+        moving_mask_[:, :, 0],
     )
     _ = apply_bspline_transform(fixed_img[:, :, 0], moving_img[:, :, 0], transform)
 
     # RGB images as input
-    transform = estimate_bspline_transform(fixed_img, moving_img, fixed_msk, moving_msk)
+    transform = estimate_bspline_transform(
+        fixed_img, moving_img, fixed_mask_, moving_mask_
+    )
 
     _ = apply_bspline_transform(fixed_img, moving_img, transform)
-    registered_msk = apply_bspline_transform(fixed_msk, moving_msk, transform)
-    mask_overlap = dice(fixed_msk, registered_msk)
+    registered_msk = apply_bspline_transform(fixed_mask_, moving_mask_, transform)
+    mask_overlap = dice(fixed_mask_, registered_msk)
     assert mask_overlap > 0.75
 
 
 def test_affine_wsi_transformer(sample_ome_tiff):
     test_locations = [(1001, 600), (1000, 500), (800, 701)]  # at base level 0
     resolution = 0
     size = (100, 100)
```

### Comparing `tiatoolbox-1.3.3/tests/test_wsimeta.py` & `tiatoolbox-1.4.0/tests/test_wsimeta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tests for obtaining whole-slide image metadata."""
 
 import numpy as np
 import pytest
 
-from tiatoolbox.wsicore import wsimeta, wsireader
+from tiatoolbox.wsicore import WSIMeta, wsimeta, wsireader
 
 
 # noinspection PyTypeChecker
 def test_wsimeta_init_fail():
     """Test incorrect init for WSIMeta raises TypeError."""
     with pytest.raises(TypeError):
         wsimeta.WSIMeta(slide_dimensions=(None, None), axes="YXS")
@@ -59,15 +59,16 @@
 
 @pytest.mark.filterwarnings("ignore")
 def test_wsimeta_validate_pass():
     """Test WSIMeta validation."""
     meta = wsimeta.WSIMeta(slide_dimensions=(512, 512), axes="YXS")
     assert meta.validate()
 
-    meta = wsimeta.WSIMeta(
+    # Test with top-level import
+    meta = WSIMeta(
         slide_dimensions=(512, 512),
         axes="YXS",
         level_dimensions=[(512, 512), (256, 256)],
         level_downsamples=[1, 2],
     )
 
     assert meta.validate()
```

### Comparing `tiatoolbox-1.3.3/tests/test_wsireader.py` & `tiatoolbox-1.4.0/tests/test_wsireader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 """Tests for reading whole-slide images."""
 
+import copy
 import json
+import logging
 import os
 import pathlib
 import random
 import re
 import shutil
 from copy import deepcopy
+from pathlib import Path
 from time import time
 
 # When no longer supporting Python <3.9 this should be collections.abc.Iterable
 from typing import Iterable
 
 import cv2
 import numpy as np
 import pytest
 import zarr
 from click.testing import CliRunner
+from packaging.version import Version
 from skimage.filters import threshold_otsu
 from skimage.metrics import peak_signal_noise_ratio, structural_similarity
 from skimage.morphology import binary_dilation, disk, remove_small_objects
 from skimage.registration import phase_cross_correlation
 
 from tiatoolbox import cli, rcParam, utils
 from tiatoolbox.annotation.storage import SQLiteStore
 from tiatoolbox.data import _fetch_remote_sample
 from tiatoolbox.utils.exceptions import FileNotSupported
 from tiatoolbox.utils.misc import imread
 from tiatoolbox.utils.transforms import imresize, locsize2bounds
 from tiatoolbox.utils.visualization import AnnotationRenderer
-from tiatoolbox.wsicore import wsireader
+from tiatoolbox.wsicore import WSIReader, wsireader
 from tiatoolbox.wsicore.wsireader import (
     AnnotationStoreReader,
     ArrayView,
     DICOMWSIReader,
     NGFFWSIReader,
     OmnyxJP2WSIReader,
     OpenSlideWSIReader,
     TIFFWSIReader,
     VirtualWSIReader,
-    WSIReader,
     is_ngff,
     is_zarr,
 )
 
 # -------------------------------------------------------------------------------------
 # Constants
 # -------------------------------------------------------------------------------------
@@ -179,15 +182,15 @@
     imgs = [wsi.read_bounds(bounds, level, "level") for level in levels_to_test]
     smallest_size = imgs[-1].shape[:2][::-1]
     resized = [cv2.resize(img, smallest_size) for img in imgs]
     # Some blurring applied to account for changes in sharpness arising
     # from interpolation when calculating the downsampled levels. This
     # adds some tolerance for the comparison.
     blurred = [cv2.GaussianBlur(img, (5, 5), cv2.BORDER_REFLECT) for img in resized]
-    as_float = [img.astype(np.float) for img in blurred]
+    as_float = [img.astype(np.float_) for img in blurred]
 
     # Pair-wise check resolutions for mean squared error
     for i, a in enumerate(as_float):
         for b in as_float[i + 1 :]:
             _, error, phase_diff = phase_cross_correlation(a, b, normalization=None)
             assert phase_diff < 0.125
             assert error < 0.125
@@ -401,36 +404,45 @@
     wsi = wsireader.OpenSlideWSIReader(sample_svs)
     with pytest.raises(ValueError, match="levels"):
         wsi.info.relative_level_scales(100, "level")
 
 
 def test_find_optimal_level_and_downsample_openslide_interpolation_warning(
     sample_ndpi,
+    caplog,
 ):
     """Test finding optimal level for mpp read with scale > 1.
 
     This tests the case where the scale is found to be > 1 and interpolation
     will be applied to the output. A UserWarning should be raised in this case.
 
     """
     wsi = wsireader.OpenSlideWSIReader(sample_ndpi)
-    with pytest.warns(UserWarning):
-        _, _ = wsi._find_optimal_level_and_downsample(0.1, "mpp")
+    _, _ = wsi._find_optimal_level_and_downsample(0.1, "mpp")
+    assert (
+        "Read: Scale > 1.This means that the desired resolution is higher"
+        in caplog.text
+    )
 
 
-def test_find_optimal_level_and_downsample_jp2_interpolation_warning(sample_jp2):
+def test_find_optimal_level_and_downsample_jp2_interpolation_warning(
+    sample_jp2, caplog
+):
     """Test finding optimal level for mpp read with scale > 1.
 
     This tests the case where the scale is found to be > 1 and interpolation
     will be applied to the output. A UserWarning should be raised in this case.
 
     """
     wsi = wsireader.OmnyxJP2WSIReader(sample_jp2)
-    with pytest.warns(UserWarning):
-        _, _ = wsi._find_optimal_level_and_downsample(0.1, "mpp")
+    _, _ = wsi._find_optimal_level_and_downsample(0.1, "mpp")
+    assert (
+        "Read: Scale > 1.This means that the desired resolution is higher"
+        in caplog.text
+    )
 
 
 def test_find_optimal_level_and_downsample_mpp(sample_ndpi):
     """Test finding optimal level for mpp read."""
     wsi = wsireader.OpenSlideWSIReader(sample_ndpi)
 
     mpps = [0.5, 10]
@@ -477,15 +489,15 @@
             level, "level"
         )
 
         assert read_level == level
         assert np.array_equal(post_read_scale_factor, [1.0, 1.0])
 
 
-def test_convert_resolution_units(sample_ndpi):
+def test_convert_resolution_units(sample_ndpi, caplog):
     """Test the resolution unit conversion code."""
     wsi = wsireader.WSIReader.open(sample_ndpi)
 
     # test for invalid input and output units
     with pytest.raises(ValueError, match=r".*Invalid input_unit.*"):
         wsi.convert_resolution_units(0, input_unit="invalid")
     with pytest.raises(ValueError, match=r".*Invalid output_unit.*"):
@@ -534,16 +546,16 @@
 
     # test when power and mpp are missing
     _info = deepcopy(org_info)
     _info.objective_power = None
     _info.mpp = None
     wsi._m_info = _info
     _ = wsi.convert_resolution_units(0, input_unit="baseline")
-    with pytest.warns(UserWarning, match=r".*output_unit is returned as None.*"):
-        _ = wsi.convert_resolution_units(0, input_unit="level", output_unit="mpp")
+    _ = wsi.convert_resolution_units(0, input_unit="level", output_unit="mpp")
+    assert "output_unit is returned as None." in caplog.text
 
 
 def test_find_read_rect_params_power(sample_ndpi):
     """Test finding read rect parameters for objective power."""
     wsi = wsireader.OpenSlideWSIReader(sample_ndpi)
 
     location = NDPI_TEST_TISSUE_LOCATION
@@ -933,15 +945,15 @@
     file_types = ("*.svs",)
     files_all = utils.misc.grab_files_from_dir(
         input_path=str(pathlib.Path(sample_svs).parent),
         file_types=file_types,
     )
     wsi = wsireader.OpenSlideWSIReader(files_all[0])
     wsi.save_tiles(
-        output_dir=str(tmp_path / ("test_wsireader_save_tiles")),
+        output_dir=str(tmp_path / "test_wsireader_save_tiles"),
         tile_objective_value=5,
         tile_read_size=(5000, 5000),
         verbose=True,
     )
     assert (
         tmp_path / "test_wsireader_save_tiles" / "CMU-1-Small-Region.svs" / "Output.csv"
     ).exists()
@@ -969,26 +981,25 @@
             ),
             tile_objective_value=3,
             tile_read_size=(5000, 5000),
             verbose=True,
         )
 
 
-def test_incompatible_level(sample_svs, tmp_path):
+def test_incompatible_level(sample_svs, tmp_path, caplog):
     """Test for incompatible objective value."""
     wsi = wsireader.OpenSlideWSIReader(sample_svs)
-    with pytest.warns(UserWarning):
-        wsi.save_tiles(
-            output_dir=str(
-                pathlib.Path(tmp_path).joinpath("test_wsireader_save_tiles2")
-            ),
-            tile_objective_value=1,
-            tile_read_size=(500, 500),
-            verbose=True,
-        )
+    wsi.save_tiles(
+        output_dir=str(pathlib.Path(tmp_path).joinpath("test_wsireader_save_tiles2")),
+        tile_objective_value=1,
+        tile_read_size=(500, 500),
+        verbose=True,
+    )
+
+    assert "Reading at tile_objective_value 1 not allowed" in caplog.text
 
 
 def test_wsireader_jp2_save_tiles(sample_jp2, tmp_path):
     """Test for save_tiles in wsireader as a python function."""
     tmp_path = pathlib.Path(tmp_path)
     wsi = wsireader.OmnyxJP2WSIReader(sample_jp2)
     wsi.save_tiles(
@@ -1004,54 +1015,55 @@
         tmp_path / "test_wsireader_jp2_save_tiles" / "test1.jp2" / "slide_thumbnail.jpg"
     ).exists()
     assert (
         tmp_path / "test_wsireader_jp2_save_tiles" / "test1.jp2" / "Tile_5_0_0.jpg"
     ).exists()
 
 
-def test_openslide_objective_power_from_mpp(sample_svs):
+def test_openslide_objective_power_from_mpp(sample_svs, caplog):
     """Test OpenSlideWSIReader approximation of objective power from mpp."""
     wsi = wsireader.OpenSlideWSIReader(sample_svs)
     wsi.openslide_wsi = DummyMutableOpenSlideObject(wsi.openslide_wsi)
     props = wsi.openslide_wsi._properties
 
     del props["openslide.objective-power"]  # skipcq
-    with pytest.warns(UserWarning, match=r"Objective power inferred"):
-        _ = wsi.info
+    _ = wsi.info
+    assert "Objective power inferred" in caplog.text
 
     del props["openslide.mpp-x"]  # skipcq
     del props["openslide.mpp-y"]  # skipcq
-    with pytest.warns(UserWarning, match=r"Unable to determine objective power"):
-        _ = wsi._info()
+    _ = wsi._info()
+    assert "Unable to determine objective power" in caplog.text
 
 
-def test_openslide_mpp_from_tiff_resolution(sample_svs):
+def test_openslide_mpp_from_tiff_resolution(sample_svs, caplog):
     """Test OpenSlideWSIReader mpp from TIFF resolution tags."""
     wsi = wsireader.OpenSlideWSIReader(sample_svs)
     wsi.openslide_wsi = DummyMutableOpenSlideObject(wsi.openslide_wsi)
     props = wsi.openslide_wsi._properties
 
     del props["openslide.mpp-x"]  # skipcq
     del props["openslide.mpp-y"]  # skipcq
     props["tiff.ResolutionUnit"] = "centimeter"
     props["tiff.XResolution"] = 1e4  # Pixels per cm
     props["tiff.YResolution"] = 1e4  # Pixels per cm
-    with pytest.warns(UserWarning, match=r"Falling back to TIFF resolution"):
-        _ = wsi.info
+    _ = wsi.info
+    assert "Falling back to TIFF resolution" in caplog.text
 
     assert np.array_equal(wsi.info.mpp, [1, 1])
 
 
-def test_virtual_wsi_reader(source_image):
+def test_virtual_wsi_reader(source_image, caplog):
     """Test VirtualWSIReader"""
     wsi = wsireader.VirtualWSIReader(pathlib.Path(source_image))
-    with pytest.warns(UserWarning, match=r"Unknown scale"):
-        _ = wsi._info()
-    with pytest.warns(UserWarning, match=r"Raw data is None"):
-        _ = wsi._info()
+    _ = wsi._info()
+    assert "Unknown scale" in caplog.text
+
+    _ = wsi._info()
+    assert "Raw data is None" in caplog.text
 
     assert wsi.img.shape == (256, 256, 3)
 
     img = wsi.read_rect(location=(0, 0), size=(100, 50))
     assert img.shape == (50, 100, 3)
 
     img = wsi.read_region(location=(0, 0), size=(100, 50), level=0)
@@ -1413,20 +1425,20 @@
     temp_file = f"{temp_dir}/sample.npy"
     np.save(temp_file, np.random.randint(1, 255, [5, 5, 5]))
     wsi_out = WSIReader.open(temp_file)
     assert isinstance(wsi_out, VirtualWSIReader)
     shutil.rmtree(temp_dir)
 
 
-def test_jp2_missing_cod(sample_jp2):
+def test_jp2_missing_cod(sample_jp2, caplog):
     """Test for warning if JP2 is missing COD segment."""
     wsi = wsireader.OmnyxJP2WSIReader(sample_jp2)
     wsi.glymur_wsi.codestream.segment = []
-    with pytest.warns(UserWarning, match="missing COD"):
-        _ = wsi.info
+    _ = wsi.info
+    assert "missing COD" in caplog.text
 
 
 def test_read_rect_at_resolution(sample_wsi_dict):
     """Test for read rect using location at requested."""
     mini_wsi2_svs = pathlib.Path(sample_wsi_dict["wsi1_8k_8k_svs"])
     mini_wsi2_jpg = pathlib.Path(sample_wsi_dict["wsi1_8k_8k_jpg"])
     mini_wsi2_jp2 = pathlib.Path(sample_wsi_dict["wsi1_8k_8k_jp2"])
@@ -1754,40 +1766,42 @@
             '<Objective ID="Objective:0:0" NominalMagnification="20.0"/>', ""
         ),
     )
     with pytest.raises(KeyError, match="No matching Instrument"):
         _ = wsi._info()
 
 
-def test_tiffwsireader_ome_metadata_missing_one_mppy(sample_ome_tiff, monkeypatch):
+def test_tiffwsireader_ome_metadata_missing_one_mppy(
+    sample_ome_tiff, monkeypatch, caplog
+):
     """Test no exception raised for missing x/y mpp but warning given."""
     for dim in "XY":
         wsi = wsireader.TIFFWSIReader(sample_ome_tiff)
         monkeypatch.setattr(
             wsi.tiff.pages[0],
             "description",
             re.sub(f'PhysicalSize{dim}="[^"]*"', "", wsi.tiff.pages[0].description),
         )
-        with pytest.warns(UserWarning, match="Only one MPP"):
-            _ = wsi._info()
+        _ = wsi._info()
+        assert "Only one MPP" in caplog.text
 
 
 def test_arrayview_unsupported_axes():
     """Test unsupported axes in ArrayView."""
     array = zarr.ones((128, 128, 3))
     array_view = ArrayView(array=array, axes="FOO")
-    with pytest.raises(Exception, match="Unsupported axes"):
+    with pytest.raises(ValueError, match="Unsupported axes"):
         array_view[:64, :64, :]
 
 
 def test_arrayview_unsupported_axes_shape(sample_ome_tiff, monkeypatch):
     """Test accessing an unspported axes in TIFFWSIReader._shape_channels_last."""
     wsi = wsireader.TIFFWSIReader(sample_ome_tiff)
     monkeypatch.setattr(wsi, "_axes", "FOO")
-    with pytest.raises(Exception, match="Unsupported axes"):
+    with pytest.raises(ValueError, match="Unsupported axes"):
         _ = wsi._info()
 
 
 def test_arrayview_incomplete_index():
     """Test reading from ArrayView without specifying all axes slices."""
     array = zarr.array(np.random.rand(128, 128, 3))
     array_view = ArrayView(array=array, axes="YXS")
@@ -1841,15 +1855,16 @@
     with pytest.raises(TypeError, match="power"):
         _ = wsireader.OpenSlideWSIReader(sample_svs, power=(42,))
 
 
 def test_tiled_tiff_openslide(remote_sample):
     """Test reading a tiled TIFF file with OpenSlide."""
     sample_path = remote_sample("tiled-tiff-1-small-jpeg")
-    wsi = wsireader.WSIReader.open(sample_path)
+    # Test with top-level import
+    wsi = WSIReader.open(sample_path)
     assert isinstance(wsi, wsireader.OpenSlideWSIReader)
 
 
 def test_tiled_tiff_tifffile(remote_sample):
     """Test fallback to tifffile for files which openslide cannot read.
 
     E.G. tiled tiffs with JPEG XL compression.
@@ -1975,36 +1990,42 @@
     wsi_reader = WSIReader.open(remote_sample("svs-1-small"))
     reader = AnnotationStoreReader(tmp_path / "store.db", wsi_reader.info)
     # shouldn't try to color by type if not present
     assert reader.renderer.score_prop is None
 
 
 def test_store_reader_info_from_base(tmp_path, remote_sample):
-    """Test that AnnotationStoreReader will correctly get metadata
-    from a provided base_wsi if the store has no wsi metadata."""
+    """Test AnnotationStoreReader with no wsi metadata.
+
+    Test that AnnotationStoreReader will correctly get metadata
+    from a provided base_wsi if the store has no wsi metadata.
+
+    """
     SQLiteStore(tmp_path / "store.db")
     wsi_reader = WSIReader.open(remote_sample("svs-1-small"))
     store_reader = AnnotationStoreReader(tmp_path / "store.db", base_wsi=wsi_reader)
     # the store reader should have the same metadata as the base wsi
     assert store_reader.info.mpp[0] == wsi_reader.info.mpp[0]
 
 
-def test_ngff_zattrs_non_micrometer_scale_mpp(tmp_path):
+def test_ngff_zattrs_non_micrometer_scale_mpp(tmp_path, caplog):
     """Test that mpp is None if scale is not in micrometers."""
     sample = _fetch_remote_sample("ngff-1")
     # Create a copy of the sample with a non-micrometer scale
     sample_copy = tmp_path / "ngff-1"
     shutil.copytree(sample, sample_copy)
     with open(sample_copy / ".zattrs", "r") as fh:
         zattrs = json.load(fh)
     zattrs["multiscales"][0]["axes"][0]["unit"] = "foo"
     with open(sample_copy / ".zattrs", "w") as fh:
         json.dump(zattrs, fh, indent=2)
-    with pytest.warns(UserWarning, match="micrometer"):
-        wsi = wsireader.NGFFWSIReader(sample_copy)
+
+    wsi = wsireader.NGFFWSIReader(sample_copy)
+    assert "micrometer" in caplog.text
+
     assert wsi.info.mpp is None
 
 
 def test_ngff_zattrs_missing_axes_mpp(tmp_path):
     """Test that mpp is None if axes are missing."""
     sample = _fetch_remote_sample("ngff-1")
     # Create a copy of the sample with no axes
@@ -2030,31 +2051,200 @@
     zattrs["multiscales"][0]["datasets"] = []
     with open(sample_copy / ".zattrs", "w") as fh:
         json.dump(zattrs, fh, indent=2)
     wsi = wsireader.NGFFWSIReader(sample_copy)
     assert wsi.info.mpp is None
 
 
-def test_nff_no_scale_transforms_mpp(tmp_path):
+def test_ngff_no_scale_transforms_mpp(tmp_path):
     """Test that mpp is None if no scale transforms are present."""
     sample = _fetch_remote_sample("ngff-1")
     # Create a copy of the sample with no axes
-    sample_copy = tmp_path / "ngff-1"
+    sample_copy = tmp_path / "ngff-1.zarr"
     shutil.copytree(sample, sample_copy)
     with open(sample_copy / ".zattrs", "r") as fh:
         zattrs = json.load(fh)
     for i, _ in enumerate(zattrs["multiscales"][0]["datasets"]):
         datasets = zattrs["multiscales"][0]["datasets"][i]
         datasets["coordinateTransformations"][0]["type"] = "identity"
     with open(sample_copy / ".zattrs", "w") as fh:
         json.dump(zattrs, fh, indent=2)
     wsi = wsireader.NGFFWSIReader(sample_copy)
     assert wsi.info.mpp is None
 
 
+def test_ngff_missing_omero_version(tmp_path):
+    """Test that the reader can handle missing omero version."""
+    sample = _fetch_remote_sample("ngff-1")
+    # Create a copy of the sample
+    sample_copy = tmp_path / "ngff-1.zarr"
+    shutil.copytree(sample, sample_copy)
+    with open(sample_copy / ".zattrs", "r") as fh:
+        zattrs = json.load(fh)
+    # Remove the omero version
+    del zattrs["omero"]["version"]
+    with open(sample_copy / ".zattrs", "w") as fh:
+        json.dump(zattrs, fh, indent=2)
+    wsireader.WSIReader.open(sample_copy)
+
+
+def test_ngff_missing_multiscales_returns_false(tmp_path):
+    """Test that missing multiscales key returns False for is_ngff."""
+    sample = _fetch_remote_sample("ngff-1")
+    # Create a copy of the sample
+    sample_copy = tmp_path / "ngff-1.zarr"
+    shutil.copytree(sample, sample_copy)
+    with open(sample_copy / ".zattrs", "r") as fh:
+        zattrs = json.load(fh)
+    # Remove the multiscales key
+    del zattrs["multiscales"]
+    with open(sample_copy / ".zattrs", "w") as fh:
+        json.dump(zattrs, fh, indent=2)
+    assert not wsireader.is_ngff(sample_copy)
+
+
+def test_ngff_wrong_format_metadata(tmp_path, caplog):
+    """Test that is_ngff is False and logs a warning if metadata is wrong."""
+    sample = _fetch_remote_sample("ngff-1")
+    # Create a copy of the sample
+    sample_copy = tmp_path / "ngff-1.zarr"
+    shutil.copytree(sample, sample_copy)
+    with open(sample_copy / ".zattrs", "r") as fh:
+        zattrs = json.load(fh)
+    # Change the format to something else
+    zattrs["multiscales"] = "foo"
+    with open(sample_copy / ".zattrs", "w") as fh:
+        json.dump(zattrs, fh, indent=2)
+    with caplog.at_level(logging.WARNING):
+        assert not wsireader.is_ngff(sample_copy)
+    assert "must be present and of the correct type" in caplog.text
+
+
+def test_ngff_omero_below_min_version(tmp_path):
+    """Test for FileNotSupported when omero version is below minimum."""
+    sample = _fetch_remote_sample("ngff-1")
+    # Create a copy of the sample
+    sample_copy = tmp_path / "ngff-1.zarr"
+    shutil.copytree(sample, sample_copy)
+    with open(sample_copy / ".zattrs", "r") as fh:
+        zattrs = json.load(fh)
+    # Change the format to something else
+    zattrs["omero"]["version"] = "0.0"
+    with open(sample_copy / ".zattrs", "w") as fh:
+        json.dump(zattrs, fh, indent=2)
+    with pytest.raises(FileNotSupported):
+        wsireader.WSIReader.open(sample_copy)
+
+
+def test_ngff_omero_above_max_version(tmp_path, caplog):
+    """Test for FileNotSupported when omero version is above maximum."""
+    sample = _fetch_remote_sample("ngff-1")
+    # Create a copy of the sample
+    sample_copy = tmp_path / "ngff-1.zarr"
+    shutil.copytree(sample, sample_copy)
+    with open(sample_copy / ".zattrs", "r") as fh:
+        zattrs = json.load(fh)
+    # Change the format to something else
+    zattrs["omero"]["version"] = "10.0"
+    with open(sample_copy / ".zattrs", "w") as fh:
+        json.dump(zattrs, fh, indent=2)
+    # Check that the warning is logged
+    with caplog.at_level(logging.WARNING):
+        wsireader.WSIReader.open(sample_copy)
+    assert "maximum supported version" in caplog.text
+
+
+def test_ngff_multiscales_below_min_version(tmp_path):
+    """Test for FileNotSupported when multiscales version is below minimum."""
+    sample = _fetch_remote_sample("ngff-1")
+    # Create a copy of the sample
+    sample_copy = tmp_path / "ngff-1.zarr"
+    shutil.copytree(sample, sample_copy)
+    with open(sample_copy / ".zattrs", "r") as fh:
+        zattrs = json.load(fh)
+    # Change the format to something else
+    zattrs["multiscales"][0]["version"] = "0.0"
+    with open(sample_copy / ".zattrs", "w") as fh:
+        json.dump(zattrs, fh, indent=2)
+    with pytest.raises(FileNotSupported):
+        wsireader.WSIReader.open(sample_copy)
+
+
+def test_ngff_multiscales_above_max_version(tmp_path, caplog):
+    """Test for FileNotSupported when multiscales version is above maximum."""
+    sample = _fetch_remote_sample("ngff-1")
+    # Create a copy of the sample
+    sample_copy = tmp_path / "ngff-1.zarr"
+    shutil.copytree(sample, sample_copy)
+    with open(sample_copy / ".zattrs", "r") as fh:
+        zattrs = json.load(fh)
+    # Change the format to something else
+    zattrs["multiscales"][0]["version"] = "10.0"
+    with open(sample_copy / ".zattrs", "w") as fh:
+        json.dump(zattrs, fh, indent=2)
+    # Check that the warning is logged
+    with caplog.at_level(logging.WARNING):
+        wsireader.WSIReader.open(sample_copy)
+    assert "maximum supported version" in caplog.text
+
+
+def test_ngff_non_numeric_version(tmp_path, monkeypatch):
+    """Test that the reader can handle non-numeric omero versions."""
+    # Patch the is_ngff function to change the min/max version
+    if_ngff = wsireader.is_ngff  # noqa: F841
+    min_version = Version("0.4")
+    max_version = Version("0.5")
+
+    def patched_is_ngff(
+        path: Path,
+        min_version: Version = min_version,
+        max_version: Version = max_version,
+    ) -> bool:
+        """Patched is_ngff function with new min/max version."""
+        return is_ngff(path, min_version, max_version)
+
+    monkeypatch.setattr(wsireader, "is_ngff", patched_is_ngff)
+
+    sample = _fetch_remote_sample("ngff-1")
+    # Create a copy of the sample
+    sample_copy = tmp_path / "ngff-1.zarr"
+    shutil.copytree(sample, sample_copy)
+    with open(sample_copy / ".zattrs", "r") as fh:
+        zattrs = json.load(fh)
+    # Set the omero version to a non-numeric string
+    zattrs["omero"]["version"] = "0.5-dev"
+    with open(sample_copy / ".zattrs", "w") as fh:
+        json.dump(zattrs, fh, indent=2)
+    wsireader.WSIReader.open(sample_copy)
+
+
+def test_ngff_inconsistent_multiscales_versions(tmp_path, caplog):
+    """Test that the reader logs a warning inconsistent multiscales versions."""
+    sample = _fetch_remote_sample("ngff-1")
+    # Create a copy of the sample
+    sample_copy = tmp_path / "ngff-1.zarr"
+    shutil.copytree(sample, sample_copy)
+    with open(sample_copy / ".zattrs", "r") as fh:
+        zattrs = json.load(fh)
+    # Set the versions to be inconsistent
+    multiscales = zattrs["multiscales"]
+    # Needs at least 2 multiscales to be inconsistent
+    if len(multiscales) < 2:
+        multiscales.append(copy.deepcopy(multiscales[0]))
+    for i, _ in enumerate(multiscales):
+        multiscales[i]["version"] = f"0.{i}-dev"
+    zattrs["omero"]["multiscales"] = multiscales
+    with open(sample_copy / ".zattrs", "w") as fh:
+        json.dump(zattrs, fh, indent=2)
+    # Capture logger output to check for warning
+    with caplog.at_level(logging.WARNING), pytest.raises(FileNotSupported):
+        wsireader.WSIReader.open(sample_copy)
+    assert "multiple versions" in caplog.text
+
+
 class TestReader:
     scenarios = [
         (
             "AnnotationReaderOverlaid",
             {
                 "reader_class": AnnotationStoreReader,
                 "sample_key": "annotation_store_svs_1",
@@ -2179,15 +2369,15 @@
         ]
         smallest_size = imgs[-1].shape[:2][::-1]
         resized = [imresize(img, output_size=smallest_size) for img in imgs]
         # Some blurring applied to account for changes in sharpness arising
         # from interpolation when calculating the downsampled levels. This
         # adds some tolerance for the comparison.
         blurred = [cv2.GaussianBlur(img, (5, 5), cv2.BORDER_REFLECT) for img in resized]
-        as_float = [img.astype(np.float) for img in blurred]
+        as_float = [img.astype(np.float_) for img in blurred]
 
         # Pair-wise check resolutions for mean squared error
         for i, a in enumerate(as_float):
             for b in as_float[i + 1 :]:
                 _, error, phase_diff = phase_cross_correlation(a, b, normalization=None)
                 assert phase_diff < 0.125
                 assert error < 0.125
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/__init__.py` & `tiatoolbox-1.4.0/tiatoolbox/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,41 +6,58 @@
 from pathlib import Path
 
 import pkg_resources
 import yaml
 
 __author__ = """TIA Lab"""
 __email__ = "tialab@dcs.warwick.ac.uk"
-__version__ = "1.3.3"
+__version__ = "1.4.0"
 
 # This will set the tiatoolbox external data
 # default to be the user home folder, should work on both Window and Unix/Linux
 # C:\Users\USER\.tiatoolbox
 # /home/USER/.tiatoolbox
 
 # Initialize internal logging facilities, such that models etc.
 # can have reporting mechanism, may need to change protocol
 import logging
 
 # We only create a logger if root has no handler to prevent overwriting use existing
 # logging
 logging.captureWarnings(True)
 if not logging.getLogger().hasHandlers():
-    handler = logging.StreamHandler()
     formatter = logging.Formatter(
         "|%(asctime)s.%(msecs)03d| [%(levelname)s] %(message)s",
         datefmt="%Y-%m-%d|%H:%M:%S",
     )
-    handler.setFormatter(formatter)
+    stdout_handler = logging.StreamHandler(sys.stdout)
+    stdout_handler.setFormatter(formatter)
+    stdout_handler.addFilter(lambda record: record.levelno <= logging.INFO)
+
+    stderr_handler = logging.StreamHandler()
+    stderr_handler.setFormatter(formatter)
+    stderr_handler.setLevel(logging.WARNING)
+
     logger = logging.getLogger()  # get root logger
     logger.setLevel(logging.INFO)
-    logger.addHandler(handler)
+    logger.addHandler(stdout_handler)
+    logger.addHandler(stderr_handler)
 else:
     logger = logging.getLogger()
 
+
+class DuplicateFilter(logging.Filter):
+    def filter(self, record):
+        current_log = (record.module, record.levelno, record.msg)
+        if current_log != getattr(self, "last_log", None):
+            self.last_log = current_log
+            return True
+        return False
+
+
 # runtime context parameters
 rcParam = {"TIATOOLBOX_HOME": os.path.join(os.path.expanduser("~"), ".tiatoolbox")}
 
 # Load a dictionary of sample files data (names and urls)
 PRETRAINED_FILES_REGISTRY_PATH = pkg_resources.resource_filename(
     "tiatoolbox", "data/pretrained_model.yaml"
 )
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/annotation/dsl.py` & `tiatoolbox-1.4.0/tiatoolbox/annotation/dsl.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         }
 
     def __str__(self) -> str:
         lhs = self.lhs
         rhs = self.rhs
         if isinstance(rhs, str):
             # is this ok? fixes categorical where predicate
-            rhs = f'"{rhs}"'
+            rhs = f'"{rhs}"'  # noqa: B028
         if lhs and self.op:
             return self.formatters[self.op](lhs, rhs)
         raise ValueError("Invalid SQLTriplet.")
 
 
 class SQLJSONDictionary(SQLExpression):
     """Representation of an SQL expression to access JSON properties."""
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/annotation/storage.py` & `tiatoolbox-1.4.0/tiatoolbox/annotation/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 import json
 import os
 import pickle
 import sqlite3
 import sys
 import tempfile
 import uuid
-import warnings
 import zlib
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from collections.abc import MutableMapping
 from dataclasses import dataclass, field
 from functools import lru_cache
 from numbers import Number
@@ -62,15 +61,15 @@
 from shapely import speedups, wkb, wkt
 from shapely.affinity import scale, translate
 from shapely.geometry import LineString, Point, Polygon
 from shapely.geometry import mapping as geometry2feature
 from shapely.geometry import shape as feature2geometry
 
 import tiatoolbox
-from tiatoolbox import logger
+from tiatoolbox import DuplicateFilter, logger
 from tiatoolbox.annotation.dsl import (
     PY_GLOBALS,
     SQL_GLOBALS,
     json_contains,
     json_list_sum,
     py_regexp,
 )
@@ -144,18 +143,30 @@
         Returns:
             str:
                 A GeoJSON representation of this annotation.
 
         """
         return json.dumps(self.to_feature())
 
+    def __repr__(self) -> str:
+        return f"Annotation({self.geometry}, {self.properties})"
+
 
 class AnnotationStore(ABC, MutableMapping):
     """Annotation store abstract base class."""
 
+    def __new__(cls, *args, **kwargs):
+        """Return an instance of a subclass of AnnotationStore."""
+        if cls is AnnotationStore:
+            raise TypeError(
+                "AnnotationStore is an abstract class and cannot be instantiated."
+                " Use a subclass such as DictionaryStore or SQLiteStore instead."
+            )
+        return super().__new__(cls)
+
     @staticmethod
     def _is_right_angle(a, b, c) -> bool:
         """Returns True if three points make a right angle.
 
         Used for optimising queries.
 
         This function will have positional only arguments when support
@@ -283,15 +294,19 @@
         "covered_by",
         "crosses",
         "disjoint",
         "intersects",
         "overlaps",
         "touches",
         "within",
-        "bbox_intersects",  # Special non-shapely case, bounding-boxes intersect
+        # Special non-shapely case, bounding-boxes intersect.
+        "bbox_intersects",
+        # Special non-shapely case, query centroid within k of
+        # annotation bounds center.
+        "centers_within_k",
     ]
 
     @classmethod  # noqa: A003
     @abstractmethod
     def open(cls, fp: Union[Path, str, IO]) -> "AnnotationStore":  # noqa: A003
         """Load a store object from a path or file-like object.
 
@@ -607,14 +622,15 @@
         return bool(predicate(properties))
 
     def query(
         self,
         geometry: Optional[QueryGeometry] = None,
         where: Optional[Predicate] = None,
         geometry_predicate: str = "intersects",
+        distance: float = 0,
     ) -> Dict[str, Annotation]:
         """Query the store for annotations.
 
         Args:
             geometry (Geometry or Iterable):
                 Geometry to use when querying. This can be a bounds
                 (iterable of length 4) or a Shapely geometry (e.g.
@@ -649,14 +665,17 @@
                 A string defining which binary geometry predicate to
                 use when comparing the query geometry and a geometry in
                 the store. Only annotations for which this binary
                 predicate is true will be returned. Defaults to
                 "intersects". For more information see the `shapely
                 documentation on binary predicates <https://shapely.
                 readthedocs.io/en/stable/manual.html#binary-predicates>`_.
+            distance (float):
+                Distance used when performing a distance based query.
+                E.g. "centers_within_k" geometry predicate.
 
             Returns:
                 list:
                     A list of Annotation objects.
 
         """
         if all(x is None for x in (geometry, where)):
@@ -665,14 +684,35 @@
             raise ValueError(
                 "Invalid geometry predicate."
                 f"Allowed values are: {', '.join(self._geometry_predicate_names)}."
             )
         query_geometry = geometry
         if isinstance(query_geometry, Iterable):
             query_geometry = Polygon.from_bounds(*query_geometry)
+        if geometry_predicate == "centers_within_k":
+            query_point = Polygon.from_bounds(*query_geometry.bounds).centroid
+
+        def bbox_intersects(
+            annotation_geometry: Geometry, query_geometry: Geometry
+        ) -> bool:
+            """True if bounding box of the annotation intersects the query geometry."""
+            return Polygon.from_bounds(*query_geometry.bounds).intersects(
+                Polygon.from_bounds(*annotation_geometry.bounds)
+            )
+
+        def centers_within_k(
+            annotation_geometry: Geometry, query_point: Point, distance: float
+        ) -> bool:
+            """True if centre of annotation within k of query geometry center.
+
+            Here the "center" is the centroid of the bounds.
+
+            """
+            ann_centre = Polygon.from_bounds(*annotation_geometry.bounds).centroid
+            return query_point.dwithin(ann_centre, distance)
 
         def filter_function(annotation: Annotation) -> bool:
             """Filter function for querying annotations.
 
             Args:
                 annotation (Annotation):
                     The annotation to filter.
@@ -681,16 +721,34 @@
                 bool:
                     True if the annotation should be included in the
                     query result.
 
             """
             return (  # Geometry is None or the geometry predicate matches
                 query_geometry is None
-                or self._geometry_predicate(
-                    geometry_predicate, query_geometry, annotation.geometry
+                or any(
+                    [
+                        (
+                            geometry_predicate == "bbox_intersects"
+                            and bbox_intersects(annotation.geometry, query_geometry)
+                        ),
+                        (
+                            geometry_predicate == "centers_within_k"
+                            and centers_within_k(
+                                annotation.geometry, query_point, distance
+                            )
+                        ),
+                        (
+                            geometry_predicate
+                            not in ("bbox_intersects", "centers_within_k")
+                            and self._geometry_predicate(
+                                geometry_predicate, query_geometry, annotation.geometry
+                            )
+                        ),
+                    ]
                 )
             ) and self._eval_where(where, annotation.properties)
 
         return {
             key: annotation
             for key, annotation in self.items()
             if filter_function(annotation)
@@ -824,18 +882,18 @@
                 the string statement.
 
             Returns:
                 list:
                     A list of bounding boxes for each Annotation.
 
             Example:
-                >>> from tiatoolbox.annotation.storage import AnnotationStore
+                >>> from tiatoolbox.annotation.storage import DictionaryStore
                 >>> from shapely.geometry import Polygon
-                >>> store = AnnotationStore()
-                >>> store.add(
+                >>> store = DictionaryStore()
+                >>> store.append(
                 ...     Annotation(
                 ...         geometry=Polygon.from_bounds(0, 0, 1, 1),
                 ...         properties={"class": 42},
                 ...     ),
                 ...     key="foo",
                 ... )
                 >>> store.bquery(where="props['class'] == 42")
@@ -846,15 +904,16 @@
         query_geometry = geometry
         if isinstance(query_geometry, Iterable):
             query_geometry = Polygon.from_bounds(*query_geometry)
         return {
             key: annotation.geometry.bounds
             for key, annotation in self.items()
             if (
-                Polygon.from_bounds(*annotation.geometry.bounds).intersects(
+                query_geometry is None
+                or Polygon.from_bounds(*annotation.geometry.bounds).intersects(
                     Polygon.from_bounds(*query_geometry.bounds)
                 )
                 and self._eval_where(where, annotation.properties)
             )
         }
 
     def pquery(
@@ -911,37 +970,37 @@
             squeeze (bool):
                 If True, when querying for a single value with
                 `unique=True`, the result will be a single set instead
                 of a list of sets.
 
         Examples:
 
-            >>> from tiatoolbox.annotation.storage import AnnotationStore
+            >>> from tiatoolbox.annotation.storage import DictionaryStore
             >>> from shapely.geometry import Point
-            >>> store = AnnotationStore()
+            >>> store = DictionaryStore()
             >>> annotation =  Annotation(
             ...     geometry=Point(0, 0),
             ...     properties={"class": 42},
             ... )
-            >>> store.add(annotation, "foo")
+            >>> store.append(annotation, "foo")
             >>> store.pquery("*", unique=False)
             ... {'foo': {'class': 42}}
 
-            >>> from tiatoolbox.annotation.storage import AnnotationStore
+            >>> from tiatoolbox.annotation.storage import DictionaryStore
             >>> from shapely.geometry import Point
-            >>> store = AnnotationStore()
+            >>> store = DictionaryStore()
             >>> annotation =  Annotation(
             ...     geometry=Point(0, 0),
             ...     properties={"class": 42},
             ... )
-            >>> store.add(annotation, "foo")
+            >>> store.append(annotation, "foo")
             >>> store.pquery("props['class']")
             ... {42}
             >>> annotation =  Annotation(Point(1, 1), {"class": 123})
-            >>> store.add(annotation, "foo")
+            >>> store.append(annotation, "foo")
             >>> store.pquery("props['class']")
             ... {42, 123}
 
         """  # noqa
         if where is not None and type(select) is not type(where):
             raise TypeError("select and where must be of the same type")
         if not isinstance(select, (str, bytes)) and not callable(select):
@@ -993,14 +1052,204 @@
 
             return select(annotation.properties)
 
         return self._handle_pquery_results(
             select, unique, squeeze, items, select_values
         )
 
+    def nquery(
+        self,
+        geometry: Optional[Geometry] = None,
+        where: Optional[Predicate] = None,
+        n_where: Optional[Predicate] = None,
+        distance: float = 5.0,
+        geometry_predicate: str = "intersects",
+        mode: str = "poly-poly",
+    ) -> Dict[str, Dict[str, Annotation]]:
+        """Query for annotations within a distance of another annotation.
+
+        Args:
+            geometry (Geometry):
+                A geometry to use to query for the initial set of
+                annotations to perform a neighbourhood search around. If
+                None, all annotations in the store are considered.
+                Defaults to None.
+            where (str or bytes or Callable):
+                A statement which should evaluate to a boolean value.
+                Only annotations for which this predicate is true will be
+                returned. Defaults to None (assume always true). This may
+                be a string, callable, or pickled function as bytes.
+                Callables are called to filter each result returned the
+                annotation store backend in python before being returned
+                to the user. A pickle object is, where possible, hooked
+                into the backend as a user defined function to filter
+                results during the backend query. Strings are expected to
+                be in a domain specific language and are converted to SQL
+                on a best-effort basis. For supported operators of the DSL
+                see :mod:`tiatoolbox.annotation.dsl`. E.g. a simple python
+                expression `props["class"] == 42` will be converted to a
+                valid SQLite predicate when using `SQLiteStore` and
+                inserted into the SQL query. This should be faster than
+                filtering in python after or during the query. It is
+                important to note that untrusted user input should never
+                be accepted to this argument as arbitrary code can be
+                run via pickle or the parsing of the string statement.
+            n_where (str or bytes or Callable):
+                Predicate to filter the nearest annotations by. Defaults
+                to None (assume always true). See `where` for more
+                details.
+            distance (float):
+                The distance to search for annotations within. Defaults to
+                5.0.
+            geometry_predicate (str):
+                The predicate to use when comparing geometries. Defaults
+                to "intersects". Other options include "within" and
+                "contains". Ignored if `mode` is "boxpoint-boxpoint" or
+                "box-box".
+            mode (tuple[str, str] or str):
+                The method to use for determining distance during the
+                query. Defaults to "box-box". This may significantly
+                change performance depending on the backend. Possible
+                options are:
+                  - "poly-poly": Polygon boundary to polygon boundary.
+                  - "boxpoint-boxpoint": Bounding box centre point to
+                    bounding box centre point.
+                  - "box-box": Bounding box to bounding box.
+                May be specified as a dash separated string or a tuple
+                of two strings. The first string is the mode for the
+                query geometry and the second string is the mode for
+                the nearest annotation geometry.
+
+        Returns:
+            Dict[str, Dict[str, Annotation]]:
+                A dictionary mapping annotation keys to another
+                dictionary which represents an annotation key and all
+                annotations within `distance` of it.
+
+        The `mode` argument is used to determine how to calculate the
+        distance between annotations. The default mode is "box-box".
+
+        The "box-box" mode uses the bounding boxes of stored annotations
+        and the query geometry when determining if annotations are
+        within the neighbourhood.
+
+        .. figure:: ../images/nquery-box-box.png
+            :width: 512
+            :alt: "box-box" mode
+
+        The "poly-poly" performs full polygon-polygon intersection with
+        the polygon boundary of stored annotations and the query
+        geometry to determine if annotations are within the
+        neighbourhood.
+
+        .. figure:: ../images/nquery-poly-poly.png
+            :width: 512
+            :alt: "poly-poly" mode
+
+
+        The "boxpoint-boxpoint" mode uses the centre point of the
+        bounding box of stored annotations and the query geometry when
+        determining if annotations are within the neighbourhood.
+
+        .. figure:: ../images/nquery-boxpoint-boxpoint.png
+            :width: 512
+            :alt: "boxpoint-boxpoint" mode
+
+
+        Examples:
+            Example bounding box query with one neighbour within a
+            distance of 2.0.
+
+            >>> from shapely.geometry import Point, Polyon
+            >>> from tiatoolbox.annotation.storage import Annotation, SQLiteStore
+            >>> store = SQLiteStore()
+            >>> annotation = Annotation(Point(0, 0), {"class": 42})
+            >>> store.append(annotation, "foo")
+            >>> neighbour = Annotation(Point(1, 1), {"class": 123})
+            >>> store.add(neighbour, "bar")
+            >>> store.nquery((-.5, -.5, .5, .5), distance=2.0)
+            {
+              "foo": {
+                Annotation(POINT (0 0), {'class': 42}): {
+                  "bar": Annotation(POINT (1 1), {'class': 123}),
+                }
+              },
+            }
+
+            Example bounding box query with no neighbours within a
+            distance of 1.0.
+
+            >>> from shapely.geometry import Point
+            >>> from tiatoolbox.annotation.storage import Annotation, SQLiteStore
+            >>> store = SQLiteStore()
+            >>> annotation = Annotation(Point(0, 0), {"class": 42})
+            >>> store.add(annotation, "foo")
+            >>> store.nquery((-.5, -.5, .5, .5), distance=1.0)
+            {"foo": {Annotation(POINT (0 0), {'class': 42}): {}}}
+
+            Example of querying for TILs - lympocytes within 3 units
+            of tumour cells.
+
+            >>> from tiatoolbox.annotation.storage import SQLiteStore
+            >>> store = SQLiteStore("hovernet-pannuke-output.db")
+            >>> tils = store.nquery(
+            ...     where="props['class'] == 1",   # Tumour cells
+            ...     n_where="props['class'] == 0",  # Lymphocytes
+            ...     distance=32.0,  # n_where within 32 units of where
+            ...     mode="point-point",  # Use point to point distance
+            ... )
+
+        """
+        # This is a naive generic implementation which can be overridden
+        # by back ends which can do this more efficiently.
+        if not isinstance(mode, (str, tuple)):
+            raise TypeError("mode must be a string or tuple of strings")
+        if isinstance(mode, str):
+            mode = tuple(mode.split("-"))
+        if mode not in (("box", "box"), ("boxpoint", "boxpoint"), ("poly", "poly")):
+            raise ValueError(
+                "mode must be one of 'box-box', 'boxpoint-boxpoint', or 'poly-poly'"
+            )
+        from_mode, _ = mode
+
+        # Initial selection of annotations to query around
+        selection = self.query(
+            geometry=geometry,
+            where=where,
+        )
+
+        # Query for others within the distance of initial selection
+        result = {}
+        for key, ann in selection.items():
+            geometry = ann.geometry
+            if from_mode == "box":
+                geometry_predicate = "bbox_intersects"
+                min_x, min_y, max_x, max_y = ann.geometry.bounds
+                geometry = Polygon.from_bounds(
+                    min_x - distance,
+                    min_y - distance,
+                    max_x + distance,
+                    max_y + distance,
+                )
+            elif from_mode == "boxpoint":
+                geometry_predicate = "centers_within_k"
+            elif from_mode == "poly":  # pragma: no branch
+                geometry = ann.geometry
+                geometry = geometry.buffer(distance)
+            subquery_result = self.query(
+                geometry=geometry,
+                where=n_where,
+                geometry_predicate=geometry_predicate,
+                distance=distance,
+            )
+            if subquery_result:
+                result[key] = subquery_result
+
+        return result
+
     @staticmethod
     def _handle_pquery_results(
         select: Select,
         unique: bool,
         squeeze: bool,
         items: Generator[Tuple[str, Properties], None, None],
         get_values: Callable[
@@ -1487,23 +1736,25 @@
         super().__init__()
         # Check that JSON and RTree support is enabled
         compile_options = self.compile_options()
         if sqlite3.sqlite_version_info >= (3, 38, 0):
             if not all(
                 ["OMIT_JSON" not in compile_options, "ENABLE_RTREE" in compile_options]
             ):
-                raise Exception(
+                raise EnvironmentError(
                     """RTREE sqlite3 compile option is required, and
                     JSON must not be disabled with OMIT_JSON compile option"""
                 )
         else:
             if not all(
                 ["ENABLE_JSON1" in compile_options, "ENABLE_RTREE" in compile_options]
             ):
-                raise Exception("RTREE and JSON1 sqlite3 compile options are required.")
+                raise EnvironmentError(
+                    "RTREE and JSON1 sqlite3 compile options are required."
+                )
 
         # Check that math functions are enabled
         if "ENABLE_MATH_FUNCTIONS" not in compile_options:
             logger.warning(
                 "SQLite math functions are not enabled."
                 " This may cause problems with some queries."
                 " For example, floor division (//) will not work."
@@ -1534,27 +1785,29 @@
             self.metadata["compression_level"] = compression_level
 
         # store locally as constantly fetching from db in (de)serialization is slow
         self.compression = self.metadata["compression"]
         self.compression_level = self.metadata["compression_level"]
 
         # Register predicate functions as custom SQLite functions
-        def wkb_predicate(name: str, wkb_a: bytes, b: bytes, cx: int, cy: int) -> bool:
+        def wkb_predicate(
+            name: str, wkb_a: bytes, b: bytes, cx: float, cy: float
+        ) -> bool:
             """Wrapper function to allow WKB as inputs to binary predicates."""
             a = wkb.loads(wkb_a)
             b = self._unpack_geometry(b, cx, cy)
             return self._geometry_predicate(name, a, b)
 
         def pickle_expression(pickle_bytes: bytes, properties: str) -> bool:
             """Function to load and execute pickle bytes with a "properties" dict."""
             fn = pickle.loads(pickle_bytes)  # skipcq: BAN-B301
             properties = json.loads(properties)
             return fn(properties)
 
-        def get_area(wkb_bytes: bytes, cx: int, cy: int) -> float:
+        def get_area(wkb_bytes: bytes, cx: float, cy: float) -> float:
             """Function to get the area of a geometry."""
             return self._unpack_geometry(
                 wkb_bytes,
                 cx,
                 cy,
             ).area
 
@@ -1598,32 +1851,32 @@
         if exists:
             self.table_columns = self._get_table_columns()
             return
 
         # Create tables for geometry and RTree index
         self.con.execute(
             """
-            CREATE VIRTUAL TABLE rtree USING rtree_i32(
+            CREATE VIRTUAL TABLE rtree USING rtree(
                 id,                      -- Integer primary key
                 min_x, max_x,            -- 1st dimension min, max
                 min_y, max_y             -- 2nd dimension min, max
             )
             """
         )
         self.con.execute(
             """
             CREATE TABLE annotations(
                 id INTEGER PRIMARY KEY,  -- Integer primary key
                 key TEXT UNIQUE,         -- Unique identifier (UUID)
                 objtype TEXT,            -- Object type
-                cx INTEGER NOT NULL,     -- X of centroid/representative point
-                cy INTEGER NOT NULL,     -- Y of centroid/representative point
+                cx FLOAT NOT NULL,       -- X of centroid/representative point
+                cy FLOAT NOT NULL,       -- Y of centroid/representative point
                 geometry BLOB,           -- Detailed geometry
                 properties TEXT,         -- JSON properties
-                area INTEGER NOT NULL    -- Area (for ordering)
+                area FLOAT NOT NULL      -- Area (for ordering)
             )
 
             """
         )
         if self.auto_commit:
             self.con.commit()
         self.table_columns = self._get_table_columns()
@@ -1648,28 +1901,30 @@
         data = geometry.wkb
         if self.compression is None:
             return data
         if self.compression == "zlib":
             return zlib.compress(data, level=self.compression_level)
         raise ValueError("Unsupported compression method.")
 
-    def _unpack_geometry(self, data: Union[str, bytes], cx: int, cy: int) -> Geometry:
+    def _unpack_geometry(
+        self, data: Union[str, bytes], cx: float, cy: float
+    ) -> Geometry:
         """Return the geometry using WKB data and rtree bounds index.
 
         For space optimisation, points are stored as centroids and all
         other geometry types are stored as WKB. This function unpacks
         the WKB data and uses the rtree index to find the centroid for
         points where the data is null.
 
         Args:
             data(bytes or str):
                 The WKB/WKT data to be unpacked.
             cx(int):
                 The X coordinate of the centroid/representative point.
-            cy(int):
+            cy(float):
                 The Y coordinate of the centroid/representative point.
 
         Returns:
             Geometry:
                 The Shapely geometry.
 
         """
@@ -1751,23 +2006,23 @@
         if geometry.geom_type == "Point":
             serialised_geometry = None
         else:
             serialised_geometry = self.serialise_geometry(geometry)
         return {
             "key": key,
             "geometry": serialised_geometry,
-            "cx": int(geometry.centroid.x),
-            "cy": int(geometry.centroid.y),
+            "cx": geometry.centroid.x,
+            "cy": geometry.centroid.y,
             "min_x": geometry.bounds[0],
             "min_y": geometry.bounds[1],
             "max_x": geometry.bounds[2],
             "max_y": geometry.bounds[3],
             "geom_type": geometry.geom_type,
             "properties": json.dumps(annotation.properties, separators=(",", ":")),
-            "area": int(geometry.area),
+            "area": geometry.area,
         }
 
     def append_many(
         self,
         annotations: Iterable[Annotation],
         keys: Optional[Iterable[str]] = None,
     ) -> List[str]:
@@ -1821,36 +2076,53 @@
                 )
                 """,
             token,
         )
 
     @staticmethod
     def _initialize_query_string_parameters(
-        query_geometry, query_parameters, geometry_predicate, columns, where
-    ):
+        query_geometry: Optional[Geometry],
+        query_parameters: Dict[str, Any],
+        geometry_predicate: Optional[str],
+        columns: str,
+        where: Union[bytes, str],
+        distance: float = 0,
+    ) -> Tuple[str, Dict[str, Any]]:
         """Initialises the query string and parameters."""
         query_string = (
             "SELECT "  # skipcq: BAN-B608
             + columns  # skipcq: BAN-B608
             + """
                  FROM annotations, rtree
                 WHERE annotations.id == rtree.id
                 """
         )
 
         # There is query geometry, add a simple rtree bounds check to
         # rapidly narrow candidates down.
         if query_geometry is not None:
-            # Add rtree index checks to the query
-            query_string += """
-                    AND max_x >= :min_x
-                    AND min_x <= :max_x
-                    AND max_y >= :min_y
-                    AND min_y <= :max_y
-                    """
+            # Add rtree index checks to the query.
+            # For special case of centers_within_k, Check for
+            # center of the annotation bounds within query geometry
+            # centroid + k.
+            if geometry_predicate == "centers_within_k":
+                # Use rtree index to check distance between points
+                query_string += (
+                    "AND (POWER((:min_x + :max_x)/2 - (min_x + max_x)/2, 2) + "
+                    " POWER((:min_y + :max_y)/2 - (min_y + max_y)/2, 2)) < :distance2 "
+                )
+                query_parameters["distance2"] = distance**2
+            # Otherwise, perform a regular bounding box intersection
+            else:
+                query_string += (
+                    "AND max_x >= :min_x "
+                    "AND min_x <= :max_x "
+                    "AND max_y >= :min_y "
+                    "AND min_y <= :max_y "
+                )
 
             # Find the bounds of the geometry for the rtree index
             min_x, min_y, max_x, max_y = query_geometry.bounds
 
             # Update query parameters
             query_parameters.update(
                 {
@@ -1861,17 +2133,17 @@
                     "geometry_predicate": geometry_predicate,
                     "query_geometry": query_geometry.wkb,
                 }
             )
 
             # The query is a full intersection check, not a simple bounds
             # check only.
-            if (
-                geometry_predicate is not None
-                and geometry_predicate != "bbox_intersects"
+            if geometry_predicate is not None and geometry_predicate not in (
+                "bbox_intersects",
+                "centers_within_k",
             ):
                 query_string += (
                     "\nAND geometry_predicate("
                     ":geometry_predicate, :query_geometry, geometry, cx, cy"
                     ") "
                 )
                 query_parameters["geometry_predicate"] = geometry_predicate
@@ -1895,14 +2167,15 @@
         callable_columns: Optional[str] = None,
         geometry_predicate="intersects",
         where: Optional[Predicate] = None,
         unique: bool = False,
         no_constraints_ok: bool = False,
         index_warning: bool = False,
         min_area=None,
+        distance: float = 0,
     ) -> sqlite3.Cursor:
         """Common query construction logic for `query` and `iquery`.
 
         Args:
             columns(str):
                 The columns to select.
             geometry(tuple or Geometry):
@@ -1921,14 +2194,17 @@
             no_constraints_ok(bool):
                 Whether to allow the query to return results without
                 constraints (e.g. when the geometry or where predicate
                 is not provided). Defaults to False.
             index_warning(bool):
                 Whether to warn if the query is not using an index.
                 Defaults to False.
+            distance (float):
+                Distance used when performing a distance based query.
+                E.g. "centers_within_k" geometry predicate.
 
         Returns:
             sqlite3.Cursor:
                 A database cursor for the current query.
 
         """
         if not no_constraints_ok and all(x is None for x in (geometry, where)):
@@ -1949,15 +2225,20 @@
 
         if isinstance(where, Callable):
             columns = callable_columns
 
         query_parameters = {}
 
         query_string, query_parameters = self._initialize_query_string_parameters(
-            query_geometry, query_parameters, geometry_predicate, columns, where
+            query_geometry,
+            query_parameters,
+            geometry_predicate,
+            columns,
+            where,
+            distance=distance,
         )
 
         if min_area is not None and "area" in self.table_columns:
             query_string += f"\nAND area > {min_area}"
         elif min_area is not None:
             raise ValueError(
                 """Cannot use `min_area` without an area column.
@@ -1969,30 +2250,32 @@
 
         # Warn if the query is not using an index
         if index_warning:
             query_plan = cur.execute(
                 "EXPLAIN QUERY PLAN " + query_string, query_parameters
             ).fetchone()
             if "USING INDEX" not in query_plan[-1]:
-                warnings.warn(
+                logger.warning(
                     "Query is not using an index. "
-                    "Consider adding an index to improve performance."
+                    "Consider adding an index to improve performance.",
+                    stacklevel=2,
                 )
         # if area column exists, sort annotations by area
         if "area" in self.table_columns:
             query_string += "\nORDER BY area DESC"
         cur.execute(query_string, query_parameters)
         return cur
 
     def iquery(
         self,
         geometry: Optional[QueryGeometry] = None,
         where: Optional[Predicate] = None,
         geometry_predicate="intersects",
         min_area=None,
+        distance: float = 0,
     ) -> List[str]:
         """Query the store for annotation keys.
 
         Acts the same as `AnnotationStore.query` except returns keys
         instead of annotations.
 
         Args:
@@ -2030,28 +2313,32 @@
                 A string which define which binary geometry predicate to
                 use when comparing the query geometry and a geometry in
                 the store. Only annotations for which this binary
                 predicate is true will be returned. Defaults to
                 "intersects". For more information see the `shapely
                 documentation on binary predicates <https://shapely.
                 readthedocs.io/en/stable/manual.html#binary-predicates>`_.
+            distance (float):
+                Distance used when performing a distance based query.
+                E.g. "centers_within_k" geometry predicate.
 
         Returns:
             list:
                 A list of keys for each Annotation.
 
         """
         query_geometry = geometry
         cur = self._query(
             "[key]",
             geometry=query_geometry,
             geometry_predicate=geometry_predicate,
             where=where,
             callable_columns="[key], properties",
             min_area=min_area,
+            distance=distance,
         )
         if isinstance(where, Callable):
             return [
                 key
                 for key, properties in cur.fetchall()
                 if where(json.loads(properties))
             ]
@@ -2059,23 +2346,25 @@
 
     def query(
         self,
         geometry: Optional[QueryGeometry] = None,
         where: Optional[Predicate] = None,
         geometry_predicate: str = "intersects",
         min_area=None,
+        distance: float = 0,
     ) -> Dict[str, Annotation]:
         """Runs Query."""
         query_geometry = geometry
         cur = self._query(
             columns="[key], properties, cx, cy, geometry",
             geometry=query_geometry,
             geometry_predicate=geometry_predicate,
             where=where,
             min_area=min_area,
+            distance=distance,
         )
         if isinstance(where, Callable):
             return {
                 key: Annotation(
                     geometry=self._unpack_geometry(blob, cx, cy),
                     properties=json.loads(properties),
                 )
@@ -2144,18 +2433,18 @@
                 the string statement.
 
         Returns:
             list:
                 A list of bounding boxes for each Annotation.
 
         Example:
-            >>> from tiatoolbox.annotation.storage import AnnotationStore
+            >>> from tiatoolbox.annotation.storage import SQLiteStore
             >>> from shapely.geometry import Polygon
-            >>> store = AnnotationStore()
-            >>> store.add(
+            >>> store = SQLiteStore()
+            >>> store.append(
             ...     Annotation(
             ...         geometry=Polygon.from_bounds(0, 0, 1, 1),
             ...         properties={"class": 42},
             ...     ),
             ...     key="foo",
             ... )
             >>> store.bquery(where="props['class'] == 42")
@@ -2399,37 +2688,37 @@
             squeeze (bool):
                 If True, when querying for a single value with
                 `unique=True`, the result will be a single set instead
                 of a list of sets.
 
         Examples:
 
-            >>> from tiatoolbox.annotation.storage import AnnotationStore
+            >>> from tiatoolbox.annotation.storage import SQLiteStore
             >>> from shapely.geometry import Point
-            >>> store = AnnotationStore()
+            >>> store = SQLiteStore()
             >>> annotation =  Annotation(
             ...     geometry=Point(0, 0),
             ...     properties={"class": 42},
             ... )
-            >>> store.add(annotation, "foo")
+            >>> store.append(annotation, "foo")
             >>> store.pquery("*", unique=False)
             ... {'foo': {'class': 42}}
 
-            >>> from tiatoolbox.annotation.storage import AnnotationStore
+            >>> from tiatoolbox.annotation.storage import SQLiteStore
             >>> from shapely.geometry import Point
-            >>> store = AnnotationStore()
+            >>> store = SQLiteStore()
             >>> annotation =  Annotation(
             ...     geometry=Point(0, 0),
             ...     properties={"class": 42},
             ... )
-            >>> store.add(annotation, "foo")
+            >>> store.append(annotation, "foo")
             >>> store.pquery("props['class']")
             ... {42}
             >>> annotation =  Annotation(Point(1, 1), {"class": 123})
-            >>> store.add(annotation, "foo")
+            >>> store.append(annotation, "foo")
             >>> store.pquery("props['class']")
             ... {42, 123}
 
         """  # noqa
 
         self._validate_select_where_type(select, where)
 
@@ -2635,15 +2924,15 @@
         Args:
             key: The key of the annotation to patch.
             geometry: The new geometry.
             cur: The cursor to use.
 
         """
         bounds = dict(zip(("min_x", "min_y", "max_x", "max_y"), geometry.bounds))
-        xy = dict(zip("xy", np.array(geometry.centroid)))
+        xy = dict(zip("xy", np.array(geometry.centroid.coords[0])))
         query_parameters = dict(
             **bounds,
             **xy,
             key=key,
             geometry=self.serialise_geometry(geometry),
         )
         cur.execute(
@@ -2751,15 +3040,15 @@
             {
                 "key": key,
                 "geometry": annotation.geometry,
                 "properties": annotation.properties,
             }
             for key, annotation in self.items()
         )
-        df = df.append(pd.json_normalize(df_rows))
+        df = pd.concat([df, pd.json_normalize(df_rows)])
         return df.set_index("key")
 
     def features(self) -> Generator[Dict[str, Any], None, None]:
         """Return annotations as a list of geoJSON features.
 
         Returns:
             list:
@@ -2772,23 +3061,38 @@
                 "geometry": geometry2feature(annotation.geometry),
                 "properties": annotation.properties,
             }
             for annotation in self.values()
         )
 
     def commit(self) -> None:
+        """Commit any in-memory changes to disk."""
         self.con.commit()
 
     def dump(self, fp: Union[Path, str, IO]) -> None:
+        """Serialise a copy of the whole store to a file-like object.
+
+        Args:
+            fp(Path or str or IO):
+                A file path or file handle object for output to disk.
+
+        """
         if hasattr(fp, "write"):
             fp = fp.name
         target = sqlite3.connect(fp)
         self.con.backup(target)
 
     def dumps(self) -> str:
+        """Serialise and return a copy of store as a string or bytes.
+
+        Returns:
+            str or bytes:
+                The serialised store.
+
+        """
         return "\n".join(self.con.iterdump())
 
     def clear(self) -> None:
         """Remove all annotations from the store."""
         cur = self.con.cursor()
         cur.execute("DELETE FROM rtree")
         cur.execute("DELETE FROM annotations")
@@ -2815,15 +3119,15 @@
             analyze (bool):
                 Whether to run the "ANALYZE" command after creating the
                 index.
 
         """
         _, minor, _ = sqlite3.sqlite_version_info
         if minor < 9:
-            raise Exception("Requires sqlite version 3.9.0 or higher.")
+            raise EnvironmentError("Requires sqlite version 3.9.0 or higher.")
         cur = self.con.cursor()
         if not isinstance(where, str):
             raise TypeError(f"Invalid type for `where` ({type(where)}).")
         sql_predicate = eval(where, SQL_GLOBALS)  # skipcq: PYL-W0123
         cur.execute(f"CREATE INDEX {name} ON annotations({sql_predicate})")
         if analyze:
             cur.execute(f"ANALYZE {name}")
@@ -2891,38 +3195,78 @@
                 properties = dictionary["properties"]
                 self.append(Annotation(geometry, properties), key=key)
 
     def append(
         self,
         annotation: Annotation,
         key: Optional[str] = None,
-    ) -> int:
+    ) -> str:
+        """Insert a new annotation, returning the key.
+
+        Args:
+            annotation (Annotation):
+                The shapely annotation to insert.
+            key (str):
+                Optional. The unique key used to identify the annotation in the
+                store. If not given a new UUID4 will be generated and returned
+                instead.
+
+        Returns:
+            str:
+                The unique key of the newly inserted annotation.
+
+        """
         if not isinstance(annotation.geometry, (Polygon, Point, LineString)):
             raise TypeError("Invalid geometry type.")
         key = key or str(uuid.uuid4())
         self._rows[key] = {"annotation": annotation}
         return key
 
     def patch(
         self,
         key: str,
         geometry: Optional[Geometry] = None,
         properties: Optional[Dict[str, Any]] = None,
     ) -> None:
+        """Patch an annotation at given key.
+
+        Partial update of an annotation. Providing only a geometry will update
+        the geometry and leave properties unchanged. Providing a properties
+        dictionary applies a patch operation to the properties. Only updating
+        the properties which are given and leaving the rest unchanged. To
+        completely replace an annotation use `__setitem__`.
+
+        Args:
+            key(str):
+                The key of the annotation to update.
+            geometry(Geometry):
+                The new geometry. If None, the geometry is not updated.
+            properties(dict):
+                A dictionary of properties to patch and their new values.
+                If None, the existing properties are not altered.
+
+        """
         if key not in self:
             self.append(Annotation(geometry, properties), key)
             return
         existing = self[key]
         geometry = geometry or existing.geometry
         properties = properties or {}
         new_properties = copy.deepcopy(existing.properties)
         new_properties.update(properties)
         self[key] = Annotation(geometry, new_properties)
 
     def remove(self, key: str) -> None:
+        """Remove annotation from the store with its unique key.
+
+        Args:
+            key (str):
+                The key of the annotation to be removed.
+
+        """
         del self._rows[key]
 
     def __getitem__(self, key: str) -> Annotation:
         return self._rows[key]["annotation"]
 
     def __setitem__(self, key: str, annotation: Annotation) -> None:
         if key in self._rows:
@@ -2938,29 +3282,47 @@
             yield key, row["annotation"]
 
     def __len__(self) -> int:
         return len(self._rows)
 
     @classmethod  # noqa: A003
     def open(cls, fp: Union[Path, str, IO]) -> "DictionaryStore":  # noqa: A003
+        """Opens :class:`DictionaryStore` from file pointer or path."""
         return cls.from_ndjson(fp)
 
     def commit(self) -> None:
+        """Commit any in-memory changes to disk."""
         if str(self.connection) == ":memory:":
-            warnings.warn("In-memory store. Nothing to commit.")
+            logger.warning("In-memory store. Nothing to commit.", stacklevel=2)
             return
         if not self.path.exists():
             self.path.touch()
         self.dump(self.connection)
 
     def dump(self, fp: Union[Path, str, IO]) -> None:
+        """Serialise a copy of the whole store to a file-like object.
+
+        Args:
+            fp(Path or str or IO):
+                A file path or file handle object for output to disk.
+
+        """
         return self.to_ndjson(fp)
 
     def dumps(self) -> str:
+        """Serialise and return a copy of store as a string or bytes.
+
+        Returns:
+            str or bytes:
+                The serialised store.
+
+        """
         return self.to_ndjson()
 
     def close(self) -> None:
-        warnings.simplefilter("ignore")
+        """Closes :class:`DictionaryStore` from file pointer or path."""
+        duplicate_filter = DuplicateFilter()
+        logger.addFilter(duplicate_filter)
         # Try to commit any changes if the file is still open.
         with contextlib.suppress(ValueError):
             self.commit()
-        warnings.resetwarnings()
+        logger.removeFilter(duplicate_filter)
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/cli/__init__.py` & `tiatoolbox-1.4.0/tiatoolbox/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/cli/common.py` & `tiatoolbox-1.4.0/tiatoolbox/cli/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,26 @@
         type=int,
         nargs=2,
         default=[5000, 5000],
         help=usage_help,
     )
 
 
+def cli_tile_format(
+    usage_help: str = "File format to save image tiles, defaults = '.jpg'",
+) -> callable:
+    """Enables --tile-format option for cli."""
+    return click.option(
+        "--tile-format",
+        type=str,
+        default=".jpg",
+        help=usage_help,
+    )
+
+
 def cli_method(
     usage_help: str = "Select method of for tissue masking.",
     default: str = "Otsu",
     input_type: click.Choice = None,
 ) -> callable:
     """Enables --method option for cli."""
     if input_type is None:
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/cli/nucleus_instance_segment.py` & `tiatoolbox-1.4.0/tiatoolbox/cli/nucleus_instance_segment.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/cli/patch_predictor.py` & `tiatoolbox-1.4.0/tiatoolbox/cli/patch_predictor.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/cli/read_bounds.py` & `tiatoolbox-1.4.0/tiatoolbox/cli/read_bounds.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/cli/save_tiles.py` & `tiatoolbox-1.4.0/tiatoolbox/cli/save_tiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """Command line interface for save_tiles."""
+import logging
+
+from tiatoolbox import logger
 from tiatoolbox.cli.common import (
     cli_file_type,
     cli_img_input,
     cli_output_path,
+    cli_tile_format,
     cli_tile_objective,
     cli_tile_read_size,
     cli_verbose,
     prepare_file_dir_cli,
     tiatoolbox_cli,
 )
 
@@ -15,31 +19,35 @@
 @cli_img_input()
 @cli_output_path(
     usage_help="Path to output directory to save the output.", default="tiles"
 )
 @cli_file_type()
 @cli_tile_objective()
 @cli_tile_read_size()
-@cli_verbose()
+@cli_tile_format()
+@cli_verbose(default=False)
 def save_tiles(
     img_input,
     output_path,
     file_types,
     tile_objective_value,
     tile_read_size,
-    verbose=True,
+    tile_format,
+    verbose=False,
 ):
     """Display or save WSI metadata."""
-    from tiatoolbox import wsicore
+    from tiatoolbox.wsicore.wsireader import WSIReader
 
     files_all, output_path = prepare_file_dir_cli(
         img_input, output_path, file_types, "save", "tiles"
     )
+    if verbose:
+        logger.setLevel(logging.DEBUG)
 
     for curr_file in files_all:
-        wsicore.save_tiles.save_tiles(
-            input_path=curr_file,
+        wsi = WSIReader.open(curr_file)
+        wsi.save_tiles(
             output_dir=output_path,
             tile_objective_value=tile_objective_value,
             tile_read_size=tile_read_size,
-            verbose=verbose,
+            tile_format=tile_format,
         )
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/cli/semantic_segment.py` & `tiatoolbox-1.4.0/tiatoolbox/cli/semantic_segment.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/cli/show_wsi.py` & `tiatoolbox-1.4.0/tiatoolbox/cli/show_wsi.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/cli/slide_info.py` & `tiatoolbox-1.4.0/tiatoolbox/cli/slide_info.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Command line interface for slide_info."""
+import logging
 import pathlib
 
+from tiatoolbox import logger
 from tiatoolbox.cli.common import (
     cli_file_type,
     cli_img_input,
     cli_mode,
     cli_output_path,
     cli_verbose,
     prepare_file_dir_cli,
@@ -16,30 +18,36 @@
 @cli_img_input()
 @cli_output_path(
     usage_help="Path to output directory to save the output. "
     "default=img_input/../meta-data"
 )
 @cli_file_type(default="*.ndpi, *.svs, *.mrxs, *.jp2")
 @cli_mode(default="show")
-@cli_verbose(default=True)
+@cli_verbose(default=False)
 def slide_info(img_input, output_path, file_types, mode, verbose):
     """Displays or saves WSI metadata depending on the mode argument."""
     from tiatoolbox import utils, wsicore
 
     files_all, output_path = prepare_file_dir_cli(
         img_input, output_path, file_types, mode, "meta-data"
     )
 
     for curr_file in files_all:
-        slide_param = wsicore.slide_info.slide_info(
-            input_path=curr_file, verbose=verbose or mode == "show"
-        )
+        curr_file = pathlib.Path(curr_file)
+        wsi = wsicore.wsireader.WSIReader.open(input_img=curr_file)
+
+        if verbose:
+            logger.setLevel(logging.DEBUG)
+            logger.debug(curr_file.name)
+
+        if mode == "show":
+            logger.info(wsi.info.as_dict())
 
         if mode == "save":
             out_path = pathlib.Path(
-                output_path, slide_param.file_path.with_suffix(".yaml").name
+                output_path, wsi.info.file_path.with_suffix(".yaml").name
             )
             utils.misc.save_yaml(
-                slide_param.as_dict(),
+                wsi.info.as_dict(),
                 out_path,
             )
-            print("Meta files saved at " + str(output_path))
+            logger.info("Meta files saved at %s.", str(output_path))
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/cli/slide_thumbnail.py` & `tiatoolbox-1.4.0/tiatoolbox/cli/slide_thumbnail.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/cli/stain_norm.py` & `tiatoolbox-1.4.0/tiatoolbox/cli/stain_norm.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/cli/tissue_mask.py` & `tiatoolbox-1.4.0/tiatoolbox/cli/tissue_mask.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/__init__.py` & `tiatoolbox-1.4.0/tiatoolbox/data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             Path within the package to the data file.
 
 
     Example:
         >>> # Get the path to a sample target image for performing
         >>> # stain normalization.
         >>> from tiatoolbox.data import stain_norm_target
-        >>> img = stainnorm_target()
+        >>> img = stain_norm_target()
 
     """
     return pkg_resources.resource_filename(
         "tiatoolbox", str(pathlib.Path("data") / path)
     )
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/pretrained_model.yaml` & `tiatoolbox-1.4.0/tiatoolbox/data/pretrained_model.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -773,52 +773,74 @@
             save_resolution: {'units': 'mpp', 'resolution': 0.25}
 
 mapde-crchisto:
     url: https://tiatoolbox.dcs.warwick.ac.uk/models/detection/mapde-crchisto.pth
     architecture:
         class: mapde.MapDe
         kwargs:
+            input_resolutions:
+                - { "units": "mpp", "resolution": 0.25 }
             num_input_channels: 3
             min_distance: 4
             threshold_abs: 250
             num_classes: 1
+            tile_shape: [ 2048, 2048 ]
+            patch_input_shape: [ 252, 252 ]
+            stride_shape: [ 150, 150 ]
 
 mapde-conic:
     url: https://tiatoolbox.dcs.warwick.ac.uk/models/detection/mapde-conic.pth
     architecture:
         class: mapde.MapDe
         kwargs:
+            input_resolutions:
+                - { "units": "mpp", "resolution": 0.25 }
             num_input_channels: 3
             min_distance: 3
             threshold_abs: 205
             num_classes: 1
+            tile_shape: [ 2048, 2048 ]
+            patch_input_shape: [ 252, 252 ]
+            stride_shape: [ 150, 150 ]
 
 sccnn-crchisto:
     url: https://tiatoolbox.dcs.warwick.ac.uk/models/detection/sccnn-crchisto.pth
     architecture:
         class: sccnn.SCCNN
         kwargs:
+            input_resolutions:
+                - { "units": "mpp", "resolution": 0.25 }
             num_input_channels: 3
             out_height: 13
             out_width: 13
             radius: 12
             min_distance: 6
             threshold_abs: 0.20
+            tile_shape: [ 2048, 2048 ]
+            patch_input_shape: [ 31, 31 ]
+            patch_output_shape: [ 13, 13 ]
+            stride_shape: [ 8, 8 ]
 
 sccnn-conic:
     url: https://tiatoolbox.dcs.warwick.ac.uk/models/detection/sccnn-conic.pth
     architecture:
         class: sccnn.SCCNN
         kwargs:
+            input_resolutions:
+                - { "units": "mpp", "resolution": 0.25 }
             num_input_channels: 3
             out_height: 13
             out_width: 13
             radius: 12
             min_distance: 5
             threshold_abs: 0.05
+            tile_shape: [ 2048, 2048 ]
+            patch_input_shape: [ 31, 31 ]
+            patch_output_shape: [ 13, 13 ]
+            stride_shape: [ 8, 8 ]
 
 nuclick_original-pannuke:
     url: https://tiatoolbox.dcs.warwick.ac.uk/models/seg/nuclick_original-pannuke.pth
     architecture:
         class: nuclick.NuClick
         kwargs:
             num_input_channels: 5
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/remote_samples.yaml` & `tiatoolbox-1.4.0/tiatoolbox/data/remote_samples.yaml`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/target_image.png` & `tiatoolbox-1.4.0/tiatoolbox/data/target_image.png`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/css/fontawesome-all.min.css` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/css/ol-ext.min.css` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/ol-ext.min.css`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/css/ol.css` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/css/ol.css`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/js/ol-ext.min.js` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/js/ol-ext.min.js`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/js/ol.js` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/js/ol.js`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.eot` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.svg` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.ttf` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff2` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.eot` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.svg` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.ttf` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff2` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.eot` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.svg` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.ttf` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff2` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/data/visualization/templates/index.html` & `tiatoolbox-1.4.0/tiatoolbox/data/visualization/templates/index.html`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/architecture/__init__.py` & `tiatoolbox-1.4.0/tiatoolbox/models/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/architecture/hovernet.py` & `tiatoolbox-1.4.0/tiatoolbox/models/architecture/hovernet.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/architecture/hovernetplus.py` & `tiatoolbox-1.4.0/tiatoolbox/models/architecture/hovernetplus.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/architecture/idars.py` & `tiatoolbox-1.4.0/tiatoolbox/models/architecture/idars.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/architecture/mapde.py` & `tiatoolbox-1.4.0/tiatoolbox/models/architecture/mapde.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/architecture/micronet.py` & `tiatoolbox-1.4.0/tiatoolbox/models/architecture/micronet.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,15 +541,15 @@
         Returns:
             :class:`numpy.ndarray`:
                 Pixel-wise nuclear instance segmentation
                 prediction.
 
         """
         pred_bin = np.argmax(image[0], axis=2)
-        pred_inst = ndimage.measurements.label(pred_bin)[0]
+        pred_inst = ndimage.label(pred_bin)[0]
         pred_inst = morphology.remove_small_objects(pred_inst, min_size=50)
         canvas = np.zeros(pred_inst.shape[:2], dtype=np.int32)
         for inst_id in range(1, np.max(pred_inst) + 1):
             inst_map = np.array(pred_inst == inst_id, dtype=np.uint8)
             inst_map = ndimage.binary_fill_holes(inst_map)
             canvas[inst_map > 0] = inst_id
         nuc_inst_info_dict = HoVerNet.get_instance_info(canvas)
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/architecture/nuclick.py` & `tiatoolbox-1.4.0/tiatoolbox/models/architecture/nuclick.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Defines original NuClick architecture
 
 Koohbanani, N. A., Jahanifar, M., Tajadin, N. Z., & Rajpoot, N. (2020).
 NuClick: a deep learning framework for interactive segmentation of microscopic images.
 Medical Image Analysis, 65, 101771.
 
 """
-import warnings
 from typing import Tuple, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 from skimage.morphology import (
     disk,
     reconstruction,
     remove_small_holes,
     remove_small_objects,
 )
 
+from tiatoolbox import logger
 from tiatoolbox.models.models_abc import ModelABC
 from tiatoolbox.utils import misc
 
 bn_axis = 1
 
 
 class ConvBnRelu(nn.Module):
@@ -57,15 +57,14 @@
         kernel_size: Union[Tuple[int, int], np.ndarray] = (3, 3),
         strides: Union[Tuple[int, int], np.ndarray] = (1, 1),
         use_bias: bool = False,
         dilation_rate: Union[Tuple[int, int], np.ndarray] = (1, 1),
         activation: str = "relu",
         do_batchnorm: bool = True,
     ):
-
         super().__init__()
         if isinstance(kernel_size, int):
             kernel_size = (kernel_size, kernel_size)
         if isinstance(strides, int):
             strides = (strides, strides)
 
         self.conv_bn_relu = self.get_block(
@@ -599,19 +598,23 @@
         masks = remove_small_holes(masks, area_threshold=min_hole_size)
         if do_reconstruction:
             for i in range(len(masks)):
                 this_mask = masks[i, :, :]
                 this_marker = nuc_points[i, :, :] > 0
 
                 if np.any(this_mask[this_marker > 0]):
-                    this_mask = reconstruction(this_marker, this_mask, selem=disk(1))
+                    this_mask = reconstruction(
+                        this_marker, this_mask, footprint=disk(1)
+                    )
                     masks[i] = np.array([this_mask])
                 else:
-                    warnings.warn(
-                        f"Nuclei reconstruction was not done for nucleus #{i}"
+                    logger.warning(
+                        "Nuclei reconstruction was not done for nucleus #%d",
+                        i,
+                        stacklevel=2,
                     )
         return masks
 
     @staticmethod
     def infer_batch(model, batch_data, on_gpu):
         """Run inference on an input batch.
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/architecture/sccnn.py` & `tiatoolbox-1.4.0/tiatoolbox/models/architecture/sccnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,21 +86,22 @@
         IEEE transactions on medical imaging 35.5 (2016): 1196-1206.
 
     """
 
     def __init__(
         self,
         num_input_channels: int = 3,
-        out_height: int = 13,
-        out_width: int = 13,
+        patch_output_shape: Tuple[int, int] = (13, 13),
         radius: int = 12,
         min_distance: int = 6,
         threshold_abs: float = 0.20,
     ) -> None:
         super().__init__()
+        out_height = patch_output_shape[0]
+        out_width = patch_output_shape[1]
         self.in_ch = num_input_channels
         self.out_height = out_height
         self.out_width = out_width
 
         # Create mesh grid and convert to 3D vector
         x, y = torch.meshgrid(
             torch.arange(start=0, end=out_height),
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/architecture/unet.py` & `tiatoolbox-1.4.0/tiatoolbox/models/architecture/unet.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,17 @@
             ...     num_input_channels,
             ...     [3, 4, 6, 3],
             ... )
 
         """
         model = ResNetEncoder(ResNetBottleneck, downsampling_levels)
         if num_input_channels != 3:
-            model.conv1 = nn.Conv2d(num_input_channels, 64, 7, stride=2, padding=3)
+            model.conv1 = nn.Conv2d(  # skipcq: PYL-W0201
+                num_input_channels, 64, 7, stride=2, padding=3
+            )
         return model
 
 
 class UnetEncoder(nn.Module):
     """Construct a basic UNet encoder.
 
     This class builds a basic UNet encoder with batch normalization.
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/architecture/utils.py` & `tiatoolbox-1.4.0/tiatoolbox/models/architecture/utils.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/architecture/vanilla.py` & `tiatoolbox-1.4.0/tiatoolbox/models/architecture/vanilla.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/dataset/classification.py` & `tiatoolbox-1.4.0/tiatoolbox/models/dataset/classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import pathlib
-import warnings
 
 import cv2
 import numpy as np
 import PIL
 import torchvision.transforms as transforms
 
+from tiatoolbox import logger
 from tiatoolbox.models.dataset import dataset_abc
 from tiatoolbox.tools.patchextraction import PatchExtractor
 from tiatoolbox.utils.misc import imread
 from tiatoolbox.wsicore.wsimeta import WSIMeta
 from tiatoolbox.wsicore.wsireader import VirtualWSIReader, WSIReader
 
 
@@ -138,34 +138,31 @@
             read from `reader` at requested `resolution` and `units`.
             Expected to be `(height, width)`.
         resolution:
             See (:class:`.WSIReader`) for details.
         units:
             See (:class:`.WSIReader`) for details.
         preproc_func:
-            Preprocessing function used to transform the input data. If
-            supplied, then torch.Compose will be used on the input
-            preprocs. preprocs is a list of torchvision transforms for
-            preprocessing the image. The transforms will be applied in
-            the order that they are given in the list. For more
-            information, visit the following link:
-            https://pytorch.org/vision/stable/transforms.html.
+            Preprocessing function used to transform the input data. It will
+            be called on each patch before returning it.
 
     """
 
     def __init__(
         self,
         img_path,
         mode="wsi",
         mask_path=None,
         patch_input_shape=None,
         stride_shape=None,
         resolution=None,
         units=None,
         auto_get_mask=True,
+        min_mask_ratio=0,
+        preproc_func=None,
     ):
         """Create a WSI-level patch dataset.
 
         Args:
             mode (str):
                 Can be either `wsi` or `tile` to denote the image to
                 read is either a whole-slide image or a large image
@@ -183,20 +180,30 @@
                 space.
             stride_shape:
                 A tuple (int, int) or ndarray of shape (2,). Expected
                 stride shape to read at requested `resolution` and
                 `units`. Expected to be positive and of (height, width).
                 Note, this is not at level 0.
             resolution:
-              Check (:class:`.WSIReader`) for details. When
-              `mode='tile'`, value is fixed to be `resolution=1.0` and
-              `units='baseline'` units: check (:class:`.WSIReader`) for
-              details.
+                Check (:class:`.WSIReader`) for details. When
+                `mode='tile'`, value is fixed to be `resolution=1.0` and
+                `units='baseline'` units: check (:class:`.WSIReader`) for
+                details.
+            units:
+                Units in which `resolution` is defined.
+            auto_get_mask:
+                If `True`, then automatically get simple threshold mask using
+                WSIReader.tissue_mask() function.
+            min_mask_ratio:
+                Only patches with positive area percentage above this value are
+                included. Defaults to 0.
             preproc_func:
-                Preprocessing function used to transform the input data.
+                Preprocessing function used to transform the input data. If
+                supplied, the function will be called on each patch before
+                returning it.
 
         Examples:
             >>> # A user defined preproc func and expected behavior
             >>> preproc_func = lambda img: img/2  # reduce intensity by half
             >>> transformed_img = preproc_func(img)
             >>> # Create a dataset to get patches from WSI with above
             >>> # preprocessing function
@@ -229,23 +236,23 @@
         if (
             not np.issubdtype(stride_shape.dtype, np.integer)
             or np.size(stride_shape) > 2
             or np.any(stride_shape < 0)
         ):
             raise ValueError(f"Invalid `stride_shape` value {stride_shape}.")
 
+        self.preproc_func = preproc_func
         img_path = pathlib.Path(img_path)
         if mode == "wsi":
             self.reader = WSIReader.open(img_path)
         else:
-            warnings.warn(
-                (
-                    "WSIPatchDataset only reads image tile at "
-                    '`units="baseline"` and `resolution=1.0`.'
-                )
+            logger.warning(
+                "WSIPatchDataset only reads image tile at "
+                '`units="baseline"` and `resolution=1.0`.',
+                stacklevel=2,
             )
             units = "baseline"
             resolution = 1.0
             img = imread(img_path)
             axes = "YXS"[: len(img.shape)]
             # initialise metadata for VirtualWSIReader.
             # here, we simulate a whole-slide image, but with a single level.
@@ -296,16 +303,16 @@
             # ? will this mess up  ?
             mask_reader.info = self.reader.info
 
         if mask_reader is not None:
             selected = PatchExtractor.filter_coordinates(
                 mask_reader,  # must be at the same resolution
                 self.inputs,  # must already be at requested resolution
-                resolution=resolution,
-                units=units,
+                wsi_shape=wsi_shape,
+                min_mask_ratio=min_mask_ratio,
             )
             self.inputs = self.inputs[selected]
 
         if len(self.inputs) == 0:
             raise ValueError("No patch coordinates remain after filtering.")
 
         self.patch_input_shape = patch_input_shape
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/dataset/dataset_abc.py` & `tiatoolbox-1.4.0/tiatoolbox/models/dataset/dataset_abc.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/dataset/info.py` & `tiatoolbox-1.4.0/tiatoolbox/models/dataset/info.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/engine/nucleus_instance_segmentor.py` & `tiatoolbox-1.4.0/tiatoolbox/models/engine/nucleus_instance_segmentor.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,173 @@
     IOSegmentorConfig,
     SemanticSegmentor,
     WSIStreamDataset,
 )
 from tiatoolbox.tools.patchextraction import PatchExtractor
 
 
+def _process_instance_predictions(
+    inst_dict,
+    ioconfig,
+    tile_shape,
+    tile_flag,
+    tile_mode,
+    tile_tl,
+    ref_inst_dict,
+):
+    """Function to merge new tile prediction with existing prediction.
+
+    Args:
+        inst_dict (dict): Dictionary containing instance information.
+        ioconfig (:class:`IOSegmentorConfig`): Object defines information
+            about input and output placement of patches.
+        tile_shape (list): A list of the tile shape.
+        tile_flag (list): A list of flag to indicate if instances within
+            an area extended from each side (by `ioconfig.margin`) of
+            the tile should be replaced by those within the same spatial
+            region in the accumulated output this run. The format is
+            [top, bottom, left, right], 1 indicates removal while 0 is not.
+            For example, [1, 1, 0, 0] denotes replacing top and bottom instances
+            within `ref_inst_dict` with new ones after this processing.
+        tile_mode (int): A flag to indicate the type of this tile. There
+            are 4 flags:
+            - 0: A tile from tile grid without any overlapping, it is not
+                an overlapping tile from tile generation. The predicted
+                instances are immediately added to accumulated output.
+            - 1: Vertical tile strip that stands between two normal tiles
+                (flag 0). It has the the same height as normal tile but
+                less width (hence vertical strip).
+            - 2: Horizontal tile strip that stands between two normal tiles
+                (flag 0). It has the the same width as normal tile but
+                less height (hence horizontal strip).
+            - 3: tile strip stands at the cross section of four normal tiles
+                (flag 0).
+        tile_tl (tuple): Top left coordinates of the current tile.
+        ref_inst_dict (dict): Dictionary contains accumulated output. The
+            expected format is {instance_id: {type: int,
+            contour: List[List[int]], centroid:List[float], box:List[int]}.
+
+    Returns:
+        new_inst_dict (dict): A dictionary contain new instances to be accumulated.
+            The expected format is {instance_id: {type: int,
+            contour: List[List[int]], centroid:List[float], box:List[int]}.
+        remove_insts_in_orig (list): List of instance id within `ref_inst_dict`
+            to be removed to prevent overlapping predictions. These instances
+            are those get cutoff at the boundary due to the tiling process.
+
+    """
+    # should be rare, no nuclei detected in input images
+    if len(inst_dict) == 0:
+        return {}, []
+
+    # !
+    m = ioconfig.margin
+    w, h = tile_shape
+    inst_boxes = [v["box"] for v in inst_dict.values()]
+    inst_boxes = np.array(inst_boxes)
+
+    geometries = [shapely_box(*bounds) for bounds in inst_boxes]
+    tile_rtree = STRtree(geometries)
+    # !
+
+    # create margin bounding box, ordering should match with
+    # created tile info flag (top, bottom, left, right)
+    boundary_lines = [
+        shapely_box(0, 0, w, 1),  # noqa top egde
+        shapely_box(0, h - 1, w, h),  # noqa bottom edge
+        shapely_box(0, 0, 1, h),  # noqa left
+        shapely_box(w - 1, 0, w, h),  # noqa right
+    ]
+    margin_boxes = [
+        shapely_box(0, 0, w, m),  # noqa top egde
+        shapely_box(0, h - m, w, h),  # noqa bottom edge
+        shapely_box(0, 0, m, h),  # noqa left
+        shapely_box(w - m, 0, w, h),  # noqa right
+    ]
+    # ! this is wrt to WSI coord space, not tile
+    margin_lines = [
+        [[m, m], [w - m, m]],  # noqa top egde
+        [[m, h - m], [w - m, h - m]],  # noqa bottom edge
+        [[m, m], [m, h - m]],  # noqa left
+        [[w - m, m], [w - m, h - m]],  # noqa right
+    ]
+    margin_lines = np.array(margin_lines) + tile_tl[None, None]
+    margin_lines = [shapely_box(*v.flatten().tolist()) for v in margin_lines]
+
+    # the ids within this match with those within `inst_map`, not UUID
+    sel_indices = []
+    if tile_mode in [0, 3]:
+        # for `full grid` tiles `cross section` tiles
+        # -- extend from the boundary by the margin size, remove
+        #    nuclei whose entire contours lie within the margin area
+        sel_boxes = [
+            box
+            for idx, box in enumerate(margin_boxes)
+            if tile_flag[idx] or tile_mode == 3
+        ]
+
+        sel_indices = [
+            geo
+            for bounds in sel_boxes
+            for geo in tile_rtree.query(bounds)
+            if bounds.contains(geometries[geo])
+        ]
+    elif tile_mode in [1, 2]:
+        # for `horizontal/vertical strip` tiles
+        # -- extend from the marked edges (top/bot or left/right) by
+        #    the margin size, remove all nuclei lie within the margin
+        #    area (including on the margin line)
+        # -- remove all nuclei on the boundary also
+
+        sel_boxes = [
+            margin_boxes[idx] if flag else boundary_lines[idx]
+            for idx, flag in enumerate(tile_flag)
+        ]
+
+        sel_indices = [geo for bounds in sel_boxes for geo in tile_rtree.query(bounds)]
+    else:
+        raise ValueError(f"Unknown tile mode {tile_mode}.")
+
+    def retrieve_sel_uids(sel_indices, inst_dict):
+        """Helper to retrieved selected instance uids."""
+        if len(sel_indices) > 0:
+            # not sure how costly this is in large dict
+            inst_uids = list(inst_dict.keys())
+        return [inst_uids[idx] for idx in sel_indices]
+
+    remove_insts_in_tile = retrieve_sel_uids(sel_indices, inst_dict)
+
+    # external removal only for tile at cross sections
+    # this one should contain UUID with the reference database
+    remove_insts_in_orig = []
+    if tile_mode == 3:
+        inst_boxes = [v["box"] for v in ref_inst_dict.values()]
+        inst_boxes = np.array(inst_boxes)
+
+        geometries = [shapely_box(*bounds) for bounds in inst_boxes]
+        ref_inst_rtree = STRtree(geometries)
+        sel_indices = [
+            geo for bounds in margin_lines for geo in ref_inst_rtree.query(bounds)
+        ]
+
+        remove_insts_in_orig = retrieve_sel_uids(sel_indices, ref_inst_dict)
+
+    # move inst position from tile space back to WSI space
+    # an also generate universal uid as replacement for storage
+    new_inst_dict = {}
+    for inst_uid, inst_info in inst_dict.items():
+        if inst_uid not in remove_insts_in_tile:
+            inst_info["box"] += np.concatenate([tile_tl] * 2)
+            inst_info["centroid"] += tile_tl
+            inst_info["contour"] += tile_tl
+            inst_uuid = uuid.uuid4().hex
+            new_inst_dict[inst_uuid] = inst_info
+    return new_inst_dict, remove_insts_in_orig
+
+
 # Python is yet to be able to natively pickle Object method/static
 # method. Only top-level function is passable to multiprocessing as
 # caller. May need 3rd party libraries to use method/static method
 # otherwise.
 def _process_tile_predictions(
     ioconfig,
     tile_bounds,
@@ -122,131 +281,23 @@
             head_tile_shape[::-1],
             head_predictions,
             head_locations,
         )
         head_raws.append(head_raw)
     _, inst_dict = postproc(head_raws)
 
-    # should be rare, no nuclei detected in input images
-    if len(inst_dict) == 0:
-        return {}, []
-
-    # !
-    m = ioconfig.margin
-    w, h = tile_shape
-    inst_boxes = [v["box"] for v in inst_dict.values()]
-    inst_boxes = np.array(inst_boxes)
-
-    geometries = [shapely_box(*bounds) for bounds in inst_boxes]
-    # An auxiliary dictionary to actually query the index within the source list
-    index_by_id = {id(geo): idx for idx, geo in enumerate(geometries)}
-    tile_rtree = STRtree(geometries)
-    # !
-
-    # create margin bounding box, ordering should match with created
-    # tile info flag (top, bottom, left, right)
-    boundary_lines = [
-        shapely_box(0, 0, w, 1),  # noqa top egde
-        shapely_box(0, h - 1, w, h),  # noqa bottom edge
-        shapely_box(0, 0, 1, h),  # noqa left
-        shapely_box(w - 1, 0, w, h),  # noqa right
-    ]
-    margin_boxes = [
-        shapely_box(0, 0, w, m),  # noqa top egde
-        shapely_box(0, h - m, w, h),  # noqa bottom edge
-        shapely_box(0, 0, m, h),  # noqa left
-        shapely_box(w - m, 0, w, h),  # noqa right
-    ]
-    # ! this is wrt to WSI coord space, not tile
-    margin_lines = [
-        [[m, m], [w - m, m]],  # noqa top egde
-        [[m, h - m], [w - m, h - m]],  # noqa bottom edge
-        [[m, m], [m, h - m]],  # noqa left
-        [[w - m, m], [w - m, h - m]],  # noqa right
-    ]
-    margin_lines = np.array(margin_lines) + tile_tl[None, None]
-    margin_lines = [shapely_box(*v.flatten().tolist()) for v in margin_lines]
-
-    # the ids within this match with those within `inst_map`, not UUID
-    sel_indices = []
-    if tile_mode in [0, 3]:
-        # for `full grid` tiles `cross-section` tiles
-        # -- extend from the boundary by the margin size, remove nuclei
-        #    whose entire contours lie within the margin area
-        sel_boxes = [
-            box
-            for idx, box in enumerate(margin_boxes)
-            if tile_flag[idx] or tile_mode == 3
-        ]
-
-        sel_indices = [
-            index_by_id[id(geo)]
-            for bounds in sel_boxes
-            for geo in tile_rtree.query(bounds)
-            if bounds.contains(geo)
-        ]
-    elif tile_mode in [1, 2]:
-        # for `horizontal/vertical strip` tiles
-        # -- extend from the marked edges (top/bot or left/right) by the
-        #    margin size, remove all nuclei lie within the margin area
-        #    (including on the margin line)
-        # -- remove all nuclei on the boundary also
-
-        sel_boxes = [
-            margin_boxes[idx] if flag else boundary_lines[idx]
-            for idx, flag in enumerate(tile_flag)
-        ]
-
-        sel_indices = [
-            index_by_id[id(geo)]
-            for bounds in sel_boxes
-            for geo in tile_rtree.query(bounds)
-        ]
-    else:
-        raise ValueError(f"Unknown tile mode {tile_mode}.")
-
-    def retrieve_sel_uids(sel_indices, inst_dict):
-        """Helper to retrieved selected instance uids."""
-        if len(sel_indices) > 0:
-            # not sure how costly this is in large dict
-            inst_uids = list(inst_dict.keys())
-            return [inst_uids[idx] for idx in sel_indices]
-        return []
-
-    remove_insts_in_tile = retrieve_sel_uids(sel_indices, inst_dict)
-
-    # external removal only for tile at cross-sections this one should
-    # contain UUID with the reference database
-    remove_insts_in_orig = []
-    if tile_mode == 3:
-        inst_boxes = [v["box"] for v in ref_inst_dict.values()]
-        inst_boxes = np.array(inst_boxes)
-
-        geometries = [shapely_box(*bounds) for bounds in inst_boxes]
-        # An auxiliary dictionary to actually query the index within the source list
-        index_by_id = {id(geo): idx for idx, geo in enumerate(geometries)}
-        ref_inst_rtree = STRtree(geometries)
-        sel_indices = [
-            index_by_id[id(geo)]
-            for bounds in margin_lines
-            for geo in ref_inst_rtree.query(bounds)
-        ]
-
-        remove_insts_in_orig = retrieve_sel_uids(sel_indices, ref_inst_dict)
-
-    # move inst position from tile space back to WSI space and also
-    # generate universal uid as replacement for storage
-    new_inst_dict = {}
-    for inst_uid, inst_info in inst_dict.items():
-        if inst_uid not in remove_insts_in_tile:
-            inst_info["box"] += np.concatenate([tile_tl] * 2)
-            inst_info["centroid"] += tile_tl
-            inst_info["contour"] += tile_tl
-            inst_uuid = uuid.uuid4().hex
-            new_inst_dict[inst_uuid] = inst_info
+    new_inst_dict, remove_insts_in_orig = _process_instance_predictions(
+        inst_dict,
+        ioconfig,
+        tile_shape,
+        tile_flag,
+        tile_mode,
+        tile_tl,
+        ref_inst_dict,
+    )
 
     return new_inst_dict, remove_insts_in_orig
 
 
 class NucleusInstanceSegmentor(SemanticSegmentor):
     """An engine specifically designed to handle tiles or WSIs inference.
 
@@ -417,22 +468,18 @@
             sel_boxes = [
                 shapely_box(0, 0, w, 0),  # top edge
                 shapely_box(0, h, w, h),  # bottom edge
                 shapely_box(0, 0, 0, h),  # left
                 shapely_box(w, 0, w, h),  # right
             ]
             geometries = [shapely_box(*bounds) for bounds in boxes]
-            # An auxiliary dictionary to actually query the index within the source list
-            index_by_id = {id(geo): idx for idx, geo in enumerate(geometries)}
             spatial_indexer = STRtree(geometries)
 
             for idx, sel_box in enumerate(sel_boxes):
-                sel_indices = [
-                    index_by_id[id(geo)] for geo in spatial_indexer.query(sel_box)
-                ]
+                sel_indices = list(spatial_indexer.query(sel_box))
                 removal_flag[sel_indices, idx] = 0
             return removal_flag
 
         w, h = image_shape
         boxes = tile_outputs
         #  expand to full four corners
         boxes_br = boxes[:, 2:]
@@ -644,16 +691,14 @@
         if mask_reader is not None:
             sel = self.filter_coordinates(mask_reader, patch_outputs, **resolution)
             patch_outputs = patch_outputs[sel]
             patch_inputs = patch_inputs[sel]
 
         # assume to be in [top_left_x, top_left_y, bot_right_x, bot_right_y]
         geometries = [shapely_box(*bounds) for bounds in patch_outputs]
-        # An auxiliary dictionary to actually query the index within the source list
-        index_by_id = {id(geo): idx for idx, geo in enumerate(geometries)}
         spatial_indexer = STRtree(geometries)
 
         # * retrieve tile placement and tile info flag
         # tile shape will always be corrected to be multiple of output
         tile_info_sets = self._get_tile_info(wsi_proc_shape, ioconfig)
 
         # ! running order of each set matters !
@@ -667,17 +712,15 @@
         for set_idx, (set_bounds, set_flags) in enumerate(tile_info_sets):
             for tile_idx, tile_bounds in enumerate(set_bounds):
                 tile_flag = set_flags[tile_idx]
 
                 # select any patches that have their output
                 # within the current tile
                 sel_box = shapely_box(*tile_bounds)
-                sel_indices = [
-                    index_by_id[id(geo)] for geo in spatial_indexer.query(sel_box)
-                ]
+                sel_indices = list(spatial_indexer.query(sel_box))
 
                 # there is nothing in the tile
                 # Ignore coverage as the condition is difficult
                 # to reproduce on travis.
                 if len(sel_indices) == 0:  # pragma: no cover
                     continue
 
@@ -725,15 +768,14 @@
             # !     will be deprecated upon finalization of SQL annotation store
             self._wsi_inst_info.update(new_inst_dict)
             for inst_uuid in remove_uuid_list:
                 self._wsi_inst_info.pop(inst_uuid, None)
             # !
 
         for future in self._futures:
-
             #  not actually future but the results
             if self._postproc_workers is None:
                 callback(*future)
                 continue
 
             # some errors happen, log it and propagate exception
             # ! this will lead to discard a bunch of
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/engine/patch_predictor.py` & `tiatoolbox-1.4.0/tiatoolbox/models/engine/patch_predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """This module implements patch level prediction."""
 
 import copy
 import os
 import pathlib
-import warnings
 from collections import OrderedDict
 from typing import Callable, Tuple, Union
 
 import numpy as np
 import torch
 import tqdm
 
+from tiatoolbox import logger
 from tiatoolbox.models.architecture import get_pretrained_model
 from tiatoolbox.models.dataset.classification import PatchDataset, WSIPatchDataset
 from tiatoolbox.models.engine.semantic_segmentor import IOSegmentorConfig
 from tiatoolbox.utils import misc
 from tiatoolbox.utils.misc import save_as_json
 from tiatoolbox.wsicore.wsireader import VirtualWSIReader, WSIReader
 
@@ -306,19 +306,18 @@
             ...    [2, 2, 0, 0],
             ...    [0, 0, 1, 1],
             ...    [0, 0, 1, 1]])
 
         """
         reader = WSIReader.open(img)
         if isinstance(reader, VirtualWSIReader):
-            warnings.warn(
-                (
-                    "Image is not pyramidal hence read is forced to be "
-                    "at `units='baseline'` and `resolution=1.0`."
-                )
+            logger.warning(
+                "Image is not pyramidal hence read is forced to be "
+                "at `units='baseline'` and `resolution=1.0`.",
+                stacklevel=2,
             )
             resolution = 1.0
             units = "baseline"
 
         canvas_shape = reader.slide_dimensions(resolution=resolution, units=units)
         canvas_shape = canvas_shape[::-1]  # XY to YX
 
@@ -415,15 +414,14 @@
         cum_output = {
             "probabilities": [],
             "predictions": [],
             "coordinates": [],
             "labels": [],
         }
         for _, batch_data in enumerate(dataloader):
-
             batch_output_probabilities = self.model.infer_batch(
                 model, batch_data["image"], on_gpu
             )
             # We get the index of the class with the maximum probability
             batch_output_predictions = self.model.postproc_func(
                 batch_output_probabilities
             )
@@ -534,25 +532,27 @@
 
         Returns:
             :class:`pathlib.Path`:
                 Path to output directory.
 
         """
         if save_dir is None and len(imgs) > 1:
-            warnings.warn(
+            logger.warning(
                 "More than 1 WSIs detected but there is no save directory set."
                 "All subsequent output will be saved to current runtime"
-                "location under folder 'output'. Overwriting may happen!"
+                "location under folder 'output'. Overwriting may happen!",
+                stacklevel=2,
             )
             save_dir = pathlib.Path(os.getcwd()).joinpath("output")
         elif save_dir is not None and len(imgs) > 1:
-            warnings.warn(
+            logger.warning(
                 "When providing multiple whole-slide images / tiles, "
                 "we save the outputs and return the locations "
-                "to the corresponding files."
+                "to the corresponding files.",
+                stacklevel=2,
             )
 
         if save_dir is not None:
             save_dir = pathlib.Path(save_dir)
             save_dir.mkdir(parents=True, exist_ok=False)
 
         return save_dir
@@ -861,18 +861,19 @@
                 f"len(masks) != len(imgs) : " f"{len(masks)} != {len(imgs)}"
             )
 
         ioconfig = self._update_ioconfig(
             ioconfig, patch_input_shape, stride_shape, resolution, units
         )
         if mode == "tile":
-            warnings.warn(
+            logger.warning(
                 "WSIPatchDataset only reads image tile at "
                 '`units="baseline"`. Resolutions will be converted '
-                "to baseline value."
+                "to baseline value.",
+                stacklevel=2,
             )
             ioconfig = ioconfig.to_baseline()
 
         fx_list = ioconfig.scale_to_highest(
             ioconfig.input_resolutions, ioconfig.input_resolutions[0]["units"]
         )
         fx_list = zip(fx_list, ioconfig.input_resolutions)
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/engine/semantic_segmentor.py` & `tiatoolbox-1.4.0/tiatoolbox/models/engine/semantic_segmentor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 
 import copy
 import logging
 import os
 import pathlib
 import shutil
-import warnings
 from concurrent.futures import ProcessPoolExecutor
 from multiprocessing.managers import Namespace
 from typing import Callable, List, Tuple, Union
 
 import cv2
 import joblib
 import numpy as np
 import torch
 import torch.multiprocessing as torch_mp
 import torch.utils.data as torch_data
 import tqdm
 
+from tiatoolbox import logger
 from tiatoolbox.models.architecture import get_pretrained_model
 from tiatoolbox.models.models_abc import IOConfigABC
 from tiatoolbox.tools.patchextraction import PatchExtractor
 from tiatoolbox.utils import misc
 from tiatoolbox.utils.misc import imread
 from tiatoolbox.wsicore.wsireader import VirtualWSIReader, WSIMeta, WSIReader
 
@@ -318,18 +318,19 @@
     ):
         super().__init__()
         self.mode = mode
         self.preproc = preproc
         self.ioconfig = copy.deepcopy(ioconfig)
 
         if mode == "tile":
-            warnings.warn(
+            logger.warning(
                 "WSIPatchDataset only reads image tile at "
                 '`units="baseline"`. Resolutions will be converted '
-                "to baseline value."
+                "to baseline value.",
+                stacklevel=2,
             )
             self.ioconfig = self.ioconfig.to_baseline()
 
         self.mp_shared_space = mp_shared_space
         self.wsi_paths = wsi_paths
         self.wsi_idx = None  # to be received externally via thread communication
         self.reader = None
@@ -988,20 +989,19 @@
             cum_canvas /= count_canvas + 1.0e-6
         return cum_canvas
 
     @staticmethod
     def _prepare_save_dir(save_dir):
         """Prepare save directory and cache."""
         if save_dir is None:
-            warnings.warn(
-                (
-                    "Segmentor will only output to directory. "
-                    "All subsequent output will be saved to current runtime "
-                    "location under folder 'output'. Overwriting may happen! "
-                )
+            logger.warning(
+                "Segmentor will only output to directory. "
+                "All subsequent output will be saved to current runtime "
+                "location under folder 'output'. Overwriting may happen! ",
+                stacklevel=2,
             )
             save_dir = os.path.join(os.getcwd(), "output")
 
         save_dir = os.path.abspath(save_dir)
         save_dir = pathlib.Path(save_dir)
         if save_dir.is_dir():
             raise ValueError(f"`save_dir` already exists! {save_dir}")
@@ -1073,18 +1073,19 @@
                 input_resolutions=[{"resolution": resolution, "units": units}],
                 output_resolutions=[{"resolution": resolution, "units": units}],
                 patch_input_shape=patch_input_shape,
                 patch_output_shape=patch_output_shape,
                 stride_shape=stride_shape,
             )
         if mode == "tile":
-            warnings.warn(
+            logger.warning(
                 "WSIPatchDataset only reads image tile at "
                 '`units="baseline"`. Resolutions will be converted '
-                "to baseline value."
+                "to baseline value.",
+                stacklevel=2,
             )
             return ioconfig.to_baseline()
 
         return ioconfig
 
     def _prepare_workers(self):
         """Prepare number of workers."""
@@ -1325,15 +1326,19 @@
         # => may not be able to retrieve the result dict
         for wsi_idx, img_path in enumerate(imgs):
             self._predict_wsi_handle_exception(
                 imgs, wsi_idx, img_path, mode, ioconfig, save_dir, crash_on_exception
             )
 
         # clean up the cache directories
-        shutil.rmtree(self._cache_dir)
+        try:
+            shutil.rmtree(self._cache_dir)
+        except PermissionError:  # pragma: no cover
+            logger.warning("Unable to remove %s", self._cache_dir)
+
         self._memory_cleanup()
 
         return self._outputs
 
 
 class DeepFeatureExtractor(SemanticSegmentor):
     """Generic CNN Feature Extractor.
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/models/models_abc.py` & `tiatoolbox-1.4.0/tiatoolbox/models/models_abc.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/tools/graph.py` & `tiatoolbox-1.4.0/tiatoolbox/tools/graph.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/tools/patchextraction.py` & `tiatoolbox-1.4.0/tiatoolbox/tools/patchextraction.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """This file defines patch extraction methods for deep learning models."""
-import warnings
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Callable, Tuple, Union
 
 import numpy as np
 from pandas import DataFrame
 
+from tiatoolbox import logger
 from tiatoolbox.utils import misc
 from tiatoolbox.utils.exceptions import MethodNotSupported
 from tiatoolbox.wsicore import wsireader
 
 
 class PatchExtractorABC(ABC):
     """Abstract base class for Patch Extraction in tiatoolbox."""
@@ -154,14 +154,17 @@
             )
         self.within_bound = within_bound
 
     def __iter__(self):
         self.n = 0
         return self
 
+    def __len__(self):
+        return self.locations_df.shape[0] if self.locations_df is not None else 0
+
     def __next__(self):
         n = self.n
 
         if n >= self.locations_df.shape[0]:
             raise StopIteration
         self.n = n + 1
         return self[n]
@@ -198,52 +201,41 @@
             image_shape=(slide_dimension[0], slide_dimension[1]),
             patch_input_shape=(self.patch_size[0], self.patch_size[1]),
             stride_shape=(self.stride[0], self.stride[1]),
             input_within_bound=self.within_bound,
         )
 
         if self.mask is not None:
-            # convert the coordinate_list resolution unit to acceptable units
-            converted_units = self.wsi.convert_resolution_units(
-                input_res=self.resolution,
-                input_unit=self.units,
-            )
-            # find the first unit which is not None
-            converted_units = {
-                k: v for k, v in converted_units.items() if v is not None
-            }
-            converted_units_keys = list(converted_units.keys())
-            selected_coord_indices = self.filter_coordinates_fast(
+            selected_coord_indices = self.filter_coordinates(
                 self.mask,
                 self.coordinate_list,
-                coordinate_resolution=converted_units[converted_units_keys[0]],
-                coordinate_units=converted_units_keys[0],
+                wsi_shape=slide_dimension,
                 min_mask_ratio=self.min_mask_ratio,
             )
             self.coordinate_list = self.coordinate_list[selected_coord_indices]
             if len(self.coordinate_list) == 0:
-                warnings.warn(
+                logger.warning(
                     "No candidate coordinates left after "
-                    "filtering by `input_mask` positions."
+                    "filtering by `input_mask` positions.",
+                    stacklevel=2,
                 )
 
         data = self.coordinate_list[:, :2]  # only use the x_start and y_start
 
         self.locations_df = misc.read_locations(input_table=np.array(data))
 
         return self
 
     @staticmethod
-    def filter_coordinates_fast(
+    def filter_coordinates(
         mask_reader: wsireader.VirtualWSIReader,
         coordinates_list: np.ndarray,
-        coordinate_resolution: float,
-        coordinate_units: str,
-        mask_resolution: float = None,
+        wsi_shape: Tuple[int, int],
         min_mask_ratio: float = 0,
+        func: Callable = None,
     ):
         """Validate patch extraction coordinates based on the input mask.
 
         This function indicates which coordinate is valid for mask-based
         patch extraction based on checks in low resolution.
 
         Args:
@@ -255,148 +247,81 @@
                 at the same resolution as requested `resolution` and
                 `units`. The shape of `coordinates_list` is (N, K) where
                 N is the number of coordinate sets and K is either 2 for
                 centroids or 4 for bounding boxes. When using the
                 default `func=None`, K should be 4, as we expect the
                 `coordinates_list` to be bounding boxes in `[start_x,
                 start_y, end_x, end_y]` format.
-            coordinate_resolution (float):
-                Resolution value at which `coordinates_list` is
-                generated.
-            coordinate_units (str):
-                Resolution unit at which `coordinates_list` is generated.
-            mask_resolution (float):
-                Resolution at which mask array is extracted. It is
-                supposed to be in the same units as `coord_resolution`
-                i.e., `coordinate_units`. If not provided, a default
-                value will be selected based on `coordinate_units`.
+            wsi_shape (tuple(int, int)):
+                Shape of the WSI in the requested `resolution` and `units`.
             min_mask_ratio (float):
                 Only patches with positive area percentage above this value are
-                included. Defaults to 0.
+                included. Defaults to 0. Has no effect if `func` is not `None`.
+            func (callable):
+                Function to be used to validate the coordinates. The function
+                must take a `numpy.ndarray` of the mask and a `numpy.ndarray`
+                of the coordinates as input and return a bool indicating
+                whether the coordinate is valid or not. If `None`, a default
+                function that accepts patches with positive area proportion above
+                `min_mask_ratio` is used.
+
 
         Returns:
             :class:`numpy.ndarray`:
                 list of flags to indicate which coordinate is valid.
 
         """
         if not isinstance(mask_reader, wsireader.VirtualWSIReader):
             raise ValueError("`mask_reader` should be wsireader.VirtualWSIReader.")
         if not isinstance(coordinates_list, np.ndarray) or not np.issubdtype(
             coordinates_list.dtype, np.integer
         ):
             raise ValueError("`coordinates_list` should be ndarray of integer type.")
         if coordinates_list.shape[-1] != 4:
             raise ValueError("`coordinates_list` must be of shape [N, 4].")
-        if isinstance(coordinate_resolution, (int, float)):
-            coordinate_resolution = [coordinate_resolution, coordinate_resolution]
 
         if not 0 <= min_mask_ratio <= 1:
             raise ValueError("`min_mask_ratio` must be between 0 and 1.")
 
-        # define default mask_resolution based on the input `coordinate_units`
-        if mask_resolution is None:
-            mask_res_dict = {"mpp": 8, "power": 1.25, "baseline": 0.03125}
-            mask_resolution = mask_res_dict[coordinate_units]
-
-        tissue_mask = mask_reader.slide_thumbnail(
-            resolution=mask_resolution, units=coordinate_units
-        )
+        # the tissue mask exists in the reader already, no need to generate it
+        tissue_mask = mask_reader.img
 
         # Scaling the coordinates_list to the `tissue_mask` array resolution
+        scale_factors = np.array(tissue_mask.shape[::-1]) / np.array(wsi_shape)
         scaled_coords = coordinates_list.copy().astype(np.float32)
-        scaled_coords[:, [0, 2]] *= coordinate_resolution[0] / mask_resolution
+        scaled_coords[:, [0, 2]] *= scale_factors[0]
         scaled_coords[:, [0, 2]] = np.clip(
             scaled_coords[:, [0, 2]], 0, tissue_mask.shape[1]
         )
-        scaled_coords[:, [1, 3]] *= coordinate_resolution[1] / mask_resolution
+        scaled_coords[:, [1, 3]] *= scale_factors[1]
         scaled_coords[:, [1, 3]] = np.clip(
             scaled_coords[:, [1, 3]], 0, tissue_mask.shape[0]
         )
         scaled_coords = list(np.int32(scaled_coords))
 
-        flag_list = []
-        for coord in scaled_coords:
+        def default_sel_func(tissue_mask, coord):
+            """Default selection function to filter coordinates.
+
+            This function selects a coordinate if the proportion of
+            positive mask in the corresponding patch is greater than
+            `min_mask_ratio`.
+
+            """
             this_part = tissue_mask[coord[1] : coord[3], coord[0] : coord[2]]
             patch_area = np.prod(this_part.shape)
             pos_area = np.count_nonzero(this_part)
-
-            if (
+            return (
                 (pos_area == patch_area) or (pos_area > patch_area * min_mask_ratio)
-            ) and (pos_area > 0 and patch_area > 0):
-                flag_list.append(True)
-            else:
-                flag_list.append(False)
-        return np.array(flag_list)
-
-    @staticmethod
-    def filter_coordinates(
-        mask_reader: wsireader.VirtualWSIReader,
-        coordinates_list: np.ndarray,
-        func: Callable = None,
-        resolution: float = None,
-        units: str = None,
-    ):
-        """Indicates which coordinate is valid for mask-based patch extraction.
-
-        Locations are validated by a custom or default filter `func`.
-
-        Args:
-            mask_reader (:class:`.VirtualReader`):
-                A virtual pyramidal reader of the mask related to the
-                WSI from which we want to extract the patches.
-            coordinates_list (ndarray and np.int32):
-                Coordinates to be checked via the `func`. They must be
-                in the same resolution as requested `resolution` and
-                `units`. The shape of `coordinates_list` is (N, K) where
-                N is the number of coordinate sets and K is either 2 for
-                centroids or 4 for bounding boxes. When using the
-                default `func=None`, K should be 4, as we expect the
-                `coordinates_list` to refer to bounding boxes in
-                `[start_x, start_y, end_x, end_y]` format.
-            func:
-                The coordinate validator function. A function that takes
-                `reader` and `coordinate` as arguments and return True
-                or False as indication of coordinate validity.
-            resolution (float):
-                The resolution value at which coordinates_list are
-                generated.
-            units (str):
-                The resolution unit at which coordinates_list are
-                generated.
-
-        Returns:
-            :class:`numpy.ndarray`:
-                List of flags to indicate which coordinates are valid.
-
-        """
+            ) and (pos_area > 0 and patch_area > 0)
 
-        def default_sel_func(reader: wsireader.VirtualWSIReader, coord: np.ndarray):
-            """Accept coord as long as its box contains bits of mask."""
-            roi = reader.read_bounds(
-                coord,
-                resolution=reader.info.mpp if resolution is None else resolution,
-                units="mpp" if units is None else units,
-                interpolation="nearest",
-                coord_space="resolution",
-            )
-            return np.sum(roi > 0) > 0
-
-        if not isinstance(mask_reader, wsireader.VirtualWSIReader):
-            raise ValueError("`mask_reader` should be wsireader.VirtualWSIReader.")
-        if not isinstance(coordinates_list, np.ndarray) or not np.issubdtype(
-            coordinates_list.dtype, np.integer
-        ):
-            raise ValueError("`coordinates_list` should be ndarray of integer type.")
-        if func is None and coordinates_list.shape[-1] != 4:
-            raise ValueError(
-                f"Default `func` does not support "
-                f"`coordinates_list` of shape {coordinates_list.shape}."
-            )
         func = default_sel_func if func is None else func
-        flag_list = [func(mask_reader, coord) for coord in coordinates_list]
+        flag_list = []
+        for coord in scaled_coords:
+            flag_list.append(func(tissue_mask, coord))
+
         return np.array(flag_list)
 
     @staticmethod
     def get_coordinates(
         image_shape: Union[Tuple[int, int], np.ndarray] = None,
         patch_input_shape: Union[Tuple[int, int], np.ndarray] = None,
         patch_output_shape: Union[Tuple[int, int], np.ndarray] = None,
@@ -689,15 +614,27 @@
             (self.patch_size[1] - 1) / 2
         )
         self.locations_df["y"] = self.locations_df["y"] - int(
             (self.patch_size[1] - 1) / 2
         )
 
 
-def get_patch_extractor(method_name: str, **kwargs: str):
+def get_patch_extractor(
+    method_name: str,
+    **kwargs: Union[
+        Path,
+        wsireader.WSIReader,
+        None,
+        str,
+        int,
+        Tuple[int, int],
+        float,
+        Tuple[float, float],
+    ],
+):
     """Return a patch extractor object as requested.
 
     Args:
         method_name (str):
             Name of patch extraction method, must be one of "point" or
             "slidingwindow". The method name is case-insensitive.
         **kwargs:
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/tools/pyramid.py` & `tiatoolbox-1.4.0/tiatoolbox/tools/pyramid.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 easily serialised via the use of an io.BytesIO object or saved directly
 to disk.
 
 """
 
 import tarfile
 import time
-import warnings
 import zipfile
 from io import BytesIO
 from pathlib import Path
 from typing import Iterable, Tuple, Union
 
 import defusedxml
 import numpy as np
 from PIL import Image
 
+from tiatoolbox import DuplicateFilter, logger
 from tiatoolbox.annotation.storage import AnnotationStore
 from tiatoolbox.utils.transforms import imresize, locsize2bounds
 from tiatoolbox.utils.visualization import AnnotationRenderer, random_colors
 from tiatoolbox.wsicore.wsireader import WSIMeta, WSIReader
 
 defusedxml.defuse_stdlib()
 
@@ -194,38 +194,39 @@
         if level > self.level_count:
             raise IndexError("Invalid level.")
 
         scale = self.level_downsample(level)
         baseline_x = (x * self.tile_size * scale) - (self.overlap * scale)
         baseline_y = (y * self.tile_size * scale) - (self.overlap * scale)
         output_size = [self.output_tile_size] * 2
-        coord = [int(baseline_x), int(baseline_y)]
+        coord = (int(baseline_x), int(baseline_y))
         if level < self.sub_tile_level_count:
             output_size = self.output_tile_size // 2 ** (
                 self.sub_tile_level_count - level
             )
             output_size = np.repeat(output_size, 2).astype(int)
             thumb = self.get_thumb_tile()
             thumb.thumbnail(output_size)
             return thumb
         slide_dimensions = np.array(self.wsi.info.slide_dimensions)
         if all(slide_dimensions < [baseline_x, baseline_y]):
             raise IndexError
 
-        # Don't print out any warnings about interpolation etc.
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            tile = self.wsi.read_rect(
-                coord,
-                size=[v * res for v in output_size],
-                resolution=res / scale,
-                units="baseline",
-                pad_mode=pad_mode,
-                interpolation=interpolation,
-            )
+        # Don't print out multiple warnings about interpolation etc.
+        duplicate_filter = DuplicateFilter()
+        logger.addFilter(duplicate_filter)
+        tile = self.wsi.read_rect(
+            coord,
+            size=[v * res for v in output_size],
+            resolution=res / scale,
+            units="baseline",
+            pad_mode=pad_mode,
+            interpolation=interpolation,
+        )
+        logger.removeFilter(duplicate_filter)
         return Image.fromarray(tile)
 
     def tile_path(self, level: int, x: int, y: int) -> Path:
         """Generate the path for a specified tile.
 
         Args:
             level (int):
@@ -488,15 +489,15 @@
 
         output_size = [self.output_tile_size] * 2
         self.empty_img = Image.fromarray(
             np.zeros((output_size[0], output_size[1], 4), dtype=np.uint8)
         )
         if self.renderer.mapper == "categorical":
             # get the possible categories for given score_prop from store
-            types = self.store.pquery(f"props['{self.renderer.score_prop}']")
+            types = self.store.pquery(f"props[{self.renderer.score_prop!r}]")
             # make a random dictionary colour map
             colors = random_colors(len(types))
             mapper = {key: (*color, 1) for key, color in zip(types, colors)}
             self.renderer.mapper = lambda x: mapper[x]
 
     def get_thumb_tile(self) -> Image:
         """Return a thumbnail which fits the whole slide in one tile.
@@ -578,16 +579,17 @@
             ...   info=wsi.info,
             ...   store=SQ,
             ... )
             >>> tile_0_0_0 = tile_generator.get_tile(level=0, x=0, y=0)
 
         """
         if pad_mode is not None or interpolation is not None:
-            warnings.warn(
-                "interpolation, pad_mode are unused by AnnotationTileGenerator"
+            logger.warning(
+                "interpolation, pad_mode are unused by AnnotationTileGenerator",
+                stacklevel=2,
             )
         if level < 0:
             raise IndexError
         if level > self.level_count:
             raise IndexError("Invalid level.")
 
         scale = self.level_downsample(level)
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/tools/registration/wsi_registration.py` & `tiatoolbox-1.4.0/tiatoolbox/tools/registration/wsi_registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import itertools
-import warnings
 from numbers import Number
 from typing import Dict, Tuple, Union
 
 import cv2
 import numpy as np
 import SimpleITK as sitk  # noqa: N813
 import torch
 import torchvision
 from numpy.linalg import inv
 from skimage import exposure, filters
 from skimage.registration import phase_cross_correlation
 from skimage.util import img_as_float
 
+from tiatoolbox import logger
 from tiatoolbox.tools.patchextraction import PatchExtractor
 from tiatoolbox.utils.metrics import dice
 from tiatoolbox.utils.transforms import imresize
 from tiatoolbox.wsicore.wsireader import VirtualWSIReader, WSIReader
 
 Resolution = Union[Number, Tuple[Number, Number], np.ndarray]
 IntBounds = Tuple[int, int, int, int]
@@ -82,14 +82,40 @@
     """
     moments = cv2.moments(mask)
     x_coord_center = moments["m10"] / moments["m00"]
     y_coord_center = moments["m01"] / moments["m00"]
     return (x_coord_center, y_coord_center)
 
 
+def apply_affine_transformation(fixed_img, moving_img, transform_initializer):
+    """Apply affine transformation using OpenCV.
+
+    Args:
+        fixed_img (:class:`numpy.ndarray`):
+            A fixed image.
+        moving_img (:class:`numpy.ndarray`):
+            A moving image.
+        transform_initializer (:class:`numpy.ndarray`):
+            A rigid transformation matrix.
+
+    Returns:
+        :class:`numpy.ndarray`:
+            A transformed image.
+
+    Examples:
+        >>> moving_image = apply_affine_transformation(
+        ...     fixed_image, moving_image, transform_initializer
+        ... )
+
+    """
+    return cv2.warpAffine(
+        moving_img, transform_initializer[0:-1][:], fixed_img.shape[:2][::-1]
+    )
+
+
 def prealignment(
     fixed_img: np.ndarray,
     moving_img: np.ndarray,
     fixed_mask: np.ndarray,
     moving_mask: np.ndarray,
     dice_overlap: float = 0.5,
     rotation_step: int = 10,
@@ -206,25 +232,24 @@
         all_transform.append(transform)
 
     if max(all_dice) >= dice_overlap:
         dice_after = max(all_dice)
         pre_transform = all_transform[all_dice.index(dice_after)]
 
         # Apply transformation to both image and mask
-        moving_img = cv2.warpAffine(
-            orig_moving_img, pre_transform[0:-1][:], orig_fixed_img.shape[:2][::-1]
-        )
-        moving_mask = cv2.warpAffine(
-            moving_mask, pre_transform[0:-1][:], fixed_img.shape[:2][::-1]
+        moving_img = apply_affine_transformation(
+            orig_fixed_img, orig_moving_img, pre_transform
         )
+        moving_mask = apply_affine_transformation(fixed_img, moving_mask, pre_transform)
+
         return pre_transform, moving_img, moving_mask, dice_after
 
-    warnings.warn(
+    logger.warning(
         "Not able to find the best transformation for pre-alignment. "
-        "Try changing the values for 'dice_overlap' and 'rotation_step'."
+        "Try changing the values for 'dice_overlap' and 'rotation_step'.",
     )
     return np.eye(3), moving_img, moving_mask, dice_before
 
 
 def match_histograms(
     image_a: np.ndarray, image_b: np.ndarray, kernel_size: int = 7
 ) -> Tuple[np.ndarray, np.ndarray]:
@@ -481,15 +506,15 @@
             np.repeat(np.expand_dims(features_x, axis=0), features_y.shape[0], axis=0)
             - np.repeat(
                 np.expand_dims(features_y, axis=1), features_x.shape[0], axis=1
             ),
             axis=len(features_x.shape),
         )
 
-        feature_size_2d = np.int(np.sqrt(feature_distance.shape[0]))
+        feature_size_2d = np.int_(np.sqrt(feature_distance.shape[0]))
         ref_feature_size_2d = factor * feature_size_2d
         feature_size, ref_feature_size = feature_size_2d**2, ref_feature_size_2d**2
         feature_grid = np.kron(
             np.arange(feature_size).reshape([feature_size_2d, feature_size_2d]),
             np.ones([factor, factor], dtype="int32"),
         )
         row_ind = np.repeat(
@@ -711,16 +736,16 @@
         kernel = np.ones((25, 25), np.uint8)
         mask = cv2.dilate(mask, kernel, iterations=1)
         mask_reader = VirtualWSIReader(mask)
 
         # convert coordinates of shape [N, 2] to [N, 4]
         end_x_y = points[:, 0:2] + 1
         bbox_coord = np.c_[points, end_x_y].astype(int)
-        return PatchExtractor.filter_coordinates_fast(
-            mask_reader, bbox_coord, 1.0, "baseline", 1.0
+        return PatchExtractor.filter_coordinates(
+            mask_reader, bbox_coord, mask.shape[::-1]
         )
 
     def filtering_matching_points(
         self,
         fixed_mask: np.ndarray,
         moving_mask: np.ndarray,
         fixed_matched_points: np.ndarray,
@@ -845,20 +870,21 @@
         )
 
         tissue_transform = DFBRegister.estimate_affine_transform(
             fixed_matched_points, moving_matched_points
         )
 
         # Apply transformation
-        moving_img = cv2.warpAffine(
-            moving_img, tissue_transform[0:-1][:], fixed_img.shape[:2][::-1]
+        moving_img = apply_affine_transformation(
+            fixed_img, moving_img, tissue_transform
         )
-        moving_mask = cv2.warpAffine(
-            moving_mask, tissue_transform[0:-1][:], fixed_img.shape[:2][::-1]
+        moving_mask = apply_affine_transformation(
+            fixed_img, moving_mask, tissue_transform
         )
+
         return tissue_transform, moving_img, moving_mask
 
     def perform_dfbregister_block_wise(
         self,
         fixed_img: np.ndarray,
         moving_img: np.ndarray,
         fixed_mask: np.ndarray,
@@ -958,19 +984,17 @@
         )
 
         block_transform = DFBRegister.estimate_affine_transform(
             fixed_matched_points, moving_matched_points
         )
 
         # Apply transformation
-        moving_img = cv2.warpAffine(
-            moving_img, block_transform[0:-1][:], fixed_img.shape[:2][::-1]
-        )
-        moving_mask = cv2.warpAffine(
-            moving_mask, block_transform[0:-1][:], fixed_img.shape[:2][::-1]
+        moving_img = apply_affine_transformation(fixed_img, moving_img, block_transform)
+        moving_mask = apply_affine_transformation(
+            fixed_img, moving_mask, block_transform
         )
 
         return block_transform, moving_img, moving_mask
 
     def register(
         self,
         fixed_img: np.ndarray,
@@ -1020,20 +1044,21 @@
         # Perform Pre-alignment
         if transform_initializer is None:
             transform_initializer, moving_img, moving_mask, before_dice = prealignment(
                 fixed_img, moving_img, fixed_mask, moving_mask
             )
         else:
             # Apply transformation to both image and mask
-            moving_img = cv2.warpAffine(
-                moving_img, transform_initializer[0:-1][:], fixed_img.shape[:2][::-1]
+            moving_img = apply_affine_transformation(
+                fixed_img, moving_img, transform_initializer
             )
-            moving_mask = cv2.warpAffine(
-                moving_mask, transform_initializer[0:-1][:], fixed_img.shape[:2][::-1]
+            moving_mask = apply_affine_transformation(
+                fixed_img, moving_mask, transform_initializer
             )
+
             before_dice = dice(fixed_mask, moving_mask)
 
         # Estimate transform using tissue regions
         (
             fixed_tissue_img,
             fixed_tissue_mask,
             moving_tissue_img,
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/tools/stainaugment.py` & `tiatoolbox-1.4.0/tiatoolbox/tools/stainaugment.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         self.sigma1 = sigma1
         self.sigma2 = sigma2
         self.method = method
         self.stain_matrix = stain_matrix
 
         if self.method.lower() not in {"macenko", "vahadane"}:
             raise ValueError(
-                f"Unsupported stain extractor method '{self.method}' for "
+                f"Unsupported stain extractor method {self.method!r} for "
                 "StainAugmentor. Choose either 'vahadane' or 'macenko'."
             )
         self.stain_normalizer = get_normalizer(self.method.lower())
 
         self.alpha = None
         self.beta = None
         self.img_shape = None
@@ -154,15 +154,18 @@
             self.stain_matrix = self.stain_normalizer.stain_matrix_target
             self.source_concentrations = self.stain_normalizer.target_concentrations
         else:
             self.source_concentrations = self.stain_normalizer.get_concentrations(
                 img, self.stain_matrix
             )
         self.n_stains = self.source_concentrations.shape[1]
-        self.tissue_mask = get_luminosity_tissue_mask(img, threshold=threshold).ravel()
+        if not self.augment_background:
+            self.tissue_mask = get_luminosity_tissue_mask(
+                img, threshold=threshold
+            ).ravel()
         self.img_shape = img.shape
 
     def augment(self):
         """Return an augmented instance based on source stain concentrations.
 
         Stain concentrations of the source image are altered (scaled and
         shifted) based on the random alpha and beta parameters, and then
@@ -187,15 +190,15 @@
         img_augmented = 255 * np.exp(
             -1 * np.dot(augmented_concentrations, self.stain_matrix)
         )
         img_augmented = img_augmented.reshape(self.img_shape)
         img_augmented = np.clip(img_augmented, 0, 255)
         return np.uint8(img_augmented)
 
-    def apply(self, img, **params):  # alpha=None, beta=None,
+    def apply(self, img, **params):  # alpha=None, beta=None,  # skipcq: PYL-W0613
         """Call the `fit` and `augment` functions to generate a stain augmented image.
 
         Args:
             img (:class:`numpy.ndarray`):
                 Input RGB image in the form of unit8 numpy array.
 
         Returns:
@@ -209,14 +212,15 @@
 
     def get_params(self):
         """Returns randomly generated parameters based on input arguments."""
         self.alpha = random.uniform(1 - self.sigma1, 1 + self.sigma1)
         self.beta = random.uniform(-self.sigma2, self.sigma2)
         return {}
 
-    def get_params_dependent_on_targets(self, params):
+    def get_params_dependent_on_targets(self, params):  # skipcq: PYL-W0613, PYL-R0201
         """Does nothing, added to resolve flake 8 error"""
         return {}
 
-    def get_transform_init_args_names(self):
+    @staticmethod
+    def get_transform_init_args_names(**kwargs):
         """Return the argument names for albumentations use."""
-        return ("method", "stain_matrix", "sigma1", "sigma2", "augment_background")
+        return "method", "stain_matrix", "sigma1", "sigma2", "augment_background"
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/tools/stainextract.py` & `tiatoolbox-1.4.0/tiatoolbox/tools/stainextract.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/tools/stainnorm.py` & `tiatoolbox-1.4.0/tiatoolbox/tools/stainnorm.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/tools/tissuemask.py` & `tiatoolbox-1.4.0/tiatoolbox/tools/tissuemask.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         Returns:
             :class:`numpy.ndarray`:
                 Map of semantic classes spatially over the WSI
                 e.g. regions of tissue vs background.
 
         """
         if not self.fitted:
-            raise Exception("Fit must be called before transform.")
+            raise SyntaxError("Fit must be called before transform.")
 
     def fit_transform(self, images: np.ndarray, **kwargs) -> np.ndarray:
         """Perform :func:`fit` then :func:`transform`.
 
         Sometimes it can be more optimal to perform both at the same
         time for a single sample. In this case the base implementation
         of :func:`fit` followed by :func:`transform` can be overridden.
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/utils/env_detection.py` & `tiatoolbox-1.4.0/tiatoolbox/utils/env_detection.py`

 * *Files identical despite different names*

### Comparing `tiatoolbox-1.3.3/tiatoolbox/utils/image.py` & `tiatoolbox-1.4.0/tiatoolbox/utils/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Miscellaneous utilities which operate on image data."""
-import warnings
 from typing import Tuple, Union
 
 import numpy as np
 from PIL import Image
 
+from tiatoolbox import logger
 from tiatoolbox.utils.misc import conv_out_size
 from tiatoolbox.utils.transforms import (
     bounds2locsize,
     bounds2slices,
     imresize,
     locsize2bounds,
     pad_bounds,
@@ -543,15 +543,17 @@
     padding = normalize_padding_size(padding)
 
     # Check the bounds are valid or have a negative size
     # The left/start_x and top/start_y values should usually be smaller
     # than the right/end_x and bottom/end_y values.
     bounds, fliplr, flipud = make_bounds_size_positive(bounds)
     if fliplr or flipud:
-        warnings.warn("Bounds have a negative size, output will be flipped.")
+        logger.warning(
+            "Bounds have a negative size, output will be flipped.", stacklevel=2
+        )
 
     if isinstance(image, Image.Image):
         image = np.array(image)
 
     # Normalize none pad_mode to None
     if pad_mode.lower() == "none":
         pad_mode = None
@@ -568,15 +570,14 @@
             bounds2locsize(find_overlap(*bounds2locsize(bounds), image_size))[1]
             * scaling
         ).astype(int)
 
     overlap_bounds = find_overlap(*bounds2locsize(bounds), image_size=image_size)
     if pad_mode is None:
         read_bounds = overlap_bounds
-    pad_width = np.zeros((2, 2), int)
 
     baseline_padding = padding
     if not pad_at_baseline:
         baseline_padding = padding * np.tile(scaling, 2)
 
     # Check the padded bounds do not have zero size
     _, padded_bounds_size = bounds2locsize(pad_bounds(bounds, baseline_padding))
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/utils/metrics.py` & `tiatoolbox-1.4.0/tiatoolbox/utils/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,13 +86,13 @@
         :class:`float`:
             A dice overlap
 
     """
     if gt_mask.shape != pred_mask.shape:
         raise ValueError(f'{"Shape mismatch between the two masks."}')
 
-    gt_mask = gt_mask.astype(np.bool)
-    pred_mask = pred_mask.astype(np.bool)
+    gt_mask = gt_mask.astype(np.bool_)
+    pred_mask = pred_mask.astype(np.bool_)
     sum_masks = gt_mask.sum() + pred_mask.sum()
     if sum_masks == 0:
         return np.NAN
     return 2 * np.logical_and(gt_mask, pred_mask).sum() / sum_masks
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/utils/misc.py` & `tiatoolbox-1.4.0/tiatoolbox/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Miscellaneous small functions repeatedly used in tiatoolbox."""
 import copy
 import json
 import os
 import pathlib
-import warnings
 import zipfile
 from typing import IO, Dict, Optional, Tuple, Union
 
 import cv2
 import joblib
 import numpy as np
 import pandas as pd
 import requests
 import torch
 import yaml
 from shapely.affinity import translate
 from shapely.geometry import shape as feature2geometry
 from skimage import exposure
 
+from tiatoolbox import logger
 from tiatoolbox.annotation.storage import Annotation, AnnotationStore, SQLiteStore
 from tiatoolbox.utils.exceptions import FileNotSupported
 
 
 def split_path_name_ext(full_path):
     """Split path of a file to directory path, file name and extensions.
 
@@ -853,15 +853,15 @@
     """
     if np.any(scale_factor > 1.0):
         return "cubic"
     return "area"
 
 
 def store_from_dat(
-    fp: Union[IO, str],
+    fp: Union[IO, str, pathlib.Path],
     scale_factor: Tuple[float, float] = (1, 1),
     typedict: Optional[Dict] = None,
     origin: Tuple[float, float] = (0, 0),
     cls: AnnotationStore = SQLiteStore,
 ) -> "AnnotationStore":
     """Load annotations from a hovernet-style .dat file.
 
@@ -910,15 +910,15 @@
 
     """
     if origin != (0, 0):
         # transform coords to be relative to given pt.
         poly = translate(poly, -origin[0], -origin[1])
     if poly.is_valid:
         return poly
-    warnings.warn("Invalid geometry found, fix using buffer().")
+    logger.warning("Invalid geometry found, fix using buffer().", stacklevel=3)
     return poly.buffer(0.01)
 
 
 def anns_from_hoverdict(data, props, typedict, origin, scale_factor):
     """Helper function to create list of Annotation objects.
 
     Creates annotations from a hovernet-style dict of segmentations, mapping types
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/utils/transforms.py` & `tiatoolbox-1.4.0/tiatoolbox/utils/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     # a list of (original type, converted type) tuple
     # all `converted type` are np.dtypes that cv2.resize
     # can work on out-of-the-box (anything else will cause
     # error). The `converted type` has been selected so that
     # they can maintain the numeric precision of the `original type`.
     dtype_mapping = [
-        (np.bool, np.uint8),
+        (np.bool_, np.uint8),
         (np.int8, np.int16),
         (np.int16, np.int16),
         (np.int32, np.float32),
         (np.uint8, np.uint8),
         (np.uint16, np.uint16),
         (np.uint32, np.float32),
         (np.int64, np.float64),
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/utils/visualization.py` & `tiatoolbox-1.4.0/tiatoolbox/utils/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Visualisation and overlay functions used in tiatoolbox."""
 import colorsys
 import random
-import warnings
 from typing import Dict, List, Tuple, Union
 
 import cv2
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
-from matplotlib import cm
+from matplotlib import colormaps
 from numpy.typing import ArrayLike
 from PIL import Image, ImageFilter, ImageOps
 from shapely import speedups
 from shapely.geometry import Polygon
 
+from tiatoolbox import logger
 from tiatoolbox.annotation.storage import Annotation, AnnotationStore
 
 if speedups.available:  # pragma: no branch
     speedups.enable()
 
 
 def random_colors(num_colors, bright=True):
@@ -54,15 +54,15 @@
             Colormap to use, must be a valid matplotlib cmap string.
 
     Returns:
         img(ndarray): An RGB image.
     """
     if len(img.shape) == 2:
         # Single channel, make into rgb with colormap.
-        c_map = cm.get_cmap(cmap)
+        c_map = colormaps[cmap]
         im_rgb = (c_map(img) * 255).astype(np.uint8)
         return im_rgb[:, :, :3]
     # Already rgb, return unaltered
     return img
 
 
 def overlay_prediction_mask(
@@ -552,17 +552,17 @@
         thickness=-1,
         edge_thickness=1,
         secondary_cmap=None,
         blur_radius=0,
         score_prop_edge=None,
     ):
         if mapper is None:
-            mapper = cm.get_cmap("jet")
+            mapper = colormaps["jet"]
         if isinstance(mapper, str) and mapper != "categorical":
-            mapper = cm.get_cmap(mapper)
+            mapper = colormaps[mapper]
         if isinstance(mapper, list):
             colors = random_colors(len(mapper))
             mapper = {key: (*color, 1) for key, color in zip(mapper, colors)}
         if isinstance(mapper, dict):
             self.mapper = lambda x: mapper[x]
         else:
             self.mapper = mapper
@@ -636,15 +636,18 @@
                 return tuple(
                     int(c * 255)
                     for c in self.mapper(
                         self.score_fn(annotation.properties[score_prop])
                     )
                 )
         except KeyError:
-            warnings.warn("score_prop not found in properties. Using default color.")
+            logger.warning(
+                "'score_prop' not found in properties. Using default color.",
+                stacklevel=2,
+            )
         if edge:
             return (0, 0, 0, 255)  # default to black for edge
         return 0, 255, 0, 255  # default color if no score_prop given
 
     def render_poly(
         self,
         tile: np.ndarray,
@@ -866,8 +869,8 @@
         elif geom_type == "Polygon":
             self.render_poly(tile, annotation, top_left, scale)
         elif geom_type == "MultiPolygon":
             self.render_multipoly(tile, annotation, top_left, scale)
         elif geom_type == "LineString":
             self.render_line(tile, annotation, top_left, scale)
         else:
-            warnings.warn(f"Unknown geometry: {geom_type}")
+            logger.warning("Unknown geometry: %s", geom_type, stacklevel=3)
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/visualization/tileserver.py` & `tiatoolbox-1.4.0/tiatoolbox/visualization/tileserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 
         # Generic layer names if none provided.
         if isinstance(layers, list):
             layers = {f"layer-{i}": p for i, p in enumerate(layers)}
         # Set up the layer dict.
         meta = None
         for i, (key, layer) in enumerate(layers.items()):
-
             layer = self._get_layer_as_wsireader(layer, meta)
 
             self.tia_layers[key] = layer
 
             if isinstance(layer, WSIReader):
                 self.tia_pyramids[key] = ZoomifyGenerator(layer)
             else:
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/wsicore/metadata/ngff.py` & `tiatoolbox-1.4.0/tiatoolbox/wsicore/metadata/ngff.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,10 +262,12 @@
         _ARRAY_DIMENSIONS (List[TCZYX]):
             The dimensions of the array, for xarray compatibility.
         omero (Omero):
             Information about the display of image data.
     """
 
     _creator: Creator = field(default_factory=Creator)
-    multiscales: List[Multiscales] = field(default_factory=lambda: [Multiscales()])
+    multiscales: Union[Multiscales, List[Multiscales]] = field(
+        default_factory=lambda: [Multiscales()]
+    )
     _ARRAY_DIMENSIONS: List[TCZYX] = field(default_factory=lambda: ["y", "x", "c"])
     omero: Omero = field(default_factory=Omero)
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/wsicore/wsimeta.py` & `tiatoolbox-1.4.0/tiatoolbox/wsicore/wsimeta.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 With this class, metadata is in a normalized consistent format
 which is quite useful when working with many different WSI formats.
 The raw metadata is also preserved and accessible via a dictionary. The
 format of this dictionary may vary between WSI formats.
 
 """
-import warnings
 from numbers import Number
 from pathlib import Path
 from typing import List, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
+from tiatoolbox import logger
+
 Resolution = Union[Number, Tuple[Number, Number], np.ndarray]
 
 
 class WSIMeta:
     """Whole slide image metadata class.
 
     Args:
@@ -138,45 +139,45 @@
 
         """
         passed = True
 
         # Fatal conditions: Should return False if not True
 
         if len(set(self.axes) - set(self._valid_axes_characters)) > 0:
-            warnings.warn(
-                "Axes contains invalid characters. "
-                f"Valid characters are '{self._valid_axes_characters}'."
+            logger.warning(
+                "Axes contains invalid characters. Valid characters are %s.",
+                self._valid_axes_characters,
             )
             passed = False
 
         if self.level_count < 1:
-            warnings.warn("Level count is not a positive integer")
+            logger.warning("Level count is not a positive integer.")
             passed = False
 
         if self.level_dimensions is None:
-            warnings.warn("level_dimensions is None")
+            logger.warning("'level_dimensions' is None.")
             passed = False
         elif len(self.level_dimensions) != self.level_count:
-            warnings.warn("Length of level dimensions != level count")
+            logger.warning("Length of level dimensions != level count")
             passed = False
 
         if self.level_downsamples is None:
-            warnings.warn("Level downsamples is None")
+            logger.warning("Level downsamples is None.")
             passed = False
         elif len(self.level_downsamples) != self.level_count:
-            warnings.warn("Length of level downsamples != level count")
+            logger.warning("Length of level downsamples != level count")
             passed = False
 
         # Non-fatal conditions: Raise warning only, do not fail validation
 
         if self.raw is None:
-            warnings.warn("Raw data is None")
+            logger.warning("Raw data is None.")
 
         if all(x is None for x in [self.objective_power, self.mpp]):
-            warnings.warn("Unknown scale (no objective_power or mpp)")
+            logger.warning("Unknown scale (no objective_power or mpp)")
 
         return passed  # noqa
 
     def level_downsample(
         self,
         level: Union[int, float],
     ) -> float:
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox/wsicore/wsireader.py` & `tiatoolbox-1.4.0/tiatoolbox/wsicore/wsireader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 """This module defines classes which can read image data from WSI formats."""
 from __future__ import annotations
 
 import copy
 import json
+import logging
 import math
 import os
 import pathlib
 import re
-import warnings
 from datetime import datetime
 from numbers import Number
 from typing import Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import openslide
 import pandas as pd
 import tifffile
 import zarr
 from defusedxml import ElementTree
+from packaging.version import Version
 from PIL import Image
 
-from tiatoolbox import utils
+from tiatoolbox import logger, utils
 from tiatoolbox.annotation.storage import AnnotationStore, SQLiteStore
 from tiatoolbox.utils.env_detection import pixman_warning
 from tiatoolbox.utils.exceptions import FileNotSupported
 from tiatoolbox.utils.visualization import AnnotationRenderer
 from tiatoolbox.wsicore.metadata.ngff import Multiscales
 from tiatoolbox.wsicore.wsimeta import WSIMeta
 
 pixman_warning()
 
 NumPair = Tuple[Number, Number]
 IntPair = Tuple[int, int]
 Bounds = Tuple[Number, Number, Number, Number]
 IntBounds = Tuple[int, int, int, int]
 Resolution = Union[Number, Tuple[Number, Number], np.ndarray]
+MIN_NGFF_VERSION = Version("0.4")
+MAX_NGFF_VERSION = Version("0.4")
 
 
 def is_dicom(path: pathlib.Path) -> bool:
     """Check if the input is a DICOM file.
 
     Args:
         path (pathlib.Path): Path to the file to check.
@@ -92,15 +95,19 @@
         _ = zarr.open(path, mode="r")
         return True
 
     except Exception:  # noqa: PIE786  # skipcq: PYL-W0703
         return False
 
 
-def is_ngff(path: pathlib.Path, min_version: Tuple[int, ...] = (0, 4)) -> bool:
+def is_ngff(
+    path: pathlib.Path,
+    min_version: Version = MIN_NGFF_VERSION,
+    max_version: Version = MAX_NGFF_VERSION,
+) -> bool:
     """Check if the input is a NGFF file.
 
     Args:
         path (pathlib.Path):
             Path to the file to check.
         min_version (Tuple[int, ...]):
             Minimum version of the NGFF file to be considered valid.
@@ -124,26 +131,69 @@
             [
                 isinstance(multiscales, list),
                 isinstance(_ARRAY_DIMENSIONS, list),
                 isinstance(omero, dict),
                 all(isinstance(m, dict) for m in multiscales),
             ]
         ):
+            logger.warning(
+                "The NGFF file is not valid. "
+                "The multiscales, _ARRAY_DIMENSIONS and omero attributes "
+                "must be present and of the correct type."
+            )
             return False
     except KeyError:
         return False
-    multiscales_versions = tuple(
-        tuple(int(part) for part in scale.get("version", "").split("."))
-        for scale in multiscales
-    )
-    omero_version = tuple(int(part) for part in omero.get("version", "").split("."))
+    multiscales_versions = {
+        Version(scale["version"]) for scale in multiscales if "version" in scale
+    }
+    omero_version: Optional[str] = omero.get("version")
+    if omero_version:
+        omero_version: Version = Version(omero_version)
+        if omero_version < min_version:
+            logger.warning(
+                "The minimum supported version of the NGFF file is %s. "
+                "But the versions of the multiscales in the file are %s.",
+                min_version,
+                multiscales_versions,
+            )
+            return False
+        if omero_version > max_version:
+            logger.warning(
+                "The maximum supported version of the NGFF file is %s. "
+                "But the versions of the multiscales in the file are %s.",
+                max_version,
+                multiscales_versions,
+            )
+            return True
+
+    if len(multiscales_versions) > 1:
+        logger.warning(
+            "Found multiple versions for NGFF multiscales: %s",
+            multiscales_versions,
+        )
+
     if any(version < min_version for version in multiscales_versions):
+        logger.warning(
+            "The minimum supported version of the NGFF file is %s. "
+            "But the versions of the multiscales in the file are %s.",
+            min_version,
+            multiscales_versions,
+        )
         return False
-    if omero_version < min_version:
-        return False
+
+    if any(version > max_version for version in multiscales_versions):
+        logger.warning(
+            "The maximum supported version of the NGFF file is %s. "
+            "But the versions of the multiscales in the file are %s.",
+            max_version,
+            multiscales_versions,
+        )
+        return True
+
     return is_zarr(path)
 
 
 class WSIReader:
     """Base whole slide image (WSI) reader class.
 
     This class defines functions for reading pixel data and metadata
@@ -417,19 +467,19 @@
             reverse_index = np.argmax(level_resolution_sufficient[::-1])
             # Convert the index from the reversed list to the regular index (level)
             level = (len(level_scales) - 1) - reverse_index
         scale = level_scales[level]
 
         # Check for requested resolution > than baseline resolution
         if any(np.array(scale) > 1):
-            warnings.warn(
+            logger.warning(
                 "Read: Scale > 1."
                 "This means that the desired resolution is higher"
                 " than the WSI baseline (maximum encoded resolution)."
-                " Interpolation of read regions may occur."
+                " Interpolation of read regions may occur.",
             )
         return level, scale
 
     def find_read_rect_params(
         self,
         location: IntPair,
         size: IntPair,
@@ -645,15 +695,20 @@
             >>> from tiatoolbox.wsicore.wsireader import WSIReader
             >>> wsi = WSIReader.open(input_img="./CMU-1.ndpi")
             >>> slide_shape = wsi.slide_dimensions(0.55, 'mpp')
 
         """
         wsi_shape_at_baseline = self.info.slide_dimensions
         # Find parameters for optimal read
-        (_, _, wsi_shape_at_resolution, _,) = self._find_read_bounds_params(
+        (
+            _,
+            _,
+            wsi_shape_at_resolution,
+            _,
+        ) = self._find_read_bounds_params(
             [0, 0] + list(wsi_shape_at_baseline), resolution, units, precisions
         )
         return wsi_shape_at_resolution
 
     def _find_read_bounds_params(
         self, bounds: Bounds, resolution: Resolution, units: str, precision: int = 3
     ) -> Tuple[int, IntBounds, IntPair, IntPair, np.ndarray]:
@@ -831,19 +886,18 @@
         )
 
         output_dict = self._prepare_output_dict(
             input_unit, input_res, baseline_mpp, baseline_power
         )
         out_res = output_dict[output_unit] if output_unit is not None else output_dict
         if out_res is None:
-            warnings.warn(
+            logger.warning(
                 "Although unit conversion from input_unit has been done, the requested "
                 "output_unit is returned as None. Probably due to missing 'mpp' or "
                 "'objective_power' in slide's meta data.",
-                UserWarning,
             )
         return out_res
 
     def _find_tile_params(
         self, tile_objective_value: Number
     ) -> Tuple[int, IntPair, int, Number]:
         """Find the params for save tiles."""
@@ -853,38 +907,36 @@
                 "Tile objective value must be an integer multiple of the "
                 "objective power of the slide."
             )
         try:
             level = np.log2(rescale)
             if not level.is_integer():
                 raise ValueError
-            level = np.int(level)
+            level = np.int_(level)
             slide_dimension = self.info.level_dimensions[level]
             rescale = 1
         # Raise index error if desired pyramid level not embedded
         # in level_dimensions
         except IndexError:
             level = 0
             slide_dimension = self.info.level_dimensions[level]
-            rescale = np.int(rescale)
-            warnings.warn(
-                "Reading WSI at level 0. Desired tile_objective_value"
-                + str(tile_objective_value)
-                + "not available.",
-                UserWarning,
+            rescale = np.int_(rescale)
+            logger.warning(
+                "Reading WSI at level 0. Desired tile_objective_value %s "
+                "not available.",
+                str(tile_objective_value),
             )
         except ValueError:
             level = 0
             slide_dimension = self.info.level_dimensions[level]
             rescale = 1
-            warnings.warn(
-                "Reading WSI at level 0. Reading at tile_objective_value"
-                + str(tile_objective_value)
-                + "not allowed.",
-                UserWarning,
+            logger.warning(
+                "Reading WSI at level 0. Reading at tile_objective_value %s "
+                "not allowed.",
+                str(tile_objective_value),
             )
             tile_objective_value = self.info.objective_power
 
         return level, slide_dimension, rescale, tile_objective_value
 
     def _read_rect_at_resolution(
         self,
@@ -970,14 +1022,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -1161,14 +1217,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -1322,59 +1382,63 @@
         elif method == "otsu":
             masker = tissuemask.OtsuTissueMasker(**masker_kwargs)
         mask_img = masker.fit_transform([thumbnail])[0]
         return VirtualWSIReader(mask_img.astype(np.uint8), info=self.info, mode="bool")
 
     def save_tiles(
         self,
-        output_dir: Union[str, pathlib.Path],
-        tile_objective_value: int,
-        tile_read_size: Tuple[int, int],
+        output_dir: Union[str, pathlib.Path] = "tiles",
+        tile_objective_value: int = 20,
+        tile_read_size: Tuple[int, int] = (5000, 5000),
         tile_format: str = ".jpg",
-        verbose: bool = True,
+        verbose: bool = False,
     ) -> None:
         """Generate image tiles from whole slide images.
 
         Args:
             output_dir(str or :obj:`pathlib.Path`):
                 Output directory to save the tiles.
             tile_objective_value (int):
-                Objective value at which tile is generated.
+                Objective value at which tile is generated, default = 20
             tile_read_size (tuple(int)):
-                Tile (width, height).
+                Tile (width, height), default = (5000, 5000).
             tile_format (str):
-                File format to save image tiles, defaults to ".jpg".
+                File format to save image tiles, defaults = ".jpg".
             verbose (bool):
-                Print output, default to True.
+                Print output, default=False
 
         Examples:
             >>> from tiatoolbox.wsicore.wsireader import WSIReader
             >>> wsi = WSIReader.open(input_img="./CMU-1.ndpi")
             >>> wsi.save_tiles(output_dir='./dev_test',
             ...     tile_objective_value=10,
             ...     tile_read_size=(2000, 2000))
 
             >>> from tiatoolbox.wsicore.wsireader import WSIReader
             >>> wsi = WSIReader.open(input_img="./CMU-1.ndpi")
             >>> slide_param = wsi.info
 
         """
+        if verbose:
+            logger.setLevel(logging.DEBUG)
+
+        logger.debug("Processing %s.", self.input_path.name)
+
         output_dir = pathlib.Path(output_dir, self.input_path.name)
 
         level, slide_dimension, rescale, tile_objective_value = self._find_tile_params(
             tile_objective_value
         )
 
         tile_read_size = np.multiply(tile_read_size, rescale)
         slide_h = slide_dimension[1]
         slide_w = slide_dimension[0]
         tile_h = tile_read_size[1]
         tile_w = tile_read_size[0]
 
-        iter_tot = 0
         output_dir = pathlib.Path(output_dir)
         output_dir.mkdir(parents=True)
         data = []
 
         vertical_tiles = int(math.ceil((slide_h - tile_h) / tile_h + 1))
         horizontal_tiles = int(math.ceil((slide_w - tile_w) / tile_w + 1))
         for iter_tot, (h, w) in enumerate(np.ndindex(vertical_tiles, horizontal_tiles)):
@@ -1388,34 +1452,25 @@
 
             # convert to baseline reference frame
             bounds = start_w, start_h, end_w, end_h
             baseline_bounds = tuple(bound * (2**level) for bound in bounds)
             # Read image region
             im = self.read_bounds(baseline_bounds, level)
 
-            if verbose:
-                format_str = (
-                    "Tile%d:  start_w:%d, end_w:%d, "
-                    "start_h:%d, end_h:%d, "
-                    "width:%d, height:%d"
-                )
-
-                print(
-                    format_str
-                    % (
-                        iter_tot,
-                        start_w,
-                        end_w,
-                        start_h,
-                        end_h,
-                        end_w - start_w,
-                        end_h - start_h,
-                    ),
-                    flush=True,
-                )
+            logger.debug(
+                "Tile %d:  start_w: %d, end_w: %d, start_h: %d, end_h: %d, "
+                "width: %d, height: %d",
+                iter_tot,
+                start_w,
+                end_w,
+                start_h,
+                end_h,
+                end_w - start_w,
+                end_h - start_h,
+            )
 
             # Rescale to the correct objective value
             if rescale != 1:
                 im = utils.transforms.imresize(img=im, scale_factor=rescale)
 
             img_save_name = (
                 "_".join(
@@ -1462,14 +1517,17 @@
 
         # Save slide thumbnail
         slide_thumb = self.slide_thumbnail()
         utils.misc.imwrite(
             output_dir / f"slide_thumbnail{tile_format}", img=slide_thumb
         )
 
+        if verbose:
+            logger.setLevel(logging.INFO)
+
 
 class OpenSlideWSIReader(WSIReader):
     """Reader for OpenSlide supported whole-slide images.
 
     Supported WSI formats:
 
     - Aperio (.svs, .tif)
@@ -1549,14 +1607,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -1788,14 +1850,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -1933,21 +1999,21 @@
 
         try:
             x_res = float(props["tiff.XResolution"])
             y_res = float(props["tiff.YResolution"])
             mpp_x = utils.misc.ppu2mpp(x_res, tiff_res_units)
             mpp_y = utils.misc.ppu2mpp(y_res, tiff_res_units)
 
-            warnings.warn(
+            logger.warning(
                 "Metadata: Falling back to TIFF resolution tag"
                 " for microns-per-pixel (MPP)."
             )
             return mpp_x, mpp_y
         except KeyError:
-            warnings.warn("Metadata: Unable to determine microns-per-pixel (MPP).")
+            logger.warning("Metadata: Unable to determine microns-per-pixel (MPP).")
 
         # Return None value if metadata cannot be determined.
         return None
 
     def _info(self):
         """Openslide WSI meta data reader.
 
@@ -1972,19 +2038,19 @@
 
         # Fallback to calculating objective power from mpp
         if objective_power is None:
             if mpp is not None:
                 objective_power = utils.misc.mpp2common_objective_power(
                     float(np.mean(mpp))
                 )
-                warnings.warn(
-                    "Metadata: Objective power inferred from microns-per-pixel (MPP)."
+                logger.warning(
+                    "Metadata: Objective power inferred from microns-per-pixel (MPP).",
                 )
             else:
-                warnings.warn("Metadata: Unable to determine objective power.")
+                logger.warning("Metadata: Unable to determine objective power.")
 
         return WSIMeta(
             file_path=self.input_path,
             axes="YXS",
             objective_power=objective_power,
             slide_dimensions=slide_dimensions,
             level_count=level_count,
@@ -2072,14 +2138,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -2308,14 +2378,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -2369,15 +2443,20 @@
                 bounds, resolution, units
             )
             _, size_at_requested = utils.transforms.bounds2locsize(bounds)
             # don't use the `output_size` (`size_at_requested`) here
             # because the rounding error at `bounds_at_baseline` leads to
             # different `size_at_requested` (keeping same read resolution
             # but base image is of different scale)
-            (read_level, _, _, post_read_scale,) = self._find_read_bounds_params(
+            (
+                read_level,
+                _,
+                _,
+                post_read_scale,
+            ) = self._find_read_bounds_params(
                 bounds_at_baseline, resolution=resolution, units=units
             )
         else:  # duplicated portion with VirtualReader, factoring out ?
             # Find parameters for optimal read
             (
                 read_level,
                 _,  # bounds_at_read_level,
@@ -2425,26 +2504,26 @@
         """
         import glymur
 
         glymur_wsi = self.glymur_wsi
         box = glymur_wsi.box
         description = box[3].xml.find("description")
         matches = re.search(r"(?<=AppMag = )\d\d", description.text)
-        objective_power = np.int(matches[0])
+        objective_power = np.int_(matches[0])
         image_header = box[2].box[0]
         slide_dimensions = (image_header.width, image_header.height)
 
         # Determine level_count
         cod = None
         for segment in glymur_wsi.codestream.segment:
             if isinstance(segment, glymur.codestream.CODsegment):
                 cod = segment
 
         if cod is None:
-            warnings.warn(
+            logger.warning(
                 "Metadata: JP2 codestream missing COD segment! "
                 "Cannot determine number of decompositions (levels)"
             )
             level_count = 1
         else:
             level_count = cod.num_res
 
@@ -2634,14 +2713,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -2779,15 +2862,21 @@
                 units=units,
                 interpolation=interpolation,
                 pad_mode=pad_mode,
                 pad_constant_values=pad_constant_values,
             )
 
         # Find parameters for optimal read
-        (_, _, _, _, baseline_read_size,) = self.find_read_rect_params(
+        (
+            _,
+            _,
+            _,
+            _,
+            baseline_read_size,
+        ) = self.find_read_rect_params(
             location=location,
             size=size,
             resolution=resolution,
             units=units,
         )
 
         image_location, image_read_size = self._find_params_from_baseline(
@@ -2866,14 +2955,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -3281,15 +3374,15 @@
         xml_series = xml.findall("ome:Image", namespaces)[self.series_n]
         xml_pixels = xml_series.find("ome:Pixels", namespaces)
         mppx = xml_pixels.attrib.get("PhysicalSizeX")
         mppy = xml_pixels.attrib.get("PhysicalSizeY")
         if mppx is not None and mppy is not None:
             return [mppx, mppy]
         if mppx is not None or mppy is not None:
-            warnings.warn("Only one MPP value found. Using it for both X  and Y.")
+            logger.warning("Only one MPP value found. Using it for both X  and Y.")
             return [mppx or mppy] * 2
 
         return None
 
     def _parse_generic_tiff_metadata(self) -> dict:
         """Extract generic tiled metadata.
 
@@ -3423,14 +3516,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -3657,14 +3754,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -3718,15 +3819,20 @@
                 bounds, resolution, units
             )
             _, size_at_requested = utils.transforms.bounds2locsize(bounds)
             # don't use the `output_size` (`size_at_requested`) here
             # because the rounding error at `bounds_at_baseline` leads to
             # different `size_at_requested` (keeping same read resolution
             # but base image is of different scale)
-            (read_level, _, _, post_read_scale,) = self._find_read_bounds_params(
+            (
+                read_level,
+                _,
+                _,
+                post_read_scale,
+            ) = self._find_read_bounds_params(
                 bounds_at_baseline, resolution=resolution, units=units
             )
         else:  # duplicated portion with VirtualReader, factoring out ?
             # Find parameters for optimal read
             (
                 read_level,
                 _,
@@ -3793,15 +3899,15 @@
                 [
                     level_dimensions[0][0] / level.size.width,
                     level_dimensions[0][1] / level.size.height,
                 ]
             )
             for level in self.wsi.levels
         ]
-        dataset = self.wsi.datasets[0]
+        dataset = self.wsi.levels.base_level.datasets[0]
         # Get pixel spacing in mm from DICOM file and convert to um/px (mpp)
         mm_per_pixel = dataset.pixel_spacing
         mpp = (mm_per_pixel.width * 1e3, mm_per_pixel.height * 1e3)
 
         return WSIMeta(
             slide_dimensions=level_dimensions[0],
             level_dimensions=level_dimensions,
@@ -3864,14 +3970,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -4034,15 +4144,16 @@
             read_location=level_location,
             read_size=level_read_size,
             image_size=level_size,
         )
         _, constrained_read_size = utils.transforms.bounds2locsize(
             constrained_read_bounds
         )
-        im_region = wsi.read_region(location, read_level, constrained_read_size)
+        dicom_level = wsi.levels[read_level].level
+        im_region = wsi.read_region(location, dicom_level, constrained_read_size)
         im_region = np.array(im_region)
 
         # Apply padding outside the slide area
         level_read_bounds = utils.transforms.locsize2bounds(
             level_location, level_read_size
         )
         im_region = utils.image.crop_and_pad_edges(
@@ -4115,14 +4226,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -4208,16 +4323,17 @@
             bounds_at_read_level
         )
         level_size = self.info.level_dimensions[read_level]
         read_bounds = utils.image.find_overlap(
             level_location, size_at_read_level, level_size
         )
         _, read_size = utils.transforms.bounds2locsize(read_bounds)
+        dicom_level = wsi.levels[read_level].level
         im_region = wsi.read_region(
-            location=location_at_baseline, level=read_level, size=read_size
+            location=location_at_baseline, level=dicom_level, size=read_size
         )
         im_region = np.array(im_region)
 
         # Apply padding outside the slide area
         im_region = utils.image.crop_and_pad_edges(
             bounds=bounds_at_read_level,
             max_dimensions=self.info.level_dimensions[read_level],
@@ -4333,17 +4449,16 @@
             return None
         x = axes_dict["x"]
         y = axes_dict["y"]
 
         # Check the units,
         # Currently only handle micrometer units
         if x.unit != y.unit != "micrometer":
-            warnings.warn(
-                f"Expected units of micrometer, got {x.unit} and {y.unit}",
-                UserWarning,
+            logger.warning(
+                "Expected units of micrometer, got %s and %s", x.unit, y.unit
             )
             return None
 
         # Check that datasets is non-empty and has at least one coordinateTransformation
         if (
             not multiscales.datasets
             or not multiscales.datasets[0].coordinateTransformations
@@ -4367,14 +4482,195 @@
         units="level",
         interpolation="optimise",
         pad_mode="constant",
         pad_constant_values=0,
         coord_space="baseline",
         **kwargs,
     ):
+        """Read a region of the whole slide image at a location and size.
+
+        Location is in terms of the baseline image (level 0  / maximum
+        resolution), and size is the output image size.
+
+        Reads can be performed at different resolutions by supplying a
+        pair of arguments for the resolution and the units of
+        resolution. If metadata does not specify `mpp` or
+        `objective_power` then `baseline` units should be selected with
+        resolution 1.0
+
+        The field of view varies with resolution. For a fixed field of
+        view see :func:`read_bounds`.
+
+        Args:
+            location (tuple(int)):
+                (x, y) tuple giving the top left pixel in the baseline
+                (level 0) reference frame.
+            size (tuple(int)):
+                (width, height) tuple giving the desired output image
+                size.
+            resolution (int or float or tuple(float)):
+                Resolution at which to read the image, default = 0.
+                Either a single number or a sequence of two numbers for
+                x and y are valid. This value is in terms of the
+                corresponding units. For example: resolution=0.5 and
+                units="mpp" will read the slide at 0.5 microns
+                per-pixel, and resolution=3, units="level" will read at
+                level at pyramid level / resolution layer 3.
+            units (str):
+                The units of resolution, default = "level". Supported
+                units are: microns per pixel (mpp), objective power
+                (power), pyramid / resolution level (level), pixels per
+                baseline pixel (baseline).
+            interpolation (str):
+                Method to use when resampling the output image. Possible
+                values are "linear", "cubic", "lanczos", "area", and
+                "optimise". Defaults to 'optimise' which will use cubic
+                interpolation for upscaling and area interpolation for
+                downscaling to avoid moiré patterns.
+            pad_mode (str):
+                Method to use when padding at the edges of the image.
+                Defaults to 'constant'. See :func:`numpy.pad` for
+                available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
+            coord_space (str):
+                Defaults to "baseline". This is a flag to indicate if
+                the input `bounds` is in the baseline coordinate system
+                ("baseline") or is in the requested resolution system
+                ("resolution").
+            **kwargs (dict):
+                Extra key-word arguments for reader specific parameters.
+                Currently only used by VirtualWSIReader. See class
+                docstrings for more information.
+
+        Returns:
+            :class:`numpy.ndarray`:
+                Array of size MxNx3 M=size[0], N=size[1]
+
+        Example:
+            >>> from tiatoolbox.wsicore.wsireader import WSIReader
+            >>> # Load a WSI image
+            >>> wsi = WSIReader.open(input_img="./CMU-1.ome.zarr")
+            >>> location = (0, 0)
+            >>> size = (256, 256)
+            >>> # Read a region at level 0 (baseline / full resolution)
+            >>> img = wsi.read_rect(location, size)
+            >>> # Read a region at 0.5 microns per pixel (mpp)
+            >>> img = wsi.read_rect(location, size, 0.5, "mpp")
+            >>> # This could also be written more verbosely as follows
+            >>> img = wsi.read_rect(
+            ...     location,
+            ...     size,
+            ...     resolution=(0.5, 0.5),
+            ...     units="mpp",
+            ... )
+
+        Note: The field of view varies with resolution when using
+        :func:`read_rect`.
+
+        .. figure:: ../images/read_rect_tissue.png
+            :width: 512
+            :alt: Diagram illustrating read_rect
+
+        As the location is in the baseline reference frame but the size
+        (width and height) is the output image size, the field of view
+        therefore changes as resolution changes.
+
+        If the WSI does not have a resolution layer corresponding
+        exactly to the requested resolution (shown above in white with a
+        dashed outline), a larger resolution is downscaled to achieve
+        the correct requested output resolution.
+
+        If the requested resolution is higher than the baseline (maximum
+        resultion of the image), then bicubic interpolation is applied
+        to the output image.
+
+        .. figure:: ../images/read_rect-interpolated-reads.png
+            :width: 512
+            :alt: Diagram illustrating read_rect interpolting between levels
+
+        When reading between the levels stored in the WSI, the
+        coordinates of the requested region are projected to the next
+        highest resolution. This resolution is then decoded and
+        downsampled to produce the desired output. This is a major
+        source of variability in the time take to perform a read
+        operation. Reads which require reading a large region before
+        downsampling will be significantly slower than reading at a
+        fixed level.
+
+        Examples:
+
+            >>> from tiatoolbox.wsicore.wsireader import WSIReader
+            >>> # Load a WSI image
+            >>> wsi = WSIReader.open(input_img="./CMU-1.ome.zarr")
+            >>> location = (0, 0)
+            >>> size = (256, 256)
+            >>> # The resolution can be different in x and y, e.g.
+            >>> img = wsi.read_rect(
+            ...     location,
+            ...     size,
+            ...     resolution=(0.5, 0.75),
+            ...     units="mpp",
+            ... )
+            >>> # Several units can be used including: objective power,
+            >>> # microns per pixel, pyramid/resolution level, and
+            >>> # fraction of baseline.
+            >>> # E.g. Read a region at an objective power of 10x
+            >>> img = wsi.read_rect(
+            ...     location,
+            ...     size,
+            ...     resolution=10,
+            ...     units="power",
+            ... )
+            >>> # Read a region at pyramid / resolution level 1
+            >>> img = wsi.read_rect(
+            ...     location,
+            ...     size,
+            ...     resolution=1,
+            ...     units="level",
+            ... )
+            >>> # Read at a fractional level, this will linearly
+            >>> # interpolate the downsampling factor between levels.
+            >>> # E.g. if levels 0 and 1 have a downsampling of 1x and
+            >>> # 2x of baseline, then level 0.5 will correspond to a
+            >>> # downsampling factor 1.5x of baseline.
+            >>> img = wsi.read_rect(
+            ...     location,
+            ...     size,
+            ...     resolution=0.5,
+            ...     units="level",
+            ... )
+            >>> # Read a region at half of the full / baseline
+            >>> # resolution.
+            >>> img = wsi.read_rect(
+            ...     location,
+            ...     size,
+            ...     resolution=0.5,
+            ...     units="baseline",
+            ... )
+            >>> # Read at a higher resolution than the baseline
+            >>> # (interpolation applied to output)
+            >>> img = wsi.read_rect(
+            ...     location,
+            ...     size,
+            ...     resolution=1.25,
+            ...     units="baseline",
+            ... )
+            >>> # Assuming the image has a native mpp of 0.5,
+            >>> # interpolation will be applied here.
+            >>> img = wsi.read_rect(
+            ...     location,
+            ...     size,
+            ...     resolution=0.25,
+            ...     units="mpp",
+            ... )
+
+        """
         if coord_space == "resolution":
             im_region = self._read_rect_at_resolution(
                 location,
                 size,
                 resolution=resolution,
                 units=units,
                 interpolation=interpolation,
@@ -4423,25 +4719,130 @@
         units="level",
         interpolation="optimise",
         pad_mode="constant",
         pad_constant_values=0,
         coord_space="baseline",
         **kwargs,
     ):
+        """Read a region of the whole slide image within given bounds.
+
+        Bounds are in terms of the baseline image (level 0  / maximum
+        resolution).
+
+        Reads can be performed at different resolutions by supplying a
+        pair of arguments for the resolution and the units of
+        resolution. If metadata does not specify `mpp` or
+        `objective_power` then `baseline` units should be selected with
+        resolution 1.0
+
+        The output image size may be different to the width and height
+        of the bounds as the resolution will affect this. To read a
+        region with a fixed output image size see :func:`read_rect`.
+
+        Args:
+            bounds (tuple(int)):
+                By default, this is a tuple of (start_x, start_y, end_x,
+                end_y) i.e. (left, top, right, bottom) of the region in
+                baseline reference frame. However, with
+                `coord_space="resolution"`, the bound is expected to be
+                at the requested resolution system.
+            resolution (int or float or tuple(float)):
+                Resolution at which to read the image, default = 0.
+                Either a single number or a sequence of two numbers for
+                x and y are valid. This value is in terms of the
+                corresponding units. For example: resolution=0.5 and
+                units="mpp" will read the slide at 0.5 microns
+                per-pixel, and resolution=3, units="level" will read at
+                level at pyramid level / resolution layer 3.
+            units (str):
+                Units of resolution, default="level". Supported units
+                are: microns per pixel (mpp), objective power (power),
+                pyramid / resolution level (level), pixels per baseline
+                pixel (baseline).
+            interpolation (str):
+                Method to use when resampling the output image. Possible
+                values are "linear", "cubic", "lanczos", "area", and
+                "optimise". Defaults to 'optimise' which will use cubic
+                interpolation for upscaling and area interpolation for
+                downscaling to avoid moiré patterns.
+            pad_mode (str):
+                Method to use when padding at the edges of the image.
+                Defaults to 'constant'. See :func:`numpy.pad` for
+                available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
+            coord_space (str):
+                Defaults to "baseline". This is a flag to indicate if
+                the input `bounds` is in the baseline coordinate system
+                ("baseline") or is in the requested resolution system
+                ("resolution").
+            **kwargs (dict):
+                Extra key-word arguments for reader specific parameters.
+                Currently only used by :obj:`VirtualWSIReader`. See
+                class docstrings for more information.
+
+        Returns:
+            :class:`numpy.ndarray`:
+                Array of size MxNx3 M=end_h-start_h, N=end_w-start_w
+
+        Examples:
+            >>> from tiatoolbox.wsicore.wsireader import WSIReader
+            >>> from matplotlib import pyplot as plt
+            >>> wsi = WSIReader.open(input_img="./CMU-1.ome.zarr")
+            >>> # Read a region at level 0 (baseline / full resolution)
+            >>> bounds = [1000, 2000, 2000, 3000]
+            >>> img = wsi.read_bounds(bounds)
+            >>> plt.imshow(img)
+            >>> # This could also be written more verbosely as follows
+            >>> img = wsi.read_bounds(
+            ...     bounds,
+            ...     resolution=0,
+            ...     units="level",
+            ... )
+            >>> plt.imshow(img)
+
+        Note: The field of view remains the same as resolution is varied
+        when using :func:`read_bounds`.
+
+        .. figure:: ../images/read_bounds_tissue.png
+            :width: 512
+            :alt: Diagram illustrating read_bounds
+
+        This is because the bounds are in the baseline (level 0)
+        reference frame. Therefore, varying the resolution does not
+        change what is visible within the output image.
+
+        If the WSI does not have a resolution layer corresponding
+        exactly to the requested resolution (shown above in white with a
+        dashed outline), a larger resolution is downscaled to achieve
+        the correct requested output resolution.
+
+        If the requested resolution is higher than the baseline (maximum
+        resultion of the image), then bicubic interpolation is applied
+        to the output image.
+
+        """
         bounds_at_baseline = bounds
         if coord_space == "resolution":
             bounds_at_baseline = self._bounds_at_resolution_to_baseline(
                 bounds, resolution, units
             )
             _, size_at_requested = utils.transforms.bounds2locsize(bounds)
             # don't use the `output_size` (`size_at_requested`) here
             # because the rounding error at `bounds_at_baseline` leads to
             # different `size_at_requested` (keeping same read resolution
             # but base image is of different scale)
-            (read_level, _, _, post_read_scale,) = self._find_read_bounds_params(
+            (
+                read_level,
+                _,
+                _,
+                post_read_scale,
+            ) = self._find_read_bounds_params(
                 bounds_at_baseline, resolution=resolution, units=units
             )
         else:  # duplicated portion with VirtualReader, factoring out ?
             # Find parameters for optimal read
             (
                 read_level,
                 _,
@@ -4484,15 +4885,15 @@
     either to render annotations as a stand-alone mask, or to render annotations
     on top of its parent WSI as a virtual 'annotated slide'.
     Note: Currently only supports annotations stored at the same resolution as
     the parent WSI base resolution. Support for annotations stored at arbitrary
     resolutions will be added in the future.
 
     Args:
-        store (AnnotationStore | str):
+        store (AnnotationStore | str | Path):
             An AnnotationStore or a path to an annotation store .db file.
         info (WSIMeta):
             Metadata of the base WSI for the annotations in the store.
             If this is not provided, will attempt to read it read from
             the store metadata, or the base_wsi if provided.
             If no source of metadata is found, will raise an error.
         renderer (AnnotationRenderer):
@@ -4507,15 +4908,15 @@
             Opacity of the overlaid annotations. Must be between 0 and 1.
             Has no effect if base_wsi is not provided.
 
     """
 
     def __init__(
         self,
-        store: Union[AnnotationStore, str],
+        store: Union[AnnotationStore, str, pathlib.Path],
         info: Optional[WSIMeta] = None,
         renderer: AnnotationRenderer = None,
         base_wsi: Union[WSIReader, str] = None,
         alpha=1.0,
         **kwargs,
     ):
         super().__init__(store, **kwargs)
@@ -4612,14 +5013,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -4895,14 +5300,18 @@
                 "optimise". Defaults to 'optimise' which will use cubic
                 interpolation for upscaling and area interpolation for
                 downscaling to avoid moiré patterns.
             pad_mode (str):
                 Method to use when padding at the edges of the image.
                 Defaults to 'constant'. See :func:`numpy.pad` for
                 available modes.
+            pad_constant_values (int, tuple(int)):
+                Constant values to use when padding with constant pad mode.
+                Passed to the :func:`numpy.pad` `constant_values` argument.
+                Default is 0.
             coord_space (str):
                 Defaults to "baseline". This is a flag to indicate if
                 the input `bounds` is in the baseline coordinate system
                 ("baseline") or is in the requested resolution system
                 ("resolution").
             **kwargs (dict):
                 Extra key-word arguments for reader specific parameters.
@@ -4957,15 +5366,20 @@
                 bounds, resolution, units
             )
             _, size_at_requested = utils.transforms.bounds2locsize(bounds)
             # don't use the `output_size` (`size_at_requested`) here
             # because the rounding error at `bounds_at_baseline` leads to
             # different `size_at_requested` (keeping same read resolution
             # but base image is of different scale)
-            (read_level, _, _, post_read_scale,) = self._find_read_bounds_params(
+            (
+                read_level,
+                _,
+                _,
+                post_read_scale,
+            ) = self._find_read_bounds_params(
                 bounds_at_baseline, resolution=resolution, units=units
             )
         else:  # duplicated portion with VirtualReader, factoring out ?
             # Find parameters for optimal read
             (
                 read_level,
                 _,
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox.egg-info/PKG-INFO` & `tiatoolbox-1.4.0/tiatoolbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tiatoolbox
-Version: 1.3.3
+Version: 1.4.0
 Summary: Computational pathology toolbox developed by TIA Centre.
 Home-page: https://github.com/TissueImageAnalytics/tiatoolbox
 Author: TIA Centre
 Author-email: tia@dcs.warwick.ac.uk
 Keywords: tiatoolbox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/develop/docs/tiatoolbox-logo.png">
 </p>
@@ -39,16 +39,16 @@
             <img src="https://shields.io/conda/dn/conda-forge/tiatoolbox"  alt="conda-forge downloads"/>
     </a>
   <br>
   <a href="https://tia-toolbox.readthedocs.io/en/latest/?badge=latest">
     <img src="https://readthedocs.org/projects/tia-toolbox/badge/?version=latest" alt="Documentation Status" />
   </a>
   <br>
-  <a href="https://github.com/TissueImageAnalytics/tiatoolbox/blob/develop/LICENSE">
-    <img alt="GitHub license" src="https://img.shields.io/github/license/TissueImageAnalytics/tiatoolbox"></a>
+  <a href="#license">
+    <img alt="GitHub license" src="https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=green"></a>
   <br>
   <br>
   <a href="https://github.com/TissueImageAnalytics/tiatoolbox/actions/workflows/pip-install.yml">
     <img src="https://img.shields.io/pypi/pyversions/tiatoolbox.svg"  alt="Supported Python versions"/>
   </a>
  <a href="https://github.com/psf/black">
       <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code Style black"/>
@@ -102,15 +102,15 @@
 
 tiatoolbox supports various features through command line. For more information, please try `tiatoolbox --help`
 
 ### Prepare for development
 
 Prepare a computer as a convenient platform for further development of the Python package `tiatoolbox` and related programs as follows.
 
-1. Install [pre-requisite software](https://tia-toolbox.readthedocs.io/en/latest/installation.html)
+1. Install [pre-requisite software](https://tia-toolbox.readthedocs.io/en/latest/installation.html#prerequisites)
 1. Open a terminal window<br/>
 
 ```sh
     $ cd <future-home-of-tiatoolbox-directory>
 ```
 
 3. Download a complete copy of the `tiatoolbox`.
@@ -124,37 +124,37 @@
 ```sh
     $ cd tiatoolbox
 ```
 
 5. Create virtual environment for TIAToolbox using
 
 ```sh
-    $ conda env create -f requirements.dev.conda.yml # for linux/mac only.
+    $ conda create -n tiatoolbox-dev python=3.8 # select version of your choice
     $ conda activate tiatoolbox-dev
+    $ pip install -r requirements/requirements_dev.txt
 ```
 
 or
 
 ```sh
-    $ conda create -n tiatoolbox-dev python=3.8 # select version of your choice
+    $ conda env create -f requirements/requirements.dev.conda.yml # for linux/mac only.
     $ conda activate tiatoolbox-dev
-    $ pip install -r requirements_dev.txt
 ```
 
 6. To use the packages installed in the environment, run the command:
 
 ```sh
     $ conda activate tiatoolbox-dev
 ```
 
 ### License
 
-The source code TIA Toolbox (tiatoolbox) as hosted on GitHub is released under the [The 3-Clause BSD License].
+The source code TIA Toolbox (tiatoolbox) as hosted on GitHub is released under the [BSD-3-Clause license](https://github.com/TissueImageAnalytics/tiatoolbox/blob/develop/LICENSE). The full text of the licence is included in [LICENSE](https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/develop/LICENSE).
 
-The full text of the licence is included in [LICENSE](https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/develop/LICENSE).
+Models weights are dependent on the datasets that they were trained on. Please refer to the [documentation](https://tia-toolbox.readthedocs.io/en/latest/pretrained.html) for more details.
 
 ### Cite this repository
 
 If you find TIAToolbox useful or use it in your research, please consider citing our paper:
 
 ```
 @article{
@@ -170,26 +170,65 @@
     title = {{TIAToolbox as an end-to-end library for advanced tissue image analytics}},
     url = {https://www.nature.com/articles/s43856-022-00186-5},
     volume = {2},
     year = {2022}
 }
 ```
 
-### Auxiliary Files
 
-Auxiliary files, such as pre-trained model weights downloaded from the TIA Centre webpage (https://warwick.ac.uk/tia/), are provided under the [Creative Commons Attribution-NonCommercial-ShareAlike Version 4 (CC BY-NC-SA 4.0) license](https://creativecommons.org/licenses/by-nc-sa/4.0/).
+# History
 
-### Dual License
+## 1.4.0 (2023-04-24)
 
-If you would like to use any of the source code or auxiliary files (e.g. pre-trained model weights) under a different license agreement please contact the Tissue Image Analytics (TIA) Centre at the University of Warwick (tia@dcs.warwick.ac.uk).
+### Major Updates and Feature Improvements
 
-[the 3-clause bsd license]: https://opensource.org/licenses/BSD-3-Clause
+- Adds Python 3.11 support \[experimental\] #500
+  - Python 3.11 is not fully supported by `pytorch` https://github.com/pytorch/pytorch/issues/86566 and `openslide` https://github.com/openslide/openslide-python/pull/188
+- Removes Python 3.7 support
+  - This allows upgrading all the dependencies which were dependent on an older version of Python.
+- Adds Neighbourhood Querying Support To AnnotationStore #540
+  - This enables easy and efficient querying of annotations within a neighbourhood of other annotations.
+- Adds `MultiTaskSegmentor` engine #424
+- Fixes an issue with stain augmentation to apply augmentation to only tissue regions.
+  - #546 contributed by @navidstuv
+- Filters logger output to stdout instead of stderr.
+  - Fixes #255
+- Allows import of some modules at higher level for improved usability
+  - `WSIReader` can now be imported as `from tiatoolbox.wsicore import WSIReader`
+  - `WSIMeta` can now be imported as `from tiatoolbox.wsicore import WSIMeta`
+  - `HoVerNet`, `HoVerNetPlus`, `IDaRS`, `MapDe`, `MicroNet`, `NuClick`, `SCCNN` can now be imported as \`from tiatoolbox.models import HoVerNet, HoVerNetPlus, IDaRS, MapDe, MicroNet, NuClick, SCCNN
+- Improves `PatchExtractor` performance. Updates `WSIPatchDataset` to be consistent. #571
+- Updates documentation for `License` for clarity on source code and model weights license.
 
+### Changes to API
 
-# History
+- Updates SCCNN architecture to make it consistent with other models. #544
+
+### Bug Fixes and Other Changes
+
+- Fixes Parsing Missing Omero Version NGFF Metadata #568
+  - Fixes #535 raised by @benkamphaus
+- Fixes reading of DICOM WSIs at the correct level #564
+  - Fixes #529
+- Fixes `scipy`, `matplotlib`, `scikit-image` deprecated code
+- Fixes breaking changes in `DICOMWSIReader` to make it compatible with latest `wsidicom` version. #539, #580
+- Updates `shapely` dependency to version >=2.0.0 and fixes any breaking changes.
+- Fixes bug with `DictionaryStore.bquery` and `geometry=None`, i.e. only a where predicate given.
+  - Partly Fixes #532 raised by @blaginin
+- Fixes local tests for Windows/Linux
+- Fixes `flake8`, `deepsource` errors.
+- Uses `logger` instead of `warnings` and `print` statements to properly log runs.
+
+### Development related changes
+
+- Upgrades dependencies which are dependent on Python 3.7
+- Moves `requirements*.txt` files to `requirements` folder
+- Removes `tox`
+- Uses `pyproject.toml` for `bdist_wheel`, `pytest` and `isort`
+- Adds `joblib` and `numba` as dependencies.
 
 ## 1.3.3 (2023-03-02)
 
 ### Major Updates and Feature Improvements
 
 - Restricts dependency versions for long term stability of the current version
 
@@ -201,15 +240,14 @@
 
 - Fix bug related to reading scikit-image
 
 ### Development related changes
 
 - Restricts dependency versions for compatibility
 
-
 ## 1.3.2 (2023-02-17)
 
 ### Major Updates and Feature Improvements
 
 None
 
 ### Changes to API
@@ -220,15 +258,14 @@
 
 - Fix bug related to reading DICOM files
 
 ### Development related changes
 
 - Restricts wsidicom version to \<0.7.0 for compatibility
 
-
 ## 1.3.1 (2022-12-20)
 
 ### Major Updates and Feature Improvements
 
 - Adds [NuClick](https://arxiv.org/abs/2005.14511) architecture #449
 - Adds Annotation Store Reader #476
 - Adds [DFBR](https://arxiv.org/abs/2202.09971) method for registering pair of images #510
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: tiatoolbox Version: 1.3.3 Summary: Computational
+Metadata-Version: 2.1 Name: tiatoolbox Version: 1.4.0 Summary: Computational
 pathology toolbox developed by TIA Centre. Home-page: https://github.com/
 TissueImageAnalytics/tiatoolbox Author: TIA Centre Author-email:
 tia@dcs.warwick.ac.uk Keywords: tiatoolbox Classifier: Development Status :: 2
 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE License-File: AUTHORS.md
   [https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/develop/
                            docs/tiatoolbox-logo.png]
                            ****** TIA Toolbox ******
      **** Computational Pathology Toolbox developed at the TIA Centre ****
 [PyPI_Status] [pypi_Downloads]
 [conda-forge_badge] [conda-forge_downloads]
@@ -67,53 +67,81 @@
 installation.html). To understand better how the programs work, study the
 jupyter notebooks referred to under the heading **Examples Taster**. ###
 Command Line tiatoolbox supports various features through command line. For
 more information, please try `tiatoolbox --help` ### Prepare for development
 Prepare a computer as a convenient platform for further development of the
 Python package `tiatoolbox` and related programs as follows. 1. Install [pre-
 requisite software](https://tia-toolbox.readthedocs.io/en/latest/
-installation.html) 1. Open a terminal window
+installation.html#prerequisites) 1. Open a terminal window
 ```sh $ cd  ``` 3. Download a complete copy of the `tiatoolbox`. ```sh $ git
 clone https://github.com/TissueImageAnalytics/tiatoolbox.git ``` 4. Change
 directory to `tiatoolbox` ```sh $ cd tiatoolbox ``` 5. Create virtual
-environment for TIAToolbox using ```sh $ conda env create -
-f requirements.dev.conda.yml # for linux/mac only. $ conda activate tiatoolbox-
-dev ``` or ```sh $ conda create -n tiatoolbox-dev python=3.8 # select version
-of your choice $ conda activate tiatoolbox-dev $ pip install -
-r requirements_dev.txt ``` 6. To use the packages installed in the environment,
-run the command: ```sh $ conda activate tiatoolbox-dev ``` ### License The
-source code TIA Toolbox (tiatoolbox) as hosted on GitHub is released under the
-[The 3-Clause BSD License]. The full text of the licence is included in
-[LICENSE](https://raw.githubusercontent.com/TissueImageAnalytics/tiatoolbox/
-develop/LICENSE). ### Cite this repository If you find TIAToolbox useful or use
-it in your research, please consider citing our paper: ``` @article
-{ Pocock2022, author = {Pocock, Johnathan and Graham, Simon and Vu, Quoc Dang
-and Jahanifar, Mostafa and Deshpande, Srijay and Hadjigeorghiou, Giorgos and
-Shephard, Adam and Bashir, Raja Muhammad Saad and Bilal, Mohsin and Lu, Wenqi
-and Epstein, David and Minhas, Fayyaz and Rajpoot, Nasir M and Raza, Shan E
-Ahmed}, doi = {10.1038/s43856-022-00186-5}, issn = {2730-664X}, journal =
-{Communications Medicine}, month = {sep}, number = {1}, pages = {120},
-publisher = {Springer US}, title = {{TIAToolbox as an end-to-end library for
-advanced tissue image analytics}}, url = {https://www.nature.com/articles/
-s43856-022-00186-5}, volume = {2}, year = {2022} } ``` ### Auxiliary Files
-Auxiliary files, such as pre-trained model weights downloaded from the TIA
-Centre webpage (https://warwick.ac.uk/tia/), are provided under the [Creative
-Commons Attribution-NonCommercial-ShareAlike Version 4 (CC BY-NC-SA 4.0)
-license](https://creativecommons.org/licenses/by-nc-sa/4.0/). ### Dual License
-If you would like to use any of the source code or auxiliary files (e.g. pre-
-trained model weights) under a different license agreement please contact the
-Tissue Image Analytics (TIA) Centre at the University of Warwick
-(tia@dcs.warwick.ac.uk). [the 3-clause bsd license]: https://opensource.org/
-licenses/BSD-3-Clause # History ## 1.3.3 (2023-03-02) ### Major Updates and
-Feature Improvements - Restricts dependency versions for long term stability of
-the current version ### Changes to API None ### Bug Fixes and Other Changes -
-Fix bug related to reading scikit-image ### Development related changes -
-Restricts dependency versions for compatibility ## 1.3.2 (2023-02-17) ### Major
-Updates and Feature Improvements None ### Changes to API None ### Bug Fixes and
-Other Changes - Fix bug related to reading DICOM files ### Development related
+environment for TIAToolbox using ```sh $ conda create -n tiatoolbox-dev
+python=3.8 # select version of your choice $ conda activate tiatoolbox-dev $
+pip install -r requirements/requirements_dev.txt ``` or ```sh $ conda env
+create -f requirements/requirements.dev.conda.yml # for linux/mac only. $ conda
+activate tiatoolbox-dev ``` 6. To use the packages installed in the
+environment, run the command: ```sh $ conda activate tiatoolbox-dev ``` ###
+License The source code TIA Toolbox (tiatoolbox) as hosted on GitHub is
+released under the [BSD-3-Clause license](https://github.com/
+TissueImageAnalytics/tiatoolbox/blob/develop/LICENSE). The full text of the
+licence is included in [LICENSE](https://raw.githubusercontent.com/
+TissueImageAnalytics/tiatoolbox/develop/LICENSE). Models weights are dependent
+on the datasets that they were trained on. Please refer to the [documentation]
+(https://tia-toolbox.readthedocs.io/en/latest/pretrained.html) for more
+details. ### Cite this repository If you find TIAToolbox useful or use it in
+your research, please consider citing our paper: ``` @article{ Pocock2022,
+author = {Pocock, Johnathan and Graham, Simon and Vu, Quoc Dang and Jahanifar,
+Mostafa and Deshpande, Srijay and Hadjigeorghiou, Giorgos and Shephard, Adam
+and Bashir, Raja Muhammad Saad and Bilal, Mohsin and Lu, Wenqi and Epstein,
+David and Minhas, Fayyaz and Rajpoot, Nasir M and Raza, Shan E Ahmed}, doi =
+{10.1038/s43856-022-00186-5}, issn = {2730-664X}, journal = {Communications
+Medicine}, month = {sep}, number = {1}, pages = {120}, publisher = {Springer
+US}, title = {{TIAToolbox as an end-to-end library for advanced tissue image
+analytics}}, url = {https://www.nature.com/articles/s43856-022-00186-5}, volume
+= {2}, year = {2022} } ``` # History ## 1.4.0 (2023-04-24) ### Major Updates
+and Feature Improvements - Adds Python 3.11 support \[experimental\] #500 -
+Python 3.11 is not fully supported by `pytorch` https://github.com/pytorch/
+pytorch/issues/86566 and `openslide` https://github.com/openslide/openslide-
+python/pull/188 - Removes Python 3.7 support - This allows upgrading all the
+dependencies which were dependent on an older version of Python. - Adds
+Neighbourhood Querying Support To AnnotationStore #540 - This enables easy and
+efficient querying of annotations within a neighbourhood of other annotations.
+- Adds `MultiTaskSegmentor` engine #424 - Fixes an issue with stain
+augmentation to apply augmentation to only tissue regions. - #546 contributed
+by @navidstuv - Filters logger output to stdout instead of stderr. - Fixes #255
+- Allows import of some modules at higher level for improved usability -
+`WSIReader` can now be imported as `from tiatoolbox.wsicore import WSIReader` -
+`WSIMeta` can now be imported as `from tiatoolbox.wsicore import WSIMeta` -
+`HoVerNet`, `HoVerNetPlus`, `IDaRS`, `MapDe`, `MicroNet`, `NuClick`, `SCCNN`
+can now be imported as \`from tiatoolbox.models import HoVerNet, HoVerNetPlus,
+IDaRS, MapDe, MicroNet, NuClick, SCCNN - Improves `PatchExtractor` performance.
+Updates `WSIPatchDataset` to be consistent. #571 - Updates documentation for
+`License` for clarity on source code and model weights license. ### Changes to
+API - Updates SCCNN architecture to make it consistent with other models. #544
+### Bug Fixes and Other Changes - Fixes Parsing Missing Omero Version NGFF
+Metadata #568 - Fixes #535 raised by @benkamphaus - Fixes reading of DICOM WSIs
+at the correct level #564 - Fixes #529 - Fixes `scipy`, `matplotlib`, `scikit-
+image` deprecated code - Fixes breaking changes in `DICOMWSIReader` to make it
+compatible with latest `wsidicom` version. #539, #580 - Updates `shapely`
+dependency to version >=2.0.0 and fixes any breaking changes. - Fixes bug with
+`DictionaryStore.bquery` and `geometry=None`, i.e. only a where predicate
+given. - Partly Fixes #532 raised by @blaginin - Fixes local tests for Windows/
+Linux - Fixes `flake8`, `deepsource` errors. - Uses `logger` instead of
+`warnings` and `print` statements to properly log runs. ### Development related
+changes - Upgrades dependencies which are dependent on Python 3.7 - Moves
+`requirements*.txt` files to `requirements` folder - Removes `tox` - Uses
+`pyproject.toml` for `bdist_wheel`, `pytest` and `isort` - Adds `joblib` and
+`numba` as dependencies. ## 1.3.3 (2023-03-02) ### Major Updates and Feature
+Improvements - Restricts dependency versions for long term stability of the
+current version ### Changes to API None ### Bug Fixes and Other Changes - Fix
+bug related to reading scikit-image ### Development related changes - Restricts
+dependency versions for compatibility ## 1.3.2 (2023-02-17) ### Major Updates
+and Feature Improvements None ### Changes to API None ### Bug Fixes and Other
+Changes - Fix bug related to reading DICOM files ### Development related
 changes - Restricts wsidicom version to \<0.7.0 for compatibility ## 1.3.1
 (2022-12-20) ### Major Updates and Feature Improvements - Adds [NuClick](https:
 //arxiv.org/abs/2005.14511) architecture #449 - Adds Annotation Store Reader
 #476 - Adds [DFBR](https://arxiv.org/abs/2202.09971) method for registering
 pair of images #510 ### Changes to API - Adds a sample SVS loading function
 `tiatoolbox.data.small_svs()` to the data module #517 ### Bug Fixes and Other
 Changes - Simplifies example notebook for image reading for better readability
```

### Comparing `tiatoolbox-1.3.3/tiatoolbox.egg-info/SOURCES.txt` & `tiatoolbox-1.4.0/tiatoolbox.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 CONTRIBUTING.rst
 HISTORY.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
-requirements.txt
 setup.cfg
 setup.py
+requirements/requirements.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_annotation_stores.py
 tests/test_annotation_tilerendering.py
 tests/test_data.py
 tests/test_docs.py
 tests/test_dsl.py
@@ -121,14 +121,15 @@
 tiatoolbox/models/architecture/utils.py
 tiatoolbox/models/architecture/vanilla.py
 tiatoolbox/models/dataset/__init__.py
 tiatoolbox/models/dataset/classification.py
 tiatoolbox/models/dataset/dataset_abc.py
 tiatoolbox/models/dataset/info.py
 tiatoolbox/models/engine/__init__.py
+tiatoolbox/models/engine/multi_task_segmentor.py
 tiatoolbox/models/engine/nucleus_instance_segmentor.py
 tiatoolbox/models/engine/patch_predictor.py
 tiatoolbox/models/engine/semantic_segmentor.py
 tiatoolbox/tools/__init__.py
 tiatoolbox/tools/graph.py
 tiatoolbox/tools/patchextraction.py
 tiatoolbox/tools/pyramid.py
@@ -145,13 +146,11 @@
 tiatoolbox/utils/metrics.py
 tiatoolbox/utils/misc.py
 tiatoolbox/utils/transforms.py
 tiatoolbox/utils/visualization.py
 tiatoolbox/visualization/__init__.py
 tiatoolbox/visualization/tileserver.py
 tiatoolbox/wsicore/__init__.py
-tiatoolbox/wsicore/save_tiles.py
-tiatoolbox/wsicore/slide_info.py
 tiatoolbox/wsicore/wsimeta.py
 tiatoolbox/wsicore/wsireader.py
 tiatoolbox/wsicore/metadata/__init__.py
 tiatoolbox/wsicore/metadata/ngff.py
```

