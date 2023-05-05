# Comparing `tmp/raillabel-2.0.4.tar.gz` & `tmp/raillabel-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raillabel-2.0.4.tar", last modified: Tue Mar 28 09:20:05 2023, max compression
+gzip compressed data, was "raillabel-2.1.0.tar", last modified: Fri May  5 13:39:13 2023, max compression
```

## Comparing `raillabel-2.0.4.tar` & `raillabel-2.1.0.tar`

### file list

```diff
@@ -1,119 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.355970 raillabel-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-28 09:19:47.000000 raillabel-2.0.4/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-28 09:19:47.000000 raillabel-2.0.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.339969 raillabel-2.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.343969 raillabel-2.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-03-28 09:19:47.000000 raillabel-2.0.4/.github/workflows/build-test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-28 09:19:47.000000 raillabel-2.0.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-28 09:19:47.000000 raillabel-2.0.4/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-03-28 09:19:47.000000 raillabel-2.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-03-28 09:19:47.000000 raillabel-2.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-28 09:19:47.000000 raillabel-2.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-03-28 09:19:47.000000 raillabel-2.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-28 09:19:47.000000 raillabel-2.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.343969 raillabel-2.0.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-28 09:19:47.000000 raillabel-2.0.4/LICENSES/.license_header.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-28 09:19:47.000000 raillabel-2.0.4/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-03-28 09:19:47.000000 raillabel-2.0.4/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-28 09:20:05.355970 raillabel-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-28 09:19:47.000000 raillabel-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.343969 raillabel-2.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-28 09:19:47.000000 raillabel-2.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-28 09:19:47.000000 raillabel-2.0.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.343969 raillabel-2.0.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.347969 raillabel-2.0.4/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-28 09:19:47.000000 raillabel-2.0.4/docs/source/_static/github-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-03-28 09:19:47.000000 raillabel-2.0.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-28 09:19:47.000000 raillabel-2.0.4/docs/source/howto.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.347969 raillabel-2.0.4/docs/source/howtos/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-28 09:19:47.000000 raillabel-2.0.4/docs/source/howtos/1 Validating Annotation Files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-28 09:19:47.000000 raillabel-2.0.4/docs/source/howtos/2 Loading Annotation Files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-28 09:19:47.000000 raillabel-2.0.4/docs/source/howtos/3 Saving Annotation Files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-28 09:19:47.000000 raillabel-2.0.4/docs/source/howtos/4 Filtering Scenes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-28 09:19:47.000000 raillabel-2.0.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-28 09:19:47.000000 raillabel-2.0.4/docs/source/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-28 09:19:47.000000 raillabel-2.0.4/git-conventional-commits.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-28 09:19:47.000000 raillabel-2.0.4/git-conventional-commits.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-03-28 09:19:47.000000 raillabel-2.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.347969 raillabel-2.0.4/raillabel/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.347969 raillabel-2.0.4/raillabel/_filter_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/_filter_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/_filter_classes/_filter_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/_filter_classes/_filter_annotation_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/_filter_classes/_filter_annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/_filter_classes/_filter_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/_filter_classes/_filter_end.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/_filter_classes/_filter_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/_filter_classes/_filter_object_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/_filter_classes/_filter_object_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/_filter_classes/_filter_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/_filter_classes/_filter_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.351970 raillabel-2.0.4/raillabel/format/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/cuboid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/frame_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/intrinsics_pinhole.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/num.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/object_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/point2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/point3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/poly2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/poly3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/seg3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/sensor_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/size2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/size3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.351970 raillabel-2.0.4/raillabel/format_loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format_loaders/_loader_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format_loaders/loader_raillabel_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format_loaders/translation.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/format_loaders/translation.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.351970 raillabel-2.0.4/raillabel/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    38262 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/schemas/raillabel_v2_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/schemas/raillabel_v2_schema.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-28 09:19:47.000000 raillabel-2.0.4/raillabel/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.347969 raillabel-2.0.4/raillabel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-28 09:20:05.000000 raillabel-2.0.4/raillabel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-03-28 09:20:05.000000 raillabel-2.0.4/raillabel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 09:20:05.000000 raillabel-2.0.4/raillabel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 09:20:04.000000 raillabel-2.0.4/raillabel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-28 09:20:05.000000 raillabel-2.0.4/raillabel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-28 09:20:05.000000 raillabel-2.0.4/raillabel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 09:20:05.355970 raillabel-2.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.355970 raillabel-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/master_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.355970 raillabel-2.0.4/tests/test_raillabel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.355970 raillabel-2.0.4/tests/test_raillabel/__test_assets__/
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/__test_assets__/metaschema.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/__test_assets__/metaschema.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    85872 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    57194 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5.license
--rw-r--r--   0 runner    (1001) docker     (123)    50508 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.355970 raillabel-2.0.4/tests/test_raillabel/format/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/format/test_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.355970 raillabel-2.0.4/tests/test_raillabel/format_loaders/
--rw-r--r--   0 runner    (1001) docker     (123)    54821 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/format_loaders/test_loader_raillabel_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:20:05.355970 raillabel-2.0.4/tests/test_raillabel/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/schemas/test_raillabel_v2_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-03-28 09:19:47.000000 raillabel-2.0.4/tests/test_raillabel/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-05 13:38:57.000000 raillabel-2.1.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-05 13:38:57.000000 raillabel-2.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.949673 raillabel-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-05 13:38:57.000000 raillabel-2.1.0/.github/workflows/build-test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-05 13:38:57.000000 raillabel-2.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-05 13:38:57.000000 raillabel-2.1.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-05 13:38:57.000000 raillabel-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-05 13:38:57.000000 raillabel-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-05 13:38:57.000000 raillabel-2.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-05 13:38:57.000000 raillabel-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 13:38:57.000000 raillabel-2.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 13:38:57.000000 raillabel-2.1.0/LICENSES/.license_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-05 13:38:57.000000 raillabel-2.1.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-05 13:38:57.000000 raillabel-2.1.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-05 13:39:13.961673 raillabel-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-05 13:38:57.000000 raillabel-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/_static/github-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/howto.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/docs/source/howtos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/howtos/1 Validating Annotation Files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/howtos/2 Loading Annotation Files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/howtos/3 Saving Annotation Files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/howtos/4 Filtering Scenes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-05 13:38:57.000000 raillabel-2.1.0/docs/source/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-05 13:38:57.000000 raillabel-2.1.0/git-conventional-commits.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/git-conventional-commits.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-05 13:38:57.000000 raillabel-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.953673 raillabel-2.1.0/raillabel/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.957673 raillabel-2.1.0/raillabel/_filter_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_annotation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_object_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_object_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_filter_classes/_filter_start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.957673 raillabel-2.1.0/raillabel/_util/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/_util/_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/raillabel/format/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/frame_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/intrinsics_pinhole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/intrinsics_radar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/num.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/object_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/point3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/poly2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/poly3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/seg3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/sensor_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/size2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/size3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/raillabel/format_loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format_loaders/_loader_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format_loaders/loader_raillabel_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format_loaders/translation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/format_loaders/translation.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/raillabel/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    39070 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/schemas/raillabel_v2_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/schemas/raillabel_v2_schema.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-05 13:38:57.000000 raillabel-2.1.0/raillabel/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.957673 raillabel-2.1.0/raillabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-05 13:39:13.000000 raillabel-2.1.0/raillabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-05 13:39:13.000000 raillabel-2.1.0/raillabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:39:13.000000 raillabel-2.1.0/raillabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:39:13.000000 raillabel-2.1.0/raillabel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 13:39:13.000000 raillabel-2.1.0/raillabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 13:39:13.000000 raillabel-2.1.0/raillabel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:39:13.961673 raillabel-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/master_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/tests/test_raillabel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/tests/test_raillabel/__test_assets__/
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/metaschema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/metaschema.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    85872 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60789 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5.license
+-rw-r--r--   0 runner    (1001) docker     (123)    54074 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/tests/test_raillabel/format/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/format/test_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/tests/test_raillabel/format_loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/format_loaders/test_loader_raillabel_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:39:13.961673 raillabel-2.1.0/tests/test_raillabel/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/schemas/test_raillabel_v2_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-05 13:38:57.000000 raillabel-2.1.0/tests/test_raillabel/test_validate.py
```

### Comparing `raillabel-2.0.4/.github/workflows/build-test-publish.yml` & `raillabel-2.1.0/.github/workflows/build-test-publish.yml`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/.github/workflows/docs.yml` & `raillabel-2.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/.github/workflows/lint.yml` & `raillabel-2.1.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/.gitignore` & `raillabel-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/.pre-commit-config.yaml` & `raillabel-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/CHANGELOG.md` & `raillabel-2.1.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,7 +43,10 @@
 - Changed name of PyPI package back to 'raillabel' because the problematic package has been removed
 
 ## 2.0.3
 - Fixed bug related to saving the annotator field in the metadata
 
 ## 2.0.4
 - Fixed bug related to the package version
+
+# 2.1.0
+- Added IntrinsicsRadar to the devkit and the json-schema
```

