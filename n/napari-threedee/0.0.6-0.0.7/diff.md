# Comparing `tmp/napari-threedee-0.0.6.tar.gz` & `tmp/napari-threedee-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-threedee-0.0.6.tar", last modified: Mon May  1 21:00:00 2023, max compression
+gzip compressed data, was "napari-threedee-0.0.7.tar", last modified: Fri May  5 09:26:48 2023, max compression
```

## Comparing `napari-threedee-0.0.6.tar` & `napari-threedee-0.0.7.tar`

### file list

```diff
@@ -1,209 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.145530 napari-threedee-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.121529 napari-threedee-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.125529 napari-threedee-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.129530 napari-threedee-0.0.6/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-01 21:00:00.145530 napari-threedee-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.129530 napari-threedee-0.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.129530 napari-threedee-0.0.6/docs/API/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/API/geometry_utilities.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/API/napari_utilities.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/API/selection_utilities.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.129530 napari-threedee-0.0.6/docs/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/annotations/io.md
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/annotations/point_spec.md
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/annotations/specifications.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/annotations/sphere_spec.md
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/annotations/spline_spec.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.129530 napari-threedee-0.0.6/docs/dev_guides/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/dev_guides/core_concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/dev_guides/manipulators.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.129530 napari-threedee-0.0.6/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.129530 napari-threedee-0.0.6/docs/examples/library/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/library/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/library/camera_spline_library.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/library/layer_manipulator_library.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/library/mesh_headlight_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/library/path_annotator_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/library/point_annotator_library.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/library/render_plane_manipulator_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/library/sphere_annotator_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/library/surface_annotator_library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.129530 napari-threedee-0.0.6/docs/examples/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/plugin/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/plugin/camera_spline_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/plugin/layer_manipulator_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/plugin/mesh_headlight_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/plugin/path_annotator_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/plugin/point_annotator_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/plugin/points_manipulator_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/plugin/render_plane_manipulator_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/plugin/sphere_annotator_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/plugin/spline_annotator_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/examples/plugin/surface_annotator_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/gallery_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.133530 napari-threedee-0.0.6/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/getting_started/developers.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/getting_started/users.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.133530 napari-threedee-0.0.6/docs/how_to/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/how_to/layer_manipulator.md
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/how_to/point_annotator.md
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/how_to/point_manipulator.md
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/how_to/render_plane_manipulator.md
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/how_to/sphere_annotator.md
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/how_to/spline_annotator.md
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.133530 napari-threedee-0.0.6/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/stylesheets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.133530 napari-threedee-0.0.6/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/docs/tutorials/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-01 21:00:00.145530 napari-threedee-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.125529 napari-threedee-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.133530 napari-threedee-0.0.6/src/napari_threedee/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.133530 napari-threedee-0.0.6/src/napari_threedee/_backend/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.137530 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.137530 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/test_axis_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/test_central_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/test_drag_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/test_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/test_manipulator_visual_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/test_rotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/axis_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/central_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/drag_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/manipulator_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/napari_manipulator_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/rotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/vispy_manipulator_visual.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/vispy_visual_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/threedee_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_backend/threedee_widget_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.137530 napari-threedee-0.0.6/src/napari_threedee/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_tests/test_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/_tests/test_mouse_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 20:59:59.000000 napari-threedee-0.0.6/src/napari_threedee/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.137530 napari-threedee-0.0.6/src/napari_threedee/annotators/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.137530 napari-threedee-0.0.6/src/napari_threedee/annotators/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/_qt/qt_path_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/_qt/qt_plane_point_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/_qt/qt_point_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/_qt/qt_sphere_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/_qt/qt_surface_annotator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.137530 napari-threedee-0.0.6/src/napari_threedee/annotators/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/_tests/test_point_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/_tests/test_sphere_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/_tests/test_spline_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.137530 napari-threedee-0.0.6/src/napari_threedee/annotators/paths/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/paths/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/paths/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/paths/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.137530 napari-threedee-0.0.6/src/napari_threedee/annotators/points/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/points/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.141530 napari-threedee-0.0.6/src/napari_threedee/annotators/points/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/points/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/points/_tests/test_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/points/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/points/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/points/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.141530 napari-threedee-0.0.6/src/napari_threedee/annotators/spheres/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/spheres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.141530 napari-threedee-0.0.6/src/napari_threedee/annotators/spheres/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/spheres/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/spheres/_tests/test_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/spheres/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/spheres/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/spheres/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.141530 napari-threedee-0.0.6/src/napari_threedee/annotators/surfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/surfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.141530 napari-threedee-0.0.6/src/napari_threedee/annotators/surfaces/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/surfaces/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/surfaces/_tests/test_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/surfaces/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/surfaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/annotators/surfaces/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.141530 napari-threedee-0.0.6/src/napari_threedee/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.141530 napari-threedee-0.0.6/src/napari_threedee/data_models/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/data_models/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/data_models/_tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/data_models/_tests/test_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/data_models/_tests/test_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/data_models/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/data_models/points.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/data_models/spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/data_models/spline_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/data_models/surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/dock_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.141530 napari-threedee-0.0.6/src/napari_threedee/manipulators/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/manipulators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.141530 napari-threedee-0.0.6/src/napari_threedee/manipulators/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/manipulators/_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/manipulators/_qt/qt_layer_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/manipulators/_qt/qt_point_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/manipulators/_qt/qt_render_plane_manipulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.141530 napari-threedee-0.0.6/src/napari_threedee/manipulators/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/manipulators/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/manipulators/_tests/test_manipulator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/manipulators/base_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/manipulators/layer_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/manipulators/manipulator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/manipulators/point_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/manipulators/render_plane_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.145530 napari-threedee-0.0.6/src/napari_threedee/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.145530 napari-threedee-0.0.6/src/napari_threedee/utils/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/utils/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/utils/_tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/utils/mouse_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/utils/napari_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/utils/selection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/vispy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.145530 napari-threedee-0.0.6/src/napari_threedee/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.145530 napari-threedee-0.0.6/src/napari_threedee/visualization/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/visualization/_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/visualization/_qt/qt_camera_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/visualization/_qt/qt_lighting_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.145530 napari-threedee-0.0.6/src/napari_threedee/visualization/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/visualization/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/visualization/_tests/test_camera_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/visualization/_tests/test_lighting_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/visualization/camera_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/src/napari_threedee/visualization/lighting_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:00:00.133530 napari-threedee-0.0.6/src/napari_threedee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-01 21:00:00.000000 napari-threedee-0.0.6/src/napari_threedee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-01 21:00:00.000000 napari-threedee-0.0.6/src/napari_threedee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:00:00.000000 napari-threedee-0.0.6/src/napari_threedee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 21:00:00.000000 napari-threedee-0.0.6/src/napari_threedee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-01 21:00:00.000000 napari-threedee-0.0.6/src/napari_threedee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 21:00:00.000000 napari-threedee-0.0.6/src/napari_threedee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-01 20:59:47.000000 napari-threedee-0.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.744616 napari-threedee-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.704615 napari-threedee-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.708615 napari-threedee-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.708615 napari-threedee-0.0.7/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-05 09:26:48.744616 napari-threedee-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.708615 napari-threedee-0.0.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.712615 napari-threedee-0.0.7/docs/API/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/API/geometry_utilities.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/API/napari_utilities.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/API/selection_utilities.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.712615 napari-threedee-0.0.7/docs/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/annotations/io.md
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/annotations/point_spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/annotations/specifications.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/annotations/sphere_spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/annotations/spline_spec.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.712615 napari-threedee-0.0.7/docs/dev_guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/dev_guides/core_concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/dev_guides/manipulators.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.712615 napari-threedee-0.0.7/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.716615 napari-threedee-0.0.7/docs/examples/library/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/library/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/library/camera_spline_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/library/layer_manipulator_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/library/mesh_headlight_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/library/path_annotator_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/library/point_annotator_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/library/render_plane_manipulator_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/library/sphere_annotator_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/library/surface_annotator_library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.716615 napari-threedee-0.0.7/docs/examples/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/plugin/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/plugin/camera_spline_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/plugin/layer_manipulator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/plugin/mesh_headlight_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/plugin/path_annotator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/plugin/point_annotator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/plugin/points_manipulator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/plugin/render_plane_manipulator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/plugin/sphere_annotator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/plugin/spline_annotator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/examples/plugin/surface_annotator_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/gallery_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.716615 napari-threedee-0.0.7/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/getting_started/developers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/getting_started/users.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.716615 napari-threedee-0.0.7/docs/how_to/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/how_to/layer_manipulator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/how_to/point_annotator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/how_to/point_manipulator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/how_to/render_plane_manipulator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/how_to/sphere_annotator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/how_to/spline_annotator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.720615 napari-threedee-0.0.7/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/stylesheets/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.720615 napari-threedee-0.0.7/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/docs/tutorials/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-05 09:26:48.744616 napari-threedee-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.704615 napari-threedee-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.720615 napari-threedee-0.0.7/src/napari_threedee/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.720615 napari-threedee-0.0.7/src/napari_threedee/_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.724615 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.724615 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/test_axis_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/test_central_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/test_drag_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/test_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/test_manipulator_visual_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/test_rotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/axis_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/central_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/drag_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/manipulator_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/napari_manipulator_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/rotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/vispy_manipulator_visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/vispy_visual_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/threedee_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_backend/threedee_widget_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.728615 napari-threedee-0.0.7/src/napari_threedee/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_tests/test_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/_tests/test_mouse_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 09:26:48.000000 napari-threedee-0.0.7/src/napari_threedee/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.728615 napari-threedee-0.0.7/src/napari_threedee/annotators/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.728615 napari-threedee-0.0.7/src/napari_threedee/annotators/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/_qt/qt_path_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/_qt/qt_plane_point_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/_qt/qt_point_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/_qt/qt_sphere_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/_qt/qt_surface_annotator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.732616 napari-threedee-0.0.7/src/napari_threedee/annotators/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/_tests/test_point_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/_tests/test_sphere_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/_tests/test_spline_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.732616 napari-threedee-0.0.7/src/napari_threedee/annotators/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/paths/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/paths/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/paths/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.732616 napari-threedee-0.0.7/src/napari_threedee/annotators/points/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/points/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/points/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/points/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.732616 napari-threedee-0.0.7/src/napari_threedee/annotators/spheres/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/spheres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.732616 napari-threedee-0.0.7/src/napari_threedee/annotators/spheres/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/spheres/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/spheres/_tests/test_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/spheres/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/spheres/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/spheres/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.732616 napari-threedee-0.0.7/src/napari_threedee/annotators/surfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/surfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.736616 napari-threedee-0.0.7/src/napari_threedee/annotators/surfaces/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/surfaces/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/surfaces/_tests/test_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/surfaces/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/surfaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/annotators/surfaces/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.736616 napari-threedee-0.0.7/src/napari_threedee/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.736616 napari-threedee-0.0.7/src/napari_threedee/data_models/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/data_models/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/data_models/_tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/data_models/_tests/test_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/data_models/_tests/test_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/data_models/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/data_models/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/data_models/spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/data_models/spline_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/data_models/surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/dock_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.736616 napari-threedee-0.0.7/src/napari_threedee/manipulators/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/manipulators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.740615 napari-threedee-0.0.7/src/napari_threedee/manipulators/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/manipulators/_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/manipulators/_qt/qt_layer_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/manipulators/_qt/qt_point_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/manipulators/_qt/qt_render_plane_manipulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.740615 napari-threedee-0.0.7/src/napari_threedee/manipulators/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/manipulators/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/manipulators/_tests/test_manipulator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/manipulators/base_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/manipulators/layer_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/manipulators/manipulator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/manipulators/point_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/manipulators/render_plane_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.740615 napari-threedee-0.0.7/src/napari_threedee/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.740615 napari-threedee-0.0.7/src/napari_threedee/utils/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/utils/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/utils/_tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/utils/mouse_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/utils/napari_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/utils/selection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/vispy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.740615 napari-threedee-0.0.7/src/napari_threedee/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.744616 napari-threedee-0.0.7/src/napari_threedee/visualization/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/visualization/_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/visualization/_qt/qt_camera_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/visualization/_qt/qt_lighting_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.744616 napari-threedee-0.0.7/src/napari_threedee/visualization/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/visualization/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/visualization/_tests/test_camera_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/visualization/_tests/test_lighting_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/visualization/camera_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/src/napari_threedee/visualization/lighting_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:26:48.720615 napari-threedee-0.0.7/src/napari_threedee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-05 09:26:48.000000 napari-threedee-0.0.7/src/napari_threedee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-05-05 09:26:48.000000 napari-threedee-0.0.7/src/napari_threedee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:26:48.000000 napari-threedee-0.0.7/src/napari_threedee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 09:26:48.000000 napari-threedee-0.0.7/src/napari_threedee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 09:26:48.000000 napari-threedee-0.0.7/src/napari_threedee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 09:26:48.000000 napari-threedee-0.0.7/src/napari_threedee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-05 09:26:32.000000 napari-threedee-0.0.7/tox.ini
```

### Comparing `napari-threedee-0.0.6/.github/workflows/test_and_deploy.yml` & `napari-threedee-0.0.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/.gitignore` & `napari-threedee-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/LICENSE` & `napari-threedee-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/PKG-INFO` & `napari-threedee-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-threedee
-Version: 0.0.6
+Version: 0.0.7
 Summary: A suite of useful tools based on 3D interactivity in napari
 Home-page: https://github.com/alisterburt/napari-threedee
 Author: napari team
 Author-email: napari-steering-council@googlegroups.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/napari-threedee/napari-threedee/issues
 Project-URL: Documentation, https://github.com/napari-threedee/napari-threedee#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-threedee Version: 0.0.6 Summary: A suite of
