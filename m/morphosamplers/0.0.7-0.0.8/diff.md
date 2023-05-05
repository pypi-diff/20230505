# Comparing `tmp/morphosamplers-0.0.7.tar.gz` & `tmp/morphosamplers-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphosamplers-0.0.7.tar", last modified: Thu May  4 14:34:47 2023, max compression
+gzip compressed data, was "morphosamplers-0.0.8.tar", last modified: Fri May  5 12:07:40 2023, max compression
```

## Comparing `morphosamplers-0.0.7.tar` & `morphosamplers-0.0.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.070617 morphosamplers-0.0.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.070617 morphosamplers-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.github_changelog_generator
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.070617 morphosamplers-0.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/examples/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/examples/sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.070617 morphosamplers-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.070617 morphosamplers-0.0.7/src/morphosamplers/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/src/morphosamplers/models/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/models/sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/models/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/sample_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/src/morphosamplers/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/point_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/pose_sampler_helical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/pose_sampler_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/tests/test_point_sampler_equidistant.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_helical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/_sphere_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/point_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/pose_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/tests/test_point_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)    19179 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/surface_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.070617 morphosamplers-0.0.7/src/morphosamplers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-04 14:34:47.000000 morphosamplers-0.0.7/src/morphosamplers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-04 14:34:47.000000 morphosamplers-0.0.7/src/morphosamplers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:34:47.000000 morphosamplers-0.0.7/src/morphosamplers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:34:46.000000 morphosamplers-0.0.7/src/morphosamplers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 14:34:47.000000 morphosamplers-0.0.7/src/morphosamplers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 14:34:47.000000 morphosamplers-0.0.7/src/morphosamplers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/tests/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/tests/test_spline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.179931 morphosamplers-0.0.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.179931 morphosamplers-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.github_changelog_generator
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.179931 morphosamplers-0.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/examples/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/examples/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.179931 morphosamplers-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.179931 morphosamplers-0.0.8/src/morphosamplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/models/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/models/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/sample_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/point_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/pose_sampler_helical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/pose_sampler_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/tests/test_point_sampler_equidistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_helical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/_sphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/point_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/pose_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/tests/test_point_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19179 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/surface_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-05 12:07:40.000000 morphosamplers-0.0.8/src/morphosamplers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-05 12:07:40.000000 morphosamplers-0.0.8/src/morphosamplers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:07:40.000000 morphosamplers-0.0.8/src/morphosamplers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:07:39.000000 morphosamplers-0.0.8/src/morphosamplers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 12:07:40.000000 morphosamplers-0.0.8/src/morphosamplers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 12:07:40.000000 morphosamplers-0.0.8/src/morphosamplers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/tests/test_spline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/tox.ini
```

### Comparing `morphosamplers-0.0.7/.cruft.json` & `morphosamplers-0.0.8/.cruft.json`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/.github/workflows/ci.yml` & `morphosamplers-0.0.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/.github/workflows/cron.yml` & `morphosamplers-0.0.8/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/.gitignore` & `morphosamplers-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/.pre-commit-config.yaml` & `morphosamplers-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/LICENSE` & `morphosamplers-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/PKG-INFO` & `morphosamplers-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphosamplers
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for sampling image data along morphological objects such as splines and surfaces.
 Author: Kevin Yamauchi
 Author-email: kevin.yamauchi@gmail.com
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/kevinyamauchi/morphosamplers
 Project-URL: repository, https://github.com/kevinyamauchi/morphosamplers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `morphosamplers-0.0.7/README.md` & `morphosamplers-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/examples/path.py` & `morphosamplers-0.0.8/examples/path.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/examples/sphere.py` & `morphosamplers-0.0.8/examples/sphere.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/pyproject.toml` & `morphosamplers-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/core.py` & `morphosamplers-0.0.8/src/morphosamplers/core.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/models/path.py` & `morphosamplers-0.0.8/src/morphosamplers/models/path.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/models/surface.py` & `morphosamplers-0.0.8/src/morphosamplers/models/surface.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/sample_types.py` & `morphosamplers-0.0.8/src/morphosamplers/sample_types.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/sampler.py` & `morphosamplers-0.0.8/src/morphosamplers/sampler.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/point_sampler.py` & `morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/point_sampler.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/pose_sampler_helical.py` & `morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/pose_sampler_helical.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/pose_sampler_parallel.py` & `morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/pose_sampler_parallel.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/tests/test_point_sampler_equidistant.py` & `morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/tests/test_point_sampler_equidistant.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_parallel.py` & `morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_parallel.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/_sphere_utils.py` & `morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/_sphere_utils.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/pose_sampler.py` & `morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/pose_sampler.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/tests/test_point_sampler.py` & `morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/tests/test_point_sampler.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/spline.py` & `morphosamplers-0.0.8/src/morphosamplers/spline.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/surface_spline.py` & `morphosamplers-0.0.8/src/morphosamplers/surface_spline.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers/utils.py` & `morphosamplers-0.0.8/src/morphosamplers/utils.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/src/morphosamplers.egg-info/PKG-INFO` & `morphosamplers-0.0.8/src/morphosamplers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphosamplers
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for sampling image data along morphological objects such as splines and surfaces.
 Author: Kevin Yamauchi
 Author-email: kevin.yamauchi@gmail.com
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/kevinyamauchi/morphosamplers
 Project-URL: repository, https://github.com/kevinyamauchi/morphosamplers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `morphosamplers-0.0.7/src/morphosamplers.egg-info/SOURCES.txt` & `morphosamplers-0.0.8/src/morphosamplers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/tests/test_sampling.py` & `morphosamplers-0.0.8/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/tests/test_spline_model.py` & `morphosamplers-0.0.8/tests/test_spline_model.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.7/tox.ini` & `morphosamplers-0.0.8/tox.ini`

 * *Files identical despite different names*