### Comparing `raillabel-2.0.4/CONTRIBUTING.md` & `raillabel-2.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/LICENSE` & `raillabel-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/LICENSES/Apache-2.0.txt` & `raillabel-2.1.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/LICENSES/CC0-1.0.txt` & `raillabel-2.1.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/PKG-INFO` & `raillabel-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raillabel
-Version: 2.0.4
+Version: 2.1.0
 Summary: A devkit for working with recorded and annotated train ride data from Deutsche Bahn.
 Author: DB Netz AG
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/DSD-DBS/raillabel
 Project-URL: Documentation, https://dsd-dbs.github.io/raillabel
 Platform: any
 Classifier: Development Status :: 1 - Planning
```

### Comparing `raillabel-2.0.4/README.md` & `raillabel-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/docs/Makefile` & `raillabel-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/docs/make.bat` & `raillabel-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/docs/source/_static/github-logo.svg` & `raillabel-2.1.0/docs/source/_static/github-logo.svg`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/docs/source/conf.py` & `raillabel-2.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/docs/source/howtos/1 Validating Annotation Files.rst` & `raillabel-2.1.0/docs/source/howtos/1 Validating Annotation Files.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/docs/source/howtos/2 Loading Annotation Files.rst` & `raillabel-2.1.0/docs/source/howtos/2 Loading Annotation Files.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/docs/source/howtos/3 Saving Annotation Files.rst` & `raillabel-2.1.0/docs/source/howtos/3 Saving Annotation Files.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/docs/source/howtos/4 Filtering Scenes.rst` & `raillabel-2.1.0/docs/source/howtos/4 Filtering Scenes.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/docs/source/index.rst` & `raillabel-2.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/docs/source/intro.rst` & `raillabel-2.1.0/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/pyproject.toml` & `raillabel-2.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
   "pytest-cov",
   "json5"
 ]
 
 [tool.black]
 line-length = 100
 target-version = ["py38"]
+force-exclude = "tests/"
 
 [tool.docformatter]
 wrap-descriptions = 72
 wrap-summaries = 79
 
 [tool.isort]
 profile = 'black'
@@ -114,32 +115,35 @@
   "broad-except",
   "global-statement",
   "import-outside-toplevel",
   "invalid-name",
   "missing-class-docstring",
   "missing-function-docstring",
   "missing-module-docstring",
+  "logging-not-lazy",
   "no-else-break",
   "no-else-continue",
   "no-else-raise",
   "no-else-return",
+  "no-self-argument",
   "protected-access",
   "redefined-builtin",
   "too-few-public-methods",
   "too-many-ancestors",
   "too-many-arguments",
   "too-many-boolean-expressions",
   "too-many-branches",
   "too-many-instance-attributes",
   "too-many-lines",
   "too-many-locals",
   "too-many-public-methods",
   "too-many-return-statements",
   "too-many-statements",
   "unspecified-encoding",
+  "unsupported-membership-test",
   "dangerous-default-value",
 
   # Auto-formatting
   "bad-indentation",
   "inconsistent-quotes",
   "missing-final-newline",
   "mixed-line-endings",
```

### Comparing `raillabel-2.0.4/raillabel/_filter_classes/__init__.py` & `raillabel-2.1.0/raillabel/_filter_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/_filter_classes/_filter_abc.py` & `raillabel-2.1.0/raillabel/_filter_classes/_filter_abc.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/_filter_classes/_filter_annotation_ids.py` & `raillabel-2.1.0/raillabel/_filter_classes/_filter_annotation_ids.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/_filter_classes/_filter_annotation_types.py` & `raillabel-2.1.0/raillabel/_filter_classes/_filter_annotation_types.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/_filter_classes/_filter_attributes.py` & `raillabel-2.1.0/raillabel/_filter_classes/_filter_attributes.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/_filter_classes/_filter_end.py` & `raillabel-2.1.0/raillabel/_filter_classes/_filter_end.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/_filter_classes/_filter_frames.py` & `raillabel-2.1.0/raillabel/_filter_classes/_filter_frames.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/_filter_classes/_filter_object_ids.py` & `raillabel-2.1.0/raillabel/_filter_classes/_filter_object_ids.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/_filter_classes/_filter_object_types.py` & `raillabel-2.1.0/raillabel/_filter_classes/_filter_object_types.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/_filter_classes/_filter_sensors.py` & `raillabel-2.1.0/raillabel/_filter_classes/_filter_sensors.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/_filter_classes/_filter_start.py` & `raillabel-2.1.0/raillabel/_filter_classes/_filter_start.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/exceptions.py` & `raillabel-2.1.0/raillabel/exceptions.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/filter.py` & `raillabel-2.1.0/raillabel/filter.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/format/__init__.py` & `raillabel-2.1.0/raillabel/format/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 """Module containing all relevant OpenLABEL format classes."""
 
 from .bbox import Bbox
 from .cuboid import Cuboid
 from .frame import Frame
 from .frame_interval import FrameInterval
 from .intrinsics_pinhole import IntrinsicsPinhole
+from .intrinsics_radar import IntrinsicsRadar
 from .metadata import Metadata
 from .num import Num
 from .object import Object
-from .object_data import AnnotationContainer, ObjectData
+from .object_data import ObjectData
 from .point2d import Point2d
 from .point3d import Point3d
 from .poly2d import Poly2d
 from .poly3d import Poly3d
 from .quaternion import Quaternion
 from .scene import Scene
 from .seg3d import Seg3d
-from .sensor import Sensor
+from .sensor import Sensor, SensorType
 from .sensor_reference import SensorReference
 from .size2d import Size2d
 from .size3d import Size3d
 from .transform import Transform
```

### Comparing `raillabel-2.0.4/raillabel/format/_annotation.py` & `raillabel-2.1.0/raillabel/format/_annotation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright DB Netz AG and contributors
 # SPDX-License-Identifier: Apache-2.0
 
 import typing as t
 from abc import ABC, abstractmethod, abstractproperty
 from dataclasses import dataclass, field
 
+from .._util._warning import _warning
 from .sensor import Sensor
 
 
 @dataclass
 class _Annotation(ABC):
 
     uid: str
@@ -17,51 +18,28 @@
     sensor: Sensor = None
 
     @property
     @abstractproperty
     def _REQ_FIELDS(self) -> t.List[str]:
         raise NotImplementedError
 
+    @property
+    @abstractproperty
+    def OPENLABEL_ID(self) -> t.List[str]:
+        raise NotImplementedError
+
     # === Public Methods =====================================================
 
     @abstractmethod
     def asdict(self) -> t.Dict:
-        """Export self as a dict compatible with the OpenLABEL schema.
-
-        Returns
-        -------
-        dict_repr: dict
-            Dict representation of this class instance.
-
-        Raises
-        ------
-        ValueError
-            if an attribute can not be converted to the type required by the OpenLabel schema.
-        """
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
-    def fromdict(self, data_dict: t.Dict, sensors: t.Dict) -> t.Tuple[t.Dict, list]:
-        """Generate a Bbox object from a dictionary in the OpenLABEL format.
-
-        Parameters
-        ----------
-        data_dict: dict
-            OpenLABEL format dictionary containing the data for the annotation.
-        sensors: dict
-            Dictionary containing all sensors for the scene.
-
-        Returns
-        -------
-        annotation: Bbox
-            Converted annotation.
-        warnings: list of str
-            List of non-critical errors, that have occurred during the conversion.
-        """
+    def fromdict(self, data_dict: t.Dict, sensors: t.Dict) -> t.Type["_Annotation"]:
         raise NotImplementedError
 
     # === Private Methods ====================================================
 
     def _annotation_required_fields_asdict(self) -> t.Dict:
         """Return the required fields from the parent class to dict."""
         return {
@@ -107,14 +85,41 @@
                 if attr_type not in dict_repr["attributes"]:
                     dict_repr["attributes"][attr_type] = []
 
                 dict_repr["attributes"][attr_type].append({"name": attr_name, "val": attr_value})
 
         return dict_repr
 
+    def _coordinate_system_fromdict(data_dict: dict, sensors: dict) -> t.Optional[Sensor]:
+
+        is_coordinate_system_in_data = (
+            "coordinate_system" in data_dict and data_dict["coordinate_system"] != ""
+        )
+
+        if not is_coordinate_system_in_data:
+            return None
+
+        if data_dict["coordinate_system"] not in sensors:
+            _warning(
+                f"{data_dict['coordinate_system']} does not exist as a coordinate system, "
+                + f"but is referenced for the annotation {data_dict['uid']}."
+            )
+            return None
+
+        return sensors[data_dict["coordinate_system"]]
+
+    def _attributes_fromdict(
+        data_dict: dict,
+    ) -> t.Dict[str, t.Union[int, float, bool, str, list]]:
+
+        if "attributes" not in data_dict:
+            return {}
+
+        return {a["name"]: a["val"] for l in data_dict["attributes"].values() for a in l}
+
     # === Special Methods ====================================================
 
     def __post_init__(self):
         """Check for required arguments after __init__.
 
         Inheritance in dataclasses has the flaw, that when the parent class has fields with
         defaults and the child class has fields without, a TypeError is raised due to required
```

### Comparing `raillabel-2.0.4/raillabel/format/bbox.py` & `raillabel-2.1.0/raillabel/format/cuboid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,93 @@
 # Copyright DB Netz AG and contributors
 # SPDX-License-Identifier: Apache-2.0
 
-import typing as t
 from dataclasses import dataclass
 
 from ._annotation import _Annotation
-from .point2d import Point2d
-from .size2d import Size2d
+from .point3d import Point3d
+from .quaternion import Quaternion
+from .size3d import Size3d
 
 
 @dataclass
-class Bbox(_Annotation):
-    """A 2D bounding box in an image.
+class Cuboid(_Annotation):
+    """3D bounding box.
 
     Parameters
     ----------
     uid: str
         This a string representing the unique universal identifier of the annotation.
     name: str
         Human readable name describing the annotation.
-    pos: raillabel.format.Point2d
-        The center point of the bbox in pixels.
-    size: raillabel.format.Size2d
-        The dimensions of the bbox in pixels from the top left corner to the bottom right corner.
+    pos: raillabel.format.Point3d
+        The center position of the cuboid in meters, where the x coordinate points ahead of the
+        vehicle, y points to the left and z points upwards.
+    quat: raillabel.format.Quaternion
+        The rotation of the cuboid in quaternions.
+    size: raillabel.format.Size3d
+        The size of the cuboid in meters.
     attributes: dict, optional
         Attributes of the annotation. Dict keys are the name str of the attribute, values are the
         attribute values. Default is {}.
     sensor: raillabel.format.CoordinateSystem, optional
         A reference to the sensor, this annotation is labeled in. Default is None.
     """
 
-    pos: Point2d = None
-    size: Size2d = None
+    pos: Point3d = None
+    quat: Quaternion = None
+    size: Size3d = None
 
-    _REQ_FIELDS = ["pos", "size"]
+    OPENLABEL_ID = "cuboid"
+    _REQ_FIELDS = ["pos", "size", "quat"]
 
     @classmethod
-    def fromdict(self, data_dict: dict, sensors: dict) -> t.Tuple["Bbox", list]:
-        """Generate a Bbox object from a dictionary in the OpenLABEL format.
+    def fromdict(
+        self,
+        data_dict: dict,
+        sensors: dict,
+    ) -> "Cuboid":
+        """Generate a Cuboid object from a dict.
 
         Parameters
         ----------
         data_dict: dict
-            OpenLABEL format dictionary containing the data for the annotation.
+            RailLabel format snippet containing the relevant data.
         sensors: dict
             Dictionary containing all sensors for the scene.
 
         Returns
         -------
-        annotation: Bbox
+        annotation: Cuboid
             Converted annotation.
-        warnings: list of str
-            List of non-critical errors, that have occurred during the conversion.
         """
 
-        warnings = []  # list of warnings, that have occurred during the parsing
-
-        # Creates the annotation with all mandatory properties
-        annotation = Bbox(
+        return Cuboid(
             uid=str(data_dict["uid"]),
             name=str(data_dict["name"]),
-            pos=Point2d(x=data_dict["val"][0], y=data_dict["val"][1]),
-            size=Size2d(x=data_dict["val"][2], y=data_dict["val"][3]),
+            pos=Point3d(
+                x=data_dict["val"][0],
+                y=data_dict["val"][1],
+                z=data_dict["val"][2],
+            ),
+            quat=Quaternion(
+                x=data_dict["val"][3],
+                y=data_dict["val"][4],
+                z=data_dict["val"][5],
+                w=data_dict["val"][6],
+            ),
+            size=Size3d(
+                x=data_dict["val"][7],
+                y=data_dict["val"][8],
+                z=data_dict["val"][9],
+            ),
+            sensor=self._coordinate_system_fromdict(data_dict, sensors),
+            attributes=self._attributes_fromdict(data_dict),
         )
 
-        # Adds the optional properties
-        if "coordinate_system" in data_dict and data_dict["coordinate_system"] != "":
-            try:
-                annotation.sensor = sensors[data_dict["coordinate_system"]]
-
-            except KeyError:
-                warnings.append(
-                    f"{data_dict['coordinate_system']} does not exist as a coordinate system, "
-                    + f"but is referenced for the annotation {data_dict['uid']}."
-                )
-
-        # Adds the attributes
-        if "attributes" in data_dict:
-            annotation.attributes = {
-                a["name"]: a["val"] for l in data_dict["attributes"].values() for a in l
-            }
-
-        return annotation, warnings
-
     def asdict(self) -> dict:
         """Export self as a dict compatible with the OpenLABEL schema.
 
         Returns
         -------
         dict_repr: dict
             Dict representation of this class instance.
@@ -98,14 +99,20 @@
         """
 
         dict_repr = self._annotation_required_fields_asdict()
 
         dict_repr["val"] = [
             float(self.pos.x),
             float(self.pos.y),
+            float(self.pos.z),
+            float(self.quat.x),
+            float(self.quat.y),
+            float(self.quat.z),
+            float(self.quat.w),
             float(self.size.x),
             float(self.size.y),
+            float(self.size.z),
         ]
 
         dict_repr.update(self._annotation_optional_fields_asdict())
 
         return dict_repr
```

### Comparing `raillabel-2.0.4/raillabel/format/frame_interval.py` & `raillabel-2.1.0/raillabel/format/frame_interval.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/format/intrinsics_pinhole.py` & `raillabel-2.1.0/raillabel/format/intrinsics_pinhole.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,14 +26,36 @@
     """
 
     camera_matrix: t.Tuple[float, ...]
     distortion: t.Tuple[float, ...]
     width_px: int
     height_px: int
 
+    @classmethod
+    def fromdict(self, data_dict: dict) -> "IntrinsicsPinhole":
+        """Generate a IntrinsicsPinhole object from a dict.
+
+        Parameters
+        ----------
+        data_dict: dict
+            RailLabel format snippet containing the relevant data.
+
+        Returns
+        -------
+        raillabel.format.IntrinsicsPinhole
+            Converted IntrinsicsPinhole object.
+        """
+
+        return IntrinsicsPinhole(
+            camera_matrix=data_dict["camera_matrix"],
+            distortion=data_dict["distortion_coeffs"],
+            width_px=data_dict["width_px"],
+            height_px=data_dict["height_px"],
+        )
+
     def asdict(self) -> dict:
         """Export self as a dict compatible with the OpenLABEL schema.
 
         Returns
         -------
         dict_repr: dict
             Dict representation of this class instance.
```

### Comparing `raillabel-2.0.4/raillabel/format/metadata.py` & `raillabel-2.1.0/raillabel/format/metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,60 +37,41 @@
     file_version: t.Optional[str] = None
     name: t.Optional[str] = None
     subschema_version: t.Optional[str] = None
     tagged_file: t.Optional[str] = None
 
     @classmethod
     def fromdict(cls, data_dict: dict, subschema_version: t.Optional[str] = None) -> "Metadata":
-        """Generate a Metadata from a dictionary in the OpenLABEL format.
+        """Generate a Metadata object from a dict.
 
         Parameters
         ----------
         data_dict: dict
-            OpenLABEL format dictionary containing the data_dict.
+            RailLabel format snippet containing the relevant data.
         subschema_version: str, optional
             Version of the RailLabel subschema
 
         Returns
         -------
         metadata: Metadata
             Converted metadata.
         warnings: list of str
             List of non-critical errors, that have occurred during the conversion.
         """
 
-        metadata = Metadata(schema_version=data_dict["schema_version"])
-
-        if subschema_version is not None:
-            metadata.subschema_version = subschema_version
-
-        if "annotator" in data_dict:
-            metadata.annotator = data_dict["annotator"]
-
-        if "file_version" in data_dict:
-            metadata.file_version = data_dict["file_version"]
-
-        if "name" in data_dict:
-            metadata.name = data_dict["name"]
-
-        if "tagged_file" in data_dict:
-            metadata.tagged_file = data_dict["tagged_file"]
-
-        if "comment" in data_dict:
-            metadata.comment = data_dict["comment"]
-
-        try:
-            exporter_version = importlib_metadata.version("raillabel")
-        except importlib_metadata.PackageNotFoundError:
-            pass
-        else:
-            version_number_length = len(exporter_version) - len(exporter_version.split(".")[-1])
-            metadata.exporter_version = exporter_version[: version_number_length - 1]
-
-        return metadata
+        return Metadata(
+            schema_version=data_dict["schema_version"],
+            subschema_version=subschema_version,
+            annotator=data_dict.get("annotator"),
+            file_version=data_dict.get("file_version"),
+            name=data_dict.get("name"),
+            tagged_file=data_dict.get("tagged_file"),
+            comment=data_dict.get("comment"),
+            exporter_version=cls._collect_exporter_version(),
+        )
 
     def asdict(self) -> dict:
         """Export self as a dict compatible with the OpenLABEL schema.
 
         Returns
         -------
         dict_repr: dict
@@ -122,7 +103,18 @@
         if self.subschema_version is not None:
             dict_repr["subschema_version"] = str(self.subschema_version)
 
         if self.tagged_file is not None:
             dict_repr["tagged_file"] = str(self.tagged_file)
 
         return dict_repr
+
+    @classmethod
+    def _collect_exporter_version(cls) -> t.Optional[str]:
+
+        try:
+            exporter_version = importlib_metadata.version("raillabel")
+        except importlib_metadata.PackageNotFoundError:
+            return None
+
+        version_number_length = len(exporter_version) - len(exporter_version.split(".")[-1])
+        return exporter_version[: version_number_length - 1]
```

### Comparing `raillabel-2.0.4/raillabel/format/num.py` & `raillabel-2.1.0/raillabel/format/num.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,64 +24,42 @@
         attribute values. Default is {}.
     sensor: raillabel.format.CoordinateSystem, optional
         A reference to the sensor, this value is represented in. Default is None.
     """
 
     val: t.Union[int, float] = None
 
+    OPENLABEL_ID = "num"
     _REQ_FIELDS = ["val"]
 
     @classmethod
-    def fromdict(self, data_dict: dict, sensors: dict) -> t.Tuple[dict, list]:
-        """Generate a Bbox object from a dictionary in the OpenLABEL format.
+    def fromdict(self, data_dict: dict, sensors: dict) -> "Num":
+        """Generate a Num object from a dict.
 
         Parameters
         ----------
         data_dict: dict
-            OpenLABEL format dictionary containing the data for the annotation.
+            RailLabel format snippet containing the relevant data.
         sensors: dict
             Dictionary containing all sensors for the scene.
 
         Returns
         -------
-        annotation: Bbox
+        annotation: Num
             Converted annotation.
-        warnings: list of str
-            List of non-critical errors, that have occurred during the conversion.
         """
 
-        warnings = []  # list of warnings, that have occurred during the parsing
-
-        # Creates the annotation with all mandatory properties
-        annotation = Num(
+        return Num(
             uid=str(data_dict["uid"]),
             name=str(data_dict["name"]),
             val=data_dict["val"],
+            sensor=self._coordinate_system_fromdict(data_dict, sensors),
+            attributes=self._attributes_fromdict(data_dict),
         )
 
-        # Adds the optional properties
-        if "coordinate_system" in data_dict and data_dict["coordinate_system"] != "":
-            try:
-                annotation.sensor = sensors[data_dict["coordinate_system"]]
-
-            except KeyError:
-                warnings.append(
-                    f"{data_dict['coordinate_system']} does not exist as a coordinate system, "
-                    + f"but is referenced for the annotation {data_dict['uid']}."
-                )
-
-        # Adds the attributes
-        if "attributes" in data_dict:
-
-            annotation.attributes = {
-                a["name"]: a["val"] for l in data_dict["attributes"].values() for a in l
-            }
-
-        return annotation, warnings
-
     def asdict(self) -> dict:
         """Export self as a dict compatible with the OpenLABEL schema.
 
         Returns
         -------
         dict_repr: dict
             Dict representation of this class instance.
```

### Comparing `raillabel-2.0.4/raillabel/format/object.py` & `raillabel-2.1.0/raillabel/format/object.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 
     uid: str
     name: str
     type: str
 
     @classmethod
     def fromdict(cls, data_dict: dict, object_uid: str) -> "Object":
-        """Generate an Object from a dictionary in the OpenLABEL format.
+        """Generate a Object from a dict.
 
         Parameters
         ----------
         data_dict: dict
-            OpenLABEL format dictionary containing the data.
+            RailLabel format snippet containing the relevant data.
         object_uid: str
             Unique identifier of the object.
 
         Returns
         -------
         object: raillabel.format.Object
             Converted object.
```

### Comparing `raillabel-2.0.4/raillabel/format/point2d.py` & `raillabel-2.1.0/raillabel/format/point2d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/format/point3d.py` & `raillabel-2.1.0/raillabel/format/point3d.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/format/poly2d.py` & `raillabel-2.1.0/raillabel/format/poly2d.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,74 +37,48 @@
         A reference to the sensor, this annotation is labeled in. Default is None.
     """
 
     points: t.List[Point2d] = None
     closed: bool = None
     mode: str = "MODE_POLY2D_ABSOLUTE"
 
+    OPENLABEL_ID = "poly2d"
     _REQ_FIELDS = ["points", "closed"]
 
     @classmethod
     def fromdict(
         self,
         data_dict: dict,
         sensors: dict,
-    ) -> t.Tuple["Poly2d", list]:
-        """Generate a Bbox object from a dictionary in the OpenLABEL format.
+    ) -> "Poly2d":
+        """Generate a Poly2d object from a dict.
 
         Parameters
         ----------
         data_dict: dict
-            OpenLABEL format dictionary containing the data for the annotation.
+            RailLabel format snippet containing the relevant data.
         sensors: dict
             Dictionary containing all sensors for the scene.
 
         Returns
         -------
-        annotation: Bbox
+        annotation: Poly2d
             Converted annotation.
-        warnings: list of str
-            List of non-critical errors, that have occurred during the conversion.
         """
 