+Metadata-Version: 2.1 Name: napari-threedee Version: 0.0.7 Summary: A suite of
 useful tools based on 3D interactivity in napari Home-page: https://github.com/
 alisterburt/napari-threedee Author: napari team Author-email: napari-steering-
 council@googlegroups.com License: BSD-3-Clause Project-URL: Bug Tracker, https:
 //github.com/napari-threedee/napari-threedee/issues Project-URL: Documentation,
 https://github.com/napari-threedee/napari-threedee#README.md Project-URL:
 Source Code, https://github.com/napari-threedee/napari-threedee Project-URL:
 User Support, https://github.com/napari-threedee/napari-threedee/issues
```

### Comparing `napari-threedee-0.0.6/README.md` & `napari-threedee-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/annotations/io.md` & `napari-threedee-0.0.7/docs/annotations/io.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/annotations/point_spec.md` & `napari-threedee-0.0.7/docs/annotations/point_spec.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/annotations/specifications.md` & `napari-threedee-0.0.7/docs/annotations/specifications.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/annotations/sphere_spec.md` & `napari-threedee-0.0.7/docs/annotations/sphere_spec.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/annotations/spline_spec.md` & `napari-threedee-0.0.7/docs/annotations/spline_spec.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/dev_guides/core_concepts.md` & `napari-threedee-0.0.7/docs/dev_guides/core_concepts.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/dev_guides/manipulators.md` & `napari-threedee-0.0.7/docs/dev_guides/manipulators.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/library/camera_spline_library.py` & `napari-threedee-0.0.7/docs/examples/library/camera_spline_library.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/library/mesh_headlight_library.py` & `napari-threedee-0.0.7/docs/examples/library/mesh_headlight_library.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/library/path_annotator_library.py` & `napari-threedee-0.0.7/docs/examples/library/path_annotator_library.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/library/point_annotator_library.py` & `napari-threedee-0.0.7/docs/examples/library/point_annotator_library.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/library/render_plane_manipulator_library.py` & `napari-threedee-0.0.7/docs/examples/library/render_plane_manipulator_library.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/library/sphere_annotator_library.py` & `napari-threedee-0.0.7/docs/examples/library/sphere_annotator_library.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/library/surface_annotator_library.py` & `napari-threedee-0.0.7/docs/examples/library/surface_annotator_library.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/plugin/camera_spline_plugin.py` & `napari-threedee-0.0.7/docs/examples/plugin/camera_spline_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/plugin/layer_manipulator_plugin.py` & `napari-threedee-0.0.7/docs/examples/plugin/layer_manipulator_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/plugin/mesh_headlight_plugin.py` & `napari-threedee-0.0.7/docs/examples/plugin/mesh_headlight_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/plugin/path_annotator_plugin.py` & `napari-threedee-0.0.7/docs/examples/plugin/path_annotator_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/plugin/point_annotator_plugin.py` & `napari-threedee-0.0.7/docs/examples/plugin/point_annotator_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/plugin/points_manipulator_plugin.py` & `napari-threedee-0.0.7/docs/examples/plugin/points_manipulator_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/plugin/render_plane_manipulator_plugin.py` & `napari-threedee-0.0.7/docs/examples/plugin/render_plane_manipulator_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/plugin/sphere_annotator_plugin.py` & `napari-threedee-0.0.7/docs/examples/plugin/sphere_annotator_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/plugin/spline_annotator_plugin.py` & `napari-threedee-0.0.7/docs/examples/plugin/spline_annotator_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/examples/plugin/surface_annotator_plugin.py` & `napari-threedee-0.0.7/docs/examples/plugin/surface_annotator_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/gallery_conf.py` & `napari-threedee-0.0.7/docs/gallery_conf.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/how_to/layer_manipulator.md` & `napari-threedee-0.0.7/docs/how_to/layer_manipulator.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/how_to/point_annotator.md` & `napari-threedee-0.0.7/docs/how_to/point_annotator.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/how_to/point_manipulator.md` & `napari-threedee-0.0.7/docs/how_to/point_manipulator.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/how_to/render_plane_manipulator.md` & `napari-threedee-0.0.7/docs/how_to/render_plane_manipulator.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/how_to/sphere_annotator.md` & `napari-threedee-0.0.7/docs/how_to/sphere_annotator.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/how_to/spline_annotator.md` & `napari-threedee-0.0.7/docs/how_to/spline_annotator.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/index.md` & `napari-threedee-0.0.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/docs/stylesheets/extra.css` & `napari-threedee-0.0.7/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/mkdocs.yml` & `napari-threedee-0.0.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/setup.cfg` & `napari-threedee-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/test_axis_model.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/test_axis_model.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/test_drag_manager.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/test_drag_manager.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/test_manipulator.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/test_manipulator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/_tests/test_manipulator_visual_data.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/_tests/test_manipulator_visual_data.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/axis_model.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/axis_model.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/central_axis.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/central_axis.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/drag_managers.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/drag_managers.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/manipulator_model.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/manipulator_model.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/napari_manipulator_backend.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/napari_manipulator_backend.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/rotator.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/rotator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/translator.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/translator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/utils.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/utils.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/vispy_manipulator_visual.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/vispy_manipulator_visual.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/manipulator/vispy_visual_data.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/manipulator/vispy_visual_data.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/threedee_model.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/threedee_model.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_backend/threedee_widget_base.py` & `napari-threedee-0.0.7/src/napari_threedee/_backend/threedee_widget_base.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_tests/test_dock_widget.py` & `napari-threedee-0.0.7/src/napari_threedee/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/_tests/test_mouse_callbacks.py` & `napari-threedee-0.0.7/src/napari_threedee/_tests/test_mouse_callbacks.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/_qt/qt_path_annotator.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/_qt/qt_path_annotator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/_qt/qt_surface_annotator.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/_qt/qt_surface_annotator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/_tests/conftest.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/_tests/test_point_annotator.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/_tests/test_point_annotator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/_tests/test_sphere_annotator.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/_tests/test_sphere_annotator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/_tests/test_spline_annotator.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/_tests/test_spline_annotator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/base.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/base.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/paths/annotator.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/paths/annotator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/paths/validation.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/paths/validation.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/points/_tests/test_data_model.py` & `napari-threedee-0.0.7/src/napari_threedee/data_models/_tests/test_points.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,19 @@
+import napari_threedee as n3d
 import numpy as np
 import zarr
 
 from napari_threedee.data_models import N3dPoints
