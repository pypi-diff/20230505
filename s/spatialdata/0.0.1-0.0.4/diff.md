# Comparing `tmp/spatialdata-0.0.1.tar.gz` & `tmp/spatialdata-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialdata-0.0.1.tar", last modified: Sat May 21 09:28:32 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `spatialdata-0.0.1.tar` & `spatialdata-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,105 @@
--rw-r--r--   0        0        0      176 2022-05-21 09:18:25.230742 spatialdata-0.0.1/.bumpversion.cfg
--rw-r--r--   0        0        0      333 2022-05-21 09:13:09.886916 spatialdata-0.0.1/.codecov.yaml
--rw-r--r--   0        0        0      178 2022-05-21 09:18:25.230982 spatialdata-0.0.1/.editorconfig
--rw-r--r--   0        0        0     1543 2022-05-21 09:19:38.868062 spatialdata-0.0.1/.flake8
--rw-r--r--   0        0        0      273 2022-05-21 09:18:25.231647 spatialdata-0.0.1/.github/workflows/pre-commit.yaml
--rw-r--r--   0        0        0     2450 2022-05-21 09:22:52.312822 spatialdata-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      230 2022-05-21 09:21:06.119315 spatialdata-0.0.1/.gitignore
--rw-r--r--   0        0        0     2202 2022-05-21 09:21:11.834464 spatialdata-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      310 2022-05-21 09:21:17.623193 spatialdata-0.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2022-05-21 09:18:25.233410 spatialdata-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1515 2022-05-21 09:21:32.319362 spatialdata-0.0.1/LICENSE
--rw-r--r--   0        0        0     1555 2022-05-21 09:19:37.716270 spatialdata-0.0.1/README.md
--rw-r--r--   0        0        0      634 2022-05-21 09:18:25.234481 spatialdata-0.0.1/docs/Makefile
--rw-r--r--   0        0        0        0 2022-05-21 09:18:25.235180 spatialdata-0.0.1/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2022-05-21 09:18:25.235690 spatialdata-0.0.1/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      464 2022-05-21 09:18:25.236006 spatialdata-0.0.1/docs/api.md
--rw-r--r--   0        0        0       34 2022-05-21 09:18:25.236234 spatialdata-0.0.1/docs/changelog.md
--rw-r--r--   0        0        0     3344 2022-05-21 09:18:25.236461 spatialdata-0.0.1/docs/conf.py
--rw-r--r--   0        0        0     3463 2022-05-21 09:18:25.236853 spatialdata-0.0.1/docs/developer_docs.md
--rw-r--r--   0        0        0        0 2022-05-21 09:18:25.237229 spatialdata-0.0.1/docs/extensions/.gitkeep
--rw-r--r--   0        0        0      148 2022-05-21 09:18:25.237640 spatialdata-0.0.1/docs/index.md
--rw-r--r--   0        0        0      765 2022-05-21 09:18:25.238001 spatialdata-0.0.1/docs/make.bat
--rw-r--r--   0        0        0     1377 2022-05-21 09:18:25.238411 spatialdata-0.0.1/docs/notebooks/example.ipynb
--rw-r--r--   0        0        0     1014 2022-05-21 09:18:25.238664 spatialdata-0.0.1/docs/references.bib
--rw-r--r--   0        0        0       44 2022-05-21 09:18:25.238914 spatialdata-0.0.1/docs/references.md
--rw-r--r--   0        0        0     1740 2022-05-21 09:20:38.934011 spatialdata-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      133 2022-05-21 09:22:23.488524 spatialdata-0.0.1/spatialdata/__init__.py
--rw-r--r--   0        0        0       30 2022-05-21 09:18:25.240219 spatialdata-0.0.1/spatialdata/pl/__init__.py
--rw-r--r--   0        0        0      208 2022-05-21 09:18:25.240515 spatialdata-0.0.1/spatialdata/pl/basic.py
--rw-r--r--   0        0        0       33 2022-05-21 09:18:25.240929 spatialdata-0.0.1/spatialdata/pp/__init__.py
--rw-r--r--   0        0        0      198 2022-05-21 09:18:25.241399 spatialdata-0.0.1/spatialdata/pp/basic.py
--rw-r--r--   0        0        0       30 2022-05-21 09:18:25.241877 spatialdata-0.0.1/spatialdata/tl/__init__.py
--rw-r--r--   0        0        0      186 2022-05-21 09:18:25.242252 spatialdata-0.0.1/spatialdata/tl/basic.py
--rw-r--r--   0        0        0      249 2022-05-21 09:20:56.576484 spatialdata-0.0.1/tests/test_basic.py
--rw-r--r--   0        0        0     2507 1970-01-01 00:00:00.000000 spatialdata-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 spatialdata-0.0.4/.bumpversion.cfg
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 spatialdata-0.0.4/.editorconfig
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spatialdata-0.0.4/.gitmodules
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 spatialdata-0.0.4/.mypy.ini
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 spatialdata-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 spatialdata-0.0.4/.readthedocs.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata-0.0.4/_version.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 spatialdata-0.0.4/.github/codecov.yml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata-0.0.4/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 spatialdata-0.0.4/.github/workflows/test_and_deploy.yaml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/Makefile
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/changelog.md
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/conf.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/contributing.md
+-rw-r--r--   0        0        0    33373 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/design_doc.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/index.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/installation.md
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    82458 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/_static/img/spatialdata_horizontal.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/_templates/autosummary/function.rst
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata-0.0.4/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/__init__.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/__main__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_compat.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_logging.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_types.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_utils.py
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_core/__init__.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_core/concatenate.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_core/data_extent.py
+-rw-r--r--   0        0        0    62204 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_core/spatialdata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_core/operations/__init__.py
+-rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_core/operations/aggregate.py
+-rw-r--r--   0        0        0    21113 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_core/operations/rasterize.py
+-rw-r--r--   0        0        0    17392 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_core/operations/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_core/query/__init__.py
+-rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_core/query/spatial_query.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_io/__init__.py
+-rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_io/_utils.py
+-rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_io/format.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_io/io_points.py
+-rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_io/io_raster.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_io/io_shapes.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_io/io_table.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/_io/io_zarr.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/dataloader/__init__.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/dataloader/_utils.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/dataloader/datasets.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/models/__init__.py
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/models/_utils.py
+-rw-r--r--   0        0        0    28610 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/models/models.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/transformations/__init__.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/transformations/_utils.py
+-rw-r--r--   0        0        0    19686 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/transformations/operations.py
+-rw-r--r--   0        0        0    35159 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/transformations/transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/transformations/ngff/__init__.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/transformations/ngff/_utils.py
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/transformations/ngff/ngff_coordinate_system.py
+-rw-r--r--   0        0        0    48237 2020-02-02 00:00:00.000000 spatialdata-0.0.4/src/spatialdata/transformations/ngff/ngff_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/core/operations/__init__.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/core/operations/test_aggregations.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/core/operations/test_rasterize.py
+-rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/core/operations/test_spatialdata_operations.py
+-rw-r--r--   0        0        0    19768 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/core/operations/test_transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/core/query/__init__.py
+-rw-r--r--   0        0        0    14078 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/core/query/test_spatial_query.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/data/multipolygon.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/data/points.json
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/data/polygon.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/dataloader/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/dataloader/test_datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/dataloader/test_transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/datasets/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/datasets/test_datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/io/__init__.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/io/test_format.py
+-rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/io/test_readwrite.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/io/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/models/__init__.py
+-rw-r--r--   0        0        0    14805 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/models/test_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/transformations/__init__.py
+-rw-r--r--   0        0        0    28221 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/transformations/test_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/transformations/ngff/__init__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/transformations/ngff/conftest.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/transformations/ngff/test_ngff_coordinate_system.py
+-rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/transformations/ngff/test_ngff_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 spatialdata-0.0.4/tests/utils/test_element_utils.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 spatialdata-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 spatialdata-0.0.4/README.md
+-rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 spatialdata-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 spatialdata-0.0.4/PKG-INFO
```

### Comparing `spatialdata-0.0.1/LICENSE` & `spatialdata-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.1/README.md` & `spatialdata-0.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,61 @@
+# Work in progress ⚠
+
+-   **The library is not ready.** We aim at a beta release in the following months. If interested in a demo/early beta, please reach out to us.
+-   To get involved in the discussion you are welcome to join our Zulip workspace and/or our community meetings every second week; [more info here](https://imagesc.zulipchat.com/#narrow/stream/329057-scverse/topic/SpatialData.20meetings).
+-   Links to the OME-NGFF specification: [0.4](https://ngff.openmicroscopy.org/latest/), [0.5-dev (tables)](https://github.com/ome/ngff/pull/64), [0.5-dev (transformations and coordinate systems)](https://github.com/ome/ngff/pull/138)
+
 # spatialdata
 
 [![Tests][badge-tests]][link-tests]
-[![Documentation][badge-docs]][link-docs]
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scverse/spatialdata/main.svg)](https://results.pre-commit.ci/latest/github/scverse/spatialdata/main)
+[![codecov](https://codecov.io/gh/scverse/spatialdata/branch/main/graph/badge.svg?token=X19DRSIMCU)](https://codecov.io/gh/scverse/spatialdata)
+[![DOI](https://zenodo.org/badge/487366481.svg)](https://zenodo.org/badge/latestdoi/487366481)
 
-[badge-tests]: https://img.shields.io/github/workflow/status/giovp/spatialdata/Test/main
-[link-tests]: https://github.com/scverse/spatialdata.git/actions/workflows/test.yml
-[badge-docs]: https://img.shields.io/readthedocs/spatialdata
+[badge-tests]: https://github.com/scverse/spatialdata/actions/workflows/test.yaml/badge.svg
+[link-tests]: https://github.com/scverse/spatialdata/actions/workflows/test.yaml
 
-Spatial data format.
+<img src='https://github.com/giovp/spatialdata-sandbox/raw/main/graphics/overview.png'/>
 
 ## Getting started
 
-Please refer to the [documentation][link-docs]. In particular, the
+Please refer to the [documentation][link-docs]. In particular:
 
 -   [API documentation][link-api].
+-   [Design doc][link-design-doc].
+-   [Example notebooks][link-notebooks].
 
 ## Installation
 
-You need to have Python 3.8 or newer installed on your system. If you don't have
-Python installed, we recommend installing `Miniconda <https://docs.conda.io/en/latest/miniconda.html>`\_.
-
-There are several alternative options to install spatialdata:
-
-<!--
-1) Install the latest release of `spatialdata` from `PyPI <https://pypi.org/project/spatialdata/>`_:
+Check out the docs for more complete installation instructions. For now you can install `spatialdata` with:
 
 ```bash
-pip install spatialdata
+pip install git+https://github.com/scverse/spatialdata.git@main
 ```
--->
-
-1. Install the latest development version:
-
-```bash
-pip install git+https://github.com/giovp/spatialdata.git@main
-```
-
-## Release notes
-
-See the [changelog][changelog].
 
 ## Contact
 
 For questions and help requests, you can reach out in the [scverse discourse][scverse-discourse].
 If you found a bug, please use the [issue tracker][issue-tracker].
 
 ## Citation
 
 > t.b.a
 
+You can cite the scverse publication as follows:
+
+> **The scverse project provides a computational ecosystem for single-cell omics data analysis**
+>
+> Isaac Virshup, Danila Bredikhin, Lukas Heumos, Giovanni Palla, Gregor Sturm, Adam Gayoso, Ilia Kats, Mikaela Koutrouli, Scverse Community, Bonnie Berger, Dana Pe’er, Aviv Regev, Sarah A. Teichmann, Francesca Finotello, F. Alexander Wolf, Nir Yosef, Oliver Stegle & Fabian J. Theis
+>
+> _Nat Biotechnol._ 2022 Apr 10. doi: [10.1038/s41587-023-01733-8](https://doi.org/10.1038/s41587-023-01733-8).
+
+<!-- Links -->
+
 [scverse-discourse]: https://discourse.scverse.org/
-[issue-tracker]: https://github.com/giovp/spatialdata/issues
+[issue-tracker]: https://github.com/scverse/spatialdata/issues
 [changelog]: https://spatialdata.readthedocs.io/latest/changelog.html
-[link-docs]: https://spatialdata.readthedocs.io
-[link-api]: https://spatialdata.readthedocs.io/latest/api.html
+[design doc]: https://scverse-spatialdata.readthedocs.io/en/latest/design_doc.html
+[link-docs]: https://spatialdata.scverse.org/en/latest/
+[link-api]: https://spatialdata.scverse.org/en/latest/api.html
+[link-design-doc]: https://spatialdata.scverse.org/en/latest/design_doc.html
+[link-notebooks]: https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks.html
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spatialdata-0.0.1/docs/references.bib` & `spatialdata-0.0.4/docs/references.bib`

 * *Files identical despite different names*