-        warnings = []  # list of warnings, that have occurred during the parsing
-
-        # Parses the points
-        points = []
-        for i in range(0, len(data_dict["val"]), 2):
-            points.append(Point2d(x=data_dict["val"][i], y=data_dict["val"][i + 1]))
-
-        # Creates the annotation with all mandatory properties
-        annotation = Poly2d(
+        return Poly2d(
             uid=str(data_dict["uid"]),
             name=str(data_dict["name"]),
             closed=data_dict["closed"],
             mode=data_dict["mode"],
-            points=points,
+            points=self._points_fromdict(data_dict),
+            sensor=self._coordinate_system_fromdict(data_dict, sensors),
+            attributes=self._attributes_fromdict(data_dict),
         )
 
-        # Adds the optional properties
-        if "coordinate_system" in data_dict and data_dict["coordinate_system"] != "":
-            try:
-                annotation.sensor = sensors[data_dict["coordinate_system"]]
-
-            except KeyError:
-                warnings.append(
-                    f"{data_dict['coordinate_system']} does not exist as a coordinate system, "
-                    + f"but is referenced for the annotation {data_dict['uid']}."
-                )
-
-        # Adds the attributes
-        if "attributes" in data_dict:
-            annotation.attributes = {
-                a["name"]: a["val"] for l in data_dict["attributes"].values() for a in l
-            }
-
-        return annotation, warnings
-
     def asdict(self) -> dict:
         """Export self as a dict compatible with the OpenLABEL schema.
 
         Returns
         -------
         dict_repr: dict
             Dict representation of this class instance.
@@ -122,7 +96,13 @@
         dict_repr["mode"] = self.mode
         for point in self.points:
             dict_repr["val"].extend(point.asdict())
 
         dict_repr.update(self._annotation_optional_fields_asdict())
 
         return dict_repr
+
+    def _points_fromdict(data_dict: dict) -> t.List[Point2d]:
+        points = []
+        for i in range(0, len(data_dict["val"]), 2):
+            points.append(Point2d(x=data_dict["val"][i], y=data_dict["val"][i + 1]))
+        return points
```

### Comparing `raillabel-2.0.4/raillabel/format/poly3d.py` & `raillabel-2.1.0/raillabel/format/poly3d.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,75 +29,47 @@
     sensor: raillabel.format.CoordinateSystem, optional
         A reference to the sensor, this annotation is labeled in. Default is None.
     """
 
     points: t.List[Point3d] = None
     closed: bool = None
 
+    OPENLABEL_ID = "poly3d"
     _REQ_FIELDS = ["points", "closed"]
 
     @classmethod
     def fromdict(
         self,
         data_dict: dict,
         sensors: dict,
-    ) -> t.Tuple["Poly3d", list]:
-        """Generate a Bbox object from a dictionary in the OpenLABEL format.
+    ) -> "Poly3d":
+        """Generate a Poly3d object from a dict.
 
         Parameters
         ----------
         data_dict: dict
-            OpenLABEL format dictionary containing the data for the annotation.
+            RailLabel format snippet containing the relevant data.
         sensors: dict
             Dictionary containing all sensors for the scene.
 
         Returns
         -------
-        annotation: Bbox
+        annotation: Poly3d
             Converted annotation.
-        warnings: list of str
-            List of non-critical errors, that have occurred during the conversion.
         """
 
-        warnings = []  # list of warnings, that have occurred during the parsing
-
-        # Parses the points
-        points = []
-        for i in range(0, len(data_dict["val"]), 3):
-            points.append(
-                Point3d(x=data_dict["val"][i], y=data_dict["val"][i + 1], z=data_dict["val"][i + 2])
-            )
-
-        # Creates the annotation with all mandatory properties
-        annotation = Poly3d(
+        return Poly3d(
             uid=str(data_dict["uid"]),
             name=str(data_dict["name"]),
             closed=data_dict["closed"],
-            points=points,
+            points=self._points_fromdict(data_dict),
+            sensor=self._coordinate_system_fromdict(data_dict, sensors),
+            attributes=self._attributes_fromdict(data_dict),
         )
 
-        # Adds the optional properties
-        if "coordinate_system" in data_dict and data_dict["coordinate_system"] != "":
-            try:
-                annotation.sensor = sensors[data_dict["coordinate_system"]]
-
-            except KeyError:
-                warnings.append(
-                    f"{data_dict['coordinate_system']} does not exist as a coordinate system, "
-                    + f"but is referenced for the annotation {data_dict['uid']}."
-                )
-
-        # Adds the attributes
-        if "attributes" in data_dict:
-            annotation.attributes = {
-                a["name"]: a["val"] for l in data_dict["attributes"].values() for a in l
-            }
-
-        return annotation, warnings
-
     def asdict(self) -> dict:
         """Export self as a dict compatible with the OpenLABEL schema.
 
         Returns
         -------
         dict_repr: dict
             Dict representation of this class instance.
@@ -114,7 +86,15 @@
         dict_repr["val"] = []
         for point in self.points:
             dict_repr["val"].extend(point.asdict())
 
         dict_repr.update(self._annotation_optional_fields_asdict())
 
         return dict_repr
+
+    def _points_fromdict(data_dict: dict) -> t.List[Point3d]:
+        points = []
+        for i in range(0, len(data_dict["val"]), 3):
+            points.append(
+                Point3d(x=data_dict["val"][i], y=data_dict["val"][i + 1], z=data_dict["val"][i + 2])
+            )
+        return points
```

### Comparing `raillabel-2.0.4/raillabel/format/quaternion.py` & `raillabel-2.1.0/raillabel/format/quaternion.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/format/scene.py` & `raillabel-2.1.0/raillabel/format/scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         The VCD visualization tool requires a short "summary" of where an object and the
         object_data_pointers occurr, which includes the frame intervals of the object and the frame
         intervals of the object_data names.
 
         Parameters
         ----------
         dict_repr : dict
-            Dictionary in the OpenLABEL format, that should be enhanced.
+            Dictionary in the RailLabel format, that should be enhanced.
 
         Returns
         -------
         dict
             Enhanced dictionary.
         """
```

### Comparing `raillabel-2.0.4/raillabel/format/seg3d.py` & `raillabel-2.1.0/raillabel/format/seg3d.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,67 +23,46 @@
         Attributes of the annotation. Default is {}.
     sensor: raillabel.format.CoordinateSystem, optional
         The sensor, this annotation is labeled in. Default is None.
     """
 
     point_ids: t.List[int] = None
 
+    OPENLABEL_ID = "vec"
     _REQ_FIELDS = ["point_ids"]
 
     @classmethod
     def fromdict(
         self,
         data_dict: dict,
         sensors: dict,
-    ) -> t.Tuple["Seg3d", list]:
-        """Generate a Bbox object from a dictionary in the OpenLABEL format.
+    ) -> "Seg3d":
+        """Generate a Seg3d object from a dict.
 
         Parameters
         ----------
         data_dict: dict
-            OpenLABEL format dictionary containing the data for the annotation.
+            RailLabel format snippet containing the relevant data.
         sensors: dict
             Dictionary containing all sensors for the scene.
 
         Returns
         -------
-        annotation: Bbox
+        annotation: Seg3d
             Converted annotation.
-        warnings: list of str
-            List of non-critical errors, that have occurred during the conversion.
         """
 
-        warnings = []  # list of warnings, that have occurred during the parsing
-
-        # Creates the annotation with all mandatory properties
-        annotation = Seg3d(
+        return Seg3d(
             uid=str(data_dict["uid"]),
             name=str(data_dict["name"]),
             point_ids=data_dict["val"],
+            sensor=self._coordinate_system_fromdict(data_dict, sensors),
+            attributes=self._attributes_fromdict(data_dict),
         )
 
-        # Adds the optional properties
-        if "coordinate_system" in data_dict and data_dict["coordinate_system"] != "":
-            try:
-                annotation.sensor = sensors[data_dict["coordinate_system"]]
-
-            except KeyError:
-                warnings.append(
-                    f"{data_dict['coordinate_system']} does not exist as a coordinate system, "
-                    + f"but is referenced for the annotation {data_dict['uid']}."
-                )
-
-        # Adds the attributes
-        if "attributes" in data_dict:
-            annotation.attributes = {
-                a["name"]: a["val"] for l in data_dict["attributes"].values() for a in l
-            }
-
-        return annotation, warnings
-
     def asdict(self) -> dict:
         """Export self as a dict compatible with the OpenLABEL schema.
 
         Returns
         -------
         dict_repr: dict
             Dict representation of this class instance.
```

### Comparing `raillabel-2.0.4/raillabel/format/sensor.py` & `raillabel-2.1.0/raillabel/format/sensor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright DB Netz AG and contributors
 # SPDX-License-Identifier: Apache-2.0
 
 import typing as t
 import warnings
 from dataclasses import dataclass
+from enum import Enum
 
 from .intrinsics_pinhole import IntrinsicsPinhole
+from .intrinsics_radar import IntrinsicsRadar
 from .point3d import Point3d
 from .quaternion import Quaternion
 from .transform import Transform
 
 
 @dataclass
 class Sensor:
@@ -23,104 +25,70 @@
     ----------
     uid: str
         This is the friendly name of the sensor as well as its identifier. Must be
         unique.
     extrinsics: raillabel.format.Transform, optional
         The external calibration of the sensor defined by the 3D transform to the coordinate
         system origin. Default is None.
-    intrinsics: raillabel.format.SensorCalibration, optional
+    intrinsics: raillabel.format.IntrinsicsPinhole or raillabel.format.IntrinsicsRadar, optional
         The intrinsic calibration of the sensor. Default is None.
-    type: str-enum
+    type: raillabel.format.SensorType, optional
         A string encoding the type of the sensor. The only valid values are 'camera', 'lidar',
-        'radar', 'gps_imu' or 'other'.
+        'radar', 'gps_imu' or 'other'. Default is None.
     uri: str, optional
         Name of the subdirectory containing the sensor files. Default is None.
     description: str, optional
         Description of the sensor. Default is None.
     """
 
     uid: str
     extrinsics: t.Optional[Transform] = None
-    intrinsics: t.Optional[IntrinsicsPinhole] = None
-    type: str = None
+    intrinsics: t.Optional[t.Union[IntrinsicsPinhole, IntrinsicsRadar]] = None
+    type: t.Optional["SensorType"] = None
     uri: t.Optional[str] = None
     description: t.Optional[str] = None
 
-    _VALID_SENSOR_TYPES = ["camera", "lidar", "radar", "gps_imu", "other"]
-
     @property
     def rostopic(self):
         """Return deprecated field containing the rostopic."""
         warnings.warn(
             "rostopic is a deprecated field and will be removed soon. Use sensor.uri instead.",
             category=DeprecationWarning,
         )
         return self.uri
 
     @classmethod
-    def fromdict(self, uid: str, cs_raw: dict, stream_raw: dict) -> "Sensor":
-        """Generate a Sensor object from a dictionary in the RailLabel format.
+    def fromdict(cls, uid: str, cs_data_dict: dict, stream_data_dict: dict) -> "Sensor":
+        """Generate a Sensor object from a dict.
 
         Parameters
         ----------
         uid: str
             Unique identifier of the sensor.
-        cs_raw: dict
+        cs_data_dict: dict
             RailLabel format dict containing the data about the coordinate system.
-        stream_raw: dict
+        stream_data_dict: dict
             RailLabel format dict containing the data about the stream.
 
         Returns
         -------
         sensor: raillabel.format.Sensor
             Converted Sensor object.
         """
 
-        sensor = Sensor(uid)
-
-        if "pose_wrt_parent" in cs_raw:
-            sensor.extrinsics = Transform(
-                pos=Point3d(
-                    x=cs_raw["pose_wrt_parent"]["translation"][0],
-                    y=cs_raw["pose_wrt_parent"]["translation"][1],
-                    z=cs_raw["pose_wrt_parent"]["translation"][2],
-                ),
-                quat=Quaternion(
-                    x=cs_raw["pose_wrt_parent"]["quaternion"][0],
-                    y=cs_raw["pose_wrt_parent"]["quaternion"][1],
-                    z=cs_raw["pose_wrt_parent"]["quaternion"][2],
-                    w=cs_raw["pose_wrt_parent"]["quaternion"][3],
-                ),
-            )
-
-        if (
-            "stream_properties" in stream_raw
-            and "intrinsics_pinhole" in stream_raw["stream_properties"]
-        ):
-            sensor.intrinsics = IntrinsicsPinhole(
-                camera_matrix=tuple(
-                    stream_raw["stream_properties"]["intrinsics_pinhole"]["camera_matrix"]
-                ),
-                distortion=tuple(
-                    stream_raw["stream_properties"]["intrinsics_pinhole"]["distortion_coeffs"]
-                ),
-                width_px=stream_raw["stream_properties"]["intrinsics_pinhole"]["width_px"],
-                height_px=stream_raw["stream_properties"]["intrinsics_pinhole"]["height_px"],
-            )
-
-        if "type" in stream_raw:
-            sensor.type = stream_raw["type"]
-
-        if "uri" in stream_raw:
-            sensor.uri = stream_raw["uri"]
-
-        if "description" in stream_raw:
-            sensor.type = stream_raw["description"]
-
-        return sensor
+        return Sensor(
+            uid=uid,
+            extrinsics=cls._extrinsics_fromdict(cs_data_dict),
+            intrinsics=cls._intrinsics_fromdict(
+                stream_data_dict, cls._type_fromdict(stream_data_dict)
+            ),
+            type=cls._type_fromdict(stream_data_dict),
+            uri=stream_data_dict.get("uri"),
+            description=stream_data_dict.get("description"),
+        )
 
     def asdict(self) -> dict:
         """Export self as a dict compatible with the RailLabel schema.
 
         Returns
         -------
         dict_repr: dict
@@ -142,24 +110,79 @@
         return coordinate_system_repr
 
     def _as_stream_dict(self) -> dict:
 
         stream_repr = {}
 
         if self.type is not None:
-            if self.type not in self._VALID_SENSOR_TYPES:
-                raise ValueError(
-                    f"Sensor.type must be one of {self._VALID_SENSOR_TYPES}, not {self.type}."
-                )
-
-            stream_repr["type"] = str(self.type)
+            stream_repr["type"] = str(self.type.value)
 
         if self.uri is not None:
             stream_repr["uri"] = str(self.uri)
 
         if self.description is not None:
             stream_repr["description"] = str(self.description)
 
-        if self.intrinsics is not None:
+        if isinstance(self.intrinsics, IntrinsicsPinhole):
             stream_repr["stream_properties"] = {"intrinsics_pinhole": self.intrinsics.asdict()}
 
+        elif isinstance(self.intrinsics, IntrinsicsRadar):
+            stream_repr["stream_properties"] = {"intrinsics_radar": self.intrinsics.asdict()}
+
         return stream_repr
+
+    def _extrinsics_fromdict(data_dict) -> t.Optional[Transform]:
+
+        if "pose_wrt_parent" not in data_dict:
+            return None
+
+        return Transform(
+            pos=Point3d(
+                x=data_dict["pose_wrt_parent"]["translation"][0],
+                y=data_dict["pose_wrt_parent"]["translation"][1],
+                z=data_dict["pose_wrt_parent"]["translation"][2],
+            ),
+            quat=Quaternion(
+                x=data_dict["pose_wrt_parent"]["quaternion"][0],
+                y=data_dict["pose_wrt_parent"]["quaternion"][1],
+                z=data_dict["pose_wrt_parent"]["quaternion"][2],
+                w=data_dict["pose_wrt_parent"]["quaternion"][3],
+            ),
+        )
+
+    def _intrinsics_fromdict(
+        data_dict, sensor_type: t.Optional["SensorType"]
+    ) -> t.Optional[IntrinsicsPinhole]:
+
+        if "stream_properties" not in data_dict:
+            return None
+
+        if sensor_type == SensorType.CAMERA:
+
+            if "intrinsics_pinhole" in data_dict["stream_properties"]:
+                return IntrinsicsPinhole.fromdict(
+                    data_dict["stream_properties"]["intrinsics_pinhole"]
+                )
+
+        elif sensor_type == SensorType.RADAR:
+
+            if "intrinsics_radar" in data_dict["stream_properties"]:
+                return IntrinsicsRadar.fromdict(data_dict["stream_properties"]["intrinsics_radar"])
+
+        return None
+
+    def _type_fromdict(data_dict) -> t.Optional["SensorType"]:
+
+        if "type" not in data_dict:
+            return None
+
+        return SensorType(data_dict["type"])
+
+
+class SensorType(Enum):
+    """Enumeration representing all possible sensor types."""
+
+    CAMERA = "camera"
+    LIDAR = "lidar"
+    RADAR = "radar"
+    GPS_IMU = "gps_imu"
+    OTHER = "other"
```

### Comparing `raillabel-2.0.4/raillabel/format/transform.py` & `raillabel-2.1.0/raillabel/format/transform.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/format_loaders/__init__.py` & `raillabel-2.1.0/raillabel/format_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/format_loaders/_loader_abc.py` & `raillabel-2.1.0/raillabel/format_loaders/_loader_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     For every annotation format, that can be loaded via raillabel, a loader class should exists,
     that inherites from this class.
 
     Attributes
     ----------
     scene: raillabel.Scene
         Loaded raillabel.Scene with the data.
-    warnings: list[str]
+    warnings: t.List[str]
         List of warning strings, that have been found during the execution of load().
     SCHEMA_PATH: Path
         Absolute path to the JSON schema.
     """
 
     scene: format.Scene
     warnings: t.List[str]
```

### Comparing `raillabel-2.0.4/raillabel/format_loaders/translation.json` & `raillabel-2.1.0/raillabel/format_loaders/translation.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/load.py` & `raillabel-2.1.0/raillabel/load.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/save.py` & `raillabel-2.1.0/raillabel/save.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel/schemas/raillabel_v2_schema.json` & `raillabel-2.1.0/raillabel/schemas/raillabel_v2_schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9441105769230771%*

 * *Differences: {"'definitions'": "{'stream_properties': {'properties': {'intrinsics_radar': "*

 * *                  "OrderedDict([('additionalProperties', False), ('description', 'This JSON object "*

 * *                  "defines an instance of the intrinsic parameters of a radar.'), ('properties', "*

 * *                  "OrderedDict([('resolution_px_per_m', OrderedDict([('type', 'number')])), "*

 * *                  "('height_px', OrderedDict([('type', 'integer')])), ('width_px', "*

 * *                  "OrderedDict([('type', 'integer')])) […]*

```diff
@@ -676,17 +676,37 @@
                     "required": [
                         "camera_matrix",
                         "distortion_coeffs",
                         "height_px",
                         "width_px"
                     ],
                     "type": "object"
+                },
+                "intrinsics_radar": {
+                    "additionalProperties": false,
+                    "description": "This JSON object defines an instance of the intrinsic parameters of a radar.",
+                    "properties": {
+                        "height_px": {
+                            "type": "integer"
+                        },
+                        "resolution_px_per_m": {
+                            "type": "number"
+                        },
+                        "width_px": {
+                            "type": "integer"
+                        }
+                    },
+                    "required": [
+                        "resolution_px_per_m",
+                        "height_px",
+                        "width_px"
+                    ],
+                    "type": "object"
                 }
-            },
-            "type": "object"
+            }
         },
         "stream_sync": {
             "additionalProperties": false,
             "description": "Syncronization information of a stream in a frame.",
             "properties": {
                 "stream_properties": {
                     "additionalProperties": false,
@@ -858,9 +878,9 @@
             "$ref": "#/definitions/openlabel"
         }
     },
     "required": [
         "openlabel"
     ],
     "type": "object",
-    "version": "2.0.0"
+    "version": "2.1.0"
 }
```

### Comparing `raillabel-2.0.4/raillabel/validate.py` & `raillabel-2.1.0/raillabel/validate.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/raillabel.egg-info/PKG-INFO` & `raillabel-2.1.0/raillabel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raillabel
-Version: 2.0.4
+Version: 2.1.0
 Summary: A devkit for working with recorded and annotated train ride data from Deutsche Bahn.
 Author: DB Netz AG
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/DSD-DBS/raillabel
 Project-URL: Documentation, https://dsd-dbs.github.io/raillabel
 Platform: any
 Classifier: Development Status :: 1 - Planning
```

### Comparing `raillabel-2.0.4/raillabel.egg-info/SOURCES.txt` & `raillabel-2.1.0/raillabel.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,21 +45,24 @@
 raillabel/_filter_classes/_filter_attributes.py
 raillabel/_filter_classes/_filter_end.py
 raillabel/_filter_classes/_filter_frames.py
 raillabel/_filter_classes/_filter_object_ids.py
 raillabel/_filter_classes/_filter_object_types.py
 raillabel/_filter_classes/_filter_sensors.py
 raillabel/_filter_classes/_filter_start.py
+raillabel/_util/__init__.py
+raillabel/_util/_warning.py
 raillabel/format/__init__.py
 raillabel/format/_annotation.py
 raillabel/format/bbox.py
 raillabel/format/cuboid.py
 raillabel/format/frame.py
 raillabel/format/frame_interval.py
 raillabel/format/intrinsics_pinhole.py
+raillabel/format/intrinsics_radar.py
 raillabel/format/metadata.py
 raillabel/format/num.py
 raillabel/format/object.py
 raillabel/format/object_data.py
 raillabel/format/point2d.py
 raillabel/format/point3d.py
 raillabel/format/poly2d.py
```

### Comparing `raillabel-2.0.4/tests/test_raillabel/__test_assets__/metaschema.json` & `raillabel-2.1.0/tests/test_raillabel/__test_assets__/metaschema.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json` & `raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_schema.json`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5` & `raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_short.json5`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9775824652777778%*

 * *Differences: {"'openlabel'": "{'metadata': {'subschema_version': '2.1.0'}, 'streams': {'radar': "*

 * *                "OrderedDict([('type', 'radar'), ('uri', '/talker1/Nvt/Cartesian'), "*

 * *                "('stream_properties', OrderedDict([('intrinsics_radar', "*

 * *                "OrderedDict([('resolution_px_per_m', 2.856), ('width_px', 2856), ('height_px', "*

 * *                "1428)]))]))])}, 'coordinate_systems': {'base': {'children': {insert: [(3, "*

 * *                "'radar')]}}, 'radar': OrderedDict([('type', 'sensor'), ('p […]*

```diff
@@ -1,15 +1,16 @@
 {
     "openlabel": {
         "coordinate_systems": {
             "base": {
                 "children": [
                     "rgb_middle",
                     "ir_middle",
-                    "lidar"
+                    "lidar",
+                    "radar"
                 ],
                 "parent": "",
                 "type": "local"
             },
             "ir_middle": {
                 "parent": "base",
                 "pose_wrt_parent": {
@@ -40,14 +41,31 @@
                         0,
                         0,
                         0
                     ]
                 },
                 "type": "sensor"
             },
+            "radar": {
+                "parent": "base",
+                "pose_wrt_parent": {
+                    "quaternion": [
+                        -0.64984101,
+                        0.18784818,
+                        -0.72563166,
+                        -0.12600959
+                    ],
+                    "translation": [
+                        2,
+                        0,
+                        1
+                    ]
+                },
+                "type": "sensor"
+            },
             "rgb_middle": {
                 "parent": "base",
                 "pose_wrt_parent": {
                     "quaternion": [
                         0.97518507,
                         -0.18529384,
                         -0.05469746,
@@ -70,14 +88,67 @@
         ],
         "frames": {
             "0": {
                 "frame_properties": {
                     "frame_data": {
                         "num": [
                             {
+                                "attributes": {
+                                    "boolean": [
+                                        {
+                                            "name": "test_bool_attr0",
+                                            "val": true
+                                        }
+                                    ],
+                                    "num": [
+                                        {
+                                            "name": "test_num_attr0",
+                                            "val": 0
+                                        },
+                                        {
+                                            "name": "test_num_attr1",
+                                            "val": 1
+                                        }
+                                    ],
+                                    "text": [
+                                        {
+                                            "name": "test_text_attr0",
+                                            "val": "test_text_attr0_val"
+                                        },
+                                        {
+                                            "name": "test_text_attr1",
+                                            "val": "test_text_attr1_val"
+                                        }
+                                    ],
+                                    "vec": [
+                                        {
+                                            "name": "test_vec_attr0",
+                                            "val": [
+                                                "0",
+                                                "1"
+                                            ]
+                                        },
+                                        {
+                                            "name": "test_vec_attr1",
+                                            "val": [
+                                                0,
+                                                1,
+                                                2
+                                            ]
+                                        },
+                                        {
+                                            "name": "test_vec_attr2",
+                                            "val": [
+                                                "a",
+                                                "b",
+                                                "c"
+                                            ]
+                                        }
+                                    ]
+                                },
                                 "coordinate_system": "rgb_middle",
                                 "name": "test_frame_data0",
                                 "uid": "a06fe567-29c7-475b-92a4-fbca64e671a7",
                                 "val": 53.1
                             },
                             {
                                 "coordinate_system": "lidar",
@@ -923,15 +994,15 @@
             }
         },
         "metadata": {
             "annotator": "test_annotator",
             "comment": "test_comment",
             "name": "test_project",
             "schema_version": "1.0.0",
-            "subschema_version": "2.0.0",
+            "subschema_version": "2.1.0",
             "tagged_file": "test_folder"
         },
         "objects": {
             "22dedd49-6dcb-413b-87ef-00ccfb532e98": {
                 "frame_intervals": [
                     {
                         "frame_end": 1,
@@ -1198,14 +1269,25 @@
                 "type": "camera",
                 "uri": "/A0001781/image"
             },
             "lidar": {
                 "type": "lidar",
                 "uri": "/lidar_merged"
             },
+            "radar": {
+                "stream_properties": {
+                    "intrinsics_radar": {
+                        "height_px": 1428,
+                        "resolution_px_per_m": 2.856,
+                        "width_px": 2856
+                    }
+                },
+                "type": "radar",
+                "uri": "/talker1/Nvt/Cartesian"
+            },
             "rgb_middle": {
                 "stream_properties": {
                     "intrinsics_pinhole": {
                         "camera_matrix": [
                             0.48,
                             0,
                             0.81,
```

### Comparing `raillabel-2.0.4/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json` & `raillabel-2.1.0/tests/test_raillabel/__test_assets__/openlabel_v1_vcd_incompatible.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9774674479166666%*

 * *Differences: {"'openlabel'": "{'streams': {'radar': OrderedDict([('type', 'radar'), ('uri', "*

 * *                "'/talker1/Nvt/Cartesian'), ('stream_properties', "*

 * *                "OrderedDict([('intrinsics_radar', OrderedDict([('resolution_px_per_m', 2.856), "*

 * *                "('width_px', 2856), ('height_px', 1428)]))]))])}, 'coordinate_systems': {'radar': "*

 * *                "OrderedDict([('type', 'sensor'), ('parent', 'base'), ('pose_wrt_parent', "*

 * *                "OrderedDict([('translation', [2, 0, 1]), ('quaternion', […]*

```diff
@@ -42,14 +42,31 @@
                         0,
                         0,
                         0
                     ]
                 },
                 "type": "sensor"
             },
+            "radar": {
+                "parent": "base",
+                "pose_wrt_parent": {
+                    "quaternion": [
+                        -0.64984101,
+                        0.18784818,
+                        -0.72563166,
+                        -0.12600959
+                    ],
+                    "translation": [
+                        2,
+                        0,
+                        1
+                    ]
+                },
+                "type": "sensor"
+            },
             "rgb_middle": {
                 "children": [],
                 "parent": "base",
                 "pose_wrt_parent": {
                     "quaternion": [
                         0.97518507,
                         -0.18529384,
@@ -67,14 +84,67 @@
         },
         "frames": {
             "0": {
                 "frame_properties": {
                     "frame_data": {
                         "num": [
                             {
+                                "attributes": {
+                                    "boolean": [
+                                        {
+                                            "name": "test_bool_attr0",
+                                            "val": true
+                                        }
+                                    ],
+                                    "num": [
+                                        {
+                                            "name": "test_num_attr0",
+                                            "val": 0
+                                        },
+                                        {
+                                            "name": "test_num_attr1",
+                                            "val": 1
+                                        }
+                                    ],
+                                    "text": [
+                                        {
+                                            "name": "test_text_attr0",
+                                            "val": "test_text_attr0_val"
+                                        },
+                                        {
+                                            "name": "test_text_attr1",
+                                            "val": "test_text_attr1_val"
+                                        }
+                                    ],
+                                    "vec": [
+                                        {
+                                            "name": "test_vec_attr0",
+                                            "val": [
+                                                "0",
+                                                "1"
+                                            ]
+                                        },
+                                        {
+                                            "name": "test_vec_attr1",
+                                            "val": [
+                                                0,
+                                                1,
+                                                2
+                                            ]
+                                        },
+                                        {
+                                            "name": "test_vec_attr2",
+                                            "val": [
+                                                "a",
+                                                "b",
+                                                "c"
+                                            ]
+                                        }
+                                    ]
+                                },
                                 "coordinate_system": "rgb_middle",
                                 "name": "test_frame_data0",
                                 "val": 53.1
                             },
                             {
                                 "coordinate_system": "lidar",
                                 "name": "test_frame_data1",
@@ -1029,14 +1099,25 @@
                 "type": "camera",
                 "uri": "/A0001781/image"
             },
             "lidar": {
                 "type": "lidar",
                 "uri": "/lidar_merged"
             },
+            "radar": {
+                "stream_properties": {
+                    "intrinsics_radar": {
+                        "height_px": 1428,
+                        "resolution_px_per_m": 2.856,
+                        "width_px": 2856
+                    }
+                },
+                "type": "radar",
+                "uri": "/talker1/Nvt/Cartesian"
+            },
             "rgb_middle": {
                 "stream_properties": {
                     "intrinsics_pinhole": {
                         "camera_matrix": [
                             0.48,
                             0,
                             0.81,
```

### Comparing `raillabel-2.0.4/tests/test_raillabel/format/test_annotation.py` & `raillabel-2.1.0/tests/test_raillabel/format/test_annotation.py`

 * *Files identical despite different names*

### Comparing `raillabel-2.0.4/tests/test_raillabel/schemas/test_raillabel_v2_schema.py` & `raillabel-2.1.0/tests/test_raillabel/schemas/test_raillabel_v2_schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,23 +3,32 @@
 
 import os
 
 import jsonschema
 import pytest
 
 
-def test_metaschema_validation(raillabel_v2_schema_data, metaschema_data):
-    assert jsonschema.validate(raillabel_v2_schema_data, metaschema_data) is None
-
-
-def test_sample_data_validation_subschema(raillabel_v2_schema_data, openlabel_v1_short_data):
-    assert jsonschema.validate(openlabel_v1_short_data, raillabel_v2_schema_data) is None
-
-
-def test_sample_data_validation_superschema(openlabel_v1_schema_data, openlabel_v1_short_data):
-    assert jsonschema.validate(openlabel_v1_short_data, openlabel_v1_schema_data) is None
+def test_metaschema_validation(json_data):
+    assert jsonschema.validate(
+        json_data["raillabel_v2_schema"],
+        json_data["metaschema"]
+    ) is None
+
+
+def test_sample_data_validation_subschema(json_data):
+    assert jsonschema.validate(
+        json_data["openlabel_v1_short"],
+        json_data["raillabel_v2_schema"]
+    ) is None
+
+
+def test_sample_data_validation_superschema(json_data):
+    assert jsonschema.validate(
+        json_data["openlabel_v1_short"],
+        json_data["openlabel_v1_schema"]
+    ) is None
 
 
 # Executes the test if the file is called
 if __name__ == "__main__":
     os.system("clear")
     pytest.main([__file__, "--disable-pytest-warnings", "--cache-clear"])
```

### Comparing `raillabel-2.0.4/tests/test_raillabel/test_save.py` & `raillabel-2.1.0/tests/test_raillabel/test_save.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 import pytest
 
 sys.path.insert(1, str(Path(__file__).parent.parent.parent))
 
 import raillabel
 
 
-def test_save_scene(openlabel_v1_short_path):
+def test_save_scene(json_paths):
     with tempfile.TemporaryDirectory("w") as temp_dir:
 
-        scene_orig = raillabel.load(openlabel_v1_short_path, False, False)
+        scene_orig = raillabel.load(json_paths["openlabel_v1_short"], False, False)
 
         raillabel.save(scene_orig, Path(temp_dir) / "test_save_file.json")
         scene_saved = raillabel.load(Path(temp_dir) / "test_save_file.json", False, False)
 
     assert scene_orig == scene_saved
 
 
-def test_save_json(openlabel_v1_short_data):
+def test_save_json(json_data):
     with tempfile.TemporaryDirectory("w") as temp_dir:
 
-        stripped_input_data = deepcopy(openlabel_v1_short_data)
+        stripped_input_data = deepcopy(json_data["openlabel_v1_short"])
 
         # Removes the object data pointers from the example file so that it needs to be generated from the data
         for object in stripped_input_data["openlabel"]["objects"].values():
             del object["frame_intervals"]
             del object["object_data_pointers"]
 
         with (Path(temp_dir) / "stripped_input_data.json").open("w") as f:
@@ -45,15 +45,15 @@
         with (Path(temp_dir) / "test_save_file.json").open() as f:
             saved_and_loaded_data = json.load(f)
 
     # Removes the exporter version from the generated file as these are hard to test for
     if "exporter_version" in saved_and_loaded_data["openlabel"]["metadata"]:
         del saved_and_loaded_data["openlabel"]["metadata"]["exporter_version"]
 
-    assert saved_and_loaded_data == openlabel_v1_short_data
+    assert saved_and_loaded_data == json_data["openlabel_v1_short"]
 
 
 def test_frame_intervals():
     data = {
         "openlabel": {
             "metadata": {"schema_version": "1.0.0"},
             "frames": {
```