-from napari_threedee.annotators.points.validation import validate_layer, validate_n3d_zarr
+from napari_threedee.annotators.points.validation import validate_layer, \
+    validate_n3d_zarr
+
+
+def test_empty_points():
+    points = n3d.data_models.N3dPoints(data=[])
+    assert points.data.shape == (0, 3)
 
 
 def test_instantiation():
     points = N3dPoints(data=np.random.uniform(low=0, high=10, size=(10, 3)))
     assert isinstance(points, N3dPoints)
 
 
@@ -20,8 +27,14 @@
 
 def test_to_and_from_n3d_zarr(tmp_path):
     points = N3dPoints(data=np.random.uniform(low=0, high=10, size=(10, 3)))
     points.to_n3d_zarr(tmp_path)
     n3d_zarr = zarr.open(tmp_path)
     validate_n3d_zarr(n3d_zarr)
     points = N3dPoints.from_n3d_zarr(tmp_path)
-    assert isinstance(points, N3dPoints)
+    assert isinstance(points, N3dPoints)
+
+
+def test_empty_points_as_layer():
+    points = N3dPoints(data=[])
+    layer = points.as_layer()
+    assert layer.ndim == 3
```

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/points/annotator.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/points/annotator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/points/validation.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/points/validation.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/spheres/_tests/test_data_model.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/spheres/_tests/test_data_model.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/spheres/annotator.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/spheres/annotator.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,26 +62,26 @@
 
     @property
     def active_sphere_radius(self) -> Union[float, None]:
         df = features_to_pandas_dataframe(self.points_layer.features)
         if len(df) == 0:
             return None
         else:
-            return float(
-                df[SPHERE_RADIUS_FEATURES_KEY].iloc[self._active_sphere_index])
+            radius = df[SPHERE_RADIUS_FEATURES_KEY].iloc[self._active_sphere_index]
+            return float(radius)
 
     @property
     def _active_sphere_index(self) -> Union[int, None]:
         """index into data/features of current sphere"""
-        if self.active_sphere_id is None:
+        if self.points_layer is None:
+            return None
+        elif list(self.points_layer.selected_data) != []:
+            return int(list(self.points_layer.selected_data)[0])
+        else:
             return None
-        df = features_to_pandas_dataframe(self.points_layer.features)
-        idx = df[SPHERE_ID_FEATURES_KEY] == self.active_sphere_id
-        df = df.loc[idx, :]
-        return df.index.values[0]
 
     @property
     def mode(self) -> SphereAnnotatorMode:
         return self._mode
 
     @mode.setter
     def mode(self, value: SphereAnnotatorMode):
@@ -236,8 +236,7 @@
     def _enable_add_mode(self, event=None):
         """Callback for enabling add mode."""
         self.mode = SphereAnnotatorMode.ADD
 
     def _on_highlight_change(self, event=None):
         """Callback for enabling edit mode."""
         self.mode = SphereAnnotatorMode.EDIT
-
```

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/spheres/validation.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/spheres/validation.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/surfaces/_tests/test_data_model.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/surfaces/_tests/test_data_model.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/surfaces/annotator.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/surfaces/annotator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/annotators/surfaces/validation.py` & `napari-threedee-0.0.7/src/napari_threedee/annotators/surfaces/validation.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/conftest.py` & `napari-threedee-0.0.7/src/napari_threedee/conftest.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/data_models/_tests/test_paths.py` & `napari-threedee-0.0.7/src/napari_threedee/data_models/_tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/data_models/paths.py` & `napari-threedee-0.0.7/src/napari_threedee/data_models/paths.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/data_models/points.py` & `napari-threedee-0.0.7/src/napari_threedee/data_models/points.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,21 @@
     data: np.ndarray
 
     @classmethod
     def from_layer(cls, layer: napari.layers.Points):
         return cls(data=layer.data)
 
     def as_layer(self) -> napari.layers.Points:
+        if len(self.data) == 0:  # workaround for napari/napari#4213
+            cls = type(self)
+            n3d_points = cls(data=[0, 0, 0])
+            layer = n3d_points.as_layer()
+            layer.selected_data = {0}
+            layer.remove_selected()
+            return layer
         metadata = {N3D_METADATA_KEY: {ANNOTATION_TYPE_KEY: POINT_ANNOTATION_TYPE_KEY}}
         layer = napari.layers.Points(
             data=self.data,
             metadata=metadata,
             name='n3d points',
             ndim=self.data.shape[-1],
         )
```

### Comparing `napari-threedee-0.0.6/src/napari_threedee/data_models/spheres.py` & `napari-threedee-0.0.7/src/napari_threedee/data_models/spheres.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/data_models/spline_sampler.py` & `napari-threedee-0.0.7/src/napari_threedee/data_models/spline_sampler.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/data_models/surfaces.py` & `napari-threedee-0.0.7/src/napari_threedee/data_models/surfaces.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/manipulators/_tests/test_manipulator_utils.py` & `napari-threedee-0.0.7/src/napari_threedee/manipulators/_tests/test_manipulator_utils.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/manipulators/base_manipulator.py` & `napari-threedee-0.0.7/src/napari_threedee/manipulators/base_manipulator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/manipulators/layer_manipulator.py` & `napari-threedee-0.0.7/src/napari_threedee/manipulators/layer_manipulator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/manipulators/manipulator_utils.py` & `napari-threedee-0.0.7/src/napari_threedee/manipulators/manipulator_utils.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/manipulators/point_manipulator.py` & `napari-threedee-0.0.7/src/napari_threedee/manipulators/point_manipulator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/manipulators/render_plane_manipulator.py` & `napari-threedee-0.0.7/src/napari_threedee/manipulators/render_plane_manipulator.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/napari.yaml` & `napari-threedee-0.0.7/src/napari_threedee/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/utils/_tests/test_geometry.py` & `napari-threedee-0.0.7/src/napari_threedee/utils/_tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/utils/geometry.py` & `napari-threedee-0.0.7/src/napari_threedee/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/utils/mouse_callbacks.py` & `napari-threedee-0.0.7/src/napari_threedee/utils/mouse_callbacks.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/utils/napari_utils.py` & `napari-threedee-0.0.7/src/napari_threedee/utils/napari_utils.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/utils/selection_utils.py` & `napari-threedee-0.0.7/src/napari_threedee/utils/selection_utils.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/visualization/_qt/qt_camera_spline.py` & `napari-threedee-0.0.7/src/napari_threedee/visualization/_qt/qt_camera_spline.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/visualization/_qt/qt_lighting_control.py` & `napari-threedee-0.0.7/src/napari_threedee/visualization/_qt/qt_lighting_control.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/visualization/_tests/test_camera_spline.py` & `napari-threedee-0.0.7/src/napari_threedee/visualization/_tests/test_camera_spline.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/visualization/_tests/test_lighting_control.py` & `napari-threedee-0.0.7/src/napari_threedee/visualization/_tests/test_lighting_control.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/visualization/camera_spline.py` & `napari-threedee-0.0.7/src/napari_threedee/visualization/camera_spline.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee/visualization/lighting_control.py` & `napari-threedee-0.0.7/src/napari_threedee/visualization/lighting_control.py`

 * *Files identical despite different names*

### Comparing `napari-threedee-0.0.6/src/napari_threedee.egg-info/PKG-INFO` & `napari-threedee-0.0.7/src/napari_threedee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-threedee
-Version: 0.0.6
+Version: 0.0.7
 Summary: A suite of useful tools based on 3D interactivity in napari
 Home-page: https://github.com/alisterburt/napari-threedee
 Author: napari team
 Author-email: napari-steering-council@googlegroups.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/napari-threedee/napari-threedee/issues
 Project-URL: Documentation, https://github.com/napari-threedee/napari-threedee#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-threedee Version: 0.0.6 Summary: A suite of
+Metadata-Version: 2.1 Name: napari-threedee Version: 0.0.7 Summary: A suite of
 useful tools based on 3D interactivity in napari Home-page: https://github.com/
 alisterburt/napari-threedee Author: napari team Author-email: napari-steering-
 council@googlegroups.com License: BSD-3-Clause Project-URL: Bug Tracker, https:
 //github.com/napari-threedee/napari-threedee/issues Project-URL: Documentation,
 https://github.com/napari-threedee/napari-threedee#README.md Project-URL:
 Source Code, https://github.com/napari-threedee/napari-threedee Project-URL:
 User Support, https://github.com/napari-threedee/napari-threedee/issues
```

### Comparing `napari-threedee-0.0.6/src/napari_threedee.egg-info/SOURCES.txt` & `napari-threedee-0.0.7/src/napari_threedee.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -108,16 +108,14 @@
 src/napari_threedee/annotators/paths/annotator.py
 src/napari_threedee/annotators/paths/constants.py
 src/napari_threedee/annotators/paths/validation.py
 src/napari_threedee/annotators/points/__init__.py
 src/napari_threedee/annotators/points/annotator.py
 src/napari_threedee/annotators/points/constants.py
 src/napari_threedee/annotators/points/validation.py
-src/napari_threedee/annotators/points/_tests/__init__.py
-src/napari_threedee/annotators/points/_tests/test_data_model.py
 src/napari_threedee/annotators/spheres/__init__.py
 src/napari_threedee/annotators/spheres/annotator.py
 src/napari_threedee/annotators/spheres/constants.py
 src/napari_threedee/annotators/spheres/validation.py
 src/napari_threedee/annotators/spheres/_tests/__init__.py
 src/napari_threedee/annotators/spheres/_tests/test_data_model.py
 src/napari_threedee/annotators/surfaces/__init__.py
```

### Comparing `napari-threedee-0.0.6/tox.ini` & `napari-threedee-0.0.7/tox.ini`

 * *Files identical despite different names*

